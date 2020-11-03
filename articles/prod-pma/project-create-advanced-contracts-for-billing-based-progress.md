---
title: Креирајте напредне уговоре за наплату на основу напретка
description: Ова тема објашњава како се креирају пројектни уговори тако да можете генерисати фактуре за клијенте на основу процента завршеног посла.
author: RadhikaRS
manager: AnnBe
ms.date: 03/26/2020
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
ms.openlocfilehash: 1a83785a9db4dffc4585acf11ef971c08594f312
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084101"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="870dc-103">Креирајте напредне уговоре за наплату на основу напретка</span><span class="sxs-lookup"><span data-stu-id="870dc-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="870dc-104">Ова тема објашњава како се креирају пројектни уговори тако да можете креирати фактуре за клијенте на основу процента завршеног посла.</span><span class="sxs-lookup"><span data-stu-id="870dc-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="870dc-105">Износи фактура се аутоматски израчунавају за буџетске категорије посла које сте поставили за пројекат.</span><span class="sxs-lookup"><span data-stu-id="870dc-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="870dc-106">Време на фактури се поставља када преговарате са клијентом о уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="870dc-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="870dc-107">Користите процедуре у овој теми за постављање уговора, придруженог пројекта и правила обрачуна који израчунавају износе фактура за буџетске категорије посла које сте поставили за пројекат.</span><span class="sxs-lookup"><span data-stu-id="870dc-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="870dc-108">Након што направите уговор и пројекат, можете да подесите детаље о пројекту.</span><span class="sxs-lookup"><span data-stu-id="870dc-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="870dc-109">На пример, можете дефинисати активности и доделити раднике пројекту.</span><span class="sxs-lookup"><span data-stu-id="870dc-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="870dc-110">Пример</span><span class="sxs-lookup"><span data-stu-id="870dc-110">Example</span></span>

<span data-ttu-id="870dc-111">Ваша организација је фирма за развој софтвера.</span><span class="sxs-lookup"><span data-stu-id="870dc-111">Your organization is a software development firm.</span></span> <span data-ttu-id="870dc-112">Пристајете да развијете пакет за обрачун зарада за клијента за укупну накнаду од 20.000 америчких долара (USD).</span><span class="sxs-lookup"><span data-stu-id="870dc-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="870dc-113">Ваша организација пристаје да фактурише клијенту како довршавате одређене проценте пројекта.</span><span class="sxs-lookup"><span data-stu-id="870dc-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="870dc-114">За рад постављате следеће категорије пројеката како бисте их могли користити у процесу наплате:</span><span class="sxs-lookup"><span data-stu-id="870dc-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="870dc-115">Консултантске услуге</span><span class="sxs-lookup"><span data-stu-id="870dc-115">Consulting</span></span>
- <span data-ttu-id="870dc-116">Дизајн</span><span class="sxs-lookup"><span data-stu-id="870dc-116">Design</span></span>
- <span data-ttu-id="870dc-117">Инсталација</span><span class="sxs-lookup"><span data-stu-id="870dc-117">Installation</span></span>

<span data-ttu-id="870dc-118">Постављате и правила наплате која аутоматски израчунавају износе фактура за проценат завршеног посла на пројекту за сваку категорију.</span><span class="sxs-lookup"><span data-stu-id="870dc-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="870dc-119">Менаџер буџета креира буџет за категорије пројеката.</span><span class="sxs-lookup"><span data-stu-id="870dc-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="870dc-120">Количина обављеног посла аутоматски се израчунава као проценат стварног посла у поређењу са планираним износима.</span><span class="sxs-lookup"><span data-stu-id="870dc-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="870dc-121">Предуслови</span><span class="sxs-lookup"><span data-stu-id="870dc-121">Prerequisites</span></span>

