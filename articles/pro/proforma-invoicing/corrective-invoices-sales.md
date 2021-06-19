---
title: Корективне фактуре за пројекат
description: Ова тема пружа информације о томе како да креирате и потврдите корективне фактуре у услузи Project Operations.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: dfa5535597ee6e144259c9246b33075f3492285e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004099"
---
# <a name="corrective-project-invoices"></a><span data-ttu-id="a9438-103">Корективне фактуре за пројекат</span><span class="sxs-lookup"><span data-stu-id="a9438-103">Corrective project invoices</span></span>

<span data-ttu-id="a9438-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="a9438-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a9438-105">Потврђена фактура пројекта може се исправити тако да обрађује промене или кредите према договору са клијентом и менаџером пројекта.</span><span class="sxs-lookup"><span data-stu-id="a9438-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="a9438-106">Да бисте извршили измене на потврђеној фактури, отворите потврђену фактуру и изаберите **Исправите ову фактуру**.</span><span class="sxs-lookup"><span data-stu-id="a9438-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="a9438-107">Овај избор није доступан уколико се не потврди фактура пројекта.</span><span class="sxs-lookup"><span data-stu-id="a9438-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="a9438-108">Из потврђене фактуре креира се нова радна верзија фактуре.</span><span class="sxs-lookup"><span data-stu-id="a9438-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="a9438-109">Сви детаљи линије фактуре из претходно потврђене фактуре копирају се у нову радну верзију.</span><span class="sxs-lookup"><span data-stu-id="a9438-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="a9438-110">Следе неке од кључних тачака које треба разумети у вези са детаљима линије на новој исправљеној фактури:</span><span class="sxs-lookup"><span data-stu-id="a9438-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="a9438-111">Све количине су ажуриране на нулу.</span><span class="sxs-lookup"><span data-stu-id="a9438-111">All quantities are updated to zero.</span></span> <span data-ttu-id="a9438-112">Апликација претпоставља да су све фактурисане ставке у потпуности задужене.</span><span class="sxs-lookup"><span data-stu-id="a9438-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="a9438-113">Ако је потребно, ове количине можете ручно ажурирати тако да одражавају количину која се фактурише, а не количину која се задужује.</span><span class="sxs-lookup"><span data-stu-id="a9438-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="a9438-114">На основу количине коју унесете, апликација израчунава задужену количину.</span><span class="sxs-lookup"><span data-stu-id="a9438-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="a9438-115">Овај износ се огледа у стварним трошковима који се задужују када се потврди исправљена фактура.</span><span class="sxs-lookup"><span data-stu-id="a9438-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="a9438-116">Ако мењате износ пореза, морате унети тачан износ пореза, а не износ пореза који се задужује.</span><span class="sxs-lookup"><span data-stu-id="a9438-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="a9438-117">Претходно потврђени предмети уговора засновани на производу се не копирају.</span><span class="sxs-lookup"><span data-stu-id="a9438-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="a9438-118">Обрада исправки на фактури пројекта заснованог на производу није подржана.</span><span class="sxs-lookup"><span data-stu-id="a9438-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="a9438-119">Исправке контролних тачака увек се обрађују као пуна задужења.</span><span class="sxs-lookup"><span data-stu-id="a9438-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="a9438-120">Износи обуставе или аванса могу се исправити ако је клијенту фактурисан нетачан износ.</span><span class="sxs-lookup"><span data-stu-id="a9438-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="a9438-121">Сравњења обустава и аванса могу се исправити ако је коришћен нетачан износ за ставњење трошкова на претходно потврђеној фактури.</span><span class="sxs-lookup"><span data-stu-id="a9438-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a9438-122">Подаци о линији фактуре који представљају исправке других већ фактурисаних трошкова имају поље **Исправка** подешено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="a9438-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="a9438-123">Фактуре које имају исправљене детаље о линији фактуре имају поље **Има исправке** које је такође постављено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="a9438-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="a9438-124">Тренутно стање креирано када је потврђена корективна фактура</span><span class="sxs-lookup"><span data-stu-id="a9438-124">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="a9438-125">Следећа табела наводи стварне податке који се креирају када се потврди фактура са исправком.</span><span class="sxs-lookup"><span data-stu-id="a9438-125">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="a9438-126">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a9438-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="a9438-127">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a9438-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="a9438-128">Потврдите исправку фактурисаног аванса или обуставе.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="a9438-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-129">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="a9438-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="a9438-130">Овај износ је позитиван јер има за циљ да поништи негатив настао приликом фактурисања обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="a9438-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-131">Стварни износ сторниране наплаћене продаје креира се за износ на обустави или авансу да би се поништила првобитна наплаћена продаја.</span><span class="sxs-lookup"><span data-stu-id="a9438-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-132">Креира се нови фактурисани стварни трошак продаје за исправљени износ или исправљеној линији фактуре на основу обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="a9438-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-133">Стварна ненаплаћена продаја негативног износа исправљене линије фактуре на основу обуставе или аванса, која ће се користити за сравњење.</span><span class="sxs-lookup"><span data-stu-id="a9438-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="a9438-134">Потврда исправке претходно сравњене обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="a9438-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-135">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="a9438-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="a9438-136">Овај износ је позитиван и има за циљ да поништи негативан износ настао приликом претходног сравњења.</span><span class="sxs-lookup"><span data-stu-id="a9438-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-137">Стварни износ сторниране наплаћене продаје за износ на претходној фактури.</span><span class="sxs-lookup"><span data-stu-id="a9438-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-138">Нови наплаћени стварни трошак продаје за исправљени износ обуставе који се примењује на исправљену фактуру.</span><span class="sxs-lookup"><span data-stu-id="a9438-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-139">Стварна ненаплаћена продаја са негативним износом са исправљене преостале обуставе или аванса, која ће се користити за сравњење на каснијим фактурама.</span><span class="sxs-lookup"><span data-stu-id="a9438-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a9438-140">Фактурисање пуног кредита претходно фактурисане временске трансакције.</span><span class="sxs-lookup"><span data-stu-id="a9438-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-141">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="a9438-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-142">Нови ненаплаћени стварни износ продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="a9438-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a9438-143">Фактурисање делимичног кредита за временску трансакцију.</span><span class="sxs-lookup"><span data-stu-id="a9438-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-144">Сторнирање наплаћене продаје за сате и износ фактурисан на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="a9438-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-145">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="a9438-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-146">Нови ненаплаћени стварни износ продаје који је наплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="a9438-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a9438-147">Фактурисање пуног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="a9438-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-148">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="a9438-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-149">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="a9438-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a9438-150">Фактурисање делимичног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="a9438-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-151">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="a9438-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-152">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије исправљене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="a9438-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-153">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="a9438-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a9438-154">Фактурисање пуног кредита претходно фактурисане материјалне трансакције.</span><span class="sxs-lookup"><span data-stu-id="a9438-154">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-155">Сторнирање наплаћене продаје за количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="a9438-155">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-156">Нова стварна вредност ненаплаћене продаје за количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="a9438-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a9438-157">Фактурисање делимичног кредита за трансакцију материјала.</span><span class="sxs-lookup"><span data-stu-id="a9438-157">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-158">Сторнирање наплаћене продаје за фактурисану количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="a9438-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-159">Нова нефактурисана стварна продаја која се наплаћује за количину и износ на измењеном детаљу ставке фактуре, сторнирање ове ставке и еквивалентни стварни износ наплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="a9438-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-160">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="a9438-160">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a9438-161">Фактурисање пуног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="a9438-161">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-162">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="a9438-162">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-163">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="a9438-163">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a9438-164">Фактурисање делимичног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="a9438-164">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-165">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="a9438-165">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-166">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене корективне фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="a9438-166">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="a9438-167">Фактурисање пуног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="a9438-167">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-168">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за контролну тачку.</span><span class="sxs-lookup"><span data-stu-id="a9438-168">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="a9438-169">Статус фактуре на контролној тачки се ажурира из <b>Прокњижена фактура за клијента</b> у <b>Спремно за фактурисање</b>.</span><span class="sxs-lookup"><span data-stu-id="a9438-169">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="a9438-170">Фактурисање делимичног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="a9438-170">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-171">Неподржано</span><span class="sxs-lookup"><span data-stu-id="a9438-171">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="a9438-172">Кредити и исправке претходно фактурисаног предмета уговора заснованог на производу.</span><span class="sxs-lookup"><span data-stu-id="a9438-172">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a9438-173">Неподржано</span><span class="sxs-lookup"><span data-stu-id="a9438-173">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
