---
title: Преглед тренутног стања
description: Ова тема пружа информације о стварним вредностима пројекта.
author: rumant
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 63ad6544f0ec0a893aebd8d81f3ee895e51c294e
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146141"
---
# <a name="actuals-overview"></a><span data-ttu-id="37ebc-103">Преглед тренутног стања</span><span class="sxs-lookup"><span data-stu-id="37ebc-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="37ebc-104">Стварне вредности представљају количину посла која је завршена за пројекат.</span><span class="sxs-lookup"><span data-stu-id="37ebc-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="37ebc-105">Стварне вредности пројекта могу да се прате до његових изворних докумената.</span><span class="sxs-lookup"><span data-stu-id="37ebc-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="37ebc-106">Ти изворни документи укључују време, трошкове и ставке књижења у главној књизи, као и фактуре.</span><span class="sxs-lookup"><span data-stu-id="37ebc-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Како се стварне вредности пројекта прате до изворних докумената](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="37ebc-108">Прослеђивање ставке времена</span><span class="sxs-lookup"><span data-stu-id="37ebc-108">Submitting a time entry</span></span>

<span data-ttu-id="37ebc-109">Код апликације PSA, када се ставка времена проследи за пројекат који је мапиран на предмет уговора о времену и материјалима, креирају се две ставке у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="37ebc-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="37ebc-110">Једна ставка је за трошкове, а друга за ненаплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="37ebc-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="37ebc-111">Када се ставка времена проследи за пројекат који је мапиран на предмет уговора о фиксној цени, креира се ставка у главној књизи само за трошкове.</span><span class="sxs-lookup"><span data-stu-id="37ebc-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="37ebc-112">Логику за унос подразумеваних цена можете да пронађете у ставки у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="37ebc-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="37ebc-113">Све вредности поља из ставке времена копирају се у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="37ebc-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="37ebc-114">Ова поља укључују датум трансакције, предмет уговора на који је пројекат мапиран и валуту која је резултат одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="37ebc-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="37ebc-115">Поља која утичу на подразумеване цене, као што су **Улога** и **Организациона јединица** проузрокују подразумевани унос одговарајуће цене у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="37ebc-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="37ebc-116">Ако у ставку времена додате прилагођено поље, а желите да се вредност поља шири на стварне вредности, креирајте поље у ентитету Стварне вредности и употребите пресликавања поља да бисте копирали поље из ставке времена у стварну вредност.</span><span class="sxs-lookup"><span data-stu-id="37ebc-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="37ebc-117">Прослеђивање ставке трошка</span><span class="sxs-lookup"><span data-stu-id="37ebc-117">Submitting an expense entry</span></span>

