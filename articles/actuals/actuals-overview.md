---
title: Тренутно стање
description: Ова тема пружа информације о томе како се ради са стварним подацима у услузи Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: intro-internal
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9e046602a3005930c41ab8c50472d5b1a72303c6
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368629"
---
# <a name="actuals"></a><span data-ttu-id="c9632-103">Тренутно стање</span><span class="sxs-lookup"><span data-stu-id="c9632-103">Actuals</span></span> 

<span data-ttu-id="c9632-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="c9632-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c9632-105">Тренутно стање представља прегледани и одобрени финансијски и временски распоред пројекта.</span><span class="sxs-lookup"><span data-stu-id="c9632-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="c9632-106">Креира се као резултат одобравања времена, трошкова, ставки употребе материјала, ставки дневника и фактура.</span><span class="sxs-lookup"><span data-stu-id="c9632-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="c9632-107">Ставке у главној књизи и време предаје</span><span class="sxs-lookup"><span data-stu-id="c9632-107">Journal lines and time submission</span></span>

<span data-ttu-id="c9632-108">За више информација о ставци времена, погледајте [Преглед уноса времена](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c9632-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="c9632-109">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="c9632-109">Time and materials</span></span>

<span data-ttu-id="c9632-110">Када је ставка времена која је прослеђена повезана са пројектом који је мапиран у предмет уговора о времену и материјалима, систем креира две ставке у главној књизи, једну за трошкове и једну за ненаплаћену продају.</span><span class="sxs-lookup"><span data-stu-id="c9632-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="c9632-111">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c9632-111">Fixed price</span></span>

<span data-ttu-id="c9632-112">Када се прослеђена ставка времена повеже са пројектом који се мапиран на предмет уговора са фиксном ценом, систем креира једну ставку у главној књизи за трошкове.</span><span class="sxs-lookup"><span data-stu-id="c9632-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="c9632-113">Подразумевано одређивање цена</span><span class="sxs-lookup"><span data-stu-id="c9632-113">Default pricing</span></span>

<span data-ttu-id="c9632-114">Логика за креирање подразумеваних цена се налази у ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="c9632-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="c9632-115">Вредности поља из ставке времена копирају се у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="c9632-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="c9632-116">Ове вредности укључују датум трансакције, предмет уговора на који је пројекат мапиран и валуту која је резултат одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="c9632-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="c9632-117">Поља која утичу на подразумеване цене, као што су **Улога** и **Јединица за одређивање ресурса**, користе се за утврђивање одговарајуће цене у ставки у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="c9632-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="c9632-118">На ставку времена можете додати прилагођено поље.</span><span class="sxs-lookup"><span data-stu-id="c9632-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="c9632-119">Ако желите да се вредност поља шири на тренутно стање, креирајте поље у табелама **Тренутно стање** и **Ставка у главној књизи**.</span><span class="sxs-lookup"><span data-stu-id="c9632-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="c9632-120">Користите прилагођени кôд за ширење изабране вредности поља из ставку времена у тренутно стање путем ставке у главној књизи користећи порекло трансакција.</span><span class="sxs-lookup"><span data-stu-id="c9632-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="c9632-121">За више информација о пореклу трансакција и везама, погледајте [Повезивање тренутног стања са оригиналним записима](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="c9632-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="c9632-122">Прослеђивање ставки у главној књизи и основних трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="c9632-123">За више информација о ставци трошка, погледајте [Преглед трошкова](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c9632-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="c9632-124">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="c9632-124">Time and materials</span></span>

<span data-ttu-id="c9632-125">Када се ставка основног трошка која је прослеђена повеже са пројектом који је мапиран у предмет уговора о времену и материјалима, систем креира две ставке у главној књизи, једну за трошкове и једну за ненаплаћену продају.</span><span class="sxs-lookup"><span data-stu-id="c9632-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="c9632-126">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c9632-126">Fixed price</span></span>

<span data-ttu-id="c9632-127">Када се прослеђена ставка трошка повеже са пројектом који се мапира на предмет уговора о фиксној цени, систем креира једну ставку у главној књизи за трошкове.</span><span class="sxs-lookup"><span data-stu-id="c9632-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="c9632-128">Подразумевано одређивање цена</span><span class="sxs-lookup"><span data-stu-id="c9632-128">Default pricing</span></span>

<span data-ttu-id="c9632-129">Логика уношења задатих цена за трошкове заснива се на категорији трошкова.</span><span class="sxs-lookup"><span data-stu-id="c9632-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="c9632-130">Датум трансакције, предмет уговора на који је пројекат мапиран и валута се користе за одређивање одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="c9632-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="c9632-131">Поља која утичу на подразумеване цене, као што су **Категорија трансакције** и **Јединица**, користе се за утврђивање одговарајуће цене у ставки у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="c9632-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="c9632-132">Међутим, то функционише само када је метода одређивања цена у ценовнику **Цена по јединици**.</span><span class="sxs-lookup"><span data-stu-id="c9632-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="c9632-133">Ако је метода одређивања цена **По цени** или **Провизија преко трошкова**, цена која се уноси када се креира ставка трошкова користи се као трошак, а цена ставке у главној књизи продаје израчунава се на основу методе одређивања цена.</span><span class="sxs-lookup"><span data-stu-id="c9632-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="c9632-134">На ставку трошкова можете додати прилагођено поље.</span><span class="sxs-lookup"><span data-stu-id="c9632-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="c9632-135">Ако желите да се вредност поља шири на тренутно стање, креирајте поље у табелама **Тренутно стање** и **Ставка у главној књизи**.</span><span class="sxs-lookup"><span data-stu-id="c9632-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="c9632-136">Користите прилагођени кôд за ширење изабране вредности поља из ставку времена у тренутно стање путем ставке у главној књизи користећи порекло трансакција.</span><span class="sxs-lookup"><span data-stu-id="c9632-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="c9632-137">За више информација о пореклу трансакција и везама, погледајте [Повезивање тренутног стања са оригиналним записима](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="c9632-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="c9632-138">Ставке у главној књизи и прослеђивање евиденције употребе материјала</span><span class="sxs-lookup"><span data-stu-id="c9632-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="c9632-139">За више информација о ставци трошкова, погледајте [Дневник употребе материјала](../material/material-usage-log.md).</span><span class="sxs-lookup"><span data-stu-id="c9632-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="c9632-140">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="c9632-140">Time and materials</span></span>

<span data-ttu-id="c9632-141">Када се прослеђена ставка евиденције употребе материјала повеже са пројектом који се мапира у предмет уговора о времену и материјалима, систем креира две ставке у главној књизи, једну за трошкове и једну за нефактурисану продају.</span><span class="sxs-lookup"><span data-stu-id="c9632-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="c9632-142">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c9632-142">Fixed price</span></span>

<span data-ttu-id="c9632-143">Када се прослеђена ставка евиденције употребе материјала повеже са пројектом који се мапира на предмет уговора о фиксној цени, систем креира једну ставку у главној књизи за трошкове.</span><span class="sxs-lookup"><span data-stu-id="c9632-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="c9632-144">Подразумевано одређивање цена</span><span class="sxs-lookup"><span data-stu-id="c9632-144">Default pricing</span></span>

<span data-ttu-id="c9632-145">Логика уношења задатих цена материјала заснива се на комбинацији производа и јединице.</span><span class="sxs-lookup"><span data-stu-id="c9632-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="c9632-146">Датум трансакције, предмет уговора на који је пројекат мапиран и валута се користе за одређивање одговарајућег ценовника.</span><span class="sxs-lookup"><span data-stu-id="c9632-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="c9632-147">Поља која утичу на подразумеване цене, као што су **ID производа** и **Јединица**, користе се за утврђивање одговарајуће цене у ставки у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="c9632-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="c9632-148">Међутим, ово важи само за каталошке производе.</span><span class="sxs-lookup"><span data-stu-id="c9632-148">However, this only works for catalog products.</span></span> <span data-ttu-id="c9632-149">За производе који се додају ручно, цена која се уноси када се креира ставка евиденције употребе материјала користи се за трошкове и продајну цену у ставкама у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="c9632-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="c9632-150">На ставку **Евиденција употребе материјала** можете додати прилагођено поље.</span><span class="sxs-lookup"><span data-stu-id="c9632-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="c9632-151">Ако желите да се вредност поља шири на тренутно стање, креирајте поље у табелама **Тренутно стање** и **Ставка у главној књизи**.</span><span class="sxs-lookup"><span data-stu-id="c9632-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="c9632-152">Користите прилагођени кôд за ширење изабране вредности поља из ставку времена у тренутно стање путем ставке у главној књизи користећи порекло трансакција.</span><span class="sxs-lookup"><span data-stu-id="c9632-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="c9632-153">За више информација о пореклу трансакција и везама, погледајте [Повезивање тренутног стања са оригиналним записима](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="c9632-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="c9632-154">Коришћење дневника за књижење за евидентирање трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-154">Use entry journals to record costs</span></span>

<span data-ttu-id="c9632-155">Можете да користите дневнике за књижење да евидентирате трошкове или приход у класама материјала, накнаде, времена, трошкова или пореских трансакција.</span><span class="sxs-lookup"><span data-stu-id="c9632-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="c9632-156">Дневници се могу користити у следеће сврхе:</span><span class="sxs-lookup"><span data-stu-id="c9632-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="c9632-157">Преместите стварне вредности трансакција из другог система у Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="c9632-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="c9632-158">Евидентирајте трошкове који су се догодили у другом систему.</span><span class="sxs-lookup"><span data-stu-id="c9632-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="c9632-159">Ови трошкови могу укључивати трошкове набавке или подуговарања.</span><span class="sxs-lookup"><span data-stu-id="c9632-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c9632-160">Апликација не потврђује тип ставке у главној књизи или повезано одређивање цена које се уноси у ставку у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="c9632-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="c9632-161">Стога само корисник који је потпуно свестан рачуноводственог утицаја који стварне вредности имају на пројекат треба да користи дневнике за књижење за креирање стварних података.</span><span class="sxs-lookup"><span data-stu-id="c9632-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="c9632-162">Због утицаја овог типа дневника, пажљиво бирајте ко има приступ креирању дневника за књижење.</span><span class="sxs-lookup"><span data-stu-id="c9632-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="c9632-163">Евидентирање стварних вредности на основу догађаја у пројекту</span><span class="sxs-lookup"><span data-stu-id="c9632-163">Record actuals based on project events</span></span>

<span data-ttu-id="c9632-164">Project Operations бележи финансијске трансакције које се дешавају током пројекта.</span><span class="sxs-lookup"><span data-stu-id="c9632-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="c9632-165">Ове трансакције се евидентирају као стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="c9632-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="c9632-166">Следеће табеле приказују различите врсте стварних вредности које се креирају, зависно од тога да ли је пројекат заснован на времену и материјалима или пројекат са фиксном ценом, да ли је у фази предпродаје или је интерни пројекат.</span><span class="sxs-lookup"><span data-stu-id="c9632-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="c9632-167">Ресурс припада истој организационој јединици као и уговорна јединица пројекта</span><span class="sxs-lookup"><span data-stu-id="c9632-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="c9632-168">Догађај</span><span class="sxs-lookup"><span data-stu-id="c9632-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="c9632-169">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="c9632-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="c9632-170">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="c9632-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="c9632-171">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="c9632-172">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="c9632-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="c9632-173">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c9632-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="c9632-174">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="c9632-174">Actuals</span></span></th>
<th><span data-ttu-id="c9632-175">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="c9632-175">Transaction currency</span></span></th>
<th><span data-ttu-id="c9632-176">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c9632-176">Fixed price</span></span></th>
<th><span data-ttu-id="c9632-177">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="c9632-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="c9632-178">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="c9632-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="c9632-179">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="c9632-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-180">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="c9632-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="c9632-181">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="c9632-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="c9632-182">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="c9632-183">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-183">Cost actual</span></span></td>
<td><span data-ttu-id="c9632-184">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-185">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-186">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="c9632-187">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-188">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-189">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="c9632-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="c9632-190">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="c9632-191">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="c9632-192">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-192">Cost actual</span></span></td>
<td><span data-ttu-id="c9632-193">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-194">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-195">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-196">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-197">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-198">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="c9632-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="c9632-199">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-200">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="c9632-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="c9632-201">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="c9632-202">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="c9632-203">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="c9632-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="c9632-204">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-205">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="c9632-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-206">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-207">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-208">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-209">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="c9632-209">Billed sales</span></span></td>
<td><span data-ttu-id="c9632-210">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="c9632-211">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="c9632-212">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="c9632-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="c9632-213">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-214">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-215">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-216">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-217">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-218">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="c9632-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="c9632-219">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-220">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="c9632-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="c9632-221">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="c9632-222">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="c9632-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="c9632-223">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="c9632-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="c9632-224">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="c9632-225">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="c9632-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="c9632-226">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="c9632-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="c9632-227">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-228">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-229">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-230">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="c9632-230">Billed sales</span></span></td>
<td><span data-ttu-id="c9632-231">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="c9632-232">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="c9632-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="c9632-233">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="c9632-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="c9632-234">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-235">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="c9632-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="c9632-236">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-237">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="c9632-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="c9632-238">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="c9632-239">Ресурс припада организационој јединици која се разликује од уговорне јединице пројекта</span><span class="sxs-lookup"><span data-stu-id="c9632-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="c9632-240">Догађај</span><span class="sxs-lookup"><span data-stu-id="c9632-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="c9632-241">Пројекат који се може наплатити или продати</span><span class="sxs-lookup"><span data-stu-id="c9632-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="c9632-242">Пројекат у фази предпродаје</span><span class="sxs-lookup"><span data-stu-id="c9632-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="c9632-243">Интерни пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="c9632-244">Време и материјали</span><span class="sxs-lookup"><span data-stu-id="c9632-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="c9632-245">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c9632-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="c9632-246">Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="c9632-246">Actuals</span></span></th>
<th><span data-ttu-id="c9632-247">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="c9632-247">Transaction currency</span></span></th>
<th><span data-ttu-id="c9632-248">Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c9632-248">Fixed price</span></span></th>
<th><span data-ttu-id="c9632-249">Валута трансакције</span><span class="sxs-lookup"><span data-stu-id="c9632-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="c9632-250">Ставка времена је креирана.</span><span class="sxs-lookup"><span data-stu-id="c9632-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="c9632-251">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="c9632-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-252">Ставка времена је прослеђена.</span><span class="sxs-lookup"><span data-stu-id="c9632-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="c9632-253">Нема активности у ентитету Стварне вредности</span><span class="sxs-lookup"><span data-stu-id="c9632-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="c9632-254">Време је одобрено, а током одобравања не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="c9632-255">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-255">Cost actual</span></span></td>
<td><span data-ttu-id="c9632-256">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="c9632-257">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="c9632-258">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="c9632-259">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="c9632-260">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-261">Ненаплаћене стварне вредности продаје – Наплативо</span><span class="sxs-lookup"><span data-stu-id="c9632-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="c9632-262">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-263">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="c9632-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="c9632-264">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="c9632-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-265">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="c9632-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="c9632-266">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="c9632-267">Време је одобрено, а током одобравања долази до смањења број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="c9632-268">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-268">Cost actual</span></span></td>
<td><span data-ttu-id="c9632-269">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-270">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-271">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-272">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-273">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="c9632-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-274">Трошкови јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="c9632-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="c9632-275">Валута јединице за обезбеђивање ресурса</span><span class="sxs-lookup"><span data-stu-id="c9632-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-276">Продаја између организација</span><span class="sxs-lookup"><span data-stu-id="c9632-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="c9632-277">Уговорна валута јединице</span><span class="sxs-lookup"><span data-stu-id="c9632-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-278">Ненаплаћене стварне вредности продаје – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="c9632-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="c9632-279">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-280">Ненаплаћене стварне вредности продаје – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="c9632-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="c9632-281">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="c9632-282">Фактура је одобрена, а не може да се промени или повећа број сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="c9632-283">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="c9632-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="c9632-284">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-285">Наплаћена продаја за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="c9632-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-286">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-287">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="c9632-288">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-289">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="c9632-289">Billed sales</span></span></td>
<td><span data-ttu-id="c9632-290">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="c9632-291">Фактура је одобрена и долази до смањења броја сати за наплату.</span><span class="sxs-lookup"><span data-stu-id="c9632-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="c9632-292">Сторнирање ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="c9632-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="c9632-293">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-294">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-295">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-296">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="c9632-297">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-298">Наплаћена продаја – наплативо за нову количину</span><span class="sxs-lookup"><span data-stu-id="c9632-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="c9632-299">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-300">Наплаћена продаја – не може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="c9632-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="c9632-301">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="c9632-302">Фактура се исправља да би се повећала наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="c9632-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="c9632-303">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="c9632-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="c9632-304">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="c9632-305">Сторнирање наплаћене продаје за контролну тачку</span><span class="sxs-lookup"><span data-stu-id="c9632-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="c9632-306">Промена статуса контролне тачке са <strong>Фактурирано</strong> на <strong>Спремно за фактурисање</strong></span><span class="sxs-lookup"><span data-stu-id="c9632-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="c9632-307">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-308">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="c9632-309">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="c9632-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-310">Наплаћена продаја</span><span class="sxs-lookup"><span data-stu-id="c9632-310">Billed sales</span></span></td>
<td><span data-ttu-id="c9632-311">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="c9632-312">Фактура се исправља да би се смањила наплатива количина.</span><span class="sxs-lookup"><span data-stu-id="c9632-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="c9632-313">Наплаћена продаја – Сторнирање</span><span class="sxs-lookup"><span data-stu-id="c9632-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="c9632-314">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-315">Наплаћена продаја за нову количину</span><span class="sxs-lookup"><span data-stu-id="c9632-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="c9632-316">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="c9632-317">Ненааплаћена продаја – може да се наплати за разлику</span><span class="sxs-lookup"><span data-stu-id="c9632-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="c9632-318">Валута уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="c9632-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
