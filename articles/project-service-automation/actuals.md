---
title: Стварне вредности
description: Ова тема пружа информације о стварним вредностима пројекта.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755438"
---
# <a name="actuals"></a><span data-ttu-id="89abf-103">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="89abf-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="89abf-104">Стварне вредности представљају количину посла која је завршена за пројекат.</span><span class="sxs-lookup"><span data-stu-id="89abf-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="89abf-105">Стварне вредности пројекта могу да се прате до његових изворних докумената.</span><span class="sxs-lookup"><span data-stu-id="89abf-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="89abf-106">Ти изворни документи укључују време, трошкове и ставке књижења у главној књизи, као и фактуре.</span><span class="sxs-lookup"><span data-stu-id="89abf-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Како се стварне вредности пројекта прате до изворних докумената](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="89abf-108">Прослеђивање ставке времена</span><span class="sxs-lookup"><span data-stu-id="89abf-108">Submitting a time entry</span></span>

<span data-ttu-id="89abf-109">Код апликације PSA, када се ставка времена проследи за пројекат који је мапиран на предмет уговора о времену и материјалима, креирају се две ставке у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="89abf-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="89abf-110">Једна ставка је за трошкове, а друга за нефактурисане продаје.</span><span class="sxs-lookup"><span data-stu-id="89abf-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="89abf-111">Када се ставка времена проследи за пројекат који је мапиран на предмет уговора о фиксној цени, креира се ставка у главној књизи само за трошкове.</span><span class="sxs-lookup"><span data-stu-id="89abf-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="89abf-112">Логику за унос подразумеваних цена можете да пронађете у ставки у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="89abf-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="89abf-113">Све вредности поља из ставке времена копирају се у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="89abf-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="89abf-114">Ова поља укључују датум трансакције, предмет уговора на који је пројекат мапиран и валуту која је резултат одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="89abf-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="89abf-115">Поља која утичу на подразумеване цене, као што су **Улога** и **Организациона јединица** проузрокују подразумевани унос одговарајуће цене у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="89abf-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="89abf-116">Ако у ставку времена додате прилагођено поље, а желите да се вредност поља шири на стварне вредности, креирајте поље у ентитету Стварне вредности и употребите пресликавања поља да бисте копирали поље из ставке времена у стварну вредност.</span><span class="sxs-lookup"><span data-stu-id="89abf-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="89abf-117">Прослеђивање ставке трошка</span><span class="sxs-lookup"><span data-stu-id="89abf-117">Submitting an expense entry</span></span>

<span data-ttu-id="89abf-118">Код апликације PSA, када се ставка трошка проследи за пројекат који је мапиран на предмет уговора о времену и материјалима, креирају се две ставке у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="89abf-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="89abf-119">Једна ставка је за трошкове, а друга за нефактурисане продаје.</span><span class="sxs-lookup"><span data-stu-id="89abf-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="89abf-120">Када се ставка трошка проследи за пројекат који је мапиран на предмет уговора о фиксној цени, креира се ставка у главној књизи само за трошкове.</span><span class="sxs-lookup"><span data-stu-id="89abf-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="89abf-121">Логика за унос подразумеваних цена за трошкове темељи се на категорији трошкова која је изабрана на страници **Ставка трошкова**.</span><span class="sxs-lookup"><span data-stu-id="89abf-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="89abf-122">Датум трансакције, предмет уговора на који је пројекат мапиран и валуту се користе за одређивање одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="89abf-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="89abf-123">Међутим, за саму цену, износ који је корисник унео подразумевано се подешава директно на повезаним ставкама трошкова у главној књизи за трошкове и продају.</span><span class="sxs-lookup"><span data-stu-id="89abf-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="89abf-124">У тренутној верзији апликације PSA, није доступна ставка заснована на категорији подразумеваних цена по јединици за ставке трошкова.</span><span class="sxs-lookup"><span data-stu-id="89abf-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="89abf-125">Коришћење главних књига за евидентирање трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-125">Using journals to record costs</span></span>

<span data-ttu-id="89abf-126">У апликацији PSA, главне књиге вам омогућавају да евидентирате трошкове или приход у класама материјала, накнаде, времена, трошкова или пореских трансакција.</span><span class="sxs-lookup"><span data-stu-id="89abf-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="89abf-127">Главна књига има заглавље, ставке и радњу **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="89abf-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="89abf-128">Ево неколико сценарија где можете да користите главну књигу:</span><span class="sxs-lookup"><span data-stu-id="89abf-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="89abf-129">Морате забележити стварне трошкове и продају материјала на пројекту.</span><span class="sxs-lookup"><span data-stu-id="89abf-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="89abf-130">Морате преместити стварне вредности трансакција из другог система у PSA.</span><span class="sxs-lookup"><span data-stu-id="89abf-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="89abf-131">Морате да евидентирате трошкове остварене у другом систему, као што су трошкови набавке или подуговарања.</span><span class="sxs-lookup"><span data-stu-id="89abf-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="89abf-132">Евидентирање стварних вредности на основу догађаја у пројекту</span><span class="sxs-lookup"><span data-stu-id="89abf-132">Recording actuals based on project events</span></span>

