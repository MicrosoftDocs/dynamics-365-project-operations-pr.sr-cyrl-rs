---
title: Анализа понуда за пројекат
description: Ова тема пружа информације о анализи понуда за пројекат.
author: rumant
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: d1b79a61147bfccf13b0a33179464af91b45121e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291277"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="e2fb5-103">Анализа понуда за пројекат</span><span class="sxs-lookup"><span data-stu-id="e2fb5-103">Analysis of project quotes</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e2fb5-104">Dynamics 365 Project Service Automation анализира понуде за пројекат ради процене профитабилности.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="e2fb5-105">Такође анализира колико је понуда усаглашена са очекивањима клијента о датуму испоруке или завршетка, као и са буџетом.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="e2fb5-106">Анализа исплативости</span><span class="sxs-lookup"><span data-stu-id="e2fb5-106">Profitability analysis</span></span>

<span data-ttu-id="e2fb5-107">Project Service Automation анализира профитабилност коришћењем бруто марже и кориговане бруто маргине.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="e2fb5-108">Бруто марже се израчунавају помоћу следеће формуле:</span><span class="sxs-lookup"><span data-stu-id="e2fb5-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="e2fb5-109">Коригована бруто маржа се израчунавају помоћу следеће формуле:</span><span class="sxs-lookup"><span data-stu-id="e2fb5-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="e2fb5-110">Ако се вредности бруто марже и кориговане бруто марже значајно разликују, већи део посла у понуди је класификован као ненаплатив.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="e2fb5-111">Анализа очекивања клијента</span><span class="sxs-lookup"><span data-stu-id="e2fb5-111">Analysis of customer expectations</span></span>

<span data-ttu-id="e2fb5-112">Можете анализирати понуде и генерисати графиконе за очекивања клијената у вези са распоредом и буџетом ако унесете вредности за следећа поља:</span><span class="sxs-lookup"><span data-stu-id="e2fb5-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="e2fb5-113">Поље **Захтевани датум испоруке** у заглављу понуде.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="e2fb5-114">Поље **Буџет клијента** за сваку ставку понуде (за ставке засноване на пројекту и ставке засноване на производу).</span><span class="sxs-lookup"><span data-stu-id="e2fb5-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="e2fb5-115">Анализа очекивања клијената у вези са распоредом се врши поређењем најновијег датума завршетка детаља ставке понуде са захтеваним датумом испоруке за све ставке понуде у понуди.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="e2fb5-116">Анализа очекивања клијената у вези са буџетом врши се поређењем збира укупног буџета клијента са понуђеним износом у свим ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="e2fb5-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]