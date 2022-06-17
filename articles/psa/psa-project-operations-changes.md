---
title: Промене функција од апликације Project Service Automation до услуге Project Operations
description: Овај чланак пружа преглед промена функција из аутоматизације услуге пројекта у Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 8a6030faf777051ea1003679589af4bdf97322ab
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925368"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Промене функција од апликације Project Service Automation до услуге Project Operations

Надоградња са Dynamics 365 Project Service Automation на Dynamics 365 Project Operations Лите биће испоручена у три фазе. Овај чланак пружа информације о великим променама које можете очекивати када се надоградња доврши.

| Надоградња испоруке | Фаза 1 <br>(јануар 2022. године) | Фаза 2 <br>(Априлски талас 2022) | Фаза 3  |
|------------------|------------------------|---------------------------|---------------------------|
| Нема зависности од структуре анализе рада (WБС) за пројекте. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WБС је укључен у тренутно подржана ограничења пројектних операција. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| WБС изван тренутно подржаних ограничења пројектних операција, укључујући подршку за клијента радне површине пројекта. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Управљање пројектима

Најзначајније промене у корисничком искуству биће у области планирања пројекта. Пројецт Оператионс усваја ново модерно искуство за управљање структуром анализе рада (WБС) тако што користи могућности [заказивања које обезбеђује Пројекат за Wеб](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Разлике у искуству са планирањем

Следећа табела резимира разлике у планирањеу између аутоматизације пројектних услуга и операција пројекта.

|  Заказивање     |   Project Operations   |   ПСА   |
|-----------------|------------------------|---------|
| Предлошци пројеката - могућност дефинисања и примене предложака пројекта приликом креирања пројекта  |  &nbsp;    | :heavy_check_mark: |
| Интеграција структуре пројектног рада (WБС) са клијентом радне површине   |    &nbsp;  | :heavy_check_mark: |
| Ограничења - Почните не раније него, завршите не касније од  | :heavy_check_mark: |   &nbsp;  |
| Прекретнице - задаци са нултим трајањем   | :heavy_check_mark:  |  &nbsp;  |
| Задаци вођени ресурсима ће поштовати доступност додељених ресурса   | :heavy_check_mark: |  &nbsp;    |
| Уређивање у фази времена - Уређивање планова и рад на дневној бази   |   &nbsp;  | :heavy_check_mark: |
| Аутоматско /ручно планирање - Користите машину за планирање пројекта да бисте аутоматски или ручно испланирали задатке |  &nbsp; | :heavy_check_mark:  |
| Уређивање великих пројеката директно у корисничком интерфејсу: не постоји ограничење величине планова који се могу уређивати  | Ограничење задатка од 500  | :heavy_check_mark:       |
| Проценат довршеног - означи ток задатка   | :heavy_check_mark:  |  &nbsp;  |
| [Режими пројектног](../project-management/scheduling-modes.md) распореда - Дефинисање пројекта као фиксних јединица, фиксни напор или фиксно трајање | :heavy_check_mark: | &nbsp; |
| Временска оса - Направите и прилагодите приказ временске осе да бисте визуелизовали детаље распореда и комуницирали са заинтересованим странама. | :heavy_check_mark:  | &nbsp; |
| Задаци вођени напором - Заказивање подршке мотора за заказивање задатка као напора вођеног  | :heavy_check_mark:  | &nbsp; |
| **Дијалог са информацијама** о задатку - чување детаља задатка помоћу дијалога | :heavy_check_mark:  |  &nbsp;  |
| Превуците и отпустите - задаци са више избора и измените њихов положај у WБС-у | :heavy_check_mark: | &nbsp;  |
| Флексибилни упорни прикази - Дефинисање гранулираних приказа атрибута задатка   | :heavy_check_mark:  | &nbsp; |
| Сортирање и филтрирање WБС-а  | :heavy_check_mark:  | &nbsp; |
| Приказ табли за испоруку пројекта без водопада  | :heavy_check_mark:   | &nbsp; |
| Приказ временске осе - Интерактивни Гантов графикон који се користи за визуелизацију и уређивање WБС-а   | :heavy_check_mark:  | &nbsp; |
| Тастерске пречице - коришћење тастерских пречица за уобичајене операције, као што су увлачење пасуса или уметање  | :heavy_check_mark:  |  &nbsp; |
| Опозив на више нивоа- Изврши анализу "шта-ако" да бисте у потпуности разумели утицај промена тако што ћете сторином и поново применити читав скуп операција | :heavy_check_mark: | &nbsp; |
| Исеци /копирај /налепити - Сарађујте по плану тако што ћете копирати и налепити детаље распореда између апликација  | :heavy_check_mark: | &nbsp; |
| Контролне листе задатака - додавање до 20 ставки контролне листе задатку   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Планирање пројекта

Страница **"Пројекат** " у области "Операције пројекта" има значајан број разлика у поређењу са страницом **"Пројекат"** у области Аутоматизације пројектних услуга.

Следеће радње су уклоњене са странице **"** Пројекти" у склопу надоградње фазе 1:

  - **Отвори у програму MS Project**
  - **Креирај предложак**
  - **Раскини везу са програмом MS Project**

Страница **"Пројекат** " у операцијама пројекта садржи следеће нове картице.

- **Процена материјала**
- **Подешавање наплате за задатак**

Картица **"** Статус" је уклоњена и поље **Статус** се сада налази **на** картици "Резиме" са режимом заказивања пројекта.

   ![Исправке странице пројекта.](media/projectform.png)

Картица **"Распоред** " је преименована у **картицу** "Задатак" и садржи ново искуство планирања пројекта са пројектом за Wеб.

   ![Картица "Нови пројектни задаци".](media/tasktab.png)

## <a name="scheduling-modes"></a>Режими планирања

Операције пројекта су представиле нову функцију, [режиме заказивања](../project-management/scheduling-modes.md). Сви постојећи пројекти аутоматизације пројектних услуга подразумевано ће бити фиксно **трајање у** операцијама пројекта. Међутим, подразумеваним вредностима за нове пројекте може се управљати одласком у режим **распореда** > **параметара "Параметри поставки** > **·** > **"**.

   ![Поставке параметара пројекта за режим "Распоред".](media/projectparameter.png)

## <a name="project-planning-limits"></a>Ограничења планирања пројекта

Операције пројекта се ослања на Пројекат за Wеб за све операције заказивања пројекта. Пројекат за Wеб управља структуром радне анализе користећи ограничења у следећој табели.

| **Поље**                                          | **Ограничење**             |
|----------------------------------------------------|-----------------------|
| Максимални укупни број задатака за пројекат                  | 500                   |
| Максимално укупно трајање за пројекат               | 3650 дана (10 година)  |
| Максимални укупни број ресурса за пројекат              | 300                   |
| Максималан укупни број веза (само наредних) за пројекат | 600                   |
| Максимални укупни број прилагођених поља за пројекат          | 1.0.                    |
| Максимални ниво хијерархије                            | 10 нивоа             |
| Максималан број веза (наредних + претходних)            | 20                    |
| Максимално трајање задатка листа                      | 1250 дана             |
| Максимално трајање задатка резимеа                 | 3650 дана (10 година)  |
| Максималан број ресурса додељених задатку               | 20 ресурса          |
| Подржани опсег датума за задатак                    | 1.1.2000. – 12.31.2149. |
| Ставке листе за проверу                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>Пројектно планирање екстензије и развоја

Након надоградње на операције пројекта, морате користити АПИ-је за планирање пројекта да бисте извршили операције креирања, ажурирања и брисања на следећим ентитетима:

|   Назив ентитета           |   Логичко име ентитета       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Пројектни задатак            | msdyn_projecttask           |
| Зависност пројектног задатка | msdyn_projecttaskdependency |
| Додела ресурса     | msdyn_resourceassignment    |
| Контејнер пројекта          | msdyn_projectbucket         |
| Члан пројектног тима     | msdyn_projectteam           |

Ако тренутно имате прилагођавања која укључују ове ентитете, погледајте чланак Коришћење [АПИ-ја са планом пројекта за извршавање операција са ентитетима за](../project-management/schedule-api-preview.md) планирање за смернице за имплементацију.

## <a name="data-model-changes"></a>Промене модела података

У склопу Фазе надоградње 1, постоје промене у моделу података. Ове промене су пре свега промене поља у постојећим ентитетима. У фази 1, ентитети, **msydn_project** и **msdyn_projectteam** су реакторизација прилагођавања. 

> [!IMPORTANT]
> Овај одељак ће се ажурирати са додатним ентитетима док се будуће фазе надоградње буду довршале.

Следећа поља су замењена новим пољима.

|   Entity          |   Старо логично име   |   Ново логичко име    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

Додата су следећа поља.

|   Entity          |   Логичко име                               |   Опис |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | Приказује збир стварне продаје накнада на пројекту. Само за коришћење у функцији Пројецт Сервице Аутоматион. |
| msdyn_project     | msdyn_actualmaterialcost                     | Приказује збир стварних трошкова материјала на пројекту. Само за коришћење у функцији Пројецт Сервице Аутоматион. |
| msdyn_project     | msdyn_actualmaterialsales                    | Приказује збир стварне продаје материјала на пројекту. Само за коришћење у функцији Пројецт Сервице Аутоматион. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Ред уговора повезан са овим пројектом. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Ово је интерно системско поље које се користи за копирање **пројекта** повезаног са идентификатором корелације. Само за коришћење у функцији Пројецт Сервице Аутоматион. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Ово је интерно системско поље које се користи за **копирање** пројекта повезаног са идентификатором сесије. Само за коришћење у функцији Пројецт Сервице Аутоматион. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Последња синхронизација XРМ глобалног симбола ревизије из услуге пројектовања. |
| msdyn_project     | msdyn_msprojectdocument                      | Мицрософт Пројецт документ који припада пројекту. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Збир планираних трошкова материјала на пројекту. Само за коришћење у функцији Пројецт Сервице Аутоматион. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Агрегат планиране продаје материјала на пројекту. Само за коришћење у функцији Пројецт Сервице Аутоматион. |
| msdyn_project     | msdyn_program                                | Програм са којим је овај пројекат повезан. |
| msdyn_project     | msdyn_quotelineproject                       | Ред понуде повезан са овим пројектом. |
| msdyn_project     | msdyn_replaylogheader                        | Заглавље евиденција поновне репродукције. |
| msdyn_project     | msdyn_schedulemode                           | Подразумевани режим заказивања који се користи за све задатке на пројекту.  |
| msdyn_project     | msdyn_taskearlieststart                      | Најранији датум почетка било ког задатка у пројекту.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Члан пројектног тима из којег је копиран овај члан пројектног тима. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | Означава да ли треба креирати захтев ресурса за новокреираног генеричког члана тима.  |
| msdyn_projectteam | msdyn_deletestatus                           | Статус брисања члана тима за праћење да ли постоји захтев за брисање послат услузи "Планирање пројекта" и да ли успешно шаље одговор у очекиваном временском прозору. |
| msdyn_projectteam | msdyn_effortcompleted                        | Прати напоре које је члан тима постигао на својим задацима. |
| msdyn_projectteam | msdyn_effortremaining                        | Прати напоре које тек треба да заврши члан тима на својим задацима. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Период чекања од времена када члан тима шаље захтев за брисање услузи за планирање пројекта док члан тима заиста не буде избрисан на Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Време које треба записати када члан тима избрише захтев за брисање шаље се услузи за планирање пројекта. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Показује члана пројектног тима са којег је копиран овај члан пројектног тима.  |

## <a name="project-templates"></a>Предлошци пројеката

Операције пројекта не пружају подршку предлошцима пројеката. Међутим, већи део основне функционалности можете да копирате коришћењем АПИ-ја [за копирање пројекта](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Подршка за програмски додатак на радној површини

Подршка за програмски додатак Мицрософт Пројецт Десктоп неће бити доступна у прве 2 фазе надоградње. У фази 3, клијенти који имају пројекте веће од тренутно подржаних ограничења пројекта за Wеб моћи ће да користе програмски додатак на радној површини.

## <a name="editing-resource-assignment-contours"></a>Уређивање контура додељивање ресурса

Могућност уређивања контура додељивања ресурса биће доступна када фаза 2 надоградње буде доступна.

## <a name="billing-and-pricing"></a>Наплата и одређивање цена

Следеће нове функције су додате у операције пројекта. Ове функције су адитив у природи и не утичу на модел података за аутоматизацију услуге пројекта.

- [Снимање коришћења материјала на пројектима и пројектне задатке](../material/material-usage-log.md)
- [Управљање подизвођачима](../pro/subcontracting/managing-subcontracts-overview.md)
- [Аванси и уговори засновани на авансним уплатама](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Статус и провере ваљаности уговора који се не премашују](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Наплата заснована на задатку](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Неодобрене компоненте

Следеће табеле документују сва неодобрена поља која су премештена у решење за застареле компоненте након надоградње. Више информација и везу ка решењу потражите у чланку [Dynamics 365 Project Service Automation 3x са операцијама пројекта 4x неодобреним компонентама](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>инвоицедетаил

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinescheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_cenovnik                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduleddurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_agregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocomplete                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicantsavailable                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinescheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_name                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>салесордердетаил

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

