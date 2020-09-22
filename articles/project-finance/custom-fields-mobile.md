---
title: Примена прилагођених поља за Microsoft Dynamics 365 Project Timesheet апликацију за мобилне уређаје на платформама iOS и Android
description: Ова тема пружа уобичајене обрасце за коришћење екстензија за примену прилагођених поља.
author: KimANelson
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: 4564bbda-34ea-4647-a9bc-f6ef17b1038b
ms.search.region: Global
ms.search.industry: Service industries
ms.author: knelson
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 16c3b79dcaaf8c5c491587618256694f82f44753
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755336"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="cc70b-103">Примена прилагођених поља за Microsoft Dynamics 365 Project Timesheet апликацију за мобилне уређаје на платформама iOS и Android</span><span class="sxs-lookup"><span data-stu-id="cc70b-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="cc70b-104">Ова тема пружа уобичајене обрасце за коришћење екстензија за примену прилагођених поља.</span><span class="sxs-lookup"><span data-stu-id="cc70b-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="cc70b-105">Обухваћене су следеће теме:</span><span class="sxs-lookup"><span data-stu-id="cc70b-105">The following topics are covered:</span></span>

- <span data-ttu-id="cc70b-106">Различити типови података које прилагођени оквир поља подржава</span><span class="sxs-lookup"><span data-stu-id="cc70b-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="cc70b-107">Како на уносима временског распореда приказати поља само за читање или уређивање и сачувати вредности које су обезбедили корисници назад у базу података</span><span class="sxs-lookup"><span data-stu-id="cc70b-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="cc70b-108">Како приказати поља само за читање у заглављу временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="cc70b-109">Како интегрисати другу прилагођену пословну логику за унос подразумеваних вредности у поља и извршити додатну проверу ваљаности</span><span class="sxs-lookup"><span data-stu-id="cc70b-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="cc70b-110">Корисници</span><span class="sxs-lookup"><span data-stu-id="cc70b-110">Audience</span></span>