<span data-ttu-id="37ebc-118">Код апликације PSA, када се ставка трошка проследи за пројекат који је мапиран на предмет уговора о времену и материјалима, креирају се две ставке у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="37ebc-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="37ebc-119">Једна ставка је за трошкове, а друга за ненаплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="37ebc-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="37ebc-120">Када се ставка трошка проследи за пројекат који је мапиран на предмет уговора о фиксној цени, креира се ставка у главној књизи само за трошкове.</span><span class="sxs-lookup"><span data-stu-id="37ebc-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="37ebc-121">Логика за унос подразумеваних цена за трошкове темељи се на категорији трошкова која је изабрана на страници **Ставка трошкова**.</span><span class="sxs-lookup"><span data-stu-id="37ebc-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="37ebc-122">Датум трансакције, предмет уговора на који је пројекат мапиран и валуту се користе за одређивање одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="37ebc-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="37ebc-123">Међутим, за саму цену, износ који је корисник унео подразумевано се подешава директно на повезаним ставкама трошкова у главној књизи за трошкове и продају.</span><span class="sxs-lookup"><span data-stu-id="37ebc-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="37ebc-124">У тренутној верзији апликације PSA, није доступна ставка заснована на категорији подразумеваних цена по јединици за ставке трошкова.</span><span class="sxs-lookup"><span data-stu-id="37ebc-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="37ebc-125">Коришћење улазних главних књига за евидентирање трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="37ebc-126">У апликацији PSA, улазне главне књиге вам омогућавају да евидентирате трошкове или приход у класама материјала, накнаде, времена, трошкова или пореских трансакција.</span><span class="sxs-lookup"><span data-stu-id="37ebc-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="37ebc-127">Главна књига има заглавље, ставке и радњу **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="37ebc-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="37ebc-128">Ево неколико сценарија где можете да користите главну књигу:</span><span class="sxs-lookup"><span data-stu-id="37ebc-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="37ebc-129">Морате забележити стварне трошкове и продају материјала на пројекту.</span><span class="sxs-lookup"><span data-stu-id="37ebc-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="37ebc-130">Морате преместити стварне вредности трансакција из другог система у PSA.</span><span class="sxs-lookup"><span data-stu-id="37ebc-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="37ebc-131">Морате да евидентирате трошкове остварене у другом систему, као што су трошкови набавке или подуговарања.</span><span class="sxs-lookup"><span data-stu-id="37ebc-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="37ebc-132">Коришћење улазних главних књига за креирање стварних података треба да ради само корисник који је у потпуности свестан рачуноводственог утицаја који стварни људи имају на пројекат.</span><span class="sxs-lookup"><span data-stu-id="37ebc-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="37ebc-133">То је зато што апликација не потврђује ваљаност типа ставке у главној књизи или сродну цену која се уноси у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="37ebc-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="37ebc-134">Због утицаја овог типа главне књиге, будите опрезни по питању коме је омогућен приступ креирања улазних главних књига.</span><span class="sxs-lookup"><span data-stu-id="37ebc-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="37ebc-135">Евидентирање стварних вредности на основу догађаја у пројекту</span><span class="sxs-lookup"><span data-stu-id="37ebc-135">Recording actuals based on project events</span></span>