<span data-ttu-id="89abf-133">PSA бележи финансијске трансакције које се дешавају током пројекта.</span><span class="sxs-lookup"><span data-stu-id="89abf-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="89abf-134">Ове трансакције се евидентирају као **стварне вредности**.</span><span class="sxs-lookup"><span data-stu-id="89abf-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="89abf-135">Следеће табеле приказују различите врсте стварних вредности које се креирају, зависно од тога да ли је пројекат заснован на времену и материјалима или пројекат са фиксном ценом, да ли је у фази предпродаје или је интерни пројекат.</span><span class="sxs-lookup"><span data-stu-id="89abf-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="89abf-136">**Ресурс припада истој организационој јединици као и уговорна јединица пројекта**</span><span class="sxs-lookup"><span data-stu-id="89abf-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="89abf-137">Догађај</span><span class="sxs-lookup"><span data-stu-id="89abf-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="89abf-138">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="89abf-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="89abf-139">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="89abf-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="89abf-140">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="89abf-141">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="89abf-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="89abf-142">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="89abf-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="89abf-143">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="89abf-143">Actuals</span></span></th>
<th><span data-ttu-id="89abf-144">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="89abf-144">Transaction currency</span></span></th>
<th><span data-ttu-id="89abf-145">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="89abf-145">Fixed price</span></span></th>
<th><span data-ttu-id="89abf-146">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="89abf-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="89abf-147">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="89abf-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="89abf-148">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="89abf-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-149">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="89abf-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="89abf-150">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="89abf-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="89abf-151">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="89abf-152">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-152">Cost actual</span></span></td>
<td><span data-ttu-id="89abf-153">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-154">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-155">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="89abf-156">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-157">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-158">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="89abf-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="89abf-159">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="89abf-160">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="89abf-161">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-161">Cost actual</span></span></td>
<td><span data-ttu-id="89abf-162">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-163">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-164">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-165">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-166">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-167">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="89abf-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="89abf-168">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-169">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="89abf-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="89abf-170">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="89abf-171">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="89abf-172">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="89abf-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="89abf-173">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-174">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="89abf-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-175">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-176">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-177">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-178">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="89abf-178">Billed sales</span></span></td>
<td><span data-ttu-id="89abf-179">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="89abf-180">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="89abf-181">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="89abf-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="89abf-182">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-183">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-184">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-185">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-186">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-187">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="89abf-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="89abf-188">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-189">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="89abf-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="89abf-190">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="89abf-191">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="89abf-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="89abf-192">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="89abf-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="89abf-193">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="89abf-194">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="89abf-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="89abf-195">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="89abf-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="89abf-196">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-197">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-198">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-199">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="89abf-199">Billed sales</span></span></td>
<td><span data-ttu-id="89abf-200">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="89abf-201">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="89abf-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="89abf-202">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="89abf-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="89abf-203">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-204">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="89abf-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="89abf-205">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-206">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="89abf-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="89abf-207">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="89abf-208">**Ресурс припада организационој јединици која се разликује од уговорне јединице пројекта**</span><span class="sxs-lookup"><span data-stu-id="89abf-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="89abf-209">Догађај</span><span class="sxs-lookup"><span data-stu-id="89abf-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="89abf-210">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="89abf-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="89abf-211">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="89abf-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="89abf-212">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="89abf-213">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="89abf-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="89abf-214">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="89abf-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="89abf-215">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="89abf-215">Actuals</span></span></th>
<th><span data-ttu-id="89abf-216">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="89abf-216">Transaction currency</span></span></th>
<th><span data-ttu-id="89abf-217">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="89abf-217">Fixed price</span></span></th>
<th><span data-ttu-id="89abf-218">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="89abf-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="89abf-219">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="89abf-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="89abf-220">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="89abf-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-221">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="89abf-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="89abf-222">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="89abf-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="89abf-223">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="89abf-224">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-224">Cost actual</span></span></td>
<td><span data-ttu-id="89abf-225">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="89abf-226">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="89abf-227">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="89abf-228">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="89abf-229">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-230">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="89abf-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="89abf-231">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-232">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="89abf-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="89abf-233">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="89abf-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-234">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="89abf-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="89abf-235">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="89abf-236">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="89abf-237">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-237">Cost actual</span></span></td>
<td><span data-ttu-id="89abf-238">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-239">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-240">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-241">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-242">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="89abf-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-243">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="89abf-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="89abf-244">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="89abf-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-245">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="89abf-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="89abf-246">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="89abf-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-247">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="89abf-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="89abf-248">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-249">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="89abf-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="89abf-250">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="89abf-251">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="89abf-252">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="89abf-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="89abf-253">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-254">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="89abf-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-255">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-256">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="89abf-257">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-258">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="89abf-258">Billed sales</span></span></td>
<td><span data-ttu-id="89abf-259">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="89abf-260">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="89abf-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="89abf-261">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="89abf-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="89abf-262">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-263">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-264">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-265">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="89abf-266">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-267">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="89abf-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="89abf-268">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-269">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="89abf-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="89abf-270">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="89abf-271">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="89abf-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="89abf-272">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="89abf-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="89abf-273">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="89abf-274">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="89abf-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="89abf-275">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="89abf-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="89abf-276">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-277">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="89abf-278">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="89abf-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-279">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="89abf-279">Billed sales</span></span></td>
<td><span data-ttu-id="89abf-280">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="89abf-281">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="89abf-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="89abf-282">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="89abf-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="89abf-283">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-284">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="89abf-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="89abf-285">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="89abf-286">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="89abf-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="89abf-287">Уговорна валута за пројекат</span><span class="sxs-lookup"><span data-stu-id="89abf-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
