---
title: Шта је ново у августу 2022. – Project Operations за сценарије засноване на ресурсима / без залиха
description: Овај чланак пружа информације о квалитетним исправкама које су доступне у издању корпорације Мицрософт Dynamics 365 Project Operations у августу 2022.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 112dbb98de09ef342c03d122a29cb8025058e47f
ms.sourcegitcommit: 6b6c2bfd04e3e613ed1f38355c7cd47c3a56748d
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/24/2022
ms.locfileid: "9348118"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Шта је ново у августу 2022. – Project Operations за сценарије засноване на ресурсима / без залиха

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Овај чланак се односи на следеће компоненте и верзије корпорације Мицрософт Dynamics 365 Project Operations:

- Операције пројекта у верзији Dataverse окружења 4.45.0.53
- Управљање пројектима и рачуноводство у Дyнамицс 365 Финанце окружењу верзија 10.0.28

## <a name="project-operations-dual-write-maps-updates"></a>Ажурирања мапа двоструког уписивања за Project Operations

У овом издању нема исправки за Project Operations мапе двоструког уписивања. За тренутну листу и верзије Project Operations мапа двоструког уписивања, погледајте [Верзије Project Operations мапа двоструког уписивања](../environment/resource-dual-write-maps.md).

Увек покрените најновију верзију мапе у окружењу и омогућите све повезане мапе табела док ажурирате решење за пројектне операције Dataverse и верзију финансијског решења. Неке функције и могућности можда неће исправно функционисати ако најновија верзија мапе није активирана. Активну верзију мапе можете видети у колони **Верзија** на страници **Двоструко уписивање**. Да бисте активирали нову верзију мапе, изаберите **Верзије табеле мапе**, изаберите најновију верзију, а затим сачувајте изабрану верзију. Ако сте прилагодили мапу табеле без оквира, поново примените промене. За још информација погледајте [Управљање животним циклусом апликације](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Ако наиђете на проблем приликом почетка мапе, следите упутства [у проблему са колонама табеле које недостају у одељку мапе](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) водича за решавање проблема са двоструким уписивања.

## <a name="quality-updates"></a>Исправке квалитета

### <a name="project-operations-on-dataverse"></a>Project Operations у услузи Dataverse

| Област функција | Референтни број | Исправка квалитета |
| --- | --- | --- |
| Управљање могућностима за пословање | 2762089. | Руковање грешком током затварања уговора као изгубљено ако је аутоматско чување онемогућено у орг.|

### <a name="project-management-and-accounting-in-finance"></a>Управљање пројектима и рачуноводство у финансијама

За информације о исправкама грешака које су укључене у ову исправку пријавите се Microsoft Dynamics у услуге животног циклуса (ЛЦС) и погледајте чланак у [бази знања](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
