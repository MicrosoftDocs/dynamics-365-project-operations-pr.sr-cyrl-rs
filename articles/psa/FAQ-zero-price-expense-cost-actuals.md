---
title: Зашто се цена подразумевано враћа на нулу на износима стварних трошкова?
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
ms.openlocfilehash: 306f169ee25d42ac3c9e63fa70956b9c50315829
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122136"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="cc1b5-103">Зашто се цена подразумевано враћа на нулу на износима стварних трошкова?</span><span class="sxs-lookup"><span data-stu-id="cc1b5-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="cc1b5-104">Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.</span><span class="sxs-lookup"><span data-stu-id="cc1b5-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="cc1b5-105">Решавање проблема са стопама трошкова у износима стварних трошкова</span><span class="sxs-lookup"><span data-stu-id="cc1b5-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="cc1b5-106">Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ.</span><span class="sxs-lookup"><span data-stu-id="cc1b5-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="cc1b5-107">Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.</span><span class="sxs-lookup"><span data-stu-id="cc1b5-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="cc1b5-108">Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.</span><span class="sxs-lookup"><span data-stu-id="cc1b5-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
