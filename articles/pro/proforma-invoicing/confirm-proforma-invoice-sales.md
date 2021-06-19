---
title: Потврда предрачуна за пројекат
description: Ова тема пружа информације о потврђивању предрачуна за пројекат у услузи Project Operations.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0ab40e38f221e57368949b7491578caa8ba88c02
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004144"
---
# <a name="confirm-a-proforma-project-invoice"></a><span data-ttu-id="95d06-103">Потврда предрачуна за пројекат</span><span class="sxs-lookup"><span data-stu-id="95d06-103">Confirm a proforma project invoice</span></span> 

<span data-ttu-id="95d06-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="95d06-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="95d06-105">Након потврде предрачуна, статус фактуре пројекта се ажурира на **Потврђено**.</span><span class="sxs-lookup"><span data-stu-id="95d06-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="95d06-106">Када се фактура потврди, постаје само за читање.</span><span class="sxs-lookup"><span data-stu-id="95d06-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="95d06-107">Убудуће се фактура може исправити само ако постоје исправке или кредити које је покренуо клијенти.</span><span class="sxs-lookup"><span data-stu-id="95d06-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits.</span></span>

<span data-ttu-id="95d06-108">У следећој табели су наведени стварни подаци које је креирао систем.</span><span class="sxs-lookup"><span data-stu-id="95d06-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="95d06-109">Ови стварни подаци се креирају када се изврше одређене радње на радној верзији фактуре пројекта пре него што се она потврди.</span><span class="sxs-lookup"><span data-stu-id="95d06-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="95d06-110">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95d06-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="95d06-111">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="95d06-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-112">Фактурисање аванса или обуставе</span><span class="sxs-lookup"><span data-stu-id="95d06-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-113">Фактурисани стварни износ продаје, <strong>Одбитак</strong> креира се за износ на авансу или обустави.</span><span class="sxs-lookup"><span data-stu-id="95d06-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-114">Стварна ненаплаћена продаја негативног износа обуставе или аванса, која ће се користити за сравњење.</span><span class="sxs-lookup"><span data-stu-id="95d06-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-115">Након потпуног сравњења обуставе или аванса на фактури.</span><span class="sxs-lookup"><span data-stu-id="95d06-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-116">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="95d06-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="95d06-117">Овај износ је позитиван јер има за циљ да поништи негатив настао приликом фактурисања обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="95d06-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-118">Стварни износ наплаћене продаје за износ на овој фактури.</span><span class="sxs-lookup"><span data-stu-id="95d06-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="95d06-119">Након делимичног сравњења обуставе или аванса на фактури.</span><span class="sxs-lookup"><span data-stu-id="95d06-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-120">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="95d06-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="95d06-121">Овај износ је позитиван јер има за циљ да поништи негатив настао приликом фактурисања обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="95d06-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-122">Стварни износ наплаћене продаје за износ на овој фактури.</span><span class="sxs-lookup"><span data-stu-id="95d06-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-123">Негативна стварна ненаплаћена продаја преосталог износа обуставе или аванса, која ће се користити за сравњење на будућим фактурама.</span><span class="sxs-lookup"><span data-stu-id="95d06-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-124">Фактурисање временске трансакције без икаквих измена на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="95d06-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-125">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="95d06-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-126">Наплаћени стварни износ продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="95d06-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="95d06-127">Фактурисање временске трансакције која је уређена да би се смањила количина.</span><span class="sxs-lookup"><span data-stu-id="95d06-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-128">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="95d06-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-129">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-130">Нови ненаплаћени стварни износ продаје који је ненаплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије уређене фактуре, сторнирање стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-131">Фактурисање временске трансакције која је уређена да би се повећала количина.</span><span class="sxs-lookup"><span data-stu-id="95d06-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-132">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="95d06-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-133">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-134">Фактурисање трансакције трошкова без икаквих измена на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="95d06-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-135">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="95d06-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-136">Наплаћени стварни износ продаје за количину и износ на оригиналном одобрењу за трошкове</span><span class="sxs-lookup"><span data-stu-id="95d06-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="95d06-137">Фактурисање трансакције трошкова која је уређена да би се смањила количина.</span><span class="sxs-lookup"><span data-stu-id="95d06-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-138">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="95d06-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-139">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-140">Нови ненаплаћени стварни износ продаје који је ненаплатив за преосталу количину и износ након одбијања исправљених цифара на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-141">Фактурисање трансакције трошкова која је уређена да би се повећала количина.</span><span class="sxs-lookup"><span data-stu-id="95d06-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-142">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="95d06-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-143">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-144">Фактурисање трансакције материјала без икаквих измена у радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="95d06-144">Invoicing a material transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-145">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу коришћења материјала.</span><span class="sxs-lookup"><span data-stu-id="95d06-145">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-146">Стварни износ наплаћене продаје за количину и износ на оригиналном одобрењу коришћења материјала.</span><span class="sxs-lookup"><span data-stu-id="95d06-146">A billed sales actual for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="95d06-147">Фактурисање материјалне трансакције која је уређена да би се смањила количина.</span><span class="sxs-lookup"><span data-stu-id="95d06-147">Invoicing a material transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-148">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу времена.</span><span class="sxs-lookup"><span data-stu-id="95d06-148">An unbilled sales reversal for the quantity and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-149">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-149">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-150">Нови ненаплаћени стварни износ продаје који је ненаплатив за преосталу количину и износ након одбијања исправљених цифара на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-150">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-151">Фактурисање трансакције материјала која је уређена да би се повећала количина.</span><span class="sxs-lookup"><span data-stu-id="95d06-151">Invoicing a material transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-152">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу коришћења материјала.</span><span class="sxs-lookup"><span data-stu-id="95d06-152">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-153">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="95d06-153">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="95d06-154">Фактурисање накнаде.</span><span class="sxs-lookup"><span data-stu-id="95d06-154">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-155">Сторнирање ненаплаћене продаје за износ накнаде у оригиналној ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="95d06-155">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-156">Наплаћени стварни износ продаје за количину и износ у оригиналној ставци у главној књизи за накнаду.</span><span class="sxs-lookup"><span data-stu-id="95d06-156">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="95d06-157">Фактурисање контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="95d06-157">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-158">Наплаћени стварни износ продаје за износ контролне тачке на оригиналној контролној тачки у предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="95d06-158">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="95d06-159">Фактурисање предмета уговора заснованог на производу.</span><span class="sxs-lookup"><span data-stu-id="95d06-159">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="95d06-160">Наплаћени стварни износ продаје за линију производа са количином и износом који потичу из предмета уговора заснованог на производу.</span><span class="sxs-lookup"><span data-stu-id="95d06-160">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
