---
title: Зашто се цена подразумевано враћа на нулу за износе стварних трошкова?
description: Решавање проблема због чега се цена подразумевано враћа на 0 на износима стварних трошкова.
author: rumant
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: f6ea664f9f38621ce5d1b0dd033d7df491f845ff
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146366"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>Зашто се цена подразумевано враћа на нулу за износе стварних трошкова?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>Решавање проблема са стопама трошкова у износима стварних трошкова

Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ. Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.
 
Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.
