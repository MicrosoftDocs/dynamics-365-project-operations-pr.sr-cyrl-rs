---
title: Почетна страница „Стварни подаци“
description: Ова тема пружа информације о начину рада са стварним подацима у услузи Microsoft Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 75ad336a995aba3505325466433a5c5e2bb3e776
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907336"
---
# <a name="actuals"></a><span data-ttu-id="46a6d-103">Тренутно стање</span><span class="sxs-lookup"><span data-stu-id="46a6d-103">Actuals</span></span>

<span data-ttu-id="46a6d-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="46a6d-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="46a6d-105">Стварне вредности представљају количину посла која је завршена за пројекат.</span><span class="sxs-lookup"><span data-stu-id="46a6d-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="46a6d-106">Креирани су као резултат ставки времена и трошкова, ставки књижења у главној књизи и фактура.</span><span class="sxs-lookup"><span data-stu-id="46a6d-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="46a6d-107">Ставке у главној књизи и време предаје</span><span class="sxs-lookup"><span data-stu-id="46a6d-107">Journal lines and time submission</span></span>

<span data-ttu-id="46a6d-108">За више информација о ставци времена, погледајте [Преглед уноса времена](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="46a6d-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="46a6d-109">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="46a6d-109">Time and materials</span></span>

<span data-ttu-id="46a6d-110">Када је ставка времена која је прослеђена повезана са пројектом који је мапиран у предмет уговора о времену и материјалима, систем креира две ставке у главној књизи, једну за трошкове и једну за ненаплаћену продају.</span><span class="sxs-lookup"><span data-stu-id="46a6d-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="46a6d-111">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-111">Fixed price</span></span>

<span data-ttu-id="46a6d-112">Када се прослеђена ставка времена повеже са пројектом који се мапиран на предмет уговора са фиксном ценом, систем креира једну ставку у главној књизи за трошкове.</span><span class="sxs-lookup"><span data-stu-id="46a6d-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="46a6d-113">Подразумевано одређивање цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-113">Default pricing</span></span>

<span data-ttu-id="46a6d-114">Логика за креирање подразумеваних цена се налази у ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="46a6d-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="46a6d-115">Вредности поља из ставке времена копирају се у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="46a6d-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="46a6d-116">Ове вредности укључују датум трансакције, предмет уговора на који је пројекат мапиран и валуту која је резултат одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="46a6d-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="46a6d-117">Поља која утичу на подразумевано одређивање цена, као што су **Улога** и **Организациона јединица**, користе се за утврђивање одговарајуће цене у ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="46a6d-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="46a6d-118">На ставку времена можете додати прилагођено поље.</span><span class="sxs-lookup"><span data-stu-id="46a6d-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="46a6d-119">Ако желите да се вредност поља шири на стварне вредности, креирајте поље у ентитету Стварне вредности и употребите мапирања поља да бисте копирали поље из ставке времена у стварну вредност.</span><span class="sxs-lookup"><span data-stu-id="46a6d-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="46a6d-120">Прослеђивање ставки у главној књизи и основних трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="46a6d-121">За више информација о ставци трошка, погледајте [Преглед трошкова](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="46a6d-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="46a6d-122">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="46a6d-122">Time and materials</span></span>

<span data-ttu-id="46a6d-123">Када се ставка основног трошка која је прослеђена повеже са пројектом који је мапиран у предмет уговора о времену и материјалима, систем креира две ставке у главној књизи, једну за трошкове и једну за ненаплаћену продају.</span><span class="sxs-lookup"><span data-stu-id="46a6d-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="46a6d-124">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-124">Fixed price</span></span>

<span data-ttu-id="46a6d-125">Када се прослеђена ставка основног трошка повеже са пројектом који се мапиран на предмет уговора са фиксном ценом, систем креира једну ставку у главној књизи за трошкове.</span><span class="sxs-lookup"><span data-stu-id="46a6d-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="46a6d-126">Подразумевано одређивање цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-126">Default pricing</span></span>

<span data-ttu-id="46a6d-127">Логика уношења задатих цена за трошкове заснива се на категорији трошкова.</span><span class="sxs-lookup"><span data-stu-id="46a6d-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="46a6d-128">Датум трансакције, предмет уговора на који је пројекат мапиран и валуту се користе за одређивање одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="46a6d-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="46a6d-129">Међутим, износ који се унесе за саму цену подразумевано се подешава директно на повезаним ставкама трошкова у главној књизи за трошкове и продају.</span><span class="sxs-lookup"><span data-stu-id="46a6d-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="46a6d-130">Није доступна ставка заснована на категорији подразумеваних цена по јединици за ставке трошкова.</span><span class="sxs-lookup"><span data-stu-id="46a6d-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="46a6d-131">Коришћење дневника за књижење за евидентирање трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-131">Use entry journals to record costs</span></span>

<span data-ttu-id="46a6d-132">Можете да користите дневнике за књижење да евидентирате трошкове или приход у класама материјала, накнаде, времена, трошкова или пореских трансакција.</span><span class="sxs-lookup"><span data-stu-id="46a6d-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="46a6d-133">Дневници се могу користити у следеће сврхе:</span><span class="sxs-lookup"><span data-stu-id="46a6d-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="46a6d-134">Забележите стварне трошкове материјала и продаје на пројекту.</span><span class="sxs-lookup"><span data-stu-id="46a6d-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="46a6d-135">Преместите стварне вредности трансакција из другог система у Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="46a6d-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="46a6d-136">Евидентирајте трошкове који су се догодили у другом систему.</span><span class="sxs-lookup"><span data-stu-id="46a6d-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="46a6d-137">Ови трошкови могу укључивати трошкове набавке или подуговарања.</span><span class="sxs-lookup"><span data-stu-id="46a6d-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="46a6d-138">Апликација не потврђује тип ставке у главној књизи или повезано одређивање цена које се уноси у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="46a6d-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="46a6d-139">Стога само корисник који је потпуно свестан рачуноводственог утицаја који стварне вредности имају на пројекат треба да користи дневнике за књижење за креирање стварних података.</span><span class="sxs-lookup"><span data-stu-id="46a6d-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="46a6d-140">Због утицаја овог типа дневника, пажљиво бирајте ко има приступ креирању дневника за књижење.</span><span class="sxs-lookup"><span data-stu-id="46a6d-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="46a6d-141">Евидентирање стварних вредности на основу догађаја у пројекту</span><span class="sxs-lookup"><span data-stu-id="46a6d-141">Record actuals based on project events</span></span>

<span data-ttu-id="46a6d-142">Project Operations бележи финансијске трансакције које се дешавају током пројекта.</span><span class="sxs-lookup"><span data-stu-id="46a6d-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="46a6d-143">Ове трансакције се евидентирају као стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="46a6d-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="46a6d-144">Следеће табеле приказују различите врсте стварних вредности које се креирају, зависно од тога да ли је пројекат заснован на времену и материјалима или пројекат са фиксном ценом, да ли је у фази предпродаје или је интерни пројекат.</span><span class="sxs-lookup"><span data-stu-id="46a6d-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="46a6d-145">Ресурс припада истој организационој јединици као и уговорна јединица пројекта</span><span class="sxs-lookup"><span data-stu-id="46a6d-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="46a6d-146">Догађај</span><span class="sxs-lookup"><span data-stu-id="46a6d-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="46a6d-147">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="46a6d-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="46a6d-148">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="46a6d-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="46a6d-149">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="46a6d-150">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="46a6d-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="46a6d-151">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="46a6d-152">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="46a6d-152">Actuals</span></span></th>
<th><span data-ttu-id="46a6d-153">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="46a6d-153">Transaction currency</span></span></th>
<th><span data-ttu-id="46a6d-154">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-154">Fixed price</span></span></th>
<th><span data-ttu-id="46a6d-155">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="46a6d-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="46a6d-156">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="46a6d-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="46a6d-157">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="46a6d-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-158">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="46a6d-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="46a6d-159">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="46a6d-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="46a6d-160">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="46a6d-161">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-161">Cost actual</span></span></td>
<td><span data-ttu-id="46a6d-162">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-163">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-164">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="46a6d-165">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-166">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-167">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="46a6d-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="46a6d-168">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="46a6d-169">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="46a6d-170">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-170">Cost actual</span></span></td>
<td><span data-ttu-id="46a6d-171">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-172">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-173">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-174">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-175">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-176">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="46a6d-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="46a6d-177">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-178">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="46a6d-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="46a6d-179">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="46a6d-180">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="46a6d-181">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="46a6d-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="46a6d-182">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-183">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="46a6d-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-184">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-185">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-186">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-187">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="46a6d-187">Billed sales</span></span></td>
<td><span data-ttu-id="46a6d-188">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="46a6d-189">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="46a6d-190">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="46a6d-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="46a6d-191">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-192">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-193">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-194">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-195">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-196">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="46a6d-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="46a6d-197">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-198">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="46a6d-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="46a6d-199">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="46a6d-200">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="46a6d-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="46a6d-201">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="46a6d-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="46a6d-202">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="46a6d-203">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="46a6d-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="46a6d-204">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="46a6d-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="46a6d-205">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-206">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-207">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-208">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="46a6d-208">Billed sales</span></span></td>
<td><span data-ttu-id="46a6d-209">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="46a6d-210">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="46a6d-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="46a6d-211">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="46a6d-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="46a6d-212">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-213">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="46a6d-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="46a6d-214">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-215">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="46a6d-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="46a6d-216">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="46a6d-217">Ресурс припада организационој јединици која се разликује од уговорне јединице пројекта</span><span class="sxs-lookup"><span data-stu-id="46a6d-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="46a6d-218">Догађај</span><span class="sxs-lookup"><span data-stu-id="46a6d-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="46a6d-219">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="46a6d-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="46a6d-220">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="46a6d-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="46a6d-221">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="46a6d-222">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="46a6d-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="46a6d-223">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="46a6d-224">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="46a6d-224">Actuals</span></span></th>
<th><span data-ttu-id="46a6d-225">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="46a6d-225">Transaction currency</span></span></th>
<th><span data-ttu-id="46a6d-226">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="46a6d-226">Fixed price</span></span></th>
<th><span data-ttu-id="46a6d-227">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="46a6d-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="46a6d-228">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="46a6d-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="46a6d-229">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="46a6d-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-230">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="46a6d-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="46a6d-231">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="46a6d-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="46a6d-232">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="46a6d-233">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-233">Cost actual</span></span></td>
<td><span data-ttu-id="46a6d-234">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="46a6d-235">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="46a6d-236">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="46a6d-237">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="46a6d-238">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-239">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="46a6d-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="46a6d-240">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-241">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="46a6d-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="46a6d-242">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="46a6d-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-243">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="46a6d-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="46a6d-244">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="46a6d-245">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="46a6d-246">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-246">Cost actual</span></span></td>
<td><span data-ttu-id="46a6d-247">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-248">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-249">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-250">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-251">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="46a6d-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-252">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="46a6d-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="46a6d-253">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="46a6d-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-254">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="46a6d-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="46a6d-255">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="46a6d-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-256">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="46a6d-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="46a6d-257">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-258">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="46a6d-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="46a6d-259">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="46a6d-260">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="46a6d-261">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="46a6d-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="46a6d-262">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-263">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="46a6d-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-264">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-265">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="46a6d-266">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-267">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="46a6d-267">Billed sales</span></span></td>
<td><span data-ttu-id="46a6d-268">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="46a6d-269">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="46a6d-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="46a6d-270">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="46a6d-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="46a6d-271">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-272">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-273">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-274">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="46a6d-275">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-276">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="46a6d-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="46a6d-277">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-278">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="46a6d-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="46a6d-279">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="46a6d-280">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="46a6d-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="46a6d-281">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="46a6d-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="46a6d-282">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="46a6d-283">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="46a6d-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="46a6d-284">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="46a6d-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="46a6d-285">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-286">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="46a6d-287">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="46a6d-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-288">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="46a6d-288">Billed sales</span></span></td>
<td><span data-ttu-id="46a6d-289">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="46a6d-290">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="46a6d-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="46a6d-291">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="46a6d-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="46a6d-292">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-293">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="46a6d-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="46a6d-294">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="46a6d-295">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="46a6d-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="46a6d-296">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="46a6d-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
