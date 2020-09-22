---
title: Зашто се цена подразумевано враћа на нулу на износима стварних трошкова?
description: Решавање проблема због чега се цена подразумевано враћа на 0 на износима стварних трошкова.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.prod: Project Service
ms.technology: ''
ms.assetid: bc1ebc58-c733-4310-8435-572ed9a9fef9
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3fb678822877a61d141de75aea29b7d5cdf292c4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755368"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="49a83-103">Зашто се цена подразумевано враћа на нулу на износима стварних трошкова?</span><span class="sxs-lookup"><span data-stu-id="49a83-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="49a83-104">Ова најчешћа питања се односе на стварне трошкове у којима је класа трансакције подешена на Трошак, а где је врста трансакције Трошак.</span><span class="sxs-lookup"><span data-stu-id="49a83-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="49a83-105">Решавање проблема са стопама трошкова у износима стварних трошкова</span><span class="sxs-lookup"><span data-stu-id="49a83-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="49a83-106">Идите на односну ставку трошка и уверите се да у пољу ставке трошка постоји износ.</span><span class="sxs-lookup"><span data-stu-id="49a83-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="49a83-107">Ако изворна ставка трошка није имала попуњено поље за износ, онда сте изоловали проблем.</span><span class="sxs-lookup"><span data-stu-id="49a83-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="49a83-108">Да бисте решили овај проблем, поново креирајте ставку трошка са важећим износом и одобрите га.</span><span class="sxs-lookup"><span data-stu-id="49a83-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
