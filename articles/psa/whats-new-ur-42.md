---
title: Шта је ново или промењено у ажурирању аутоматизације услуге пројекта Издање 42, V3
description: Овај чланак наводи функције и исправке које су доступне у издању Microsoft Dynamics 365 Project Service Automation Упдате Релеасе 42, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/05/2022
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
ms.openlocfilehash: e9911531e4acbd78db416f554c8d85c4f1fee1cf
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912733"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>Шта је ново или промењено у ажурирању аутоматизације услуге пројекта Издање 42, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Компатибилна је са системом Dynamics 365 9.x. Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

Овај чланак наводи функције и исправке које су нове или промењене за исправку за аутоматизацију услуге пројекта Релеасе 42, V3. Број израде ове верзије је V3.10.73.61 и углавном је доступна путем самосталног ажурирања у априлу 2022. године.

## <a name="update-release-42"></a>Издање исправке 42

### <a name="bug-fixes"></a>Исправке грешака

Поправљени су следећи проблеми.

**Време и трошак**

- Када је временски лист одбијен, корисник који га је одбацио је нетачно идентификован као **Систем**.
- Када се ставке времена увезу, недостаје **вредност "Категорија** ресурса".
- Особе које врше одобравање пројекта могу да одобре прослеђене пројекте када њихове дозволе нису посебно подешене на "Може **да одобри"**.

**Продаја**

- Када се стварне датотеке евидентирају на задацима који нису основног нивоа, стварни трошкови се неправилно агрегирају.
