---
title: Примена прилагођених поља за Microsoft Dynamics 365 Project Timesheet апликацију за мобилне уређаје на платформама iOS и Android
description: Овај чланак пружа уобичајене обрасце за коришћење екстензија за примену прилагођених поља.
author: Yowelle
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 03b79d58d1f91e07034b8c9efb408e6d7a9c29a8
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8913730"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>Примена прилагођених поља за Microsoft Dynamics 365 Project Timesheet апликацију за мобилне уређаје на платформама iOS и Android

[!include [banner](../includes/banner.md)]

Овај чланак пружа уобичајене обрасце за коришћење екстензија за примену прилагођених поља. Обухваћени су следећи чланци:

- Различити типови података које прилагођени оквир поља подржава
- Како на уносима временског распореда приказати поља само за читање или уређивање и сачувати вредности које су обезбедили корисници назад у базу података
- Како приказати поља само за читање у заглављу временског распореда
- Како интегрисати другу прилагођену пословну логику за унос подразумеваних вредности у поља и извршити додатну проверу ваљаности

## <a name="audience"></a>Корисници

Овај чланак је намењен програмерима који интегришу прилагођена поља у Microsoft Dynamics 365 Project Timesheet апликацију за мобилне уређаје која је доступна за Apple iOS и Google Android. Претпоставља се да су читаоци упознати са X++ развојем и функционалношћу временског распореда пројекта.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>Уговор о подацима – TSTimesheetCustomField X++ класа

Класа **TSTimesheetCustomField** је X++ класа уговора података која представља информације о прилагођеном пољу за функцију временског распореда. Листе прилагођених објеката поља прослеђују се и у TSTimesheetDetails уговору података и у TSTimesheetEntry уговору података да би се приказала прилагођена поља у апликацији за мобилне уређаје.

- **TSTimesheetDetails** – Уговор за заглавље временског листа.
- **TSTimesheetEntry** – Уговор о трансакцији временског распореда. Групе ових објеката које имају исте информације о пројекту и вредност **timesheetLineRecId** чине линију.

### <a name="fieldbasetype-types"></a>fieldBaseType (Типови)

Својство **FieldBaseType** на објекту **TsTimesheetCustom** одређује тип поља које се приказује у апликацији. Следеће вредности **Типова** које су подржане.

| Вредности типова | Тип              | Напомене |
|-------------|-------------------|-------|
| 0           | Стринг (и нумеричка вредност) | Поље се приказује као текстуално поље. |
| 1           | Integer           | Вредност се приказује као број без децималних места. |
| 2           | Реални број              | Вредност се приказује као број који има децимална места.<p>Да бисте приказали стварну вредност као валуту у апликацији, користите својство **fieldExtenededType**. Можете користити својство **numberOfDecimals** за подешавање броја децималних места која су приказана.</p> |
| 3           | Датум              | Формати датума се одређују према корисниковом подешавању **Датум, време и формат броја** које је наведено у одељку **Жељене опције језика и земље/региона** у делу **Корисничке опције**. |
| 4           | Boolean           | |
| 15          | GUID              | |
| 16          | Int64             | |

- Ако је својство **stringOptions** није наведено на објекту **TSTimesheetCustomField**, кориснику се пружа поље слободног текста.

    Својство **stringLength** се може користити за подешавање максималне дужине низа коју корисници могу унети.

- Ако је својство **stringOptions** наведено на објекту **TSTimesheetCustomField**, ти елементи листе су једине вредности које корисници могу да изаберу помоћу дугмади са опцијама (радио дугмад).

    У овом случају, поље низа може деловати као нумеричка вредност у сврху уноса корисника. Да бисте сачували вредност у бази података као набрајање, ручно мапирајте вредност низа на вредност набрајања пре него што је сачувате у бази података помоћу ланца команди (као пример, погледајте одељак „Употреба ланца команди у класи TSTimesheetEntryService ради чувања ставке временског распореда из апликације назад у базу података“ касније у овом чланку).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType (TSCustomFieldExtendedType)

Ово својство можете користити за форматирање стварних вредности као валуте. Овај приступ је применљив само када **fieldBaseType** има вредност **Реални број**.

- **TSCustomFieldExtendedType:None** – Није примењено форматирање.
- **TSCustomFieldExtendedType::Currency** – Форматирајте вредност као валуту.

    Када је форматирање валута активно, поље **stringValue** се може користити за додавање кода валуте који би требало да буде приказан у апликацији. Та вредност је само за читање.

    Поље **realValue** садржи износ новца који треба сачувати у бази података.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

