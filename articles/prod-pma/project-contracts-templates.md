---
title: Синхронизовање пројектних уговора и пројеката директно из услуге Project Service Automation са услугом Finance
description: Ова тема описује предложак и основне задатке који се користе за синхронизацију уговора о пројекту и пројекта директно из услуге Microsoft Dynamics 365 Project Service Automation у Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 12/17/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 1a470fd86ceccd7b6058da6972399a6d6be2a991
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764837"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance"></a>Синхронизовање пројектних уговора и пројеката директно из услуге Project Service Automation са услугом Finance 

[!include[banner](../includes/banner.md)]

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Ова тема описује предложак и основне задатке који се користе за синхронизацију уговора о пројекту и пројекта директно из услуге Dynamics 365 Project Service Automation у Dynamics 365 Finance.

> [!NOTE] 
> Ако користите Enterprise Edition 7.3.0, морате инсталирати KB 4074835.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Ток података из услуге Project Service Automation у Finance

> [!NOTE]
> Пре него што будете могли да користите решење за интеграцију услуге Project Service Automation са услугом Finance, требало би да сте упознати са функцијом интеграције података у систему Dynamics 365.

Решење за интеграцију из услуге Project Service Automation у Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Project Service Automation и Finance. Предложак интеграције који је доступан са функцијом Интеграција података омогућава ток података о уговорима за пројекте, пројекте, предмете уговора о пројекту и контролне тачке предмета уговора о пројекту из услуге Project Service Automation у Finance.

Следећа илустрација приказује како се подаци синхронизују између услуга Project Service Automation и Finance.

