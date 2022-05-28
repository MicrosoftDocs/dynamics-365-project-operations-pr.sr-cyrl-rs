---
title: Синхронизуј пројектне задатке директно из аутоматизације пројектних услуга у финансије и операције
description: Овај тема описује предложак и основни задатак који се користи за синхронизацију пројектног задатка директно из Microsoft Dynamics 365 Project Service Automation Дyнамицс 365 Финанце.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 666e0d757969b32f16e08128d9f78a2ffe1e8357
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/04/2022
ms.locfileid: "8683328"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>Синхронизуј пројектне задатке директно из аутоматизације пројектних услуга у финансије и операције

[!include[banner](../includes/banner.md)]

Овај тема описује предложак и основни задатак који се користи за синхронизацију пројектног задатка директно из Dynamics 365 Project Service Automation Дyнамицс 365 Финанце.

> [!NOTE]
> - Интеграција пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и закључавање функционалности доступни су у верзији 8.0.
> - Ако користите Enterprise Edition 7.3.0, када инсталирате KB 4132657 и KB 4132660, моћи ћете да користите предлошке за интегрисање пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и стварних података, као и да конфигуришите закључавање функционалности. Ако морате да ресетујете рачуноводствене дистрибуције, препоручили смо да инсталирате и KB 4131710.
> - Интеграција стварних података доступна је у верзији 8.0.1 или новијој.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Ток података из услуге Project Service Automation у Finance

Решење за интеграцију из услуге Project Service Automation у Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Project Service Automation и Finance. Предложак за интеграцију који је доступан са функцијом Интеграција података омогућава ток података о пројектним задацима из услуге Project Service Automation у Finance.

Следећа илустрација приказује како се подаци синхронизују између услуга Project Service Automation и Finance.

[![Ток података за интеграцију услуге Project Service Automation са услугом Finance.](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>Предложак и задатак

Да бисте приступили предлошку, у Microsoft Power Apps центру администрације изаберите **Пројекти**, а затим у горњем десном углу изаберите **Нови пројекат** за одабир јавних образаца.

Следећи предложак и основни задатак који се користе за синхронизацију пројектних задатака из услуге Project Service Automation у Finance:

- **Назив предлошка у Интеграцији података:** Пројектни задаци (из PSA у Fin and Ops)
- **Назив задатка у пројекту:** Пројектни задаци

Да би могло да дође до синхронизације пројектних задатака, морате синхронизовати уговоре о пројекту и пројекте.

## <a name="entity-set"></a>Скуп ентитета

| Project Service Automation | Finance                             |
|----------------------------|-------------------------------------|
| Пројектни задаци              | Ентитет интеграције за пројектни задатак |

## <a name="entity-flow"></a>Ток ентитета

Пројектним задацима се управља у услузи Project Service Automation и они се синхронизују са услугом Finance као активности пројекта.

## <a name="prerequisites-and-mapping-setup"></a>Предуслови и подешавање мапирања

Да би могло да дође до синхронизације пројектних задатака, морате синхронизовати уговоре о пројекту и пројекте.

## <a name="power-query"></a>Power Query

Мицрософт за Еxцел морате да Power Query користите за филтрирање података ако је овај услов испуњен:

- У пројектном задатку имате записе специфичне за ресурсе.

Ако морате да користите Power Query, следите ово упутство:

- Предложак пројектних задатака (из PSA у Fin and Ops) има подразумевани филтер који из пројектног задатка искључује записе специфичне за ресурсе постављањем филтера на **IsLineTask** на **Нетачно**. Ако креирате сопствени образац, морате додати овај филтер.

## <a name="template-mapping-in-data-integration"></a>Мапирање предложака у услузи Data Integration

Следећа илустрација приказује пример мапирања задатака предлошка у интеграцији података. Мапирање приказује информације о терену које ће се синхронизовати из услуге Project Service Automation у Finance.

[![Мапирање предложака.](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]