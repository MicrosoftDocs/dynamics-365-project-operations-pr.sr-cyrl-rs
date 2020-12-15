---
title: Преглед услуге Project Service Automation
description: Ова тема пружа информације о решењу за интеграцију услуге Dynamics 365 Project Service Automation са услугом Dynamics 365 Finance.
author: ruhercul
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d9ccbb29d5035ea061d232011af87cef2c81e76c
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642471"
---
# <a name="project-service-automation-overview"></a>Преглед услуге Project Service Automation

[!include[banner](../includes/banner.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Решење за интеграцију из Project Service Automation у Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Dynamics 365 Finance и Dynamics 365 Project Service Automation преко услуге Common Data Service. Предлошци интеграције који су доступни са функцијом Интеграција података омогућавају ток пројеката, уговоре о пројекту, предмете уговора о пројекту, контролне тачке предмета уговора о пројекту, пројектне задатке, категорије трансакција трошкова, процене сати и процене трошкова из услуге Project Service Automation у Finance.

> [!NOTE]
> - Ако користите верзију 7.3.0, морате инсталирати KB 4074835. Тада ћете моћи да интегришете пројекте са фиксном ценом.
> - Ако користите верзију 7.3.0, а трансакције накнада преносите из услуге Project Service Automation, морате инсталирати KB 4345320 да бисте те накнаде укључили у фактуру пројекта.
> - Ако користите верзију 8.0, моћи ћете да користите интеграцију пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и закључавање функционалности.
> - Ако користите верзију 8.0.1 или новију, моћи ћете да синхронизујете актуелне податке.

Да бисте могли да интегришете Project Service Automation Finance, морате конфигурисати параметре интеграције услуге Project Service Automation. За више информација, погледајте: [Интегрисање параметара услуге Project Service Automation](PSA-parameters.md).

Ово решење за интеграцију омогућава директну синхронизацију у следећим сценаријима:

- Одржавајте уговоре о пројекту у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.
- Креирајте пројекте у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.
- Одржавајте предмете уговора о пројекту у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.
- Одржавајте контролне тачке предмета уговора о пројекту у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.
- Одржавајте пројектне задатке у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.
- Одржавајте категорије трансакција трошкова у услузи Finance и синхронизујте их директно из услуге Finance у Project Service Automation.
- Креирајте процене часова пројекта у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.
- Креирајте процене трошкова пројекта у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.
- Креирајте актуелне податке о времену, трошковима и накнадама у услузи Project Service Automation и креирајте пројектне трансакције у дневнику Project Service Automation интеграције тако да могу бити прокњижени у услузи Finance.

## <a name="data-synchronization"></a>Синхронизација података

Следећа илустрација приказује како се подаци синхронизују као део интеграције између услуга Project Service Automation и Finance.

> [!NOTE]
> Тренутно нису доступни сви предлошци. Предлошци ће бити објављени по завршетку.

[![Интеграција услуге Project Service Automation са услугом Finance](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>Системски захтеви за Finance

Да бисте користили решење за интеграцију услуге Project Service Automation у Finance, морате инсталирати Enterprise Edition 7.3 са исправком платформе 12 или новијом.

## <a name="system-requirements-for-project-service-automation"></a>Системски захтеви за Project Service Automation

Да бисте користили решење за интеграцију услуге Project Service Automation у Finance, морате инсталирати следеће компоненте:

- Dynamics 365 Project Service Automation верзија 9.0.0.0 или новија
- Могуће решење за готовину за Dynamics 365 Sales, верзија 1.14.0.0 (v14) или новија
- Решење Project Service Automation у Finance за Dynamics 365 Project Service Automation верзија 1.0.0.0 или новија

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>Инсталирање решења за интеграцију услуге Project Service Automation у Finance у вашој инстанци услуге Project Service Automation

Преузмите решење за интеграцију Project Service Automation у Finance из [Microsoft центра за преузимање](https://www.microsoft.com/download/details.aspx?id=57016) и следите упутства која сте добили уз решење.