<span data-ttu-id="870dc-122">Пре него што креирате пројекат који користи правила наплате, морате подесити секвенце бројева за правила наплате и дневник накнада који се користи за књижење напредовања.</span><span class="sxs-lookup"><span data-stu-id="870dc-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="870dc-123">Идите на **Управљање пројектима и рачуноводство** \> **Подешавање** \> **Управљање пројектом и рачуноводствени параметри**.</span><span class="sxs-lookup"><span data-stu-id="870dc-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="870dc-124">На страници **Управљање пројектом и рачуноводствени параметри** , на картици **Бројчане секвенце** подесите редослед бројева који желите да користите приликом креирања правила за обрачун.</span><span class="sxs-lookup"><span data-stu-id="870dc-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="870dc-125">Идите на **Управљање пројектима и рачуноводство** \> **Дневници** \> **Накнада**.</span><span class="sxs-lookup"><span data-stu-id="870dc-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="870dc-126">На страници **Дневник накнада** , изаберите **Ново** и унесите назив дневника.</span><span class="sxs-lookup"><span data-stu-id="870dc-126">On the **Fee journal** page, select **New** , and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="870dc-127">Направите уговор за напредак фактурисања</span><span class="sxs-lookup"><span data-stu-id="870dc-127">Create a contract for progress billings</span></span>

<span data-ttu-id="870dc-128">Користите овај поступак за креирање уговора о пројекту за пројекат са фиксном ценом.</span><span class="sxs-lookup"><span data-stu-id="870dc-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="870dc-129">Фактуру за пројекат креирате када посао који је завршен на пројекту достигне одређени проценат.</span><span class="sxs-lookup"><span data-stu-id="870dc-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="870dc-130">Идите на **Управљање пројектима и рачуноводство** \> **Пројекти** \> **Уговори пројеката**.</span><span class="sxs-lookup"><span data-stu-id="870dc-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="870dc-131">На страници **Уговори пројеката** изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="870dc-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="870dc-132">У дијалогу **Нови уговор о пројекту** поставите следећа поља:</span><span class="sxs-lookup"><span data-stu-id="870dc-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="870dc-133">**Именуј**</span><span class="sxs-lookup"><span data-stu-id="870dc-133">**Name**</span></span>
    - <span data-ttu-id="870dc-134">**Тип финансирања**</span><span class="sxs-lookup"><span data-stu-id="870dc-134">**Funding type**</span></span>
    - <span data-ttu-id="870dc-135">**Извор финансирања**</span><span class="sxs-lookup"><span data-stu-id="870dc-135">**Funding source**</span></span>
    - <span data-ttu-id="870dc-136">**Валута продаје** - Ова валута се подразумевано користи за рачуне купаца који су повезани са пројектним уговором.</span><span class="sxs-lookup"><span data-stu-id="870dc-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="870dc-137">Међутим, валуту продаје можете променити на одређеној фактури купца.</span><span class="sxs-lookup"><span data-stu-id="870dc-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="870dc-138">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="870dc-138">Select **OK**.</span></span> <span data-ttu-id="870dc-139">Подаци се копирају у заглавље странице **Пројектни уговори**.</span><span class="sxs-lookup"><span data-stu-id="870dc-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="870dc-140">На страници **Пројектни уговори** , попуните остатак потребних података за пројекат.</span><span class="sxs-lookup"><span data-stu-id="870dc-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="870dc-141">Направите пројекат за напредак фактурисања</span><span class="sxs-lookup"><span data-stu-id="870dc-141">Create a project for progress billings</span></span>

<span data-ttu-id="870dc-142">Следите ове кораке да бисте креирали пројекат и све потпројекте који су повезани са пројектним уговором.</span><span class="sxs-lookup"><span data-stu-id="870dc-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="870dc-143">Идите на **Управљање пројектима и рачуноводство** \> **Пројекти** \> **Сви пројекти**.</span><span class="sxs-lookup"><span data-stu-id="870dc-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="870dc-144">На страници **Сви уговори** изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="870dc-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="870dc-145">У дијалогу **Нови пројекат** , у пољу **Тип пројекта** изаберите **Време и материјал**.</span><span class="sxs-lookup"><span data-stu-id="870dc-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="870dc-146">Изаберите групу пројеката.</span><span class="sxs-lookup"><span data-stu-id="870dc-146">Select a project group.</span></span> <span data-ttu-id="870dc-147">Пројектна група дефинише информације о објављивању за пројекте који су додељени групи.</span><span class="sxs-lookup"><span data-stu-id="870dc-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="870dc-148">Изаберите **Креирајте пројекат**.</span><span class="sxs-lookup"><span data-stu-id="870dc-148">Select **Create project**.</span></span>
6. <span data-ttu-id="870dc-149">Након креирања пројекта, поставите фазу пројекта на **У току**.</span><span class="sxs-lookup"><span data-stu-id="870dc-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="870dc-150">Креирање буџета за пројекат</span><span class="sxs-lookup"><span data-stu-id="870dc-150">Create a budget for a project</span></span>

