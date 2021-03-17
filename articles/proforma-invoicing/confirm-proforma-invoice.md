---
title: Потврда предрачуна
description: Ова тема пружа информације о потврђивању предрачуна.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b2ed241509d2643d841ce55777e6e316612f70b8
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287886"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="cbaf7-103">Потврда предрачуна</span><span class="sxs-lookup"><span data-stu-id="cbaf7-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="cbaf7-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="cbaf7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="cbaf7-105">Након потврде предрачуна, статус фактуре пројекта се ажурира на **Потврђено**.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="cbaf7-106">Када се фактура потврди, постаје само за читање.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="cbaf7-107">Убудуће се фактура може исправити само ако постоје исправке или кредити које је покренуо клијент, или када је фактура означена као плаћена.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="cbaf7-108">У следећој табели су наведени стварни подаци које је креирао систем.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="cbaf7-109">Ови стварни подаци се креирају када се изврше одређене радње на радној верзији фактуре пројекта пре него што се она потврди.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="cbaf7-110">
                    <strong>Сценарио</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cbaf7-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="cbaf7-111">
                    <strong>Стварни подаци креирани приликом потврде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cbaf7-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="cbaf7-112">Фактурисање временске трансакције без икаквих измена на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-113">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-114">Наплаћени стварни износ продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="cbaf7-115">Фактурисање временске трансакције која је уређена да би се смањила количина.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-116">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-117">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-118">Нови ненаплаћени стварни износ продаје који је ненаплатив за преостале сате и износ након одбијања исправљених цифара на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="cbaf7-119">Фактурисање временске трансакције која је уређена да би се повећала количина.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-120">Сторнирање ненаплаћене продаје за сате и износ на оригиналном одобрењу за време.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-121">Нови ненаплаћени стварни износ продаје који је наплатив за сате и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="cbaf7-122">Фактурисање трансакције трошкова без икаквих измена на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-123">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-124">Наплаћени стварни износ продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="cbaf7-125">Фактурисање трансакције трошкова која је уређена да би се смањила количина.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-126">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-127">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-128">Нови ненаплаћени стварни износ продаје који је ненаплатив за преосталу количину и износ након одбијања исправљених цифара на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="cbaf7-129">Фактурисање трансакције трошкова која је уређена да би се повећала количина.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-130">Сторнирање ненаплаћене продаје за количину и износ на оригиналном одобрењу за трошкове.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-131">Нови ненаплаћени стварни износ продаје који је наплатив за количину и износ на детаљу линије уређене фактуре, сторнирање ненаплаћеног стварног износа продаје и еквивалентан стварни наплаћени износ продаје.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="cbaf7-132">Фактурисање накнаде.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-133">Сторнирање ненаплаћене продаје за износ накнаде у оригиналној ставци у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-134">Наплаћени стварни износ продаје за количину и износ у оригиналној ставци у главној књизи за накнаду.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="cbaf7-135">Фактурисање контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="cbaf7-136">Наплаћени стварни износ продаје за износ контролне тачке на оригиналној контролној тачки у предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="cbaf7-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]