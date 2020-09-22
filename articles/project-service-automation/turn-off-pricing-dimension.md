---
title: Искључивање димензије за одређивање цена
description: Ова тема показује како се подешавају димензије за одређивање цена у решењу Project Service.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 689e5a8d-e39a-471d-a6c4-7e2fc3bb5590
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 5cf2cd86fb1eba50c8e08b2bd624669ab0b1deb3
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755414"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="fdf3c-103">Искључивање димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="fdf3c-103">Turn off a pricing dimension</span></span>

<span data-ttu-id="fdf3c-104">Можда ћете морати да прегледате и ажурирате своју стратегију одређивања цена сваких неколико година.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="fdf3c-105">Све исправке које унесете могу захтевати да искључите постојећу димензију за одређивање цена и креирате нову.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="fdf3c-106">На пример, можда сте претходно одређивали цену по **улози**, али сте сада одлучили да то радите према **радном искуству**.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="fdf3c-107">Ово може захтевати да искључите димензију за одређивање цена **Улога** и да креирате **Радно искуство** као нову димензију за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="fdf3c-108">Димензија за одређивање цена, без обзира на то да ли је унапред дефинисана или прилагођена, може се искључити у ако поља **Применљиво на трошкове** и **Применљиво на продају** у оквиру димензије за одређивање цена подесите на **Не**.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="fdf3c-109">Међутим, када то урадите, можда ћете добити следећу поруку о грешци.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-109">However, when you do this, you might receive the following error message.</span></span>

![Грешка пословног процеса је могућа када искључујете димензију за одређивање цена](media/Business-Process-Error.png)


<span data-ttu-id="fdf3c-111">Ова порука о грешци указује на то да постоје записи цена који су претходно подешени за димензију која је искључена.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="fdf3c-112">Све записе **Цена улоге** и **Провизија на цену улоге** који се односе на димензију морате избрисати пре него што се примењивост димензије подеси на **Не**.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="fdf3c-113">Ово правило примењује се на унапред дефинисане димензије за одређивање цена и све прилагођене димензије за одређивање цена које сте можда креирали.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="fdf3c-114">Разлог ове валидације је што Project Service има ограничење да сваки запис **Цена улоге** мора да има јединствену комбинацију димензија.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="fdf3c-115">На пример, у ценовнику под називом **Стопе трошка у САД за 2018**, имате следеће редове **Цена улоге**.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="fdf3c-116">Стандардна позиција</span><span class="sxs-lookup"><span data-stu-id="fdf3c-116">Standard Title</span></span>         | <span data-ttu-id="fdf3c-117">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="fdf3c-117">Org Unit</span></span>    |<span data-ttu-id="fdf3c-118">Јединица</span><span class="sxs-lookup"><span data-stu-id="fdf3c-118">Unit</span></span>   |<span data-ttu-id="fdf3c-119">Цена</span><span class="sxs-lookup"><span data-stu-id="fdf3c-119">Price</span></span>  |<span data-ttu-id="fdf3c-120">Валута</span><span class="sxs-lookup"><span data-stu-id="fdf3c-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="fdf3c-121">Инжењер система</span><span class="sxs-lookup"><span data-stu-id="fdf3c-121">Systems Engineer</span></span>|<span data-ttu-id="fdf3c-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="fdf3c-122">Contoso US</span></span>|<span data-ttu-id="fdf3c-123">Hour</span><span class="sxs-lookup"><span data-stu-id="fdf3c-123">Hour</span></span>| <span data-ttu-id="fdf3c-124">100.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-124">100</span></span>|<span data-ttu-id="fdf3c-125">USD</span><span class="sxs-lookup"><span data-stu-id="fdf3c-125">USD</span></span>|
| <span data-ttu-id="fdf3c-126">Виши инжењер система</span><span class="sxs-lookup"><span data-stu-id="fdf3c-126">Senior Systems Engineer</span></span>|<span data-ttu-id="fdf3c-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="fdf3c-127">Contoso US</span></span>|<span data-ttu-id="fdf3c-128">Hour</span><span class="sxs-lookup"><span data-stu-id="fdf3c-128">Hour</span></span>| <span data-ttu-id="fdf3c-129">150</span><span class="sxs-lookup"><span data-stu-id="fdf3c-129">150</span></span>| <span data-ttu-id="fdf3c-130">USD</span><span class="sxs-lookup"><span data-stu-id="fdf3c-130">USD</span></span>|


<span data-ttu-id="fdf3c-131">Када искључите поље **Стандардна позиција** као димензију за одређивање цена, а Project Service механизам за одређивање цена претражује цену, користиће само вредност **Организациона јединица** из контекста уноса.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="fdf3c-132">Ако је **Организациона јединица** контекста уноса „Contoso US“, резултат ће бити неодређен јер ће се оба реда подударати.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="fdf3c-133">Да бисте избегли овај сценарио, када креирате записе **Цена улоге**, Project Service проверава да ли је комбинације димензија јединствена.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="fdf3c-134">Ако је димензија искључена након креирања записа **Цена улоге**, ово ограничење може да се прекрши.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="fdf3c-135">Због тога је неопходно да пре искључивања димензије избришете све редове **Цена улоге** и **Провизија на цену улоге** у којима је та вредност димензије попуњена.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>

