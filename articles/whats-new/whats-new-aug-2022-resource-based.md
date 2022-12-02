---
title: Шта је ново у августу 2022. – Project Operations за сценарије засноване на ресурсима / без залиха
description: Овај чланак пружа информације о исправкама квалитета које су доступне у издању услуге Microsoft Dynamics 365 Project Operations за август 2022. за сценарије засноване на ресурсима/без залиха.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 4042dca72a33f48e04e51af2a3cfd2da83146afd
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/02/2022
ms.locfileid: "9403875"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Шта је ново у августу 2022. – Project Operations за сценарије засноване на ресурсима / без залиха

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Овај чланак се односи на следеће компоненте и верзије услуге Microsoft Dynamics 365 Project Operations:

- Project Operations у Dataverse окружењу верзије 4.45.0.53
- Управљање пројектима и рачуноводство у Dynamics 365 Finance окружењу верзије 10.0.28

## <a name="project-operations-dual-write-maps-updates"></a>Ажурирања мапа двоструког уписивања за Project Operations

У овом издању нема исправки за Project Operations мапе двоструког уписивања. За тренутну листу и верзије Project Operations мапа двоструког уписивања, погледајте [Верзије Project Operations мапа двоструког уписивања](../environment/resource-dual-write-maps.md).

Увек покрените најновију верзију мапе у свом окружењу и омогућите све повезане мапе табела док ажурирате своје Project Operations Dataverse решење и верзија решења услуге Finance. Неке функције и могућности можда неће радити исправно ако се не активира најновија верзија мапе. Активну верзију мапе можете видети у колони **Верзија** на страници **Двоструко уписивање**. Да бисте активирали нову верзију мапе, изаберите **Верзије табеле мапе**, изаберите најновију верзију, а затим сачувајте изабрану верзију. Ако сте прилагодили мапу табеле која је готова, поново примените. За још информација погледајте [Управљање животним циклусом апликације](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Ако наиђете на проблем када покренете мапу, следите упутства у одељку [Недостаје издање колона табеле на мапама](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) водича за решавање проблема са двоструким уписивањем.

## <a name="quality-updates"></a>Исправке квалитета

### <a name="project-operations-on-dataverse"></a>Project Operations у услузи Dataverse

| Област функција | Референтни број | Исправка квалитета |
| --- | --- | --- |
| Управљање могућностима за пословање | 2762089. | Грешка при руковању током затварања уговора као неоствареног ако је аутоматско чување онемогућено у организацији.|
|Планирање и праћење пројекта | 2767841. | Телеметрија ажурира сценарије креирања или ажурирања ентитета пројекта.|
|Наплата и одређивање цена | 2771072. | Обрада изузетка нулте референце током освајања понуде.|
|Наплата и одређивање цена | 2844181. |Није успело добијање ID-а корелације и блокирање креирања фактуре.|
|Наплата и одређивање цена | 2852836. | Недостају међукомпанијске стварне вредности за међукомпанијски трошак креиран и одобрен у CE.|


### <a name="project-management-and-accounting-in-finance"></a>Управљање пројектима и рачуноводство у услузи Finance

За информације о исправкама грешака које су укључене у ову исправку, пријавите се на Microsoft Dynamics Lifecycle Services (LCS) и погледајте [чланак у бази знања](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
