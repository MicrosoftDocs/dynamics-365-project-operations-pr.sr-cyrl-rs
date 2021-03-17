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
ms.openlocfilehash: 742b0b9c495b4b3ecb4705be3ece5656f0322ca9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285872"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="1974d-103">Зашто се цена подразумевано враћа на нулу за износе стварних трошкова?</span><span class="sxs-lookup"><span data-stu-id="1974d-103">Why is the price defaulting to zero on expense cost actuals</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="1974d-104">Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.</span><span class="sxs-lookup"><span data-stu-id="1974d-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="1974d-105">Решавање проблема са стопама трошкова у износима стварних трошкова</span><span class="sxs-lookup"><span data-stu-id="1974d-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="1974d-106">Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ.</span><span class="sxs-lookup"><span data-stu-id="1974d-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="1974d-107">Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.</span><span class="sxs-lookup"><span data-stu-id="1974d-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="1974d-108">Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.</span><span class="sxs-lookup"><span data-stu-id="1974d-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]