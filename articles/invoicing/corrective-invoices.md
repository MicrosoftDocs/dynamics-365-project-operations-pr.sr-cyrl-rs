---
title: Креирање корективних фактура заснованих на пројекту
description: Ова тема пружа информације о корективним фактурама у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 03/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32772d64b3fc77f0af9618edff40e3b295593454
ms.sourcegitcommit: 504c09365bf404c1f1aa9b5034c1e1e5bc9d0d54
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788894"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="bc4bd-103">Креирање корективних фактура заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="bc4bd-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="bc4bd-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="bc4bd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="bc4bd-105">Потврђена фактура пројекта може се исправити тако да обрађује промене или кредите према договору са клијентом и менаџером пројекта.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="bc4bd-106">Да бисте извршили измене на потврђеној фактури, отворите потврђену фактуру и изаберите **Исправите ову фактуру**.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="bc4bd-107">Овај избор није доступан уколико се не потврди фактура пројекта.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="bc4bd-108">Из потврђене фактуре креира се нова радна верзија фактуре.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="bc4bd-109">Сви детаљи линије фактуре из претходно потврђене фактуре копирају се у нову радну верзију.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="bc4bd-110">Следе неке кључне тачке које ће вам помоћи да разумете више о детаљима ставки на новој исправљеној фактури:</span><span class="sxs-lookup"><span data-stu-id="bc4bd-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="bc4bd-111">Све количине су ажуриране на нулу.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-111">All quantities are updated to zero.</span></span> <span data-ttu-id="bc4bd-112">То претпоставља да су све фактурисане ставке у потпуности задужене.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="bc4bd-113">Ако је потребно, ове количине можете ручно ажурирати тако да одражавају количину која се фактурише, а не количину која се задужује.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="bc4bd-114">На основу количине коју унесете, апликација израчунава задужену количину.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="bc4bd-115">Овај износ се огледа у стварним трошковима који се задужују када се потврди исправљена фактура.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="bc4bd-116">Ако мењате износ пореза, морате унети тачан износ пореза, а не износ пореза који се задужује.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="bc4bd-117">Исправке контролних тачака увек се обрађују као пуна задужења.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="bc4bd-118">Износи обуставе или аванса могу се исправити ако је клијенту фактурисан нетачан износ.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="bc4bd-119">Сравњења обустава и аванса могу се исправити ако је коришћен нетачан износ за ставњење трошкова на претходно потврђеној фактури.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bc4bd-120">Детаљи ставке фактуре које представљају исправке за друге већ фактурисане трошкове садрже поље **Исправка** подешено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="bc4bd-121">Фактуре које имају исправљене детаље о линији фактуре имају поље **Има исправке** које је такође постављено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="bc4bd-122">Тренутно стање креирано на потврди корективне фактуре</span><span class="sxs-lookup"><span data-stu-id="bc4bd-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="bc4bd-123">Следећа табела наводи стварне податке који се креирају када се потврди фактура са исправком.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="bc4bd-124">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bc4bd-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="bc4bd-125">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bc4bd-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="bc4bd-126">Потврдите исправку фактурисаног аванса или обуставе.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="bc4bd-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-127">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="bc4bd-128">Овај износ је позитиван јер има за циљ да поништи негатив настао приликом фактурисања обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-129">Стварни износ сторниране наплаћене продаје креира се за износ на обустави или авансу да би се поништила првобитна наплаћена продаја.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-130">Креира се нови фактурисани стварни трошак продаје за исправљени износ или исправљеној линији фактуре на основу обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-131">Стварна ненаплаћена продаја негативног износа исправљене линије фактуре на основу обуставе или аванса, која ће се користити за сравњење.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="bc4bd-132">Потврда исправке претходно сравњене обуставе или аванса.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-133">Сторнирање ненаплаћене продаје за обуставу или аванс који је креиран за сравњење.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="bc4bd-134">Овај износ је позитиван и има за циљ да поништи негативан износ настао приликом претходног сравњења.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-135">Стварни износ сторниране наплаћене продаје за износ на претходној фактури.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-136">Нови наплаћени стварни трошак продаје за исправљени износ обуставе који се примењује на исправљену фактуру.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-137">Стварна ненаплаћена продаја са негативним износом са исправљене преостале обуставе или аванса, која ће се користити за сравњење на каснијим фактурама.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bc4bd-138">Фактурисање пуног кредита претходно фактурисане временске трансакције.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-139">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-140">Нови ненаплаћени стварни износ продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="bc4bd-141">Фактурисање делимичног кредита за временску трансакцију.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-142">Сторнирање наплаћене продаје за сате и износ фактурисан на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-143">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-144">Нови ненаплаћени стварни износ продаје који је наплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bc4bd-145">Фактурисање пуног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-146">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-147">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="bc4bd-148">Фактурисање делимичног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-149">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-150">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије исправљене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-151">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bc4bd-152">Фактурисање пуног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-153">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-154">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bc4bd-155">Фактурисање делимичног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-156">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-157">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене корективне фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="bc4bd-158">Фактурисање пуног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-159">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за контролну тачку.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="bc4bd-160">Статус фактуре на контролној тачки се ажурира из <b>Прокњижена фактура за клијента</b> у <b>Спремно за фактурисање</b>.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="bc4bd-161">Фактурисање делимичног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="bc4bd-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="bc4bd-162">Неподржано</span><span class="sxs-lookup"><span data-stu-id="bc4bd-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