[![Ток података за интеграцију услуге Project Service Automation са услугом Finance](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)

## <a name="templates-and-tasks"></a>Предлошци и задаци

Да бисте приступили доступним предлошцима, у Microsoft Power Apps центру администрације изаберите **Пројекти**, а затим у горњем десном углу изаберите **Нови пројекат** за избор јавних предложака.

Следећи предлошци и основни задаци који се користе за синхронизацију уговора о пројекту и пројеката из услуге Project Service Automation у Finance:

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a>Интегрисање са услугом Dynamics 365 Project Service Automation верзије 2.x
- **Назив предлошка у интеграцији података:** Пројекти и уговори (Project Service Automation у Finance)
- **Назив задатака у пројекту:**

    - Уговори за пројекат: Project Service Automation у Finance
    - Пројекти: Project Service Automation у Finance
    - Предмети уговора за пројекат: Project Service Automation у Finance
    - Контролне тачке предмета уговора за пројекат: Project Service Automation у Finance
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a>Интегрисање са услугом Dynamics 365 Project Service Automation верзије 3.x
Дошло је до промене шеме у услузи Project Service Automation која утиче на предложак контролне тачке предмета уговора о пројекту, а за интеграцију услуге Project Service Automation верзије 3.x са системом Dynamics 365 потребно је да користите предложак верзије 2.

- **Назив предлошка у интеграцији података:** Пројекти и уговори (Project Service Automation 3.x у Finance), v2
- **Назив задатака у пројекту:**

    - Уговори за пројекат: Project Service Automation у Finance
    - Пројекти: Project Service Automation у Finance
    - Предмети уговора за пројекат: Project Service Automation у Finance
    - Контролне тачке предмета уговора за пројекат: Project Service Automation у Finance

Да би могло да дође до синхронизације уговора о пројекту и пројеката, морате синхронизовати налоге.

## <a name="entity-set"></a>Скуп ентитета

| Project Service Automation       | Finance                                                |
|----------------------------------|--------------------------------------------------------|
| Поруџбине                           | Ентитет интеграције за уговор о пројекту                |
| Пројекти                         | Ентитет интеграције за пројекат                         |
| Ставке поруџбине                      | Ентитет интеграције за предмет уговора о пројекту           |
| Контролне тачке предмета уговора о пројекту | Ентитет интеграције за контролну тачку предмета уговора о пројекту |

## <a name="entity-flow"></a>Ток ентитета

Уговорима о пројекту се управља у услузи Project Service Automation и они се синхронизују са услугом Finance као уговори о пројекту. Као део предлошка за интеграцију, можете да поставите извор интеграције у услузи Finance за уговор о пројекту.

Временом и материјалом и пројектима са фиксном ценом управља се у услузи Project Service Automation и синхронизују са услугом Finance као пројекти. Као део интеграције предлошка, можете да подесите извор интеграције за пројекат у услузи Finance. Тренутно су подржани само време, материјал и пројекти са фиксном ценом.


Предметима уговора о пројекту се управља у услузи Project Service Automation и они се синхронизују са услугом Finance као правилима наплате по уговору о пројекту. Ако се начин наплате разликује од подразумеваног типа пројекта, синхронизација ажурира тип пројекта за пројекат предмета уговора и групу пројеката.

Контролним тачкама предмета уговора о пројекту се управља у услузи Project Service Automation и они се синхронизују са услугом Finance као контролне тачке правила наплате по уговору о пројекту.

## <a name="project-service-automation-to-finance-integration-solution"></a>Решење за интеграцију услуге Project Service Automation са услугом Finance

Поље **ИД уговора о пројекту** је доступно на страници **Уговори о пројекту**. Ово поље је учињено природним и јединственим кључем за подршку интеграцији.

Када се креира нови уговор о пројекту, ако вредност **ID уговора о пројекту** већ не постоји, она се аутоматски генерише помоћу низа бројева. Вредност се састоји од речи **ORD** праћене растућим низом бројева, а затим суфиксом од шест знакова. Ево примера: **ORD-01022-Z4M9Q0**.

Поље **Број пројекта** је доступно на страници **Пројекти**. Ово поље је учињено природним и јединственим кључем за подршку интеграцији.

Када се креира нови пројекат, ако вредност **Број пројекта** већ не постоји, она се аутоматски генерише помоћу низа бројева. Вредност се састоји од речи **PRJ** праћене растућим низом бројева, а затим суфиксом од шест знакова. Ево примера: **PRJ-01049-CCNID0**.

Када се примени решење интеграције услуге Project Service Automation са Finance, скрипта за надоградњу поставља поље **ID уговора о пројекту** за постојеће уговоре о пројекту и поље **Број пројекта** за постојеће пројекте у услузи Project Service Automation.

## <a name="prerequisites-and-mapping-setup"></a>Предуслови и подешавање мапирања

- Да би могло да дође до синхронизације уговора о пројекту и пројеката, морате синхронизовати налоге.
- У свом скупу веза додајте мапирање поља кључа за интеграцију за **msdyn\_organizationalunits** у **msdyn\_name \[Name\]**. Можда ћете прво морати да додате пројекат у скуп веза. За више информација, погледајте [Интегрисање података у Common Data Service за апликације](https://docs.microsoft.com/powerapps/administrator/data-integrator).
- У свом скупу веза, додајте мапирање поља кључа за интеграцију за **msdyn\_projects** у **msdynce\_projectnumber \[Project Number\]**. Можда ћете прво морати да додате пројекат у скуп веза. За више информација, погледајте [Интегрисање података у Common Data Service за апликације](https://docs.microsoft.com/powerapps/administrator/data-integrator).
- **SourceDataID** за уговоре о пројекту и пројекте могу се ажурирати на другу вредност или уклонити из мапирања. Подразумевана вредност предлошка је **Project Service Automation**.
- Мапирање **Услови плаћања** се мора ажурирати тако да одражава важеће услове плаћања у услузи Finance. Такође можете да уклоните мапирање из пројектног задатка. Мапа подразумеваних вредности има подразумеване вредности за демо податке. Следећа табела приказује вредности у услузи Project Service Automation.

    | Вредност | Опис   |
    |-------|---------------|
    | 1     | Нето 30        |
    | 2     | 2% 10, нето 30 |
    | 3     | Нето 45        |
    | 4     | Нето 60        |

## <a name="power-query"></a>Power Query

Користите Microsoft Power Query for Excel за филтрирање података ако су испуњени следећи услови:

- Имате улазне поруџбине у услузи Dynamics 365 Sales.
- Имате више организационих јединица у услузи Project Service Automation и те организационе јединице биће мапиране у више правних лица у услузи Finance.

Ако морате да користите Power Query, следите ове смернице:

- Предложак Пројекти и уговори (из PSA у Fin and Ops) има подразумевани филтер који укључује само улазне поруџбине типа **Радни предмет (msdyn\_ordertype = 192350001)**. Овај филтер вам гарантује да се уговори о пројекту неће креирати за улазне поруџбине у услузи Finance. Ако креирате сопствени образац, морате додати овај филтер.
- Направите Power Query филтер који укључује само уговорне организације које треба синхронизовати са правним лицем скупа интеграционих веза. На пример, уговори о пројекту које имате са уговорном организационом јединицом Contoso US треба да се синхронизују са правним лицем USSI, али уговори о пројекту које имате са уговорном организационом јединицом Contoso Global треба да се синхронизују са правним лицем USMF. Ако не додате овај филтер у мапирање задатака, сви уговори о пројекту биће синхронизовани са правним лицем које је дефинисано за скуп веза, без обзира на организациону јединицу уговора.

## <a name="template-mapping-in-data-integration"></a>Мапирање предложака у услузи Data Integration

> [!NOTE] 
> Поља **CustomerReference**, **AddressCity**, **AddressCountryRegionID**, **AddressDescription**, **AddressLine1**, **AddressLine2**, **AddressState** и **AddressZipCode** нису укључена у подразумевано мапирање за уговоре о пројекту. Мапирања можете додати ако желите да се ови подаци синхронизују за уговоре о пројекту.
>
> Поља **Description**, **ParentID**, **ProjectGroup**, **ProjectManagerPersonnelNumber** и **ProjectType** нису укључена у подразумевано мапирање за пројекте. Мапирања можете додати ако желите да се ови подаци синхронизују за пројекте.

Следеће илустрације приказују примере мапирања задатака предлошка у услузи Data Integration. Мапирање приказује информације о терену које ће се синхронизовати из услуге Project Service Automation у Finance.

[![Мапирање предлошка пројектног уговора](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)

[![Мапирање предлошка пројекта](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)

[![Мапирање предлошка предмета уговора](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)

[![Мапирање предлошка контролне тачке предмета уговора](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a>Мапирање контролних тачака предмета уговора о пројекту у пројектима и уговорима (из PSA 3.x у Dynamics) – предложак верзије 2:

[![Мапирање контролне тачке предмета уговора са предлошком верзије два](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]