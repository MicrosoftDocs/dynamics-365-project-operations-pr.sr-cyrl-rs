---
title: Шта је ново или промењено у издању 17.5 исправке Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 17 исправке за Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: 364a64e0ea501ac5b7faaf254c7af3648cfe1f9b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006709"
---
# <a name="project-service-automation-update-release-17-v3"></a>Project Service Automation издање исправке 17, у верзији 3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.  Ово издање је компатибилно са услугом Dynamics 365 9.x. Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

У овој теми дате су функције и исправке које су нове или су промењене у решењу PSA верзије 3, издање исправке 17. Ова верзија има број верзије V3.10.6.34 и опште је доступна путем само-исправке у марту 2020. године.


## <a name="update-release-17"></a>Издање исправке 17

### <a name="bug-fixes"></a>Исправке грешака

**Општи проблеми**

- Исправљено: ажурирајте Project Service Automation за спровођење лиценци за чланове тима (Чвориште ресурса за пројекат ће укључити 3.x метаподатке плана услуге за чланове тима)
 
**Време и трошак**

- Исправљено: немогућност промене процене трошкова из цене различите од нуле у нулу (0). Промена се игнорише.

**Управљање пројектима**

- Исправљено: додата је провера нултих вредности у име позиције члана тима.
- Исправљено: поље **msdyn_userresourceid** поље у ентитету **msdyn_resourceassignment** није одобрено.
- Исправљено: надоградња са 2.x на 3.x сада управља празним контурама ангажовања у доделама задатака.

**Sales**

- Исправљено: **Invoice.PreValidateInvoiceUpdate** сада правилно управља сценаријем поновног додељивања власништва записа.
- Исправљено: када је класа трансакције **Време**, **UnitGroup** не може да се уређује ни за један ентитет, укључујући **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail** и **ContractLineDetails**. Међутим, **Јединица** не може да се уређује само за **JournalLine** и **InvoiceLineDetails**.




[!INCLUDE[footer-include](../includes/footer-banner.md)]