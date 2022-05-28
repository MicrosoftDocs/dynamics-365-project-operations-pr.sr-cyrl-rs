---
title: Project Operations интеграција двоструког уписивања
description: Ова тема пружа преглед Project Operations интеграцији двоструког уписивања.
author: sigitac
ms.date: 04/28/2021
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 9b57b8bab9a6821e71a16b191804af21ae5d0b5a
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582774"
---
# <a name="project-operations-dual-write-integration-overview"></a>Преглед Project Operations интеграције двоструког уписивања

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Операције пројекта користе [могућности двоструког писања за](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) синхронизацију података преко Microsoft Dataverse и Дyнамицс 365 Финанце.

Следећа илустрација показује како се подаци синхронизују као део ове интеграције између Dataverse и Finance.

![Преглед Project Operations токова података.](./media/ProjectOperationsFlows.jpg)

Project Operations у Dataverse пружа модеран кориснички интерфејс (UI) и једноставну проширивост без кодирања/са мало кодирања помоћу Power Platform могућности. Менаџери пројеката, менаџери ресурса, чланови пројектног тима и особе које раде са клијентима обављају своје активности у Project Operations у Dataverse.

Project Operations у Finance пружа подршку пројектном рачуноводству и признавању прихода. Project Operations се укључују у финансијски оквир у Finance за обрачун пореза на промет, курсеве валута, извештавање о финансијској димензији и још много тога. Искуства рачуновођа на пројекту углавном се темеље на Finance.

Project Operations интеграција састоји се од следеће интеграције компонената:


- [Project Operations подешавање и интеграција података о конфигурацији](resource-dual-write-setup-integration.md) 
- [Процене и стварне вредности у пројекту](resource-dual-write-estimates-actuals.md)
- [Фактуре пројекта](resource-dual-write-project-invoice.md)
- [Управљање трошковима](resource-dual-write-expense.md)
- [Фактура продавца](resource-dual-write-vendor-invoice.md)
