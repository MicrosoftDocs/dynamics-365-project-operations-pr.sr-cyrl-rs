---
title: Тренутно стање
description: Ова тема пружа информације о начину рада са стварним подацима у услузи Microsoft Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 93a945ffbe9c6dd998456b506b95e717ab8fbab7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083962"
---
# <a name="actuals"></a><span data-ttu-id="3481a-103">Тренутно стање</span><span class="sxs-lookup"><span data-stu-id="3481a-103">Actuals</span></span> 

<span data-ttu-id="3481a-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="3481a-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3481a-105">Стварне вредности представљају количину посла која је завршена за пројекат.</span><span class="sxs-lookup"><span data-stu-id="3481a-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="3481a-106">Креирани су као резултат ставки времена и трошкова, ставки књижења у главној књизи и фактура.</span><span class="sxs-lookup"><span data-stu-id="3481a-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="3481a-107">Ставке у главној књизи и време предаје</span><span class="sxs-lookup"><span data-stu-id="3481a-107">Journal lines and time submission</span></span>

<span data-ttu-id="3481a-108">За више информација о ставци времена, погледајте [Преглед уноса времена](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="3481a-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="3481a-109">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="3481a-109">Time and materials</span></span>

<span data-ttu-id="3481a-110">Када је ставка времена која је прослеђена повезана са пројектом који је мапиран у предмет уговора о времену и материјалима, систем креира две ставке у главној књизи, једну за трошкове и једну за ненаплаћену продају.</span><span class="sxs-lookup"><span data-stu-id="3481a-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="3481a-111">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="3481a-111">Fixed price</span></span>

<span data-ttu-id="3481a-112">Када се прослеђена ставка времена повеже са пројектом који се мапиран на предмет уговора са фиксном ценом, систем креира једну ставку у главној књизи за трошкове.</span><span class="sxs-lookup"><span data-stu-id="3481a-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="3481a-113">Подразумевано одређивање цена</span><span class="sxs-lookup"><span data-stu-id="3481a-113">Default pricing</span></span>

<span data-ttu-id="3481a-114">Логика за креирање подразумеваних цена се налази у ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="3481a-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="3481a-115">Вредности поља из ставке времена копирају се у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="3481a-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="3481a-116">Ове вредности укључују датум трансакције, предмет уговора на који је пројекат мапиран и валуту која је резултат одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="3481a-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="3481a-117">Поља која утичу на подразумевано одређивање цена, као што су **Улога** и **Организациона јединица** , користе се за утврђивање одговарајуће цене у ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="3481a-117">The fields that affect default pricing, such as **Role** and **Org Unit** , are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="3481a-118">На ставку времена можете додати прилагођено поље.</span><span class="sxs-lookup"><span data-stu-id="3481a-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="3481a-119">Ако желите да се вредност поља шири на стварне вредности, креирајте поље у ентитету Стварне вредности и употребите мапирања поља да бисте копирали поље из ставке времена у стварну вредност.</span><span class="sxs-lookup"><span data-stu-id="3481a-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="3481a-120">Прослеђивање ставки у главној књизи и основних трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="3481a-121">За више информација о ставци трошка, погледајте [Преглед трошкова](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="3481a-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="3481a-122">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="3481a-122">Time and materials</span></span>

<span data-ttu-id="3481a-123">Када се ставка основног трошка која је прослеђена повеже са пројектом који је мапиран у предмет уговора о времену и материјалима, систем креира две ставке у главној књизи, једну за трошкове и једну за ненаплаћену продају.</span><span class="sxs-lookup"><span data-stu-id="3481a-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="3481a-124">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="3481a-124">Fixed price</span></span>

<span data-ttu-id="3481a-125">Када се прослеђена ставка основног трошка повеже са пројектом који се мапиран на предмет уговора са фиксном ценом, систем креира једну ставку у главној књизи за трошкове.</span><span class="sxs-lookup"><span data-stu-id="3481a-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="3481a-126">Подразумевано одређивање цена</span><span class="sxs-lookup"><span data-stu-id="3481a-126">Default pricing</span></span>

<span data-ttu-id="3481a-127">Логика уношења задатих цена за трошкове заснива се на категорији трошкова.</span><span class="sxs-lookup"><span data-stu-id="3481a-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="3481a-128">Датум трансакције, предмет уговора на који је пројекат мапиран и валуту се користе за одређивање одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="3481a-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="3481a-129">Међутим, износ који се унесе за саму цену подразумевано се подешава директно на повезаним ставкама трошкова у главној књизи за трошкове и продају.</span><span class="sxs-lookup"><span data-stu-id="3481a-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="3481a-130">Није доступна ставка заснована на категорији подразумеваних цена по јединици за ставке трошкова.</span><span class="sxs-lookup"><span data-stu-id="3481a-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="3481a-131">Коришћење дневника за књижење за евидентирање трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-131">Use entry journals to record costs</span></span>

<span data-ttu-id="3481a-132">Можете да користите дневнике за књижење да евидентирате трошкове или приход у класама материјала, накнаде, времена, трошкова или пореских трансакција.</span><span class="sxs-lookup"><span data-stu-id="3481a-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="3481a-133">Дневници се могу користити у следеће сврхе:</span><span class="sxs-lookup"><span data-stu-id="3481a-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="3481a-134">Забележите стварне трошкове материјала и продаје на пројекту.</span><span class="sxs-lookup"><span data-stu-id="3481a-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="3481a-135">Преместите стварне вредности трансакција из другог система у Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="3481a-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="3481a-136">Евидентирајте трошкове који су се догодили у другом систему.</span><span class="sxs-lookup"><span data-stu-id="3481a-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="3481a-137">Ови трошкови могу укључивати трошкове набавке или подуговарања.</span><span class="sxs-lookup"><span data-stu-id="3481a-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3481a-138">Апликација не потврђује тип ставке у главној књизи или повезано одређивање цена које се уноси у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="3481a-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="3481a-139">Стога само корисник који је потпуно свестан рачуноводственог утицаја који стварне вредности имају на пројекат треба да користи дневнике за књижење за креирање стварних података.</span><span class="sxs-lookup"><span data-stu-id="3481a-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="3481a-140">Због утицаја овог типа дневника, пажљиво бирајте ко има приступ креирању дневника за књижење.</span><span class="sxs-lookup"><span data-stu-id="3481a-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="3481a-141">Евидентирање стварних вредности на основу догађаја у пројекту</span><span class="sxs-lookup"><span data-stu-id="3481a-141">Record actuals based on project events</span></span>

<span data-ttu-id="3481a-142">Project Operations бележи финансијске трансакције које се дешавају током пројекта.</span><span class="sxs-lookup"><span data-stu-id="3481a-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="3481a-143">Ове трансакције се евидентирају као стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="3481a-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="3481a-144">Следеће табеле приказују различите врсте стварних вредности које се креирају, зависно од тога да ли је пројекат заснован на времену и материјалима или пројекат са фиксном ценом, да ли је у фази предпродаје или је интерни пројекат.</span><span class="sxs-lookup"><span data-stu-id="3481a-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="3481a-145">Ресурс припада истој организационој јединици као и уговорна јединица пројекта</span><span class="sxs-lookup"><span data-stu-id="3481a-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="3481a-146">Догађај</span><span class="sxs-lookup"><span data-stu-id="3481a-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="3481a-147">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="3481a-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="3481a-148">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="3481a-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="3481a-149">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="3481a-150">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="3481a-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="3481a-151">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="3481a-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="3481a-152">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="3481a-152">Actuals</span></span></th>
<th><span data-ttu-id="3481a-153">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="3481a-153">Transaction currency</span></span></th>
<th><span data-ttu-id="3481a-154">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="3481a-154">Fixed price</span></span></th>
<th><span data-ttu-id="3481a-155">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="3481a-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="3481a-156">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="3481a-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="3481a-157">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="3481a-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-158">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="3481a-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="3481a-159">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="3481a-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3481a-160">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3481a-161">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-161">Cost actual</span></span></td>
<td><span data-ttu-id="3481a-162">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-163">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-164">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="3481a-165">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-166">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-167">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="3481a-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="3481a-168">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3481a-169">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3481a-170">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-170">Cost actual</span></span></td>
<td><span data-ttu-id="3481a-171">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-172">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-173">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-174">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-175">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-176">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="3481a-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3481a-177">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-178">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="3481a-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3481a-179">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3481a-180">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3481a-181">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="3481a-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3481a-182">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-183">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="3481a-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-184">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-185">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-186">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-187">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="3481a-187">Billed sales</span></span></td>
<td><span data-ttu-id="3481a-188">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3481a-189">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3481a-190">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="3481a-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3481a-191">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-192">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-193">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-194">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-195">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-196">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="3481a-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3481a-197">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-198">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="3481a-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3481a-199">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3481a-200">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="3481a-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3481a-201">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="3481a-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3481a-202">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="3481a-203">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="3481a-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="3481a-204">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="3481a-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="3481a-205">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-206">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-207">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-208">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="3481a-208">Billed sales</span></span></td>
<td><span data-ttu-id="3481a-209">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3481a-210">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="3481a-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3481a-211">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="3481a-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3481a-212">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-213">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="3481a-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="3481a-214">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-215">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="3481a-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="3481a-216">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="3481a-217">Ресурс припада организационој јединици која се разликује од уговорне јединице пројекта</span><span class="sxs-lookup"><span data-stu-id="3481a-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="3481a-218">Догађај</span><span class="sxs-lookup"><span data-stu-id="3481a-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="3481a-219">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="3481a-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="3481a-220">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="3481a-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="3481a-221">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="3481a-222">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="3481a-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="3481a-223">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="3481a-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="3481a-224">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="3481a-224">Actuals</span></span></th>
<th><span data-ttu-id="3481a-225">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="3481a-225">Transaction currency</span></span></th>
<th><span data-ttu-id="3481a-226">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="3481a-226">Fixed price</span></span></th>
<th><span data-ttu-id="3481a-227">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="3481a-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="3481a-228">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="3481a-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="3481a-229">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="3481a-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-230">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="3481a-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="3481a-231">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="3481a-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="3481a-232">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3481a-233">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-233">Cost actual</span></span></td>
<td><span data-ttu-id="3481a-234">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="3481a-235">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="3481a-236">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="3481a-237">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="3481a-238">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-239">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="3481a-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="3481a-240">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-241">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="3481a-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="3481a-242">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="3481a-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-243">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="3481a-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="3481a-244">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="3481a-245">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3481a-246">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-246">Cost actual</span></span></td>
<td><span data-ttu-id="3481a-247">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-248">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-249">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-250">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-251">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="3481a-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-252">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="3481a-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="3481a-253">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="3481a-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-254">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="3481a-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="3481a-255">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="3481a-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-256">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="3481a-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3481a-257">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-258">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="3481a-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3481a-259">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3481a-260">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3481a-261">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="3481a-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3481a-262">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-263">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="3481a-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-264">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-265">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="3481a-266">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-267">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="3481a-267">Billed sales</span></span></td>
<td><span data-ttu-id="3481a-268">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3481a-269">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="3481a-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3481a-270">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="3481a-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3481a-271">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-272">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-273">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-274">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3481a-275">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-276">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="3481a-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3481a-277">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-278">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="3481a-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3481a-279">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3481a-280">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="3481a-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3481a-281">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="3481a-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3481a-282">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="3481a-283">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="3481a-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="3481a-284">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="3481a-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="3481a-285">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-286">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="3481a-287">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="3481a-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-288">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="3481a-288">Billed sales</span></span></td>
<td><span data-ttu-id="3481a-289">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3481a-290">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="3481a-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3481a-291">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="3481a-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3481a-292">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-293">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="3481a-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="3481a-294">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3481a-295">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="3481a-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="3481a-296">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="3481a-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
