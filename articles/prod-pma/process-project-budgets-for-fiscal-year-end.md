---
title: Пренос буџета пројеката на крај фискалне године
description: Овај чланак даје информације о томе како пренети преостале износе буџета у будуће године и створити детаље буџетског регистра.
author: Yowelle
manager: AnnBe
ms.date: 03/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 1f601be072e84fc04246cd55a260c8004f6fb3e5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289747"
---
# <a name="transfer-project-budgets-at-fiscal-year-end"></a><span data-ttu-id="1dc44-103">Пренос буџета пројеката на крај фискалне године</span><span class="sxs-lookup"><span data-stu-id="1dc44-103">Transfer project budgets at fiscal year end</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1dc44-104">Када радите на вишегодишњем пројекту, можда ћете имати преостали буџет на крају фискалне године.</span><span class="sxs-lookup"><span data-stu-id="1dc44-104">When working on a multi-year project, you might have remaining budget at the end of the fiscal year.</span></span> <span data-ttu-id="1dc44-105">Преостале износе буџета можете пренети у будућу годину и створити детаље регистра буџета за износе на повезаним рачунима главне књиге.</span><span class="sxs-lookup"><span data-stu-id="1dc44-105">You can transfer the remaining budget amounts to a future year, and create budget register details for the amounts in the associated general ledger accounts.</span></span> <span data-ttu-id="1dc44-106">Пре него што пренесете преостале износе, прегледајте и анализирајте преостале износе буџета.</span><span class="sxs-lookup"><span data-stu-id="1dc44-106">Before you carry forward the remaining amounts, review and analyze the remaining budget amounts.</span></span>

## <a name="review-and-analyze-remaining-budget-amounts"></a><span data-ttu-id="1dc44-107">Прегледајте и анализирајте преостале износе буџета</span><span class="sxs-lookup"><span data-stu-id="1dc44-107">Review and analyze remaining budget amounts</span></span>

<span data-ttu-id="1dc44-108">Довршите следеће кораке да бисте прегледали износе буџета на крају године за пројекте, али не и да бисте их пренели даље.</span><span class="sxs-lookup"><span data-stu-id="1dc44-108">Complete the following steps to review the year-end budget amounts for projects, but not carry the amounts forward.</span></span>

1. <span data-ttu-id="1dc44-109">Идите на **Управљање пројектима и рачуноводство** > **Периодично** > **Буџети** > **Пренеси буџете**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-109">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="1dc44-110">На страници **Процес преноса буџета пројекта**, на картици **Опције за крај године**, потврдите да опција **Пренесите преостале износе буџета пројекта** није омогућена.</span><span class="sxs-lookup"><span data-stu-id="1dc44-110">On the **Project budget carry-forward process** page, on the **Year-end options** tab, verify that **Carry forward remaining project budget amounts** is not enabled.</span></span>
3. <span data-ttu-id="1dc44-111">На картици **Параметри** у пољу **Година буџета пројекта** одаберите фискалну годину за коју желите да видите преостали износ буџета.</span><span class="sxs-lookup"><span data-stu-id="1dc44-111">On the **Parameters** tab, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
4. <span data-ttu-id="1dc44-112">У пољу **Почетна фискална година** одаберите фискалну годину за коју желите да видите преостали износ буџета.</span><span class="sxs-lookup"><span data-stu-id="1dc44-112">In the **Opening fiscal year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
5. <span data-ttu-id="1dc44-113">У пољу **Из модела прогнозе** изаберите **Преостали буџет**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-113">In the **From forecast model** field, select **Remaining budget**.</span></span> 
6. <span data-ttu-id="1dc44-114">Да бисте укључили пројекте који испуњавају изабране критеријуме и немају преостали буџет, изаберите **Покажи преосталу нулу**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-114">To include projects that meet your selected criteria and have no remaining budget, select **Show zero remaining**.</span></span>  
7. <span data-ttu-id="1dc44-115">На картици **Изаберите буџете** изаберите **Преузмите све буџете** да бисте учитали све буџете који одговарају одабраним критеријумима, а затим изаберите **Обради**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-115">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match your selected criteria, and then select **Process**.</span></span> 
8. <span data-ttu-id="1dc44-116">Да бисте дизајнирали упит базе података који учитава одређени скуп буџета у окно, изаберите **Преузимање изабраних буџета**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-116">To design a database query that loads a specific set of budgets into the pane, select **Retrieve selected budgets**.</span></span>

