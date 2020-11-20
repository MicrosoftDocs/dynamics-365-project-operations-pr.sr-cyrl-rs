---
title: Исправљене фактуре – једноставно
description: Ова тема пружа информације о исправљеним фактурама у услузи Project Operations
author: rumant
manager: Annbe
ms.date: 10/15/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 55bec8ad1d9c2b55cabb453321f13df8b7cd1614
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176449"
---
# <a name="corrected-invoices---lite"></a><span data-ttu-id="35ac4-103">Исправљене фактуре – једноставно</span><span class="sxs-lookup"><span data-stu-id="35ac4-103">Corrected invoices - lite</span></span>

<span data-ttu-id="35ac4-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="35ac4-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="35ac4-105">Потврђена фактура пројекта може се исправити тако да обрађује промене или кредите према договору са клијентом и менаџером пројекта.</span><span class="sxs-lookup"><span data-stu-id="35ac4-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="35ac4-106">Да бисте извршили измене на потврђеној фактури, отворите потврђену фактуру и изаберите **Исправите ову фактуру**.</span><span class="sxs-lookup"><span data-stu-id="35ac4-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="35ac4-107">Овај избор није доступан уколико се не потврди фактура пројекта.</span><span class="sxs-lookup"><span data-stu-id="35ac4-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="35ac4-108">Из потврђене фактуре креира се нова радна верзија фактуре.</span><span class="sxs-lookup"><span data-stu-id="35ac4-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="35ac4-109">Сви детаљи линије фактуре из претходно потврђене фактуре копирају се у нову радну верзију.</span><span class="sxs-lookup"><span data-stu-id="35ac4-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="35ac4-110">Следе неке од кључних тачака које треба разумети у вези са детаљима линије на новој исправљеној фактури:</span><span class="sxs-lookup"><span data-stu-id="35ac4-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="35ac4-111">Све количине су ажуриране на нулу.</span><span class="sxs-lookup"><span data-stu-id="35ac4-111">All quantities are updated to zero.</span></span> <span data-ttu-id="35ac4-112">Апликација претпоставља да су све фактурисане ставке у потпуности задужене.</span><span class="sxs-lookup"><span data-stu-id="35ac4-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="35ac4-113">Ако је потребно, ове количине можете ручно ажурирати тако да одражавају количину која се фактурише, а не количину која се задужује.</span><span class="sxs-lookup"><span data-stu-id="35ac4-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="35ac4-114">На основу количине коју унесете, апликација израчунава задужену количину.</span><span class="sxs-lookup"><span data-stu-id="35ac4-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="35ac4-115">Овај износ се огледа у стварним трошковима који се задужују када се потврди исправљена фактура.</span><span class="sxs-lookup"><span data-stu-id="35ac4-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="35ac4-116">Ако мењате износ пореза, морате унети тачан износ пореза, а не износ пореза који се задужује.</span><span class="sxs-lookup"><span data-stu-id="35ac4-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="35ac4-117">Претходно потврђени предмети уговора засновани на производу се не копирају.</span><span class="sxs-lookup"><span data-stu-id="35ac4-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="35ac4-118">Обрада исправки на фактури пројекта заснованог на производу није подржана.</span><span class="sxs-lookup"><span data-stu-id="35ac4-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="35ac4-119">Исправке контролних тачака увек се обрађују као пуна задужења.</span><span class="sxs-lookup"><span data-stu-id="35ac4-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="35ac4-120">Износи обуставе или аванса могу се исправити ако је клијенту фактурисан нетачан износ.</span><span class="sxs-lookup"><span data-stu-id="35ac4-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="35ac4-121">Сравњења обустава и аванса могу се исправити ако је коришћен нетачан износ за ставњење трошкова на претходно потврђеној фактури.</span><span class="sxs-lookup"><span data-stu-id="35ac4-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="35ac4-122">Подаци о линији фактуре који представљају исправке других већ фактурисаних трошкова имају поље **Исправка** подешено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="35ac4-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="35ac4-123">Фактуре које имају исправљене детаље о линији фактуре имају поље **Има исправке** које је такође постављено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="35ac4-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="35ac4-124">Стварни трошкови креирани на потврди корективне фактуре:</span><span class="sxs-lookup"><span data-stu-id="35ac4-124">Actuals created on Confirmation of a corrective invoice:</span></span>

