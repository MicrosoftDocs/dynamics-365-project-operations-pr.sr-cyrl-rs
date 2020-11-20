---
title: Потврђивање предрачуна – једноставно
description: Ова тема пружа информације о потврђивању предрачуна у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 02b671e4ad327b2448529d7119211613f3a9cb27
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176539"
---
# <a name="confirm-a-proforma-invoice---lite"></a><span data-ttu-id="36b83-103">Потврђивање предрачуна – једноставно</span><span class="sxs-lookup"><span data-stu-id="36b83-103">Confirm a proforma invoice - lite</span></span>

<span data-ttu-id="36b83-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="36b83-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="36b83-105">Након потврде предрачуна, статус фактуре пројекта се ажурира на **Потврђено**.</span><span class="sxs-lookup"><span data-stu-id="36b83-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="36b83-106">Када се фактура потврди, постаје само за читање.</span><span class="sxs-lookup"><span data-stu-id="36b83-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="36b83-107">Убудуће се фактура може исправити само ако постоје исправке или кредити које је покренуо клијент, или уколико је фактура означена као плаћена.</span><span class="sxs-lookup"><span data-stu-id="36b83-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, of if the invoice is marked as paid.</span></span>

<span data-ttu-id="36b83-108">У следећој табели су наведени стварни подаци које је креирао систем.</span><span class="sxs-lookup"><span data-stu-id="36b83-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="36b83-109">Ови стварни подаци се креирају када се изврше одређене радње на радној верзији фактуре пројекта пре него што се она потврди.</span><span class="sxs-lookup"><span data-stu-id="36b83-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="36b83-110">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="36b83-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="36b83-111">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="36b83-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="36b83-112">Фактурисање аванса или одбитка</span><span class="sxs-lookup"><span data-stu-id="36b83-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-113">Фактурисани стварни износ продаје, <strong>Одбитак</strong> креира се за износ на авансу или обустави.</span><span class="sxs-lookup"><span data-stu-id="36b83-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-114">Стварна ненаплаћена продаја негативног износа обуставе или аванса, која ће се користити за сравњење.</span><span class="sxs-lookup"><span data-stu-id="36b83-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="36b83-115">Након потпуног сравњења обуставе или аванса на фактури.</span><span class="sxs-lookup"><span data-stu-id="36b83-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-116">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="36b83-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="36b83-117">Овај износ је позитиван јер има за циљ да поништи негатив настао приликом фактурисања обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="36b83-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-118">Стварни износ наплаћене продаје за износ на овој фактури.</span><span class="sxs-lookup"><span data-stu-id="36b83-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="36b83-119">Након делимичног сравњења обуставе или аванса на фактури.</span><span class="sxs-lookup"><span data-stu-id="36b83-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-120">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="36b83-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="36b83-121">Овај износ је позитиван јер има за циљ да поништи негатив настао приликом фактурисања обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="36b83-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-122">Стварни износ наплаћене продаје за износ на овој фактури.</span><span class="sxs-lookup"><span data-stu-id="36b83-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-123">Негативна стварна ненаплаћена продаја преосталог износа обуставе или аванса, која ће се користити за сравњење на будућим фактурама.</span><span class="sxs-lookup"><span data-stu-id="36b83-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="36b83-124">Фактурисање временске трансакције без икаквих измена на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="36b83-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-125">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="36b83-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-126">Наплаћени стварни износ продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="36b83-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="36b83-127">Фактурисање временске трансакције која је уређена да би се смањила количина.</span><span class="sxs-lookup"><span data-stu-id="36b83-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-128">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="36b83-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-129">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="36b83-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-130">Нови ненаплаћени стварни износ продаје који је ненаплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије уређене фактуре, сторнирање стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="36b83-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="36b83-131">Фактурисање временске трансакције која је уређена да би се повећала количина.</span><span class="sxs-lookup"><span data-stu-id="36b83-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-132">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="36b83-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-133">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="36b83-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="36b83-134">Фактурисање трансакције трошкова без икаквих измена на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="36b83-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-135">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="36b83-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-136">Наплаћени стварни износ продаје за количину и износ на оригиналном одобрењу за трошкове</span><span class="sxs-lookup"><span data-stu-id="36b83-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="36b83-137">Фактурисање трансакције трошкова која је уређена да би се смањила количина.</span><span class="sxs-lookup"><span data-stu-id="36b83-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-138">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="36b83-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-139">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="36b83-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-140">Нови ненаплаћени стварни износ продаје који је ненаплатив за преосталу количину и износ након одбијања исправљених цифара на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="36b83-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="36b83-141">Фактурисање трансакције трошкова која је уређена да би се повећала количина.</span><span class="sxs-lookup"><span data-stu-id="36b83-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-142">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="36b83-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-143">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="36b83-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="36b83-144">Фактурисање накнаде.</span><span class="sxs-lookup"><span data-stu-id="36b83-144">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-145">Сторнирање ненаплаћене продаје за износ накнаде у оригиналној ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="36b83-145">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-146">Наплаћени стварни износ продаје за количину и износ у оригиналној ставци у главној књизи за накнаду.</span><span class="sxs-lookup"><span data-stu-id="36b83-146">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="36b83-147">Фактурисање контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="36b83-147">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-148">Наплаћени стварни износ продаје за износ контролне тачке на оригиналној контролној тачки у предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="36b83-148">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="36b83-149">Фактурисање предмета уговора заснованог на производу.</span><span class="sxs-lookup"><span data-stu-id="36b83-149">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="36b83-150">Наплаћени стварни износ продаје за линију производа са количином и износом који потичу из предмета уговора заснованог на производу.</span><span class="sxs-lookup"><span data-stu-id="36b83-150">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