<span data-ttu-id="1dc44-117">За више информација о одређеној линији у окну одаберите линију, а затим изаберите **Прикажи детаље о буџету** или **Прикажи налоге**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-117">For more information about a specific line in the pane, select the line, and then select **View budget details** or **View accounts**.</span></span>

## <a name="carry-forward-remaining-budget-amounts"></a><span data-ttu-id="1dc44-118">Пренесите преостале износе буџета</span><span class="sxs-lookup"><span data-stu-id="1dc44-118">Carry forward remaining budget amounts</span></span> 

<span data-ttu-id="1dc44-119">Када обрађујете преостале износе буџета, можете да креирате трансакције у главној књизи за износе које преносите даље.</span><span class="sxs-lookup"><span data-stu-id="1dc44-119">When you process remaining budget amounts, you can create transactions in the general ledger for the amounts that you are carrying forward.</span></span> <span data-ttu-id="1dc44-120">Да бисте креирали трансакције главне књиге, извршите кораке у одељку [Пренесите буџетске износе и креирајте трансакције из главне књиге](#carry-forward).</span><span class="sxs-lookup"><span data-stu-id="1dc44-120">To create general ledger transactions, complete the steps in the section, [Carry forward budget amounts and create general ledger transactions](#carry-forward).</span></span> 

> [!NOTE]
> <span data-ttu-id="1dc44-121">Износи буџета који се преносе, пребацују се на модел предвиђања који је изабран на страници **Модели предвиђања** као модел прогнозе преноса.</span><span class="sxs-lookup"><span data-stu-id="1dc44-121">Budget amounts that are carried forward are transferred to the forecast model that is selected in the **Forecast models** page as the carry-forward forecast model.</span></span>  

## <a name="carry-forward-budget-amounts-and-create-general-ledger-transactions"></a><a name="carry-forward"></a><span data-ttu-id="1dc44-122">Пренесите буџетске износе и креирајте трансакције из главне књиге</span><span class="sxs-lookup"><span data-stu-id="1dc44-122">Carry forward budget amounts and create general ledger transactions</span></span>

1.  <span data-ttu-id="1dc44-123">Изаберите **Управљање пројектима и рачуноводство** > **Периодично** > **Буџети** > **Пренеси буџете**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-123">Select **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="1dc44-124">На страници **Процес преноса буџета пројекта** изаберите **Крај године**, а затим омогућите **Пренесите преостале износе буџета пројекта** и **Креирајте уносе у регистру буџета у главној књизи**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-124">On the **Project budget carry-forward process** page, select **Year-end**, and then enable **Carry forward remaining project budget amounts** and **Create budget register entries in general ledger**.</span></span> 
3. <span data-ttu-id="1dc44-125">На картици **Параметри**, у групи поља **Параметри пројекта** изаберите следеће:</span><span class="sxs-lookup"><span data-stu-id="1dc44-125">On the **Parameters** tab, in the **Project parameters** field group, select the following:</span></span>

   - <span data-ttu-id="1dc44-126">**Година буџета пројекта**: Одаберите почетак фискалне године за коју желите да видите преостале износе буџета.</span><span class="sxs-lookup"><span data-stu-id="1dc44-126">**Project budget year**: Select the beginning of the fiscal year for which you want to view the remaining budget amounts.</span></span> 
   - <span data-ttu-id="1dc44-127">**Профит и губитак**: Креирајте трансакције добити и губитка у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="1dc44-127">**Profit and loss**: Create profit and loss transactions in the general ledger.</span></span> 
   -  <span data-ttu-id="1dc44-128">**WIP**: Креирајте трансакције у току (WIP) у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="1dc44-128">**WIP**: Create Work in Progress (WIP) transactions in the general ledger.</span></span>
   -  <span data-ttu-id="1dc44-129">**Зарада**: Креирајте трансакције расподеле зарада у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="1dc44-129">**Payroll**: Create payroll allocation transactions in the general ledger.</span></span> 

5. <span data-ttu-id="1dc44-130">У групи поља **Главна књига** наведите следеће информације:</span><span class="sxs-lookup"><span data-stu-id="1dc44-130">In the **General ledger** field group, provide the following information:</span></span> 

   - <span data-ttu-id="1dc44-131">У пољу **Почетна фискална година** одаберите фискалну годину на коју желите да пренесете преостале износе буџета за пројекте.</span><span class="sxs-lookup"><span data-stu-id="1dc44-131">In the **Opening fiscal year** field, select the fiscal year that you want to transfer remaining budget amounts to for the projects.</span></span> <span data-ttu-id="1dc44-132">Подразумевана вредност је годину дана након вредности у пољу **Година буџета пројекта**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-132">The default value is one year after the value in the **Project budget year** field.</span></span>
   -  <span data-ttu-id="1dc44-133">У пољу **Период преноса** одаберите период за који желите да креирате детаље буџетског регистра у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="1dc44-133">In the **Carry-forward period** field, select the period that you want to create the budget register details for in the general ledger.</span></span> <span data-ttu-id="1dc44-134">Ово је обично први период почетне фискалне године.</span><span class="sxs-lookup"><span data-stu-id="1dc44-134">This is typically the first period in the opening fiscal year.</span></span>

6. <span data-ttu-id="1dc44-135">У групи поља **Копирање из/у** наведите следеће информације:</span><span class="sxs-lookup"><span data-stu-id="1dc44-135">In the **Copy from/to** field group, provide the following information:</span></span>

   - <span data-ttu-id="1dc44-136">У пољу **Из модела прогнозе** изаберите модел предвиђања буџета пројекта повезан са преосталим износима буџета које желите да пренесете за пројекте.</span><span class="sxs-lookup"><span data-stu-id="1dc44-136">In the **From forecast model** field, select the project budget forecast model associated with the remaining budget amounts you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="1dc44-137">У пољу **Ка моделу буџета књиге** изаберите модел буџета књиге пројекта повезан са преосталим износима буџета које желите да пренесете у главну књигу.</span><span class="sxs-lookup"><span data-stu-id="1dc44-137">In the **To ledger budget model** field, select the ledger budget model associated with the budget amounts you want to transfer to the general ledger.</span></span> 
   -  <span data-ttu-id="1dc44-138">Изаберите **Пренесите валуту продаје** да бисте користили валуту продаје пројекта за трансакције главне књиге које се креирају када пренесете износе буџета за пројекте.</span><span class="sxs-lookup"><span data-stu-id="1dc44-138">Select **Transfer sales currency** to use the project's sales currency for the general ledger transactions that are created when you transfer the budget amounts for the projects.</span></span> <span data-ttu-id="1dc44-139">Када опција није изабрана, трансакције користе рачуноводствену валуту.</span><span class="sxs-lookup"><span data-stu-id="1dc44-139">When the option is not selected, the transactions use the accounting currency.</span></span> 
   -  <span data-ttu-id="1dc44-140">Изаберите **Покажи преосталу нулу** да бисте укључили пројекте који немају преостали износ буџета, али испуњавају остале критеријуме које одаберете у пројектима приказаним у доњем окну.</span><span class="sxs-lookup"><span data-stu-id="1dc44-140">Select **Show zero remaining** to include projects that have no remaining budget amounts, but meet the other criteria that you select in the projects displayed in the bottom pane.</span></span>

7. <span data-ttu-id="1dc44-141">На картици **Изаберите буџете** изаберите **Преузмите све буџете** да бисте учитали све буџете који одговарају одабраним критеријумима.</span><span class="sxs-lookup"><span data-stu-id="1dc44-141">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match the criteria you selected.</span></span> <span data-ttu-id="1dc44-142">Ако желите да дизајнирате упит базе података који учитава одређени скуп буџета пројеката у окно, изаберите **Преузимање изабраних буџета**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-142">If you prefer to design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>
8. <span data-ttu-id="1dc44-143">За сваки пројекат који желите да обрадите одаберите опцију на почетку реда за пројекат.</span><span class="sxs-lookup"><span data-stu-id="1dc44-143">For each project that you want to process, select the option at the beginning of the line for the project.</span></span>

    > [!TIP]
    > <span data-ttu-id="1dc44-144">Да бисте изабрали све или већину пројеката, изаберите потврдни знак у горњем левом углу.</span><span class="sxs-lookup"><span data-stu-id="1dc44-144">To select all or most of the projects, select the check mark in the top upper-left corner.</span></span> <span data-ttu-id="1dc44-145">Да бисте искључили обраду било ког пројекта, уклоните ознаку за тај пројекат.</span><span class="sxs-lookup"><span data-stu-id="1dc44-145">To exclude processing any project, clear the check mark for that project.</span></span>

9. <span data-ttu-id="1dc44-146">Да бисте пребацили преостале износе буџета за изабране пројекте на изабрану фискалну годину и креирали детаље буџетског регистра у главној књизи, изаберите **Обради**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-146">To transfer the remaining budget amounts for the selected projects to the selected fiscal year and create budget register details in the general ledger, select **Process**.</span></span>

## <a name="carry-forward-budget-amounts-without-creating-general-ledger-transactions"></a><span data-ttu-id="1dc44-147">Пренесите буџетске износе без креирања трансакција из главне књиге</span><span class="sxs-lookup"><span data-stu-id="1dc44-147">Carry forward budget amounts without creating general ledger transactions</span></span>

1. <span data-ttu-id="1dc44-148">Идите на **Управљање пројектима и рачуноводство** > **Периодично** > **Буџети** > **Пренеси буџете**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-148">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span>
2. <span data-ttu-id="1dc44-149">На страници **Процес преноса буџета пројекта**, у пољу **Опције за крај године**, изаберите **Пренесите преостале износе буџета пројекта**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-149">On the **Project budget carry-forward process** page, in the **Year-end options** field, select **Carry forward remaining project budget amounts**.</span></span>
3. <span data-ttu-id="1dc44-150">У групи **Параметри** у пољу **Година буџета пројекта** одаберите фискалну годину за коју желите да видите преостале износе буџета.</span><span class="sxs-lookup"><span data-stu-id="1dc44-150">In the **Parameters** group, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amounts.</span></span>
4. <span data-ttu-id="1dc44-151">У групи **Копирање из/у** наведите следеће информације:</span><span class="sxs-lookup"><span data-stu-id="1dc44-151">In the **Copy from/to** group, provide the following information:</span></span>

   - <span data-ttu-id="1dc44-152">У пољу **Из модела прогнозе** изаберите модел предвиђања буџета пројекта који је повезан са преосталим износима буџета које желите да пренесете за пројекте.</span><span class="sxs-lookup"><span data-stu-id="1dc44-152">In the **From forecast model** field, select the project budget forecast model that is associated with the remaining budget amounts that you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="1dc44-153">Изаберите **Покажи преосталу нулу** да бисте укључили пројекте који немају преостали буџет, али испуњавају друге изабране критеријуме.</span><span class="sxs-lookup"><span data-stu-id="1dc44-153">Select **Show zero remaining** to include projects that have no remaining budget amounts, but that meet the other criteria you selected.</span></span>
   - <span data-ttu-id="1dc44-154">У групи **Изаберите буџете** изаберите **Преузмите све буџете** да бисте учитали све буџете који одговарају одабраним критеријумима.</span><span class="sxs-lookup"><span data-stu-id="1dc44-154">In the **Select Budgets** group, select **Retrieve all budgets** to load all budgets that match the criteria that you selected.</span></span> <span data-ttu-id="1dc44-155">Да бисте дизајнирали упит базе података који учитава одређени скуп буџета пројеката у окно, изаберите **Преузимање изабраних буџета**.</span><span class="sxs-lookup"><span data-stu-id="1dc44-155">To design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>

5. <span data-ttu-id="1dc44-156">За сваки пројекат који желите да обрадите одаберите опцију на почетку реда за пројекат.</span><span class="sxs-lookup"><span data-stu-id="1dc44-156">For each project that you want to process, select the option at the beginning of the line for the project.</span></span> 
6. <span data-ttu-id="1dc44-157">Изаберите **Обради** да бисте пренели преостале износе буџета за одабране пројекте на изабрану фискалну годину.</span><span class="sxs-lookup"><span data-stu-id="1dc44-157">Select **Process** to transfer the remaining budget amounts for the selected projects to the selected fiscal year.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]