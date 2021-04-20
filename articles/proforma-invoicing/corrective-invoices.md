---
title: Корективне фактуре засноване на пројекту
description: Ова тема пружа информације о томе како да креирате и потврдите корективне фактуре засноване на пројекту у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 03/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fc96bb40f5207efc381986d46a3e37dfc1dc111c
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/07/2021
ms.locfileid: "5867059"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="2bfea-103">Корективне фактуре засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="2bfea-103">Corrective project-based invoices</span></span>

<span data-ttu-id="2bfea-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="2bfea-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2bfea-105">Потврђена фактура пројекта може се исправити тако да обрађује промене или кредите према договору са клијентом и менаџером пројекта.</span><span class="sxs-lookup"><span data-stu-id="2bfea-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="2bfea-106">Да бисте извршили измене на потврђеној фактури, отворите потврђену фактуру и изаберите **Исправите ову фактуру**.</span><span class="sxs-lookup"><span data-stu-id="2bfea-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="2bfea-107">Овај избор није доступан осим ако фактура пројекта није потврђена или ако фактура заснована на пројекту садржи авансе или обуставе или усаглашавање аванса или обустава.</span><span class="sxs-lookup"><span data-stu-id="2bfea-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="2bfea-108">Из потврђене фактуре креира се нова радна верзија фактуре.</span><span class="sxs-lookup"><span data-stu-id="2bfea-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="2bfea-109">Сви детаљи линије фактуре из претходно потврђене фактуре копирају се у нову радну верзију.</span><span class="sxs-lookup"><span data-stu-id="2bfea-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="2bfea-110">Следе неке од кључних тачака које треба разумети у вези са детаљима линије на новој исправљеној фактури:</span><span class="sxs-lookup"><span data-stu-id="2bfea-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="2bfea-111">Све количине су ажуриране на нулу.</span><span class="sxs-lookup"><span data-stu-id="2bfea-111">All quantities are updated to zero.</span></span> <span data-ttu-id="2bfea-112">Dynamics 365 Project Operations претпоставља да су све фактурисане ставке у потпуности задужене.</span><span class="sxs-lookup"><span data-stu-id="2bfea-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="2bfea-113">Ако је потребно, ове количине можете ручно ажурирати тако да одражавају количину која се фактурише, а не количину која се задужује.</span><span class="sxs-lookup"><span data-stu-id="2bfea-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="2bfea-114">На основу количине коју унесете, апликација израчунава задужену количину.</span><span class="sxs-lookup"><span data-stu-id="2bfea-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="2bfea-115">Овај износ се огледа у стварним трошковима који се задужују када се потврди исправљена фактура.</span><span class="sxs-lookup"><span data-stu-id="2bfea-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="2bfea-116">Ако мењате износ пореза, морате унети тачан износ пореза, а не износ пореза који се задужује.</span><span class="sxs-lookup"><span data-stu-id="2bfea-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="2bfea-117">Исправке контролних тачака увек се обрађују као пуна задужења.</span><span class="sxs-lookup"><span data-stu-id="2bfea-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="2bfea-118">За детаље о ставки фактуре које представљају исправке за друге већ фактурисане трошкове, поље **Исправка** се поставља на **Да**.</span><span class="sxs-lookup"><span data-stu-id="2bfea-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="2bfea-119">За фактуре имају исправљене детаље ставки фактуре, поље **Има исправке** се поставља на **Да**.</span><span class="sxs-lookup"><span data-stu-id="2bfea-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="2bfea-120">Тренутно стање креирано када је потврђена корективна фактура</span><span class="sxs-lookup"><span data-stu-id="2bfea-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="2bfea-121">Следећа табела наводи стварне податке који се креирају када се потврди фактура са исправком.</span><span class="sxs-lookup"><span data-stu-id="2bfea-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="2bfea-122">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2bfea-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="2bfea-123">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2bfea-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2bfea-124">Фактурисање пуног кредита претходно фактурисане временске трансакције.</span><span class="sxs-lookup"><span data-stu-id="2bfea-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-125">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="2bfea-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-126">Нови ненаплаћени стварни износ продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="2bfea-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="2bfea-127">Фактурисање делимичног кредита за временску трансакцију.</span><span class="sxs-lookup"><span data-stu-id="2bfea-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-128">Сторнирање наплаћене продаје за сате и износ фактурисан на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="2bfea-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-129">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="2bfea-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-130">Нови ненаплаћени стварни износ продаје који је наплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="2bfea-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2bfea-131">Фактурисање пуног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="2bfea-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-132">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="2bfea-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-133">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="2bfea-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="2bfea-134">Фактурисање делимичног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="2bfea-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-135">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="2bfea-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-136">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије исправљене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="2bfea-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-137">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="2bfea-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2bfea-138">Фактурисање пуног кредита претходно фактурисане материјалне трансакције.</span><span class="sxs-lookup"><span data-stu-id="2bfea-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-139">Сторнирање наплаћене продаје за количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="2bfea-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-140">Нова стварна вредност ненаплаћене продаје за количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="2bfea-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="2bfea-141">Фактурисање делимичног кредита за трансакцију материјала.</span><span class="sxs-lookup"><span data-stu-id="2bfea-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-142">Сторнирање наплаћене продаје за фактурисану количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="2bfea-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-143">Нова нефактурисана стварна продаја која се наплаћује за количину и износ на измењеном детаљу ставке фактуре, сторнирање ове ставке и еквивалентни стварни износ наплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="2bfea-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-144">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="2bfea-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2bfea-145">Фактурисање пуног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="2bfea-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-146">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="2bfea-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-147">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="2bfea-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2bfea-148">Фактурисање делимичног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="2bfea-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-149">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="2bfea-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-150">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене корективне фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="2bfea-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="2bfea-151">Фактурисање пуног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="2bfea-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-152">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за контролну тачку.</span><span class="sxs-lookup"><span data-stu-id="2bfea-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="2bfea-153">Статус фактуре на контролној тачки се ажурира из <b>Прокњижена фактура за клијента</b> у <b>Спремно за фактурисање</b>.</span><span class="sxs-lookup"><span data-stu-id="2bfea-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="2bfea-154">Фактурисање делимичног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="2bfea-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2bfea-155">Овај сценарио није подржан.</span><span class="sxs-lookup"><span data-stu-id="2bfea-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
