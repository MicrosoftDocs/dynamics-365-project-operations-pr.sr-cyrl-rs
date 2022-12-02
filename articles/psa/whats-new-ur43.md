---
title: Шта је ново или промењено у издању 43 исправке Project Service Automation верзије 3
description: У овом чланку наведене су функције и исправке које су доступне у издању 43 исправке услуге Microsoft Dynamics 365 Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 05/04/2022
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
ms.openlocfilehash: b12cfda08f1ea1fc441782003130be445a437f7c
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8915340"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-43-v3"></a>Шта је ново или промењено у издању 43 исправке Project Service Automation верзије 3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Компатибилна је са системом Dynamics 365 9.x. Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

У овом чланку дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 43. Број израде ове верзије је V3.10.74.200 и углавном је доступна путем самосталног ажурирања у мају 2022. године.

## <a name="update-release-43"></a>Издање исправке 43

### <a name="bug-fixes"></a>Исправке грешака

Поправљени су следећи проблеми.


**Време и трошак**

- Приликом увоза ставки времена из резервација или додељивања ресурса, референца на повезани ресурс који се може резервисати се не одржава.
- Када се матрица координатне мреже за унос времена прошири на цео екран, кретање кроз матрицу координатне мреже помоћу табулатора не функционише.
- Приликом прослеђивања ставке времена коју је креирао други корисник, поље **Проследио** се неправилно попуњава корисником који је креирао временски лист.
