---
title: Промене функција од апликације Project Service Automation до услуге Project Operations
description: Овај чланак пружа преглед промена функција из услуге Project Service Automation у Dynamics 365 Project Operations.
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
ms.openlocfilehash: a9c69fc4296d30763f3994a4955e64ab258ceb4f
ms.sourcegitcommit: 675e9f3615e701c5f998de3a5ea3e25df11ae107
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/09/2022
ms.locfileid: "9459945"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Промене функција од апликације Project Service Automation до услуге Project Operations

Надоградња са услуге Dynamics 365 Project Service Automation на Dynamics 365 Project Operations једноставну примену биће испоручена у три фазе. Овај чланак пружа информације о великим променама које можете очекивати када се надоградња доврши.

| Испорука надоградње | Фаза 1 <br>(јануар 2022.) | Фаза 2 <br>(новембар 2022.) | Фаза 3  |
|------------------|------------------------|---------------------------|---------------------------|
| Нема зависности на структурној анализи посла (САП) за пројекте. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| САП је укључен у тренутно подржана ограничења за Project Operations. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| САП изван тренутно подржаних ограничења за Project Operations, укључујући подршку за Project Desktop Client. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Управљање пројектима

Најзначајније промене у корисничком искуству биће у области планирања пројекта. Project Operations усваја ново модерно искуство за управљање структурном анализом посла (САП) тако што користи могућности заказивања које пружа [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Разлике у искуству заказивања

Следећа табела резимира разлике у заказивању између услуга Project Service Automation и Project Operations.

|  Заказивање     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Предлошци пројеката – могућност дефинисања и примене предложака пројекта приликом креирања пројекта  |  &nbsp;    | :heavy_check_mark: |
| Интеграција структурне анализе посла (САП) са клијентом за рачунаре   |    &nbsp;  | :heavy_check_mark: |
| Ограничења – немојте почети пре, немојте завршити након  | :heavy_check_mark: |   &nbsp;  |
| Контролне тачке – задаци са нултим трајањем   | :heavy_check_mark:  |  &nbsp;  |
| Задаци засновани на ресурсима поштоваће доступност додељених ресурса   | :heavy_check_mark: |  &nbsp;    |
| Временско уређивање – уређујте планове и радите на дневној основи   |   &nbsp;  | :heavy_check_mark: |
| Аутоматско/ручно заказивање – користите механизам за заказивање пројекта да бисте аутоматски или ручно заказали задатке |  &nbsp; | :heavy_check_mark:  |
| Уређивање великих пројеката директно у корисничком интерфејсу: не постоји ограничење по питању величине планова који се могу уређивати  | Ограничење од 500 задатака  | :heavy_check_mark:       |
| Проценат довршеног – означите ток задатка   | :heavy_check_mark:  |  &nbsp;  |
| [Режими распореда пројекта](../project-management/scheduling-modes.md) – дефинишите пројекат као фиксне јединице, фиксно ангажовање или фиксно трајање | :heavy_check_mark: | &nbsp; |
| Временска оса – направите и прилагодите приказ временске осе да бисте визуелизовали детаље распореда и комуницирали са заинтересованим странама. | :heavy_check_mark:  | &nbsp; |
| Задаци засновани на ангажовању – подршке механизма за заказивање за заказивања задатка као заснованог на ангажовању  | :heavy_check_mark:  | &nbsp; |
| Дијалог **Информације о задатку** – чувајте детаље о задатку користећи дијалог | :heavy_check_mark:  |  &nbsp;  |
| Превуците и отпустите – изаберите више задатака и измените њихове положају у САП-у | :heavy_check_mark: | &nbsp;  |
| Флексибилни трајни прикази – дефинишите детаљније приказе атрибута задатка   | :heavy_check_mark:  | &nbsp; |
| Сортирање и филтрирање САП-а  | :heavy_check_mark:  | &nbsp; |
| Приказ табли за испоруку пројекта без „водопада“  | :heavy_check_mark:   | &nbsp; |
| Приказ временске осе – интерактивни Гантов графикон који се користи за визуелизацију и уређивање САП-а   | :heavy_check_mark:  | &nbsp; |
| Тастерске пречице – користите тастерске пречице за уобичајене операције, као што су увлачење пасуса или уметање  | :heavy_check_mark:  |  &nbsp; |
| Опозив у више нивоа – обавите „шта-ако“ анализу да бисте у потпуности разумели утицај промена тако што ћете сторнирати и поново применити читав скуп операција | :heavy_check_mark: | &nbsp; |
| Исеците/Копирајте/Налепите – сарађујте на развоју распореда копирањем и лепљењем детаља о распореду између апликација  | :heavy_check_mark: | &nbsp; |
| Контролне листе задатака – додајте до 20 ставки контролне листе задатку   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Планирање пројекта

Страница **Пројекат** у услузи Project Operations има значајан број разлика у поређењу са страницом **Пројекат** у услузи Project Service Automation.

Следеће радње су уклоњене са странице **Пројекти** у склопу надоградње фазе 1:

  - **Отвори у програму MS Project**
  - **Креирај предложак**
  - **Раскини везу са програмом MS Project**

Страница **Пројекат** у услузи Project Operations садржи следеће нове картице.

- **Процена материјала**
- **Подешавање наплате за задатак**

Картица **Статус** је уклоњена и поље **Статус** се сада налази на картици **Резиме** са режимом заказивања пројекта.

   ![Ажурирања странице „Пројекат“.](media/projectform.png)

Картица **Распоред** је преименована у картицу **Задатак** и садржи ново искуство планирања пројекта са услугом Project for the Web.

   ![Нова картица задатака пројекта.](media/tasktab.png)

## <a name="scheduling-modes"></a>Режими планирања

Project Operations је увео нову функцију, [Режими заказивања](../project-management/scheduling-modes.md). Сви постојећи Project Service Automation пројекти подразумевано ће имати **Фиксно трајање** у услузи Project Operations. Међутим, подразумеваним вредностима за нове пројекте можете управљати одласком у **Поставке** > **Параметри** > **Параметар** > **Режим распореда**.

   ![Поставке параметара пројекта за режим распореда.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Ограничења у планирању пројекта

Project Operations се ослања на Project for the Web за све операције планирања пројекта. Project for the Web управља структурном анализом посла користећи ограничења у следећој табели.

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

## <a name="project-planning-extensibility-and-development"></a>Могућност проширења и развоја планирања пројекта

Након надоградње на Project Operations, морате користити API-је за планирање пројекта да бисте извршили операције креирања, ажурирања и брисања на следећим ентитетима:

|   Назив ентитета           |   Логичко име ентитета       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Пројектни задатак            | msdyn_projecttask           |
| Зависност пројектног задатка | msdyn_projecttaskdependency |
| Додела ресурса     | msdyn_resourceassignment    |
| Контејнер пројекта          | msdyn_projectbucket         |
| Члан пројектног тима     | msdyn_projectteam           |

Ако тренутно имате прилагођавања која обухватају ове ентитете, погледајте чланак [Коришћење API-ја за планирање пројекта за обављање операција са ентитетима планирања](../project-management/schedule-api-preview.md) где ћете пронаћи смернице за примену.

## <a name="data-model-changes"></a>Промене у моделу података

У склопу фазе 1 надоградње, постоје промене у моделу података. Ове промене су пре свега промене поља у постојећим ентитетима. У фази 1, ентитети **msydn_project** и **msdyn_projectteam** су рефакторизација прилагођавања. 

> [!IMPORTANT]
> Овај одељак ће се ажурирати са додатним ентитетима док се будуће фазе надоградње буду довршавале.

Следећа поља су замењена новим пољима.

|   Entity          |   Старо логичко име   |   Ново логичко име    |
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
| msdyn_project     | msdyn_actualfeesales                         | Приказује агрегирани износ стварне накнаде продаје у пројекту. За коришћење само у услузи Project Service Automation. |
| msdyn_project     | msdyn_actualmaterialcost                     | Приказује агрегиране стварне материјалне трошкове у пројекту. За коришћење само у услузи Project Service Automation. |
| msdyn_project     | msdyn_actualmaterialsales                    | Приказује агрегирани износ стварне продаје материјала у пројекту. За коришћење само у услузи Project Service Automation. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Предмет уговора повезан са овим пројектом. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Ово је интерно системско поље које се користи за **копирање пројекта** повезаног са идентификатором корелације. За коришћење само у услузи Project Service Automation. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Ово је интерно системско поље које се користи за **копирање пројекта** повезаног са идентификатором сесије. За коришћење само у услузи Project Service Automation. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Последња синхронизација xRM токена за глобалну ревизију из услуге планирања пројекта. |
| msdyn_project     | msdyn_msprojectdocument                      | Microsoft Project документ који припада пројекту. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Збир планираних материјалних трошкова у пројекту. За коришћење само у услузи Project Service Automation. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Збир планиране продаје материјала у пројекту. За коришћење само у услузи Project Service Automation. |
| msdyn_project     | msdyn_program                                | Програм са којим је овај пројекат повезан. |
| msdyn_project     | msdyn_quotelineproject                       | Ставка понуде повезана са овим пројектом. |
| msdyn_project     | msdyn_replaylogheader                        | Заглавље за поновну репродукцију евиденције. |
| msdyn_project     | msdyn_schedulemode                           | Подразумевани режим распореда који се користи за све задатке у пројекту.  |
| msdyn_project     | msdyn_taskearlieststart                      | Најранији датум почетка било ког задатка у пројекту.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Члан пројектног тима са којег је копиран овај члан пројектног тима. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | Означава да ли треба да се креира захтев за ресурс за недавно креираног генеричког члана тима.  |
| msdyn_projectteam | msdyn_deletestatus                           | Статус брисања члана тима за праћење да ли се услузи планирања пројекта шаље захтев за брисање и да ли она успешно враћа одговор и у очекиваном временском року. |
| msdyn_projectteam | msdyn_effortcompleted                        | Прати ангажовање које је члан тима довршио за своје доделе. |
| msdyn_projectteam | msdyn_effortremaining                        | Прати ангажовање које члан тима треба да заврши за своје доделе. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Период чекања од времена када члан тима шаље захтев за брисање услузи планирања пројекта док члан тима заиста не буде избрисан у услузи Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Временска ознака за евидентирање када се захтев за брисање члана тима пошаље у услугу планирања пројекта. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Показује члана пројектног тима са којег је копиран овај члан пројектног тима.  |

## <a name="project-templates"></a>Предлошци пројеката

Project Operations не обезбеђује подршку за шаблоне пројекта. Међутим, већи део основне функционалности можете да реплицирате коришћењем [Project Copy API-ја](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Подршка за програмски додатак за рачунаре

Подршка за Microsoft Project програмски додатак за рачунаре неће бити доступна током прве 2 фазе надоградње. У фази 3, клијенти који имају пројекте веће од тренутно подржаних ограничења услуге Project for the Web моћи ће да користе програмски додатак за рачунаре.

## <a name="editing-resource-assignment-contours"></a>Уређивање контура додељивања ресурса

Могућност уређивања контура доделе ресурса биће доступна када фаза 2 надоградње буде доступна.

## <a name="billing-and-pricing"></a>Наплата и одређивање цена

Следеће нове функције су додате у услузи Project Operations. Ове функције су по природи додатне и не утичу на Project Service Automation модел података.

- [Евидентирање коришћења материјала на пројектима и пројектним задацима](../material/material-usage-log.md)
- [Управљање подуговорима](../pro/subcontracting/managing-subcontracts-overview.md)
- [Аванси и уговори засновани на авансним уплатама](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Статусом и провере уговора које не смете премашити](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Наплата заснована на задатку](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Застареле компоненте

Следеће табеле документују сва застарела поља која су премештена у решење са застарелим компонентама након надоградње. Више информација и везу ка решењу потражите у чланку [Dynamics 365 Project Service Automation 3x у Project Operations 4x застареле компоненте](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>invoicedetail

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
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
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
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
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

### <a name="salesorderdetail"></a>salesorderdetail

| Поља                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

