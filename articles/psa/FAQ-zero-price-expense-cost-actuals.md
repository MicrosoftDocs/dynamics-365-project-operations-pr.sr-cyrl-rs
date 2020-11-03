---
title: Зашто се цена подразумевано враћа на нулу на износима стварних трошкова?
description: Решавање проблема због чега се цена подразумевано враћа на 0 на износима стварних трошкова.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 9f4ff8a96250d675faeda3246c2d0a6c5bd83286
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083993"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>Зашто се цена подразумевано враћа на нулу на износима стварних трошкова?

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>Решавање проблема са стопама трошкова у износима стварних трошкова

Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ. Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.
 
Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.
