---
title: Project Operations интеграција двоструког уписивања
description: Овај чланак пружа преглед Project Operations интеграцији двоструког уписивања.
author: sigitac
ms.date: 04/28/2021
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d365a036f96ff4f7b14107b43e8c6b70df0b5362
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927990"
---
# <a name="project-operations-dual-write-integration-overview"></a>Преглед Project Operations интеграције двоструког уписивања

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Project Operations користи [могућности двоструког уписивања](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) за синхронизацију података у решењу Microsoft Dataverse и Dynamics 365 Finance.

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
