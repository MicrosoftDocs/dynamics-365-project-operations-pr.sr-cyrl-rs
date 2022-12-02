---
title: Шта је ново у мају 2022. – Project Operations за сценарије засноване на ресурсима / без залиха
description: Овај чланак пружа информације о исправкама квалитета које су доступне у издању услуге Microsoft Dynamics 365 Project Operations за мај 2022. за сценарије засноване на ресурсима/без залиха.
author: sigitac
ms.date: 05/02/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: beb75fc4b721d52cddbdaf2d20194218cefced5e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921412"
---
# <a name="whats-new-may-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Шта је ново у мају 2022. – Project Operations за сценарије засноване на ресурсима / без залиха

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Овај чланак се односи на следеће компоненте и верзије услуге Microsoft Dynamics 365 Project Operations:

- Project Operations у Dataverse окружењу верзије 4.42.0.70
- Управљање пројектима и рачуноводство у Dynamics 365 Finance окружењу верзије 10.0.26

## <a name="project-operations-dual-write-maps-updates"></a>Ажурирања мапа двоструког уписивања за Project Operations

У овом издању нема исправки за Project Operations мапе двоструког уписивања. За тренутну листу и верзије Project Operations мапа двоструког уписивања, погледајте [Верзије Project Operations мапа двоструког уписивања](../environment/resource-dual-write-maps.md).

Увек покрените најновију верзију мапе у свом окружењу и омогућите све повезане мапе табела док ажурирате своје Project Operations Dataverse решење и верзија решења услуге Finance. Неке функције и могућности можда неће радити исправно ако се не активира најновија верзија мапе. Активну верзију мапе можете видети у колони **Верзија** на страници **Двоструко уписивање**. Да бисте активирали нову верзију мапе, изаберите **Верзије табеле мапе**, изаберите најновију верзију, а затим сачувајте изабрану верзију. Ако сте прилагодили мапу табеле која је готова, поново примените. За још информација погледајте [Управљање животним циклусом апликације](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Ако наиђете на проблем када покренете мапу, следите упутства у одељку [Недостаје издање колона табеле на мапама](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) водича за решавање проблема са двоструким уписивањем.

## <a name="quality-updates"></a>Исправке квалитета
### <a name="project-operations-on-dataverse"></a>Project Operations у услузи Dataverse

| Област функција | Референтни број | Исправка квалитета |
| --- | --- | --- |
| Управљање ресурсима | 2634019. | Побољшане поруке о грешкама за пословне провере ваљаности приликом додавања генеричких чланова тима као ресурса. |
| Планирање и праћење пројекта | 2648515. | Ограничене исправке за **ownerid**, **стање** и **статус** у ентитетима планирања. |
| Наплата и одређивање цена | 2653167. | Знак за раздвајање децимала матрице координатне мреже **Процене** мора да прати поставке формата у **Личним опцијама**. |
| Наплата и одређивање цена| 2662251. | Вредности у пољима **Коригована јединица** и **Група јединица** постају подразумеване приликом креирања записа у проценама материјала. |
| Наплата и одређивање цена| 2571408. | Ненаплаћене стварне вредности продаје добијају ID-а профактуре приликом креирања радне верзије фактуре. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Управљање пројектима и рачуноводство у решењу Dynamics 365 Finance

За информације о исправкама грешака које су укључене у ову исправку, пријавите се на Microsoft Dynamics Lifecycle Services (LCS) и погледајте [чланак у бази знања](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864).