<span data-ttu-id="cc70b-111">Ова тема је намењена програмерима који интегришу прилагођена поља у Microsoft Dynamics 365 Project Timesheet апликацију за мобилне уређаје која је доступна за Apple iOS и Google Android.</span><span class="sxs-lookup"><span data-stu-id="cc70b-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="cc70b-112">Претпоставља се да су читаоци упознати са X++ развојем и функционалношћу временског распореда пројекта.</span><span class="sxs-lookup"><span data-stu-id="cc70b-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="cc70b-113">Уговор о подацима – TSTimesheetCustomField X++ класа</span><span class="sxs-lookup"><span data-stu-id="cc70b-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="cc70b-114">Класа **TSTimesheetCustomField** је X++ класа уговора података која представља информације о прилагођеном пољу за функцију временског распореда.</span><span class="sxs-lookup"><span data-stu-id="cc70b-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="cc70b-115">Листе прилагођених објеката поља прослеђују се и у TSTimesheetDetails уговору података и у TSTimesheetEntry уговору података да би се приказала прилагођена поља у апликацији за мобилне уређаје.</span><span class="sxs-lookup"><span data-stu-id="cc70b-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="cc70b-116">**TSTimesheetDetails** – Уговор за заглавље временског листа.</span><span class="sxs-lookup"><span data-stu-id="cc70b-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="cc70b-117">**TSTimesheetEntry** – Уговор о трансакцији временског распореда.</span><span class="sxs-lookup"><span data-stu-id="cc70b-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="cc70b-118">Групе ових објеката које имају исте информације о пројекту и вредност **timesheetLineRecId** чине линију.</span><span class="sxs-lookup"><span data-stu-id="cc70b-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="cc70b-119">fieldBaseType (Типови)</span><span class="sxs-lookup"><span data-stu-id="cc70b-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="cc70b-120">Својство **FieldBaseType** на објекту **TsTimesheetCustom** одређује тип поља које се приказује у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="cc70b-121">Следеће вредности **Типова** које су подржане.</span><span class="sxs-lookup"><span data-stu-id="cc70b-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="cc70b-122">Вредности типова</span><span class="sxs-lookup"><span data-stu-id="cc70b-122">Types value</span></span> | <span data-ttu-id="cc70b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cc70b-123">Type</span></span>              | <span data-ttu-id="cc70b-124">Напомене</span><span class="sxs-lookup"><span data-stu-id="cc70b-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="cc70b-125">0</span><span class="sxs-lookup"><span data-stu-id="cc70b-125">0</span></span>           | <span data-ttu-id="cc70b-126">Стринг (и нумеричка вредност)</span><span class="sxs-lookup"><span data-stu-id="cc70b-126">String (and Enum)</span></span> | <span data-ttu-id="cc70b-127">Поље се приказује као текстуално поље.</span><span class="sxs-lookup"><span data-stu-id="cc70b-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="cc70b-128">1</span><span class="sxs-lookup"><span data-stu-id="cc70b-128">1</span></span>           | <span data-ttu-id="cc70b-129">Integer</span><span class="sxs-lookup"><span data-stu-id="cc70b-129">Integer</span></span>           | <span data-ttu-id="cc70b-130">Вредност се приказује као број без децималних места.</span><span class="sxs-lookup"><span data-stu-id="cc70b-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="cc70b-131">2</span><span class="sxs-lookup"><span data-stu-id="cc70b-131">2</span></span>           | <span data-ttu-id="cc70b-132">Реални број</span><span class="sxs-lookup"><span data-stu-id="cc70b-132">Real</span></span>              | <span data-ttu-id="cc70b-133">Вредност се приказује као број који има децимална места.</span><span class="sxs-lookup"><span data-stu-id="cc70b-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="cc70b-134">Да бисте приказали стварну вредност као валуту у апликацији, користите својство **fieldExtenededType**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="cc70b-135">Можете користити својство **numberOfDecimals** за подешавање броја децималних места која су приказана.</span><span class="sxs-lookup"><span data-stu-id="cc70b-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="cc70b-136">3</span><span class="sxs-lookup"><span data-stu-id="cc70b-136">3</span></span>           | <span data-ttu-id="cc70b-137">Датум</span><span class="sxs-lookup"><span data-stu-id="cc70b-137">Date</span></span>              | <span data-ttu-id="cc70b-138">Формати датума се одређују према корисниковом подешавању **Датум, време и формат броја** које је наведено у одељку **Жељене опције језика и земље/региона** у делу **Корисничке опције**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="cc70b-139">4</span><span class="sxs-lookup"><span data-stu-id="cc70b-139">4</span></span>           | <span data-ttu-id="cc70b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc70b-140">Boolean</span></span>           | |
| <span data-ttu-id="cc70b-141">15</span><span class="sxs-lookup"><span data-stu-id="cc70b-141">15</span></span>          | <span data-ttu-id="cc70b-142">GUID</span><span class="sxs-lookup"><span data-stu-id="cc70b-142">GUID</span></span>              | |
| <span data-ttu-id="cc70b-143">16</span><span class="sxs-lookup"><span data-stu-id="cc70b-143">16</span></span>          | <span data-ttu-id="cc70b-144">Int64</span><span class="sxs-lookup"><span data-stu-id="cc70b-144">Int64</span></span>             | |

