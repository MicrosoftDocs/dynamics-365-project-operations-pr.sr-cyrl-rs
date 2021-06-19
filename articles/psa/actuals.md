---
title: Преглед тренутног стања
description: Ова тема пружа информације о стварним вредностима пројекта.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
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
ms.openlocfilehash: 73f1b14bbb4cc53111a1b3a93756a86db04475ab
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014674"
---
# <a name="actuals-overview"></a><span data-ttu-id="ec0b3-103">Преглед тренутног стања</span><span class="sxs-lookup"><span data-stu-id="ec0b3-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ec0b3-104">Стварне вредности представљају количину посла која је завршена за пројекат.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="ec0b3-105">Стварне вредности пројекта могу да се прате до његових изворних докумената.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="ec0b3-106">Ти изворни документи укључују време, трошкове и ставке књижења у главној књизи, као и фактуре.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Како се стварне вредности пројекта прате до изворних докумената](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="ec0b3-108">Прослеђивање ставке времена</span><span class="sxs-lookup"><span data-stu-id="ec0b3-108">Submitting a time entry</span></span>

<span data-ttu-id="ec0b3-109">Код апликације PSA, када се ставка времена проследи за пројекат који је мапиран на предмет уговора о времену и материјалима, креирају се две ставке у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="ec0b3-110">Једна ставка је за трошкове, а друга за ненаплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="ec0b3-111">Када се ставка времена проследи за пројекат који је мапиран на предмет уговора о фиксној цени, креира се ставка у главној књизи само за трошкове.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="ec0b3-112">Логику за унос подразумеваних цена можете да пронађете у ставки у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="ec0b3-113">Све вредности поља из ставке времена копирају се у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="ec0b3-114">Ова поља укључују датум трансакције, предмет уговора на који је пројекат мапиран и валуту која је резултат одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="ec0b3-115">Поља која утичу на подразумеване цене, као што су **Улога** и **Организациона јединица** проузрокују подразумевани унос одговарајуће цене у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="ec0b3-116">Ако у ставку времена додате прилагођено поље, а желите да се вредност поља шири на стварне вредности, креирајте поље у ентитету Стварне вредности и употребите пресликавања поља да бисте копирали поље из ставке времена у стварну вредност.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="ec0b3-117">Прослеђивање ставке трошка</span><span class="sxs-lookup"><span data-stu-id="ec0b3-117">Submitting an expense entry</span></span>

<span data-ttu-id="ec0b3-118">Код апликације PSA, када се ставка трошка проследи за пројекат који је мапиран на предмет уговора о времену и материјалима, креирају се две ставке у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="ec0b3-119">Једна ставка је за трошкове, а друга за ненаплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="ec0b3-120">Када се ставка трошка проследи за пројекат који је мапиран на предмет уговора о фиксној цени, креира се ставка у главној књизи само за трошкове.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="ec0b3-121">Логика за унос подразумеваних цена за трошкове темељи се на категорији трошкова која је изабрана на страници **Ставка трошкова**.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="ec0b3-122">Датум трансакције, предмет уговора на који је пројекат мапиран и валуту се користе за одређивање одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="ec0b3-123">Међутим, за саму цену, износ који је корисник унео подразумевано се подешава директно на повезаним ставкама трошкова у главној књизи за трошкове и продају.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="ec0b3-124">У тренутној верзији апликације PSA, није доступна ставка заснована на категорији подразумеваних цена по јединици за ставке трошкова.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="ec0b3-125">Коришћење улазних главних књига за евидентирање трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="ec0b3-126">У апликацији PSA, улазне главне књиге вам омогућавају да евидентирате трошкове или приход у класама материјала, накнаде, времена, трошкова или пореских трансакција.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="ec0b3-127">Главна књига има заглавље, ставке и радњу **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="ec0b3-128">Ево неколико сценарија где можете да користите главну књигу:</span><span class="sxs-lookup"><span data-stu-id="ec0b3-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="ec0b3-129">Морате забележити стварне трошкове и продају материјала на пројекту.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="ec0b3-130">Морате преместити стварне вредности трансакција из другог система у PSA.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="ec0b3-131">Морате да евидентирате трошкове остварене у другом систему, као што су трошкови набавке или подуговарања.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ec0b3-132">Коришћење улазних главних књига за креирање стварних података треба да ради само корисник који је у потпуности свестан рачуноводственог утицаја који стварни људи имају на пројекат.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="ec0b3-133">То је зато што апликација не потврђује ваљаност типа ставке у главној књизи или сродну цену која се уноси у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="ec0b3-134">Због утицаја овог типа главне књиге, будите опрезни по питању коме је омогућен приступ креирања улазних главних књига.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="ec0b3-135">Евидентирање стварних вредности на основу догађаја у пројекту</span><span class="sxs-lookup"><span data-stu-id="ec0b3-135">Recording actuals based on project events</span></span>

