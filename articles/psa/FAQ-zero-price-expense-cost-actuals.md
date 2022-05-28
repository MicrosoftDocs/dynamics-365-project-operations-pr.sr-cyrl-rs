---
title: Зашто се цена подразумевано враћа на нулу за износе стварних трошкова?
description: Решавање проблема због чега се цена подразумевано враћа на 0 на износима стварних трошкова.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.author: rumant
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
ms.openlocfilehash: 7de9f660bf38629bb2af4e0fb1ebf815f5e525e2
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/14/2022
ms.locfileid: "8595608"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>Зашто се цена подразумевано враћа на нулу за износе стварних трошкова?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>Решавање проблема са стопама трошкова у износима стварних трошкова

Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ. Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.
 
Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
