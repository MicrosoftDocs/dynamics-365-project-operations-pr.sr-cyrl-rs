---
title: Шта је ново или промењено у издању 28 исправке Project Service Automation верзије 3
description: У овој теми су наведене функције и исправке које су доступне у издању исправке 28 за Project Service Automation верзије 3.
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
ms.openlocfilehash: fed18ba292943f53965ee518afb5cbb13427ca60f32451edb49f67e6f10d24fe
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994969"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>Шта је ново или промењено у издању 28 исправке Project Service Automation верзије 3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Ово издање је компатибилно са услугом Dynamics 365 9.x. Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

У овој теми су наведене функције и исправке које су нове или промењене у издању исправке 28 за Project Service Automation верзије 3. Ова верзија има број верзије V3.10.46.32 и постала је опште доступна путем самосталне исправке у јануару 2021.

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