- <span data-ttu-id="cc70b-145">Ако је својство **stringOptions** није наведено на објекту **TSTimesheetCustomField**, кориснику се пружа поље слободног текста.</span><span class="sxs-lookup"><span data-stu-id="cc70b-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="cc70b-146">Својство **stringLength** се може користити за подешавање максималне дужине низа коју корисници могу унети.</span><span class="sxs-lookup"><span data-stu-id="cc70b-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="cc70b-147">Ако је својство **stringOptions** наведено на објекту **TSTimesheetCustomField**, ти елементи листе су једине вредности које корисници могу да изаберу помоћу дугмади са опцијама (радио дугмад).</span><span class="sxs-lookup"><span data-stu-id="cc70b-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="cc70b-148">У овом случају, поље низа може деловати као нумеричка вредност у сврху уноса корисника.</span><span class="sxs-lookup"><span data-stu-id="cc70b-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="cc70b-149">Да бисте сачували вредност у бази података као набрајање, ручно мапирајте вредност низа на вредност набрајања пре него што је сачувате у бази података помоћу ланца команди (као пример, погледајте одељак „Употреба ланца команди у класи TSTimesheetEntryService ради чувања ставке временског распореда из апликације назад у базу података“ касније у овој теми).</span><span class="sxs-lookup"><span data-stu-id="cc70b-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="cc70b-150">fieldExtendedType (TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="cc70b-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="cc70b-151">Ово својство можете користити за форматирање стварних вредности као валуте.</span><span class="sxs-lookup"><span data-stu-id="cc70b-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="cc70b-152">Овај приступ је применљив само када **fieldBaseType** има вредност **Реални број**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="cc70b-153">**TSCustomFieldExtendedType:None** – Није примењено форматирање.</span><span class="sxs-lookup"><span data-stu-id="cc70b-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="cc70b-154">**TSCustomFieldExtendedType::Currency** – Форматирајте вредност као валуту.</span><span class="sxs-lookup"><span data-stu-id="cc70b-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="cc70b-155">Када је форматирање валута активно, поље **stringValue** се може користити за додавање кода валуте који би требало да буде приказан у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="cc70b-156">Та вредност је само за читање.</span><span class="sxs-lookup"><span data-stu-id="cc70b-156">The value is a read-only value.</span></span>

    <span data-ttu-id="cc70b-157">Поље **realValue** садржи износ новца који треба сачувати у бази података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="cc70b-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="cc70b-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="cc70b-159">Овим својством можете да одредите где би прилагођено поље требало да се појави у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="cc70b-160">**TSCustomFieldSection::Header** – Поље ће се приказати у одељку **Погледајте више детаља** у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="cc70b-161">Ова поља су увек само за читање.</span><span class="sxs-lookup"><span data-stu-id="cc70b-161">These fields are always read-only.</span></span>
- <span data-ttu-id="cc70b-162">**TSCustomFieldSection::Line** – Поље ће се приказати након свих унапред припремљених поља реда у временском распореду.</span><span class="sxs-lookup"><span data-stu-id="cc70b-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="cc70b-163">Ова поља могу бити за уређивање или само за читање.</span><span class="sxs-lookup"><span data-stu-id="cc70b-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="cc70b-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="cc70b-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="cc70b-165">Ово својство идентификује поље када се вредности које апликација пружа поново сачувају у бази података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="cc70b-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="cc70b-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="cc70b-167">Ово својство идентификује поље када се вредности које апликација пружа поново сачувају у бази података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="cc70b-168">isEditable (NoYes)</span><span class="sxs-lookup"><span data-stu-id="cc70b-168">isEditable (NoYes)</span></span>

<span data-ttu-id="cc70b-169">Подесите ово својство на **Да** како бисте навели да корисници могу да уређују поље у одељку ставке временског распореда.</span><span class="sxs-lookup"><span data-stu-id="cc70b-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="cc70b-170">Подесите својство на **Не** како би поље било само за читање.</span><span class="sxs-lookup"><span data-stu-id="cc70b-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="cc70b-171">isMandatory (NoYes)</span><span class="sxs-lookup"><span data-stu-id="cc70b-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="cc70b-172">Подесите ово својство на **Да** како бисте навели да поље у одељку ставке временског распореда треба да буде обавезно.</span><span class="sxs-lookup"><span data-stu-id="cc70b-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="cc70b-173">label (str)</span><span class="sxs-lookup"><span data-stu-id="cc70b-173">label (str)</span></span>