<span data-ttu-id="870dc-151">Категорије буџета се користе за аутоматско израчунавање износа фактура за проценат завршеног посла за сваку категорију.</span><span class="sxs-lookup"><span data-stu-id="870dc-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="870dc-152">Следите ове кораке да бисте креирали буџетске категорије за процењене трошкове.</span><span class="sxs-lookup"><span data-stu-id="870dc-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="870dc-153">Идите на **Управљање пројектима и рачуноводство** \> **Пројекти** \> **Сви пројекти**.</span><span class="sxs-lookup"><span data-stu-id="870dc-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="870dc-154">На страници **Сви пројекти** изаберите и отворите пројекат који желите.</span><span class="sxs-lookup"><span data-stu-id="870dc-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="870dc-155">На страници **Пројекти** , у окну акција, на картици **План** , у групи **Буџет** изаберите **Буџет пројекта**.</span><span class="sxs-lookup"><span data-stu-id="870dc-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="870dc-156">На страници **Буџет пројекта** унесите процењени трошак за сваку категорију у пројекту.</span><span class="sxs-lookup"><span data-stu-id="870dc-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="870dc-157">Креирајте правила наплате за напредовање рачуна</span><span class="sxs-lookup"><span data-stu-id="870dc-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="870dc-158">Идите на **Управљање пројектима и рачуноводство** \> **Пројекти** \> **Уговори пројеката**.</span><span class="sxs-lookup"><span data-stu-id="870dc-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="870dc-159">На страници **Уговори о пројектима** изаберите и отворите уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="870dc-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="870dc-160">На страници уговора о пројекту, на брзој картици **Правила за наплату** изаберите **Додај**.</span><span class="sxs-lookup"><span data-stu-id="870dc-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="870dc-161">На страници **Правило за обрачун** , у пољу **Тип линије** изаберите **Напредак**.</span><span class="sxs-lookup"><span data-stu-id="870dc-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="870dc-162">На брзој картици **Детаљи линије правила за обрачун** , у пољу **Вредност уговора** унесите укупну вредност уговора.</span><span class="sxs-lookup"><span data-stu-id="870dc-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="870dc-163">У пољу **Категорија** одаберите категорију у којој ћете објавити трансакцију накнаде.</span><span class="sxs-lookup"><span data-stu-id="870dc-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="870dc-164">У пољу **Пројекат** изаберите пројекат који користи ово правило наплате.</span><span class="sxs-lookup"><span data-stu-id="870dc-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="870dc-165">Опционално: Доделите правило наплате додатним пројектима.</span><span class="sxs-lookup"><span data-stu-id="870dc-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="870dc-166">На брзој картици **Пројекат** , у одељку **Доступни пројекти** изаберите пројекат, а затим притисните дугме са стрелицом удесно да бисте додали пројекат у одељак **Одабрани пројекти**.</span><span class="sxs-lookup"><span data-stu-id="870dc-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="870dc-167">Опционално: Израчунајте процентуални износ који купац задржава од плаћања на рачуну.</span><span class="sxs-lookup"><span data-stu-id="870dc-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="870dc-168">На брзој картици **Услови задржавања плаћања** изаберите извор финансирања, а затим у пољу **Проценат задржавања** унесите проценат задржавања.</span><span class="sxs-lookup"><span data-stu-id="870dc-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="870dc-169">Поновите ове кораке да бисте креирали додатна правила за обрачун за пројектни уговор.</span><span class="sxs-lookup"><span data-stu-id="870dc-169">Repeat these steps to create additional billing rules for the project contract.</span></span>