Овим својством можете да одредите где би прилагођено поље требало да се појави у апликацији.

- **TSCustomFieldSection::Header** – Поље ће се приказати у одељку **Погледајте више детаља** у апликацији. Ова поља су увек само за читање.
- **TSCustomFieldSection::Line** – Поље ће се приказати након свих унапред припремљених поља реда у временском распореду. Ова поља могу бити за уређивање или само за читање.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

Ово својство идентификује поље када се вредности које апликација пружа поново сачувају у бази података.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

Ово својство идентификује поље када се вредности које апликација пружа поново сачувају у бази података.

### <a name="iseditable-noyes"></a>isEditable (NoYes)

Подесите ово својство на **Да** како бисте навели да корисници могу да уређују поље у одељку ставке временског распореда. Подесите својство на **Не** како би поље било само за читање.

### <a name="ismandatory-noyes"></a>isMandatory (NoYes)

Подесите ово својство на **Да** како бисте навели да поље у одељку ставке временског распореда треба да буде обавезно.

### <a name="label-str"></a>label (str)

Ово својство наводи ознаку која се приказује поред поља у апликацији.

### <a name="stringoptions-list-of-strings"></a>stringOptions (List of Strings)

Ово својство је применљиво само када се **fieldBaseType** подеси на **Низ**. Ако је **stringOptions** постављено, вредности низа које су доступне за избор преко опционалних дугмади (радио дугмади) одређене су низовима на листи. Ако нису обезбеђене ниске, дозвољен је унос слободног текста у поље ниске (као пример, погледајте одељак „Употребите ланац команди у класи TSTimesheetEntryService да бисте сачували ставку временског распореда из апликације назад у базу података“, касније у овом чланку).

### <a name="stringlength-int"></a>stringLength (int)

Ово својство наводи максималну дужину поља ниске. Ово својство је применљиво само када се **fieldBaseType** подеси на **Ниска**.

### <a name="numberofdecimals-int"></a>numberOfDecimals (int)

Ово својство наводи број децималних места која су приказана за стварно поље. Ово својство је применљиво само када се **fieldBaseType** подеси на **Реални број**.

### <a name="ordersequence-int"></a>orderSequence (int)

Ово својство контролише редослед приказивања прилагођених поља у апликацији када је наведено више од једног прилагођеног поља. Прво се приказују поља која имају мање бројеве.

### <a name="booleanvalue-boolean"></a>booleanValue (boolean)

За поља типа **Логичка вредност**, ово својство преноси логичку вредност поља између сервера и апликације.

### <a name="guidvalue-guid"></a>guidValue (guid)

За поља типа **GUID**, ово својство преноси вредност глобалног јединственог идентификатора (GUID) између сервера и апликације.

### <a name="int64value-int64"></a>int64Value (int64)

За поља типа **Int64**, ово својство преноси int64 вредност поља између сервера и апликације.

### <a name="intvalue-int"></a>intValue (int)

За поља типа **Int**, ово својство преноси int вредност поља између сервера и апликације.

### <a name="realvalue-real"></a>realValue (real)

За поља типа **Реални број**, ово својство преноси реалну вредност поља између сервера и апликације.

### <a name="stringvalue-str"></a>stringValue (str)

За поља типа **Ниска**, ово својство преноси вредност ниске поља између сервера и апликације. Такође се користи за поља типа **Реални број** који су форматирани као валута. За та поља, својство се користи за прослеђивање кода валуте апликацији.

### <a name="datevalue-date"></a>dateValue (date)

За поља типа **Датум**, ово својство преноси вредност датума поља између сервера и апликације.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>Прикажите и сачувајте прилагођено поље у одељку ставке временског распореда

У наставку се налази снимак екрана из апликације за мобилне уређаје где се креира ставка временског распореда. Показује унапред припремљена поља и прилагођена поља у одељку „Ставка времена“ под називом „Тест ниска“ са већ постављеном нумеричком вредношћу „Друга опција“.

![Прилагођено поље за тестирање ниски у апликацији.](media/timesheet-entry.jpg)



У наставку се налази снимак екрана из апликације за мобилне уређаје корисника који бира једну од опција набрајања доступних за прилагођено поље „Тест ниска“.  Две опције су „Прва опција“ и „Друга опција“, приказане као радио дугмад. Тренутно је изабрана друга опција.