<span data-ttu-id="cc70b-174">Ово својство наводи ознаку која се приказује поред поља у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="cc70b-175">stringOptions (List of Strings)</span><span class="sxs-lookup"><span data-stu-id="cc70b-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="cc70b-176">Ово својство је применљиво само када се **fieldBaseType** подеси на **Низ**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="cc70b-177">Ако је **stringOptions** постављено, вредности низа које су доступне за избор преко опционалних дугмади (радио дугмади) одређене су низовима на листи.</span><span class="sxs-lookup"><span data-stu-id="cc70b-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="cc70b-178">Ако нису обезбеђене ниске, дозвољен је унос слободног текста у поље ниске (као пример, погледајте одељак „Употребите ланац команди у класи TSTimesheetEntryService да бисте сачували ставку временског распореда из апликације назад у базу података“, касније у овој теми).</span><span class="sxs-lookup"><span data-stu-id="cc70b-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="cc70b-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="cc70b-179">stringLength (int)</span></span>

<span data-ttu-id="cc70b-180">Ово својство наводи максималну дужину поља ниске.</span><span class="sxs-lookup"><span data-stu-id="cc70b-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="cc70b-181">Ово својство је применљиво само када се **fieldBaseType** подеси на **Ниска**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="cc70b-182">numberOfDecimals (int)</span><span class="sxs-lookup"><span data-stu-id="cc70b-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="cc70b-183">Ово својство наводи број децималних места која су приказана за стварно поље.</span><span class="sxs-lookup"><span data-stu-id="cc70b-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="cc70b-184">Ово својство је применљиво само када се **fieldBaseType** подеси на **Реални број**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="cc70b-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="cc70b-185">orderSequence (int)</span></span>

<span data-ttu-id="cc70b-186">Ово својство контролише редослед приказивања прилагођених поља у апликацији када је наведено више од једног прилагођеног поља.</span><span class="sxs-lookup"><span data-stu-id="cc70b-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="cc70b-187">Прво се приказују поља која имају мање бројеве.</span><span class="sxs-lookup"><span data-stu-id="cc70b-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="cc70b-188">booleanValue (boolean)</span><span class="sxs-lookup"><span data-stu-id="cc70b-188">booleanValue (boolean)</span></span>

<span data-ttu-id="cc70b-189">За поља типа **Логичка вредност**, ово својство преноси логичку вредност поља између сервера и апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="cc70b-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="cc70b-190">guidValue (guid)</span></span>

<span data-ttu-id="cc70b-191">За поља типа **GUID**, ово својство преноси вредност глобалног јединственог идентификатора (GUID) између сервера и апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="cc70b-192">int64Value (int64)</span><span class="sxs-lookup"><span data-stu-id="cc70b-192">int64Value (int64)</span></span>

<span data-ttu-id="cc70b-193">За поља типа **Int64**, ово својство преноси int64 вредност поља између сервера и апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="cc70b-194">intValue (int)</span><span class="sxs-lookup"><span data-stu-id="cc70b-194">intValue (int)</span></span>

<span data-ttu-id="cc70b-195">За поља типа **Int**, ово својство преноси int вредност поља између сервера и апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="cc70b-196">realValue (real)</span><span class="sxs-lookup"><span data-stu-id="cc70b-196">realValue (real)</span></span>

<span data-ttu-id="cc70b-197">За поља типа **Реални број**, ово својство преноси реалну вредност поља између сервера и апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="cc70b-198">stringValue (str)</span><span class="sxs-lookup"><span data-stu-id="cc70b-198">stringValue (str)</span></span>

<span data-ttu-id="cc70b-199">За поља типа **Ниска**, ово својство преноси вредност ниске поља између сервера и апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="cc70b-200">Такође се користи за поља типа **Реални број** који су форматирани као валута.</span><span class="sxs-lookup"><span data-stu-id="cc70b-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="cc70b-201">За та поља, својство се користи за прослеђивање кода валуте апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="cc70b-202">dateValue (date)</span><span class="sxs-lookup"><span data-stu-id="cc70b-202">dateValue (date)</span></span>