<span data-ttu-id="35ac4-125">Испод су стварни трошкови које је креирала апликација по потврди исправке на основу операција извршених на радној верзији корективне фактуре пре потврде.</span><span class="sxs-lookup"><span data-stu-id="35ac4-125">Below are the actuals created by the application on confirmation of a corrective based on the operations performed on the draft corrective invoice before confirmation.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="35ac4-126">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35ac4-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="35ac4-127">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35ac4-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="35ac4-128">Потврдите исправку фактурисаног аванса или обуставе.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="35ac4-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-129">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="35ac4-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="35ac4-130">Овај износ је позитиван јер има за циљ да поништи негатив настао приликом фактурисања обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="35ac4-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-131">Стварни износ сторниране наплаћене продаје креира се за износ на обустави или авансу да би се поништила првобитна наплаћена продаја.</span><span class="sxs-lookup"><span data-stu-id="35ac4-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-132">Креира се нови фактурисани стварни трошак продаје за исправљени износ или исправљеној линији фактуре на основу обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="35ac4-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-133">Стварна ненаплаћена продаја негативног износа исправљене линије фактуре на основу обуставе или аванса, која ће се користити за сравњење.</span><span class="sxs-lookup"><span data-stu-id="35ac4-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="35ac4-134">Потврда исправке претходно сравњене обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="35ac4-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-135">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="35ac4-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="35ac4-136">Овај износ је позитиван и има за циљ да поништи негативан износ настао приликом претходног сравњења.</span><span class="sxs-lookup"><span data-stu-id="35ac4-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-137">Стварни износ сторниране наплаћене продаје за износ на претходној фактури.</span><span class="sxs-lookup"><span data-stu-id="35ac4-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-138">Нови наплаћени стварни трошак продаје за исправљени износ обуставе који се примењује на исправљену фактуру.</span><span class="sxs-lookup"><span data-stu-id="35ac4-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-139">Стварна ненаплаћена продаја са негативним износом са исправљене преостале обуставе или аванса, која ће се користити за сравњење на каснијим фактурама.</span><span class="sxs-lookup"><span data-stu-id="35ac4-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35ac4-140">Фактурисање пуног кредита претходно фактурисане временске трансакције.</span><span class="sxs-lookup"><span data-stu-id="35ac4-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-141">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="35ac4-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-142">Нови ненаплаћени стварни износ продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="35ac4-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="35ac4-143">Фактурисање делимичног кредита за временску трансакцију.</span><span class="sxs-lookup"><span data-stu-id="35ac4-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-144">Сторнирање наплаћене продаје за сате и износ фактурисан на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="35ac4-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-145">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="35ac4-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-146">Нови ненаплаћени стварни износ продаје који је наплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="35ac4-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35ac4-147">Фактурисање пуног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="35ac4-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-148">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="35ac4-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-149">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="35ac4-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="35ac4-150">Фактурисање делимичног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="35ac4-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-151">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="35ac4-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-152">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије исправљене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="35ac4-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-153">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="35ac4-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35ac4-154">Фактурисање пуног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="35ac4-154">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-155">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="35ac4-155">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-156">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="35ac4-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35ac4-157">Фактурисање делимичног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="35ac4-157">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-158">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="35ac4-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-159">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене корективне фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="35ac4-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="35ac4-160">Фактурисање пуног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="35ac4-160">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-161">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за контролну тачку.</span><span class="sxs-lookup"><span data-stu-id="35ac4-161">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="35ac4-162">Фактура контролне тачке или статус наплате на предмету пројектног уговора ажурира се на **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="35ac4-162">The milestone invoice or billing status on the project contract line is updated to **Ready to Invoice**.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="35ac4-163">Фактурисање делимичног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="35ac4-163">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-164">Неподржано</span><span class="sxs-lookup"><span data-stu-id="35ac4-164">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="35ac4-165">Кредити и исправке претходно фактурисаног предмета уговора заснованог на производу.</span><span class="sxs-lookup"><span data-stu-id="35ac4-165">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="35ac4-166">Неподржано</span><span class="sxs-lookup"><span data-stu-id="35ac4-166">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>
