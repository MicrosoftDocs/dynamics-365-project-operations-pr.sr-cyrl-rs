---
title: Project Operations интеграција двоструког уписивања
description: Ова тема пружа преглед Project Operations интеграцији двоструког уписивања.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ce4f7bf8185e6f3f942df14d30d7b8d0a3e4444a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998699"
---
# <a name="project-operations-dual-write-integration-overview"></a>Преглед Project Operations интеграције двоструког уписивања

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Project Operations користи [могућности двоструког уписивања](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) за синхронизацију података у Microsoft Dataverse и Dynamics 365 Finance.

Следећа илустрација показује како се подаци синхронизују као део ове интеграције између Dataverse и Finance.

![Преглед Project Operations токова података](./media/ProjectOperationsFlows.jpg)

Project Operations у Dataverse пружа модеран кориснички интерфејс (UI) и једноставну проширивост без кодирања/са мало кодирања помоћу Power Platform могућности. Менаџери пројеката, менаџери ресурса, чланови пројектног тима и особе које раде са клијентима обављају своје активности у Project Operations у Dataverse.

Project Operations у Finance пружа подршку пројектном рачуноводству и признавању прихода. Project Operations се укључују у финансијски оквир у Finance за обрачун пореза на промет, курсеве валута, извештавање о финансијској димензији и још много тога. Искуства рачуновођа на пројекту углавном се темеље на Finance.

Project Operations интеграција састоји се од следеће интеграције компонената:


- [Project Operations подешавање и интеграција података о конфигурацији](resource-dual-write-setup-integration.md) 
- [Процене и стварне вредности у пројекту](resource-dual-write-estimates-actuals.md)
- [Фактуре пројекта](resource-dual-write-project-invoice.md)
- [Управљање трошковима](resource-dual-write-expense.md)
- [Фактура продавца](resource-dual-write-vendor-invoice.md)