<span data-ttu-id="cc70b-203">За поља типа **Датум**, ово својство преноси вредност датума поља између сервера и апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="cc70b-204">Прикажите и сачувајте прилагођено поље у одељку ставке временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="cc70b-205">У наставку се налази снимак екрана из апликације за мобилне уређаје где се креира ставка временског распореда.</span><span class="sxs-lookup"><span data-stu-id="cc70b-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="cc70b-206">Показује унапред припремљена поља и прилагођена поља у одељку „Ставка времена“ под називом „Тест ниска“ са већ постављеном нумеричком вредношћу „Друга опција“.</span><span class="sxs-lookup"><span data-stu-id="cc70b-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![Прилагођено поље за тестирање ниски у апликацији](media/timesheet-entry.jpg)



<span data-ttu-id="cc70b-208">У наставку се налази снимак екрана из апликације за мобилне уређаје корисника који бира једну од опција набрајања доступних за прилагођено поље „Тест ниска“.</span><span class="sxs-lookup"><span data-stu-id="cc70b-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="cc70b-209">Две опције су „Прва опција“ и „Друга опција“, приказане као радио дугмад.</span><span class="sxs-lookup"><span data-stu-id="cc70b-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="cc70b-210">Тренутно је изабрана друга опција.</span><span class="sxs-lookup"><span data-stu-id="cc70b-210">The second option is currently selected.</span></span>

