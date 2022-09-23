---
title: Шта је ново или промењено у ажурирању аутоматизације пројектне услуге Релеасе 47, V3
description: Овај чланак наводи функције и исправке које су доступне у издању Microsoft Dynamics 365 Project Service Automation Упдате Релеасе 47, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 09/14/2022
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
ms.openlocfilehash: 08e8fa9c41bdd77d93e4d5207266115022fba1b2
ms.sourcegitcommit: 498a5d5a33c47cab788fac4215fc47662042155a
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/14/2022
ms.locfileid: "9477289"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-47-v3"></a>Шта је ново или промењено у ажурирању аутоматизације пројектне услуге Релеасе 47, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Компатибилна је са системом Dynamics 365 9.x. Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

Овај чланак наводи функције и исправке које су нове или промењене за исправку за аутоматизацију услуге пројекта Релеасе 45, V3. Ова верзија има број верзије В 3.10.78.8 и обично је доступна путем самосталног ажурирања у јулу 2022.

## <a name="update-release-47"></a>Издање исправке 47

### <a name="bug-fixes"></a>Исправке грешака

Поправљени су следећи проблеми.

**Управљање ресурсима**
- Провера ваљаности је ажурирана да би се осигурало да корисници не могу да изазову изузетак без референце када покушавају да креирају члана пројектног тима без ресурса **који се може резервисати**.
