---
title: Корективне фактуре засноване на пројекту
description: Ова тема пружа информације о томе како да креирате и потврдите корективне фактуре засноване на пројекту у услузи Project Operations.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6b6670f823577bf7f784443f97f0b77e1e9a6aa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012289"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="1d8b4-103">Корективне фактуре засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="1d8b4-103">Corrective project-based invoices</span></span>

<span data-ttu-id="1d8b4-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="1d8b4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1d8b4-105">Потврђена фактура пројекта може се исправити тако да обрађује промене или кредите према договору са клијентом и менаџером пројекта.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="1d8b4-106">Да бисте извршили измене на потврђеној фактури, отворите потврђену фактуру и изаберите **Исправите ову фактуру**.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="1d8b4-107">Овај избор није доступан осим ако фактура пројекта није потврђена или ако фактура заснована на пројекту садржи авансе или обуставе или усаглашавање аванса или обустава.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="1d8b4-108">Из потврђене фактуре креира се нова радна верзија фактуре.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="1d8b4-109">Сви детаљи линије фактуре из претходно потврђене фактуре копирају се у нову радну верзију.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="1d8b4-110">Следе неке од кључних тачака које треба разумети у вези са детаљима линије на новој исправљеној фактури:</span><span class="sxs-lookup"><span data-stu-id="1d8b4-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="1d8b4-111">Све количине су ажуриране на нулу.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-111">All quantities are updated to zero.</span></span> <span data-ttu-id="1d8b4-112">Dynamics 365 Project Operations претпоставља да су све фактурисане ставке у потпуности задужене.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="1d8b4-113">Ако је потребно, ове количине можете ручно ажурирати тако да одражавају количину која се фактурише, а не количину која се задужује.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="1d8b4-114">На основу количине коју унесете, апликација израчунава задужену количину.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="1d8b4-115">Овај износ се огледа у стварним трошковима који се задужују када се потврди исправљена фактура.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="1d8b4-116">Ако мењате износ пореза, морате унети тачан износ пореза, а не износ пореза који се задужује.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="1d8b4-117">Исправке контролних тачака увек се обрађују као пуна задужења.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="1d8b4-118">За детаље о ставки фактуре које представљају исправке за друге већ фактурисане трошкове, поље **Исправка** се поставља на **Да**.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="1d8b4-119">За фактуре имају исправљене детаље ставки фактуре, поље **Има исправке** се поставља на **Да**.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="1d8b4-120">Тренутно стање креирано када је потврђена корективна фактура</span><span class="sxs-lookup"><span data-stu-id="1d8b4-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="1d8b4-121">Следећа табела наводи стварне податке који се креирају када се потврди фактура са исправком.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="1d8b4-122">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1d8b4-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="1d8b4-123">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1d8b4-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1d8b4-124">Фактурисање пуног кредита претходно фактурисане временске трансакције.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-125">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-126">Нови ненаплаћени стварни износ продаје за сате и износ на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="1d8b4-127">Фактурисање делимичног кредита за временску трансакцију.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-128">Сторнирање наплаћене продаје за сате и износ фактурисан на оригиналном детаљу линије фактуре за време.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-129">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-130">Нови ненаплаћени стварни износ продаје који је наплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1d8b4-131">Фактурисање пуног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-132">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-133">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="1d8b4-134">Фактурисање делимичног кредита претходно фактурисане трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-135">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за трошак.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-136">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије исправљене фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-137">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1d8b4-138">Фактурисање пуног кредита претходно фактурисане материјалне трансакције.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-139">Сторнирање наплаћене продаје за количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-140">Нова стварна вредност ненаплаћене продаје за количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="1d8b4-141">Фактурисање делимичног кредита за трансакцију материјала.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-142">Сторнирање наплаћене продаје за фактурисану количину и износ на детаљима ставки оригиналне фактуре за материјал.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-143">Нова нефактурисана стварна продаја која се наплаћује за количину и износ на измењеном детаљу ставке фактуре, сторнирање ове ставке и еквивалентни стварни износ наплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-144">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ након одбијања исправљених цифара на детаљу линије фактуре.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1d8b4-145">Фактурисање пуног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-146">Сторнирање наплаћене продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-147">Нови ненаплаћени стварни износ продаје за количину и износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1d8b4-148">Фактурисање делимичног кредита претходно фактурисане трансакције накнаде.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-149">Сторнирање наплаћене продаје за количину и фактурисани износ на оригиналном детаљу линије фактуре за накнаду.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-150">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене корективне фактуре, сторнирање ове ставке и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="1d8b4-151">Фактурисање пуног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-152">Сторнирање наплаћене продаје за сате и износ на оригиналном детаљу линије фактуре за контролну тачку.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="1d8b4-153">Статус фактуре на контролној тачки се ажурира из <b>Прокњижена фактура за клијента</b> у <b>Спремно за фактурисање</b>.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="1d8b4-154">Фактурисање делимичног кредита претходно фактурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1d8b4-155">Овај сценарио није подржан.</span><span class="sxs-lookup"><span data-stu-id="1d8b4-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