![Дугмад са опцијама (радио дугмад) за прилагођено поље Тест ниска](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="cc70b-212">Проширите табелу TSTimesheetLine тако да има прилагођено поље</span><span class="sxs-lookup"><span data-stu-id="cc70b-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="cc70b-213">У типичним сценаријима, вероватно ће подаци за прилагођено поље у одељку ставке временског распореда бити сачувани у табели TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="cc70b-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="cc70b-214">Међутим, друге табеле се могу користити ако се подаци могу добити на основу TSTimesheetTrans записа који је наведен или ако нема одређени контекст записа (на пример, ако је поље постављено као само за читање у параметрима пројекта).</span><span class="sxs-lookup"><span data-stu-id="cc70b-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="cc70b-215">Имајте на уму да прилагођена поља не морају имати никакве пратеће записе базе података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="cc70b-216">Могу се динамички генерисати на основу X++ логике.</span><span class="sxs-lookup"><span data-stu-id="cc70b-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="cc70b-217">Овај приступ може бити користан у сценаријима само за читање (погледајте одељак „Користите ланац команди на класи TSTimesheetDetails, методи buildCustomFieldListForHeader за попуњавање детаља временског распореда“ за пример динамички генерисаних вредности прилагођених поља.)</span><span class="sxs-lookup"><span data-stu-id="cc70b-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="cc70b-218">У наставку се налази снимак екрана са Visual Studio стаблом објеката апликације.</span><span class="sxs-lookup"><span data-stu-id="cc70b-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="cc70b-219">Приказује се проширење табеле TSTimesheetLine са пољем TestLineString које је додато као прилагођено поље.</span><span class="sxs-lookup"><span data-stu-id="cc70b-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![Ниска линије](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="cc70b-221">Користите ланац команди на методи buildCustomFieldList класе TSTimesheetSettings да бисте приказали поље у одељку ставке временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="cc70b-222">Овај кôд контролише поставке приказа за поље у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="cc70b-223">На пример, контролише тип поља, ознаку, да ли је поље обавезно и у ком одељку се поље приказује.</span><span class="sxs-lookup"><span data-stu-id="cc70b-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="cc70b-224">Следећи пример приказује поље низа за ставке времена.</span><span class="sxs-lookup"><span data-stu-id="cc70b-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="cc70b-225">Ово поље има две опције, **Прва опција** и **Друга опција**, које су доступне преко дугмади опција (радио дугмади).</span><span class="sxs-lookup"><span data-stu-id="cc70b-225">This field has two options, **First option** and **Second option**, that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="cc70b-226">Поље у апликацији је повезано са пољем **TestLineString** које се додаје у табелу TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="cc70b-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="cc70b-227">Обратите пажњу на употребу методе **TSTimesheetCustomField::newFromMetatdata()** за поједностављивање иницијализације својстава прилагођеног поља: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** и **numberOfDecimals**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength**, and **numberOfDecimals**.</span></span> <span data-ttu-id="cc70b-228">Ове параметре можете такође ручно да подесите како желите.</span><span class="sxs-lookup"><span data-stu-id="cc70b-228">You can also set these parameters manually, as you prefer.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="cc70b-229">Користите ланац команди на методи buildCustomFieldListForEntry класе TSTimesheetEntry да бисте уносили вредности у ставку временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="cc70b-230">Метода **buildCustomFieldListForEntry** се користи за унос вредности у сачуване редове временског распореда у апликацији за мобилне уређаје.</span><span class="sxs-lookup"><span data-stu-id="cc70b-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="cc70b-231">Као параметар узима се запис TSTimesheetTrans.</span><span class="sxs-lookup"><span data-stu-id="cc70b-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="cc70b-232">Поља из тог записа могу се користити за попуњавање вредности прилагођеног поља у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="cc70b-233">Употреба ланца команди у класи TSTimesheetEntryService ради чувања ставке временског распореда из апликације назад у базу података</span><span class="sxs-lookup"><span data-stu-id="cc70b-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="cc70b-234">Да бисте сачували прилагођено поље у базу података у уобичајеној употреби, морате проширити више метода:</span><span class="sxs-lookup"><span data-stu-id="cc70b-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="cc70b-235">Метода **timesheetLineNeedsUpdating** се користи да би се утврдило да ли је корисник у апликацији променио запис линије и да ли запис мора да буде сачуван у бази података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="cc70b-236">Ако перформансе нису проблем, ова метода се може поједноставити тако да се увек враћа **тачно**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="cc70b-237">Методе **populateTimesheetLineFromEntryDuringCreate** и **populateTimesheetLineFromEntryDuringUpdate** се могу проширити тако да уносе вредности у запис базе података TSTimesheetLine из обезбеђеног записа TSTimesheetEntry уговора података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="cc70b-238">У примеру који следи обратите пажњу како се преко X++ кода обавља ручно мапирање између поља базе података и поља ставке.</span><span class="sxs-lookup"><span data-stu-id="cc70b-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="cc70b-239">Метода **populateTimesheetWeekFromEntry** се такође може проширити ако се прилагођено поље које се мапира на објекат **TSTimesheetEntry** мора уписати назад у табелу базе података TSTimesheetLineweek.</span><span class="sxs-lookup"><span data-stu-id="cc70b-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="cc70b-240">Следећи пример чува вредност **firstOption** или **secondOption** коју корисник бира у базу података као сирову вредност низа.</span><span class="sxs-lookup"><span data-stu-id="cc70b-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="cc70b-241">Ако је поље базе података поље **Набрајање**, те вредности се могу ручно мапирати на вредност набрајања, а затим сачувати у пољу набрајања у табели базе података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="cc70b-242">Прикажите прилагођено поље у одељку заглавља временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="cc70b-243">У наставку се налази снимак екрана из апликације за мобилне уређаје где корисник прегледа временски распоред.</span><span class="sxs-lookup"><span data-stu-id="cc70b-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="cc70b-244">У горњем десном углу је изабрано дугме „Више информација“ да би се приказала опција „Прикажи више детаља“.</span><span class="sxs-lookup"><span data-stu-id="cc70b-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![Команда Прикажи више детаља](media/show-more.png)

<span data-ttu-id="cc70b-246">У наставку се налази снимак екрана из апликације за мобилне уређаје где се приказује одељак „Још“ временског распореда.</span><span class="sxs-lookup"><span data-stu-id="cc70b-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="cc70b-247">Прилагођено поље под називом „Стопа искоришћености овог временског распореда (израчунато прилагођено поље)“ додато је у одељак заглавља временског распореда.</span><span class="sxs-lookup"><span data-stu-id="cc70b-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="cc70b-248">Вредност само за читање „0,667“ постављена је у прилагођеном пољу.</span><span class="sxs-lookup"><span data-stu-id="cc70b-248">A read-only value of "0.667" is set on the custom field.</span></span>

![Одељак „Још“](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="cc70b-250">Проширите табелу TSTimesheetTable тако да има прилагођено поље</span><span class="sxs-lookup"><span data-stu-id="cc70b-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="cc70b-251">У типичним сценаријима, вероватно ће подаци за прилагођено поље у одељку заглавља бити повучени из табеле TSTimesheetHeader.</span><span class="sxs-lookup"><span data-stu-id="cc70b-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="cc70b-252">Међутим, друге табеле се могу користити ако се подаци могу добити на основу записа TSTimesheetTable који је наведен или ако нема одређени контекст записа (на пример, ако је поље постављено као само за читање у параметрима пројекта).</span><span class="sxs-lookup"><span data-stu-id="cc70b-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="cc70b-253">Имајте на уму да прилагођена поља не морају имати никакве пратеће записе базе података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="cc70b-254">Могу се динамички генерисати на основу X++ логике.</span><span class="sxs-lookup"><span data-stu-id="cc70b-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="cc70b-255">Пример који следи показује овај приступ.</span><span class="sxs-lookup"><span data-stu-id="cc70b-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="cc70b-256">Поља у одељку заглавља у апликацији су увек само за читање.</span><span class="sxs-lookup"><span data-stu-id="cc70b-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="cc70b-257">Користите ланац команди на методи buildCustomFieldList класе TSTimesheetSettings да бисте приказали поље у одељку заглавља временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="cc70b-258">Овај кôд контролише поставке приказа за поље у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="cc70b-259">На пример, контролише тип поља, ознаку, да ли је поље обавезно и у ком одељку се поље приказује.</span><span class="sxs-lookup"><span data-stu-id="cc70b-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="cc70b-260">Следећи пример приказује израчунату вредност у одељку заглавља у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-260">The following example shows a computed value in the header section in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="cc70b-261">Користите ланац команди на методи buildCustomFieldListForHeader класе TSTimesheetDetails да бисте попуњавали детаље временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="cc70b-262">Метода **buildCustomFieldListForHeader** се користи за попуну детаља заглавља временског распореда у апликацији за мобилне уређаје.</span><span class="sxs-lookup"><span data-stu-id="cc70b-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="cc70b-263">Као параметар се узима запис TSTimesheetTable.</span><span class="sxs-lookup"><span data-stu-id="cc70b-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="cc70b-264">Поља из тог записа могу се користити за попуњавање вредности прилагођеног поља у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="cc70b-265">Следећи пример не чита ниједну вредност из базе података.</span><span class="sxs-lookup"><span data-stu-id="cc70b-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="cc70b-266">Уместо тога, користи X++ логику за генерисање израчунате вредности која се затим приказује у апликацији.</span><span class="sxs-lookup"><span data-stu-id="cc70b-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


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

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="cc70b-267">Остале могућности прилагодљивости/проширивости</span><span class="sxs-lookup"><span data-stu-id="cc70b-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="cc70b-268">Додавање додатне провере за апликацију</span><span class="sxs-lookup"><span data-stu-id="cc70b-268">Adding additional validation for the app</span></span>

<span data-ttu-id="cc70b-269">Постојећа логика за функционалност временског листа на нивоу базе података и даље ће радити како се очекивало.</span><span class="sxs-lookup"><span data-stu-id="cc70b-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="cc70b-270">Да бисте прекинули довршавање операција чувања или слања и приказали одређену поруку о грешци, можете да додате **throw error("порука кориснику")** у кôд преко ланца додатка команди.</span><span class="sxs-lookup"><span data-stu-id="cc70b-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="cc70b-271">Следе три примера корисних проширивих метода:</span><span class="sxs-lookup"><span data-stu-id="cc70b-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="cc70b-272">Ако **validateWrite** на табели TSTimesheetLine врати **нетачно** током операције чувања за ред временског распореда, порука о грешци се приказује у апликацији за мобилне уређаје.</span><span class="sxs-lookup"><span data-stu-id="cc70b-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="cc70b-273">Ако **validateSubmit** на табели TSTimesheetTable врати **нетачно** током прослеђивања временског распореда у апликацији, кориснику се приказује порука о грешци.</span><span class="sxs-lookup"><span data-stu-id="cc70b-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="cc70b-274">Логика која попуњава поља (на пример, **Својство реда**) током методе **insert** на табели TSTimesheetLine и даље ће бити активна.</span><span class="sxs-lookup"><span data-stu-id="cc70b-274">Logic that fills in fields (for example, **Line Property**) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="cc70b-275">Сакривање и означавање поља изван оквира као само за читање путем конфигурације</span><span class="sxs-lookup"><span data-stu-id="cc70b-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="cc70b-276">Из параметара пројекта можете да направите унапред припремљена поља која су само за читање или скривена у апликацији за мобилне уређаје.</span><span class="sxs-lookup"><span data-stu-id="cc70b-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="cc70b-277">Поставите опције у одељку **Мобилни временски распореди** на картици **Временски распоред** на страници **Параметри управљања пројектом и рачуноводством**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![Параметри пројекта](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="cc70b-279">Промена активности које су доступне за избор путем додатака</span><span class="sxs-lookup"><span data-stu-id="cc70b-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="cc70b-280">Активности које су на располагању за одабир за пројекат попуњавају се путем метода **getActivitiesForProject()** и **getActivityQuery()** у класи **TsTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="cc70b-281">Можете да користите ланац команди да бисте ово понашање променили тако да одговара вашем пословном сценарију за активности које су доступне за одабир за одређени пројекат.</span><span class="sxs-lookup"><span data-stu-id="cc70b-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="cc70b-282">Унос подразумеване категорије пројекта у ставке временског распореда</span><span class="sxs-lookup"><span data-stu-id="cc70b-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="cc70b-283">Унос подразумеване категорије пројекта у ставке временског распореда одвија се на три нивоа.</span><span class="sxs-lookup"><span data-stu-id="cc70b-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="cc70b-284">Можете користити ланац команди да проширите понашање на било ком или свим овим нивоима како бисте постигли жељено понашање.</span><span class="sxs-lookup"><span data-stu-id="cc70b-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="cc70b-285">Користи се следећа хијерархија:</span><span class="sxs-lookup"><span data-stu-id="cc70b-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="cc70b-286">Апликација покушава да постави подразумевану категорију из ресурса пројекта.</span><span class="sxs-lookup"><span data-stu-id="cc70b-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="cc70b-287">Ова подразумевана категорија је подешена у методама **getCurrentUserResource** и **getDelegatedResourcesForCurrentUser** у класи **TSTimesheetSettingsService**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="cc70b-288">Ако подразумевана категорија није наведена на нивоу ресурса пројекта, апликација покушава да је повуче из активности пројекта.</span><span class="sxs-lookup"><span data-stu-id="cc70b-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="cc70b-289">Ова подразумевана категорија је постављена у методи **getActivitiesForProject** у класи **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="cc70b-290">Ако подразумевана категорија није наведена на нивоу активности пројекта, подразумевана категорија се преузима из параметара пројекта.</span><span class="sxs-lookup"><span data-stu-id="cc70b-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="cc70b-291">Ова подразумевана категорија се поставља у методи **getProjectDetailsbyRule** у класи **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="cc70b-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>