![Дугмад са опцијама (радио дугмад) за поље за тестирање ниски.](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>Проширите табелу TSTimesheetLine тако да има прилагођено поље

У типичним сценаријима, вероватно ће подаци за прилагођено поље у одељку ставке временског распореда бити сачувани у табели TSTimesheetLine. Међутим, друге табеле се могу користити ако се подаци могу добити на основу TSTimesheetTrans записа који је наведен или ако нема одређени контекст записа (на пример, ако је поље постављено као само за читање у параметрима пројекта).

Имајте на уму да прилагођена поља не морају имати никакве пратеће записе базе података. Могу се динамички генерисати на основу X++ логике. Овај приступ може бити користан у сценаријима само за читање (погледајте одељак „Користите ланац команди на класи TSTimesheetDetails, методи buildCustomFieldListForHeader за попуњавање детаља временског распореда“ за пример динамички генерисаних вредности прилагођених поља.)

У наставку се налази снимак екрана са Visual Studio стаблом објеката апликације. Приказује се проширење табеле TSTimesheetLine са пољем TestLineString које је додато као прилагођено поље.

![Ниска линије.](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>Користите ланац команди на методи buildCustomFieldList класе TSTimesheetSettings да бисте приказали поље у одељку ставке временског распореда

Овај кôд контролише поставке приказа за поље у апликацији. На пример, контролише тип поља, ознаку, да ли је поље обавезно и у ком одељку се поље приказује.

Следећи пример приказује поље низа за ставке времена. Ово поље има две опције, **Прва опција** и **Друга опција**, које су доступне преко дугмади опција (радио дугмади). Поље у апликацији је повезано са пољем **TestLineString** које се додаје у табелу TSTimesheetLine.

Обратите пажњу на употребу методе **TSTimesheetCustomField::newFromMetatdata()** за поједностављивање иницијализације својстава прилагођеног поља: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** и **numberOfDecimals**. Ове параметре можете такође ручно да подесите како желите.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>Користите ланац команди на методи buildCustomFieldListForEntry класе TSTimesheetEntry да бисте уносили вредности у ставку временског распореда

Метода **buildCustomFieldListForEntry** се користи за унос вредности у сачуване редове временског распореда у апликацији за мобилне уређаје. Као параметар узима се запис TSTimesheetTrans. Поља из тог записа могу се користити за попуњавање вредности прилагођеног поља у апликацији.

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>Употреба ланца команди у класи TSTimesheetEntryService ради чувања ставке временског распореда из апликације назад у базу података

Да бисте сачували прилагођено поље у базу података у уобичајеној употреби, морате проширити више метода:

- Метода **timesheetLineNeedsUpdating** се користи да би се утврдило да ли је корисник у апликацији променио запис линије и да ли запис мора да буде сачуван у бази података. Ако перформансе нису проблем, ова метода се може поједноставити тако да се увек враћа **тачно**.
- Методе **populateTimesheetLineFromEntryDuringCreate** и **populateTimesheetLineFromEntryDuringUpdate** се могу проширити тако да уносе вредности у запис базе података TSTimesheetLine из обезбеђеног записа TSTimesheetEntry уговора података. У примеру који следи обратите пажњу како се преко X++ кода обавља ручно мапирање између поља базе података и поља ставке.
- Метода **populateTimesheetWeekFromEntry** се такође може проширити ако се прилагођено поље које се мапира на објекат **TSTimesheetEntry** мора уписати назад у табелу базе података TSTimesheetLineweek.

> [!NOTE]
> Следећи пример чува вредност **firstOption** или **secondOption** коју корисник бира у базу података као сирову вредност низа. Ако је поље базе података поље **Набрајање**, те вредности се могу ручно мапирати на вредност набрајања, а затим сачувати у пољу набрајања у табели базе података.

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>Прикажите прилагођено поље у одељку заглавља временског распореда

У наставку се налази снимак екрана из апликације за мобилне уређаје где корисник прегледа временски распоред. У горњем десном углу је изабрано дугме „Више информација“ да би се приказала опција „Прикажи више детаља“.  

![Команда Прикажи више детаља.](media/show-more.png)

У наставку се налази снимак екрана из апликације за мобилне уређаје где се приказује одељак „Још“ временског распореда. Прилагођено поље под називом „Стопа искоришћености овог временског распореда (израчунато прилагођено поље)“ додато је у одељак заглавља временског распореда. Вредност само за читање „0,667“ постављена је у прилагођеном пољу.

![Одељак „Још“.](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>Проширите табелу TSTimesheetTable тако да има прилагођено поље

У типичним сценаријима, вероватно ће подаци за прилагођено поље у одељку заглавља бити повучени из табеле TSTimesheetHeader. Међутим, друге табеле се могу користити ако се подаци могу добити на основу записа TSTimesheetTable који је наведен или ако нема одређени контекст записа (на пример, ако је поље постављено као само за читање у параметрима пројекта).

Имајте на уму да прилагођена поља не морају имати никакве пратеће записе базе података. Могу се динамички генерисати на основу X++ логике. Пример који следи показује овај приступ.

Поља у одељку заглавља у апликацији су увек само за читање.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>Користите ланац команди на методи buildCustomFieldList класе TSTimesheetSettings да бисте приказали поље у одељку заглавља временског распореда

Овај кôд контролише поставке приказа за поље у апликацији. На пример, контролише тип поља, ознаку, да ли је поље обавезно и у ком одељку се поље приказује.

Следећи пример приказује израчунату вредност у одељку заглавља у апликацији.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>Користите ланац команди на методи buildCustomFieldListForHeader класе TSTimesheetDetails да бисте попуњавали детаље временског распореда

Метода **buildCustomFieldListForHeader** се користи за попуну детаља заглавља временског распореда у апликацији за мобилне уређаје. Као параметар се узима запис TSTimesheetTable. Поља из тог записа могу се користити за попуњавање вредности прилагођеног поља у апликацији. Следећи пример не чита ниједну вредност из базе података. Уместо тога, користи X++ логику за генерисање израчунате вредности која се затим приказује у апликацији.


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a>Остале могућности прилагодљивости/проширивости

### <a name="adding-additional-validation-for-the-app"></a>Додавање додатне провере за апликацију

Постојећа логика за функционалност временског листа на нивоу базе података и даље ће радити како се очекивало. Да бисте прекинули довршавање операција чувања или слања и приказали одређену поруку о грешци, можете да додате **throw error("порука кориснику")** у кôд преко ланца додатка команди. Следе три примера корисних проширивих метода:

- Ако **validateWrite** на табели TSTimesheetLine врати **нетачно** током операције чувања за ред временског распореда, порука о грешци се приказује у апликацији за мобилне уређаје.
- Ако **validateSubmit** на табели TSTimesheetTable врати **нетачно** током прослеђивања временског распореда у апликацији, кориснику се приказује порука о грешци.
- Логика која попуњава поља (на пример, **Својство реда**) током методе **insert** на табели TSTimesheetLine и даље ће бити активна.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>Сакривање и означавање поља изван оквира као само за читање путем конфигурације

Из параметара пројекта можете да направите унапред припремљена поља која су само за читање или скривена у апликацији за мобилне уређаје. Поставите опције у одељку **Мобилни временски распореди** на картици **Временски распоред** на страници **Параметри управљања пројектом и рачуноводством**.

![Параметри пројекта.](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>Промена активности које су доступне за избор путем додатака

Активности које су на располагању за одабир за пројекат попуњавају се путем метода **getActivitiesForProject()** и **getActivityQuery()** у класи **TsTimesheetProjectService**. Можете да користите ланац команди да бисте ово понашање променили тако да одговара вашем пословном сценарију за активности које су доступне за одабир за одређени пројекат.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>Унос подразумеване категорије пројекта у ставке временског распореда

Унос подразумеване категорије пројекта у ставке временског распореда одвија се на три нивоа. Можете користити ланац команди да проширите понашање на било ком или свим овим нивоима како бисте постигли жељено понашање. Користи се следећа хијерархија:

1. Апликација покушава да постави подразумевану категорију из ресурса пројекта. Ова подразумевана категорија је подешена у методама **getCurrentUserResource** и **getDelegatedResourcesForCurrentUser** у класи **TSTimesheetSettingsService**.
2. Ако подразумевана категорија није наведена на нивоу ресурса пројекта, апликација покушава да је повуче из активности пројекта. Ова подразумевана категорија је постављена у методи **getActivitiesForProject** у класи **TSTimesheetProjectService**.
3. Ако подразумевана категорија није наведена на нивоу активности пројекта, подразумевана категорија се преузима из параметара пројекта. Ова подразумевана категорија се поставља у методи **getProjectDetailsbyRule** у класи **TSTimesheetProjectService**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]