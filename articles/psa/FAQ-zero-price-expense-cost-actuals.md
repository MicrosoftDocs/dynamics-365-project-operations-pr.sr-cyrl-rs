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
ms.openlocfilehash: a6e971ff0477d5a9cb8652541095538b9f9039c0870362077218df609871ed4f
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "6990964"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>Зашто се цена подразумевано враћа на нулу за износе стварних трошкова?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>Решавање проблема са стопама трошкова у износима стварних трошкова

Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ. Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.
 
Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.


[!INCLUDE[footer-include](../includes/footer-banner.md)]