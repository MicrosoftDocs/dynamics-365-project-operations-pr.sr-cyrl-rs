---
title: Шта је ново или промењено у издању 28 исправке Project Service Automation верзије 3
description: Овај чланак наводи функције и исправке које су доступне у издању за ажурирање аутоматизације услуге пројекта Релеасе 28, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 56a87bce55c560e541e20709b10d38b9512ffcee
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930612"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>Шта је ново или промењено у издању 28 исправке Project Service Automation верзије 3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Ово издање је компатибилно са услугом Dynamics 365 9.x. Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

Овај чланак наводи функције и исправке које су нове или промењене за Пројецт Сервице Аутоматион V3, Упдате Релеасе 28 Ова верзија има број верзије В3.10.46.32 и обично је доступна путем самосталног ажурирања у јануару 2021.

## <a name="update-release-28"></a>Издање исправке 28

### <a name="bug-fixes"></a>Исправке грешака

**Време и трошак**

Поправљени су следећи проблеми:

- Корисници могу да користе **Масовно уређивање** за ажурирање записа времена који су одобрени и послати.

**Управљање пројектима**

Поправљени су следећи проблеми:

- У случајевима када се GUID задатка тумачи као број, задаци се не могу отворити за уређивање помоћу опције **Уреди задатак** у траци на страници **Структурна анализа посла**.

**Sales**

Поправљени су следећи проблеми:

- Изузетак празне референце се генерише када се позива додатна компонента **GetEstimatesForProject**.
- **Означи као спремно за фактурисање** у мрежи контролних тачака само делимично ажурира атрибуте, осим атрибута **InvoiceStatus**, који се ажурира.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
