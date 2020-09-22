---
title: Конфигурисање фактурисања међукомпанијских пројеката
description: Ова тема показује како да подесите фактурисање пројеката између две компаније у вашој организацији.
author: KimANelson
manager: AnnBe
ms.date: 07/29/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendTable, InterCompanyTradingRelationSetupVendor, SysDataAreaSelectLookup, ProjParameters, ProjPosting, ProjTransferPrice
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.assetid: 72d6c257-f2d3-483b-8ff2-445263796963
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 7b199c85736f6268bc5914fddaa10e4cabd44ef1
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755334"
---
# <a name="configure-intercompany-project-invoicing"></a><span data-ttu-id="cb18a-103">Конфигурисање фактурисања међукомпанијских пројеката</span><span class="sxs-lookup"><span data-stu-id="cb18a-103">Configure intercompany project invoicing</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="cb18a-104">Ова тема показује како да подесите фактурисање пројеката између две компаније у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="cb18a-104">This topic shows how to set up project invoicing between two companies in your organization.</span></span> <span data-ttu-id="cb18a-105">Овај задатке користи USSI скуп података.</span><span class="sxs-lookup"><span data-stu-id="cb18a-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="cb18a-106">У окну за навигацију идите на **Модули > Дуговања > Продавци > Сви продавци**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-106">In the navigation pane, go to **Modules > Accounts payable > Vendors > All vendors**.</span></span>
2. <span data-ttu-id="cb18a-107">На листи **Сви продавци** пронађите и изаберите жељени запис.</span><span class="sxs-lookup"><span data-stu-id="cb18a-107">In the **All vendors** list, find and select the desired record.</span></span>
3. <span data-ttu-id="cb18a-108">У окну радњи изаберите **Општи подаци**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-108">On the Action Pane, select **General**.</span></span>
4. <span data-ttu-id="cb18a-109">Изаберите **Међукомпанијски**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-109">Select **Intercompany**.</span></span>
5. <span data-ttu-id="cb18a-110">Подесите **Активно** на **Да** како би се омогућило међукомпанијско трговање.</span><span class="sxs-lookup"><span data-stu-id="cb18a-110">Set **Active** to **Yes** to enable intercompany trading.</span></span>
6. <span data-ttu-id="cb18a-111">У поље **Компанија клијента** унесите или изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="cb18a-111">In the **Customer company** field, enter or select a value.</span></span>
7. <span data-ttu-id="cb18a-112">У поље **Мој пословни контакт** унесите или изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="cb18a-112">In the **My account** field, enter or select a value.</span></span>
8. <span data-ttu-id="cb18a-113">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-113">Select **Save**.</span></span>
9. <span data-ttu-id="cb18a-114">Затворите странице да бисте се вратили на почетну страницу.</span><span class="sxs-lookup"><span data-stu-id="cb18a-114">Close the pages to return to the home page.</span></span>
10. <span data-ttu-id="cb18a-115">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Подешавање > Цене > Параметри управљања пројектима и рачуноводством**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-115">In the navigation pane, go to **Modules > Project management and accounting > Setup > Project management and accounting parameters**.</span></span>
11. <span data-ttu-id="cb18a-116">Изаберите картицу **Међукомпанијски**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-116">Select the **Intercompany** tab.</span></span>
12. <span data-ttu-id="cb18a-117">Померите клизач на **Да** како би се омогућило међукомпанијско распоређивање ресурса и временски распореди.</span><span class="sxs-lookup"><span data-stu-id="cb18a-117">Move the slider to **Yes** to enable intercompany resource scheduling and timesheets.</span></span>
13. <span data-ttu-id="cb18a-118">Означите изабрани ред на листи.</span><span class="sxs-lookup"><span data-stu-id="cb18a-118">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="cb18a-119">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-119">Select **New**.</span></span>
15. <span data-ttu-id="cb18a-120">У поље **Правно лице које позајмљује** унесите или изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="cb18a-120">In the **Borrowing legal entity** field, enter or select a value.</span></span>
16. <span data-ttu-id="cb18a-121">Изаберите поље за потврду **Припадајући приход**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-121">Select the **Accrue revenue** check box.</span></span>
17. <span data-ttu-id="cb18a-122">У поље **Подразумевана категорија временског распореда** унесите или изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="cb18a-122">In the **Default timesheet category** field, enter or select a value.</span></span>
18. <span data-ttu-id="cb18a-123">У поље **Подразумевана категорија трошка** унесите или изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="cb18a-123">In the **Default expense category** field, enter or select a value.</span></span>
19. <span data-ttu-id="cb18a-124">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-124">Select **Save**.</span></span>
20. <span data-ttu-id="cb18a-125">Затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="cb18a-125">Close the page.</span></span>
21. <span data-ttu-id="cb18a-126">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Књижење > Подешавање књижења у главној књизи**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-126">In the navigation pane, go to **Modules > Project management and accounting > Setup > Posting > Ledger posting setup**.</span></span>
22. <span data-ttu-id="cb18a-127">У пољу **Врсте рачуна главне књиге**, изаберите опцију.</span><span class="sxs-lookup"><span data-stu-id="cb18a-127">In the **Ledger account types** field, select an option.</span></span>
23. <span data-ttu-id="cb18a-128">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-128">Select **New**.</span></span>
24. <span data-ttu-id="cb18a-129">У пољу **Главни рачун** новог реда, наведите жељене вредности.</span><span class="sxs-lookup"><span data-stu-id="cb18a-129">In the **Main account** field of the new row, specify the desired values.</span></span>
25. <span data-ttu-id="cb18a-130">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-130">Select **Save**.</span></span>
26. <span data-ttu-id="cb18a-131">Затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="cb18a-131">Close the page.</span></span>
27. <span data-ttu-id="cb18a-132">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Подешавање > Цене > Цена трансфера**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-132">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Transfer price**.</span></span>
28. <span data-ttu-id="cb18a-133">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-133">Select **New**.</span></span>
29. <span data-ttu-id="cb18a-134">У поље **Важећи датум** унесите датум.</span><span class="sxs-lookup"><span data-stu-id="cb18a-134">In the **Effective date** field, enter a date.</span></span>
30. <span data-ttu-id="cb18a-135">У поље **Правно лице које позајмљује** унесите или изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="cb18a-135">In the **Borrowing legal entity** field, enter or select a value.</span></span>
31. <span data-ttu-id="cb18a-136">У пољу **Модел цене трансфера** изаберите опцију.</span><span class="sxs-lookup"><span data-stu-id="cb18a-136">In the **Transfer price model** field, select an option.</span></span>
32. <span data-ttu-id="cb18a-137">У поље **Цена** унесите број.</span><span class="sxs-lookup"><span data-stu-id="cb18a-137">In the **Pricing** field, enter a number.</span></span>
33. <span data-ttu-id="cb18a-138">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="cb18a-138">Select **Save**.</span></span>