<span data-ttu-id="37ebc-136">PSA бележи финансијске трансакције које се дешавају током пројекта.</span><span class="sxs-lookup"><span data-stu-id="37ebc-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="37ebc-137">Ове трансакције се евидентирају као **стварне вредности**.</span><span class="sxs-lookup"><span data-stu-id="37ebc-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="37ebc-138">Следеће табеле приказују различите врсте стварних вредности које се креирају, зависно од тога да ли је пројекат заснован на времену и материјалима или пројекат са фиксном ценом, да ли је у фази предпродаје или је интерни пројекат.</span><span class="sxs-lookup"><span data-stu-id="37ebc-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="37ebc-139">**Ресурс припада истој организационој јединици као и уговорна јединица пројекта**</span><span class="sxs-lookup"><span data-stu-id="37ebc-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="37ebc-140">Догађај</span><span class="sxs-lookup"><span data-stu-id="37ebc-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="37ebc-141">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="37ebc-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="37ebc-142">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="37ebc-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="37ebc-143">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="37ebc-144">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="37ebc-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="37ebc-145">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="37ebc-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="37ebc-146">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="37ebc-146">Actuals</span></span></th>
<th><span data-ttu-id="37ebc-147">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="37ebc-147">Transaction currency</span></span></th>
<th><span data-ttu-id="37ebc-148">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="37ebc-148">Fixed price</span></span></th>
<th><span data-ttu-id="37ebc-149">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="37ebc-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="37ebc-150">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="37ebc-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="37ebc-151">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="37ebc-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-152">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="37ebc-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="37ebc-153">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="37ebc-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="37ebc-154">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="37ebc-155">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-155">Cost actual</span></span></td>
<td><span data-ttu-id="37ebc-156">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-157">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-158">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="37ebc-159">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-160">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-161">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="37ebc-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="37ebc-162">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="37ebc-163">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="37ebc-164">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-164">Cost actual</span></span></td>
<td><span data-ttu-id="37ebc-165">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-166">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-167">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-168">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-169">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-170">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="37ebc-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="37ebc-171">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-172">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="37ebc-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="37ebc-173">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="37ebc-174">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="37ebc-175">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="37ebc-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="37ebc-176">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-177">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="37ebc-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-178">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-179">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-180">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-181">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="37ebc-181">Billed sales</span></span></td>
<td><span data-ttu-id="37ebc-182">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="37ebc-183">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="37ebc-184">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="37ebc-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="37ebc-185">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-186">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-187">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-188">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-189">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-190">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="37ebc-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="37ebc-191">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-192">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="37ebc-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="37ebc-193">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="37ebc-194">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="37ebc-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="37ebc-195">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="37ebc-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="37ebc-196">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="37ebc-197">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="37ebc-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="37ebc-198">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="37ebc-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="37ebc-199">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-200">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-201">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-202">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="37ebc-202">Billed sales</span></span></td>
<td><span data-ttu-id="37ebc-203">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="37ebc-204">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="37ebc-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="37ebc-205">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="37ebc-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="37ebc-206">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-207">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="37ebc-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="37ebc-208">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-209">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="37ebc-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="37ebc-210">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="37ebc-211">**Ресурс припада организационој јединици која се разликује од уговорне јединице пројекта**</span><span class="sxs-lookup"><span data-stu-id="37ebc-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="37ebc-212">Догађај</span><span class="sxs-lookup"><span data-stu-id="37ebc-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="37ebc-213">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="37ebc-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="37ebc-214">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="37ebc-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="37ebc-215">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="37ebc-216">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="37ebc-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="37ebc-217">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="37ebc-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="37ebc-218">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="37ebc-218">Actuals</span></span></th>
<th><span data-ttu-id="37ebc-219">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="37ebc-219">Transaction currency</span></span></th>
<th><span data-ttu-id="37ebc-220">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="37ebc-220">Fixed price</span></span></th>
<th><span data-ttu-id="37ebc-221">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="37ebc-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="37ebc-222">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="37ebc-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="37ebc-223">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="37ebc-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-224">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="37ebc-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="37ebc-225">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="37ebc-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="37ebc-226">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="37ebc-227">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-227">Cost actual</span></span></td>
<td><span data-ttu-id="37ebc-228">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="37ebc-229">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="37ebc-230">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="37ebc-231">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="37ebc-232">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-233">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="37ebc-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="37ebc-234">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-235">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="37ebc-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="37ebc-236">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="37ebc-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-237">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="37ebc-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="37ebc-238">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="37ebc-239">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="37ebc-240">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-240">Cost actual</span></span></td>
<td><span data-ttu-id="37ebc-241">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-242">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-243">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-244">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-245">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="37ebc-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-246">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="37ebc-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="37ebc-247">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="37ebc-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-248">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="37ebc-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="37ebc-249">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="37ebc-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-250">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="37ebc-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="37ebc-251">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-252">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="37ebc-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="37ebc-253">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="37ebc-254">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="37ebc-255">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="37ebc-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="37ebc-256">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-257">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="37ebc-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-258">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-259">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="37ebc-260">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-261">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="37ebc-261">Billed sales</span></span></td>
<td><span data-ttu-id="37ebc-262">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="37ebc-263">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="37ebc-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="37ebc-264">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="37ebc-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="37ebc-265">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-266">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-267">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-268">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="37ebc-269">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-270">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="37ebc-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="37ebc-271">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-272">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="37ebc-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="37ebc-273">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="37ebc-274">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="37ebc-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="37ebc-275">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="37ebc-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="37ebc-276">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="37ebc-277">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="37ebc-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="37ebc-278">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="37ebc-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="37ebc-279">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-280">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="37ebc-281">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="37ebc-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-282">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="37ebc-282">Billed sales</span></span></td>
<td><span data-ttu-id="37ebc-283">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="37ebc-284">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="37ebc-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="37ebc-285">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="37ebc-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="37ebc-286">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-287">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="37ebc-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="37ebc-288">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="37ebc-289">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="37ebc-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="37ebc-290">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="37ebc-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
