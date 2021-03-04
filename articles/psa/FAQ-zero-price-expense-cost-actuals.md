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
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="de6cf-103">Зашто се цена подразумевано враћа на нулу за износе стварних трошкова?</span><span class="sxs-lookup"><span data-stu-id="de6cf-103">Why is the price defaulting to zero on expense cost actuals</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="de6cf-104">Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.</span><span class="sxs-lookup"><span data-stu-id="de6cf-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="de6cf-105">Решавање проблема са стопама трошкова у износима стварних трошкова</span><span class="sxs-lookup"><span data-stu-id="de6cf-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="de6cf-106">Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ.</span><span class="sxs-lookup"><span data-stu-id="de6cf-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="de6cf-107">Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.</span><span class="sxs-lookup"><span data-stu-id="de6cf-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="de6cf-108">Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.</span><span class="sxs-lookup"><span data-stu-id="de6cf-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
