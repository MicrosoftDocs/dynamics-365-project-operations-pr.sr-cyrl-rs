---
title: Конфигурисање стандардне цене рада и трошкова
description: Ова тема објашњава како да поставите стандардну цену рада и трошкове пројекта.
author: Yowelle
manager: AnnBe
ms.date: 08/02/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjCostPriceHour, ProjSalesPriceHour, ProjCostPriceExpense, ProjSalesPriceCost
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b3eb6b1d4d75b095383689dd53a59a15fe9e884a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084029"
---
# <a name="configure-standard-costs-for-labor-and-expenses"></a><span data-ttu-id="074c4-103">Конфигурисање стандардне цене рада и трошкова</span><span class="sxs-lookup"><span data-stu-id="074c4-103">Configure standard costs for labor and expenses</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="074c4-104">Ова тема објашњава како да поставите стандардну цену рада и трошкове пројекта.</span><span class="sxs-lookup"><span data-stu-id="074c4-104">This topic explains how to set up standard costs for labor and expenses for a project.</span></span> <span data-ttu-id="074c4-105">Овај задатке користи USSI скуп података.</span><span class="sxs-lookup"><span data-stu-id="074c4-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="074c4-106">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Подешавање > Цене > Цена коштања (сат)**.</span><span class="sxs-lookup"><span data-stu-id="074c4-106">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (hour)**.</span></span>
2. <span data-ttu-id="074c4-107">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="074c4-107">Select **New**.</span></span>
3. <span data-ttu-id="074c4-108">У поље **Важећи датум** унесите датум.</span><span class="sxs-lookup"><span data-stu-id="074c4-108">In the **Effective date** field, enter a date.</span></span>
4. <span data-ttu-id="074c4-109">У поље **Цена коштања** унесите број.</span><span class="sxs-lookup"><span data-stu-id="074c4-109">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="074c4-110">Можете да подесите стандардну цену коштања за категорију пројекта или можете поставити цену коштања према броју радника, броју пројекта, категорији, датуму или било којој њиховој комбинацији.</span><span class="sxs-lookup"><span data-stu-id="074c4-110">You can set up a standard cost price for the project category, or you can set up a cost price by worker number, project number, category, date, or any combination of these.</span></span> <span data-ttu-id="074c4-111">Цена коштања која се примењује је цена коштања са највишим нивоом детаља.</span><span class="sxs-lookup"><span data-stu-id="074c4-111">The cost price that is applied is the cost price with the highest level of detail.</span></span>  
5. <span data-ttu-id="074c4-112">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="074c4-112">Select **Save**.</span></span>
6. <span data-ttu-id="074c4-113">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Подешавање > Цене > Продајна цена (сат)**.</span><span class="sxs-lookup"><span data-stu-id="074c4-113">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (hour)**.</span></span>
7. <span data-ttu-id="074c4-114">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="074c4-114">Select **New**.</span></span>
8. <span data-ttu-id="074c4-115">У поље **Важећи датум** унесите датум.</span><span class="sxs-lookup"><span data-stu-id="074c4-115">In the **Effective date** field, enter a date.</span></span>
9. <span data-ttu-id="074c4-116">У пољу **Рок важења** изаберите опцију.</span><span class="sxs-lookup"><span data-stu-id="074c4-116">In the **Valid for** field, select an option.</span></span>
10. <span data-ttu-id="074c4-117">У поље **Цена** унесите број.</span><span class="sxs-lookup"><span data-stu-id="074c4-117">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="074c4-118">Можете да поставите стандардну продајну цену за трансакције по сату или за категорију пројекта.</span><span class="sxs-lookup"><span data-stu-id="074c4-118">You can set up a standard sales price for hour transactions or for a project category.</span></span> <span data-ttu-id="074c4-119">Такође можете да подесите продајне цене према броју радника, броју пројекта, категорији, датуму трансакције или било којој њиховој комбинацији.</span><span class="sxs-lookup"><span data-stu-id="074c4-119">You can also set up sales prices by worker number, project number, category, transaction date, or any combination of these.</span></span> <span data-ttu-id="074c4-120">Стварна продајна цена, која се примењује када радник уноси трансакцију у дневник часова, јесте продајна цена са највишим нивоом детаља.</span><span class="sxs-lookup"><span data-stu-id="074c4-120">The actual sales price, which is applied when a worker enters a transaction in the Hour journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="074c4-121">На пример, ако су постављене и општа продајна цена и продајна цена специфична за радника, користи се продајна цена специфична за радника.</span><span class="sxs-lookup"><span data-stu-id="074c4-121">For example, if both a general sales price and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
11. <span data-ttu-id="074c4-122">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="074c4-122">Select **Save**.</span></span>
12. <span data-ttu-id="074c4-123">Затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="074c4-123">Close the page.</span></span>
13. <span data-ttu-id="074c4-124">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Подешавање > Цене > Цена коштања (трошак)**.</span><span class="sxs-lookup"><span data-stu-id="074c4-124">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (expense)**.</span></span>
14. <span data-ttu-id="074c4-125">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="074c4-125">Select **New**.</span></span>
15. <span data-ttu-id="074c4-126">У поље **Важећи датум** унесите датум.</span><span class="sxs-lookup"><span data-stu-id="074c4-126">In the **Effective date** field, enter a date.</span></span>
16. <span data-ttu-id="074c4-127">У поље **Цена коштања** унесите број.</span><span class="sxs-lookup"><span data-stu-id="074c4-127">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="074c4-128">Може се попунити више поља, али ово је минимум потребан за чување записа.</span><span class="sxs-lookup"><span data-stu-id="074c4-128">Multiple fields can be filled in, but this is the minimum needed to save the record.</span></span>  
17. <span data-ttu-id="074c4-129">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="074c4-129">Select **Save**.</span></span>
18. <span data-ttu-id="074c4-130">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Подешавање > Цене > Продајна цена (трошак)**.</span><span class="sxs-lookup"><span data-stu-id="074c4-130">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (expense)**.</span></span>
19. <span data-ttu-id="074c4-131">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="074c4-131">Select **New**.</span></span>
20. <span data-ttu-id="074c4-132">У поље **Важећи датум** унесите датум.</span><span class="sxs-lookup"><span data-stu-id="074c4-132">In the **Effective date** field, enter a date.</span></span>
21. <span data-ttu-id="074c4-133">У пољу **Рок важења** изаберите опцију.</span><span class="sxs-lookup"><span data-stu-id="074c4-133">In the **Valid for** field, select an option.</span></span>
22. <span data-ttu-id="074c4-134">У поље **Цена** унесите број.</span><span class="sxs-lookup"><span data-stu-id="074c4-134">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="074c4-135">Стварна продајна цена, која се примењује када радник уноси трансакције у дневник трошкова, јесте продајна цена са највишим нивоом детаља.</span><span class="sxs-lookup"><span data-stu-id="074c4-135">The actual sales price, which is applied when a worker enters transactions in an expense journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="074c4-136">На пример, ако су постављене и општа продајна цена и продајна цена специфична за радника, користи се продајна цена специфична за радника.</span><span class="sxs-lookup"><span data-stu-id="074c4-136">For example, if both a general and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
23. <span data-ttu-id="074c4-137">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="074c4-137">Select **Save**.</span></span>

