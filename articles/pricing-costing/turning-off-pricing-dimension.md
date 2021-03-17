---
title: Искључивање димензије за одређивање цена
description: Ова тема пружа информације о искључивању димензија за одређивање цена.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d2e10c9ce782697fa4cbbe6eb63491ebb573a6f6
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274746"
---
# <a name="turning-off-a-pricing-dimension"></a><span data-ttu-id="94a61-103">Искључивање димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="94a61-103">Turning off a pricing dimension</span></span>

<span data-ttu-id="94a61-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="94a61-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="94a61-105">Можда ћете морати да прегледате и ажурирате своју стратегију одређивања цена сваких неколико година.</span><span class="sxs-lookup"><span data-stu-id="94a61-105">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="94a61-106">Све исправке које унесете могу захтевати да искључите постојећу димензију за одређивање цена и креирате нову.</span><span class="sxs-lookup"><span data-stu-id="94a61-106">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="94a61-107">На пример, можда сте претходно одређивали цену по **улози**, али сте сада одлучили да то радите према **радном искуству**.</span><span class="sxs-lookup"><span data-stu-id="94a61-107">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="94a61-108">Ово може захтевати да искључите димензију за одређивање цена **Улога** и да креирате **Радно искуство** као нову димензију за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="94a61-108">This may require you to turn off **Role** as a pricing dimension and create **Work Experience** as a new pricing dimension.</span></span> 

<span data-ttu-id="94a61-109">Димензија за одређивање цена, без обзира на то да ли је унапред дефинисана или прилагођена, може се искључити у ако поља **Применљиво на трошкове** и **Применљиво на продају** у оквиру димензије за одређивање цена подесите на **Не**.</span><span class="sxs-lookup"><span data-stu-id="94a61-109">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="94a61-110">Међутим, када то учините, можда ћете добити поруку о грешци, **Димензија за одређивање цене се не може ажурирати или избрисати ако постоје повезани записи цена.**</span><span class="sxs-lookup"><span data-stu-id="94a61-110">However, when you do this, you might receive the error message, **Pricing dimension cannot be updated or deleted if there are associated price records.**</span></span>

![Грешка пословног процеса је могућа када искључујете димензију за одређивање цена](media/Business-Process-Error.png)

<span data-ttu-id="94a61-112">Ова порука о грешци указује на то да постоје записи цена који су претходно подешени за димензију која је искључена.</span><span class="sxs-lookup"><span data-stu-id="94a61-112">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="94a61-113">Све записе **Цена улоге** и **Провизија на цену улоге** који се односе на димензију морате избрисати пре него што се примењивост димензије подеси на **Не**.</span><span class="sxs-lookup"><span data-stu-id="94a61-113">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="94a61-114">Ово правило примењује се на унапред дефинисане димензије за одређивање цена и све прилагођене димензије за одређивање цена које сте можда креирали.</span><span class="sxs-lookup"><span data-stu-id="94a61-114">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="94a61-115">Разлог ове валидације је што сваки запис **Цена улоге** мора да има јединствену комбинацију димензија.</span><span class="sxs-lookup"><span data-stu-id="94a61-115">The reason for this validation is because each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="94a61-116">На пример, у ценовнику под називом **Стопе трошка у САД за 2018**, имате следеће редове **Цена улоге**.</span><span class="sxs-lookup"><span data-stu-id="94a61-116">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="94a61-117">Стандардна позиција</span><span class="sxs-lookup"><span data-stu-id="94a61-117">Standard Title</span></span>         | <span data-ttu-id="94a61-118">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="94a61-118">Org Unit</span></span>    |<span data-ttu-id="94a61-119">Јединица</span><span class="sxs-lookup"><span data-stu-id="94a61-119">Unit</span></span>   |<span data-ttu-id="94a61-120">Цена</span><span class="sxs-lookup"><span data-stu-id="94a61-120">Price</span></span>  |<span data-ttu-id="94a61-121">Валута</span><span class="sxs-lookup"><span data-stu-id="94a61-121">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="94a61-122">Инжењер система</span><span class="sxs-lookup"><span data-stu-id="94a61-122">Systems Engineer</span></span>|<span data-ttu-id="94a61-123">Contoso US</span><span class="sxs-lookup"><span data-stu-id="94a61-123">Contoso US</span></span>|<span data-ttu-id="94a61-124">Hour</span><span class="sxs-lookup"><span data-stu-id="94a61-124">Hour</span></span>| <span data-ttu-id="94a61-125">100.</span><span class="sxs-lookup"><span data-stu-id="94a61-125">100</span></span>|<span data-ttu-id="94a61-126">USD</span><span class="sxs-lookup"><span data-stu-id="94a61-126">USD</span></span>|
| <span data-ttu-id="94a61-127">Виши инжењер система</span><span class="sxs-lookup"><span data-stu-id="94a61-127">Senior Systems Engineer</span></span>|<span data-ttu-id="94a61-128">Contoso US</span><span class="sxs-lookup"><span data-stu-id="94a61-128">Contoso US</span></span>|<span data-ttu-id="94a61-129">Hour</span><span class="sxs-lookup"><span data-stu-id="94a61-129">Hour</span></span>| <span data-ttu-id="94a61-130">150</span><span class="sxs-lookup"><span data-stu-id="94a61-130">150</span></span>| <span data-ttu-id="94a61-131">USD</span><span class="sxs-lookup"><span data-stu-id="94a61-131">USD</span></span>|


<span data-ttu-id="94a61-132">Када искључите поље **Стандардна позиција** као димензију за одређивање цена, а механизам за одређивање цена претражује цену, користиће само вредност **Организациона јединица** из контекста уноса.</span><span class="sxs-lookup"><span data-stu-id="94a61-132">When you turn off **Standard Title** as the pricing dimension, and the pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="94a61-133">Ако је **Организациона јединица** контекста уноса „Contoso US“, резултат ће бити неодређен јер ће се оба реда подударати.</span><span class="sxs-lookup"><span data-stu-id="94a61-133">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="94a61-134">Да бисте избегли овај сценарио, када креирате записе **Цена улоге**, систем проверава да ли је комбинације димензија јединствена.</span><span class="sxs-lookup"><span data-stu-id="94a61-134">To avoid this scenario, when you create **Role Price** records, the system validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="94a61-135">Ако је димензија искључена након креирања записа **Цена улоге**, ово ограничење може да се прекрши.</span><span class="sxs-lookup"><span data-stu-id="94a61-135">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="94a61-136">Због тога је неопходно да пре искључивања димензије избришете све редове **Цена улоге** и **Провизија на цену улоге** у којима је та вредност димензије попуњена.</span><span class="sxs-lookup"><span data-stu-id="94a61-136">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]