<span data-ttu-id="ec0b3-136">PSA бележи финансијске трансакције које се дешавају током пројекта.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="ec0b3-137">Ове трансакције се евидентирају као **стварне вредности**.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="ec0b3-138">Следеће табеле приказују различите врсте стварних вредности које се креирају, зависно од тога да ли је пројекат заснован на времену и материјалима или пројекат са фиксном ценом, да ли је у фази предпродаје или је интерни пројекат.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="ec0b3-139">**Ресурс припада истој организационој јединици као и уговорна јединица пројекта**</span><span class="sxs-lookup"><span data-stu-id="ec0b3-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ec0b3-140">Догађај</span><span class="sxs-lookup"><span data-stu-id="ec0b3-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ec0b3-141">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="ec0b3-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ec0b3-142">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="ec0b3-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ec0b3-143">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ec0b3-144">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="ec0b3-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ec0b3-145">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="ec0b3-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ec0b3-146">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="ec0b3-146">Actuals</span></span></th>
<th><span data-ttu-id="ec0b3-147">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="ec0b3-147">Transaction currency</span></span></th>
<th><span data-ttu-id="ec0b3-148">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="ec0b3-148">Fixed price</span></span></th>
<th><span data-ttu-id="ec0b3-149">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="ec0b3-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ec0b3-150">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ec0b3-151">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="ec0b3-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-152">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ec0b3-153">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="ec0b3-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ec0b3-154">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ec0b3-155">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-155">Cost actual</span></span></td>
<td><span data-ttu-id="ec0b3-156">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-157">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-158">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="ec0b3-159">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-160">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-161">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="ec0b3-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ec0b3-162">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ec0b3-163">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ec0b3-164">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-164">Cost actual</span></span></td>
<td><span data-ttu-id="ec0b3-165">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-166">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-167">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-168">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-169">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-170">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="ec0b3-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ec0b3-171">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-172">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="ec0b3-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ec0b3-173">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ec0b3-174">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ec0b3-175">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="ec0b3-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ec0b3-176">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-177">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="ec0b3-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-178">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-179">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-180">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-181">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="ec0b3-181">Billed sales</span></span></td>
<td><span data-ttu-id="ec0b3-182">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ec0b3-183">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ec0b3-184">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="ec0b3-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ec0b3-185">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-186">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-187">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-188">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-189">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-190">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="ec0b3-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ec0b3-191">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-192">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="ec0b3-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ec0b3-193">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ec0b3-194">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ec0b3-195">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="ec0b3-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ec0b3-196">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ec0b3-197">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="ec0b3-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ec0b3-198">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="ec0b3-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ec0b3-199">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-200">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-201">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-202">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="ec0b3-202">Billed sales</span></span></td>
<td><span data-ttu-id="ec0b3-203">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ec0b3-204">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ec0b3-205">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="ec0b3-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ec0b3-206">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-207">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="ec0b3-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ec0b3-208">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-209">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="ec0b3-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ec0b3-210">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="ec0b3-211">**Ресурс припада организационој јединици која се разликује од уговорне јединице пројекта**</span><span class="sxs-lookup"><span data-stu-id="ec0b3-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ec0b3-212">Догађај</span><span class="sxs-lookup"><span data-stu-id="ec0b3-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ec0b3-213">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="ec0b3-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ec0b3-214">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="ec0b3-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ec0b3-215">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ec0b3-216">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="ec0b3-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ec0b3-217">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="ec0b3-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ec0b3-218">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="ec0b3-218">Actuals</span></span></th>
<th><span data-ttu-id="ec0b3-219">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="ec0b3-219">Transaction currency</span></span></th>
<th><span data-ttu-id="ec0b3-220">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="ec0b3-220">Fixed price</span></span></th>
<th><span data-ttu-id="ec0b3-221">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="ec0b3-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ec0b3-222">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ec0b3-223">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="ec0b3-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-224">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ec0b3-225">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="ec0b3-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="ec0b3-226">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ec0b3-227">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-227">Cost actual</span></span></td>
<td><span data-ttu-id="ec0b3-228">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ec0b3-229">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ec0b3-230">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ec0b3-231">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ec0b3-232">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-233">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="ec0b3-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ec0b3-234">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-235">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="ec0b3-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ec0b3-236">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="ec0b3-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-237">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="ec0b3-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ec0b3-238">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="ec0b3-239">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ec0b3-240">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-240">Cost actual</span></span></td>
<td><span data-ttu-id="ec0b3-241">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-242">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-243">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-244">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-245">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="ec0b3-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-246">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="ec0b3-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ec0b3-247">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="ec0b3-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-248">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="ec0b3-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ec0b3-249">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="ec0b3-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-250">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="ec0b3-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ec0b3-251">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-252">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="ec0b3-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ec0b3-253">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ec0b3-254">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ec0b3-255">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="ec0b3-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ec0b3-256">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-257">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="ec0b3-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-258">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-259">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ec0b3-260">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-261">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="ec0b3-261">Billed sales</span></span></td>
<td><span data-ttu-id="ec0b3-262">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ec0b3-263">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ec0b3-264">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="ec0b3-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ec0b3-265">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-266">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-267">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-268">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ec0b3-269">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-270">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="ec0b3-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ec0b3-271">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-272">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="ec0b3-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ec0b3-273">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ec0b3-274">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ec0b3-275">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="ec0b3-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ec0b3-276">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ec0b3-277">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="ec0b3-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ec0b3-278">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="ec0b3-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ec0b3-279">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-280">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ec0b3-281">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="ec0b3-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-282">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="ec0b3-282">Billed sales</span></span></td>
<td><span data-ttu-id="ec0b3-283">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ec0b3-284">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="ec0b3-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ec0b3-285">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="ec0b3-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ec0b3-286">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-287">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="ec0b3-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ec0b3-288">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ec0b3-289">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="ec0b3-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ec0b3-290">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0b3-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]