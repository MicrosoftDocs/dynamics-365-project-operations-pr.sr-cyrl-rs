---
title: Анализа понуда за пројекат
description: Ова тема пружа информације о анализи понуда за пројекат.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
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
ms.openlocfilehash: acb3f1a2020cfd59f60f828e9092bd7ccde00077
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012469"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="7810c-103">Анализа понуда за пројекат</span><span class="sxs-lookup"><span data-stu-id="7810c-103">Analysis of project quotes</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="7810c-104">Dynamics 365 Project Service Automation анализира понуде за пројекат ради процене профитабилности.</span><span class="sxs-lookup"><span data-stu-id="7810c-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="7810c-105">Такође анализира колико је понуда усаглашена са очекивањима клијента о датуму испоруке или завршетка, као и са буџетом.</span><span class="sxs-lookup"><span data-stu-id="7810c-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="7810c-106">Анализа исплативости</span><span class="sxs-lookup"><span data-stu-id="7810c-106">Profitability analysis</span></span>

<span data-ttu-id="7810c-107">Project Service Automation анализира профитабилност коришћењем бруто марже и кориговане бруто маргине.</span><span class="sxs-lookup"><span data-stu-id="7810c-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="7810c-108">Бруто марже се израчунавају помоћу следеће формуле:</span><span class="sxs-lookup"><span data-stu-id="7810c-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="7810c-109">Коригована бруто маржа се израчунавају помоћу следеће формуле:</span><span class="sxs-lookup"><span data-stu-id="7810c-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="7810c-110">Ако се вредности бруто марже и кориговане бруто марже значајно разликују, већи део посла у понуди је класификован као ненаплатив.</span><span class="sxs-lookup"><span data-stu-id="7810c-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="7810c-111">Анализа очекивања клијента</span><span class="sxs-lookup"><span data-stu-id="7810c-111">Analysis of customer expectations</span></span>

<span data-ttu-id="7810c-112">Можете анализирати понуде и генерисати графиконе за очекивања клијената у вези са распоредом и буџетом ако унесете вредности за следећа поља:</span><span class="sxs-lookup"><span data-stu-id="7810c-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="7810c-113">Поље **Захтевани датум испоруке** у заглављу понуде.</span><span class="sxs-lookup"><span data-stu-id="7810c-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="7810c-114">Поље **Буџет клијента** за сваку ставку понуде (за ставке засноване на пројекту и ставке засноване на производу).</span><span class="sxs-lookup"><span data-stu-id="7810c-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="7810c-115">Анализа очекивања клијената у вези са распоредом се врши поређењем најновијег датума завршетка детаља ставке понуде са захтеваним датумом испоруке за све ставке понуде у понуди.</span><span class="sxs-lookup"><span data-stu-id="7810c-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="7810c-116">Анализа очекивања клијената у вези са буџетом врши се поређењем збира укупног буџета клијента са понуђеним износом у свим ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="7810c-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]