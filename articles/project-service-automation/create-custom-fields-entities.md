---
title: Креирање прилагођених поља и ентитета
description: Ова тема објашњава како се креирају скупови опција и ентитети у решењу платформе Power Apps.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755441"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="96f3d-103">Креирање прилагођених поља и ентитета</span><span class="sxs-lookup"><span data-stu-id="96f3d-103">Create custom fields and entities</span></span> 

<span data-ttu-id="96f3d-104">Обавите следеће кораке када желите да креирате прилагођени скуп опција или ентитет на Power Apps платформи.</span><span class="sxs-lookup"><span data-stu-id="96f3d-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="96f3d-105">Процедуре у овој теми би требало да буду завршене коришћењем веб интерфејса апликације Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="96f3d-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="96f3d-106">Препоручује се да се све промене димензије прилагођене цене уносе у одвојеном решењу.</span><span class="sxs-lookup"><span data-stu-id="96f3d-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="96f3d-107">Ова важна најбоља пракса пружа флексибилност у будућности за ажурирање или уклањање промена по потреби, помоћи ће при поновној употреби посла и олакшава прилагођавање ових промена другој инстанци.</span><span class="sxs-lookup"><span data-stu-id="96f3d-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="96f3d-108">Након што унесете све потребне промене, извезите ово решење као **Комплетно решење** и увезите га у друге инстанце да бисте поново користили подешавање цена.</span><span class="sxs-lookup"><span data-stu-id="96f3d-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="96f3d-109">Креирање прилагођеног решења за димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="96f3d-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="96f3d-110">У апликацији PSA, кликните на **Подешавања** > **Решења**, а затим кликните на **Ново** да бисте креирали ново решење.</span><span class="sxs-lookup"><span data-stu-id="96f3d-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="96f3d-111">Именујте решење, **\<име организације > димензије за одређивање цена**, унесите преостале захтеване информације, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![Креирање прилагођеног решења за димензије за одређивање цена](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="96f3d-113">Креирање прилагођених поља и скупова опција у решењу за димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="96f3d-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="96f3d-114">Димензија одређивања цена може бити скуп опција или ентитет.</span><span class="sxs-lookup"><span data-stu-id="96f3d-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="96f3d-115">И једно и друго морате да креирате у решењу за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="96f3d-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="96f3d-116">Кораци у овој процедури објашњавају како да креирате димензије засноване на ентитетима и димензије засноване на скупу опција.</span><span class="sxs-lookup"><span data-stu-id="96f3d-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="96f3d-117">Димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="96f3d-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="96f3d-118">У апликацији PSA кликните на **Подешавања** > **Решења**, а затим двапут на **\<име организације > димензије одређивања цена**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="96f3d-119">У левом окну за навигацију истраживача решења изаберите **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="96f3d-120">Кликните на **Нови** да бисте креирали нови ентитет под називом **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="96f3d-121">Унесите преостале потребне информације, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![Дефиниција стандардног ентитета назива](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="96f3d-123">Димензије засноване на скупу опција</span><span class="sxs-lookup"><span data-stu-id="96f3d-123">Option set-based dimensions</span></span> 
<span data-ttu-id="96f3d-124">Можете креирати две димензије засноване на скуповима опција.</span><span class="sxs-lookup"><span data-stu-id="96f3d-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="96f3d-125">Помоћу поља **Радна локација ресурса** пратите цену радне локације **Код куће** и **На локацији** и користите **Радно време ресурса** са вредностима **Стандардно** и **Прековремено** да бисте применили провизију када се посао заврши.</span><span class="sxs-lookup"><span data-stu-id="96f3d-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="96f3d-126">У апликацији PSA кликните на **Подешавања** > **Решења**, а затим двапут на **\<име организације > димензије одређивања цена**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="96f3d-127">У левом окну за навигацију истраживача решења изаберите **Скупови опција**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="96f3d-128">Кликните на **Ново** да бисте креирали нови скуп опција, унесите преостале захтеване информације, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="96f3d-129">Димензија одређивања цена заснована на скупу опција под називом Радна локација ресурса</span><span class="sxs-lookup"><span data-stu-id="96f3d-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="96f3d-130">Димензија одређивања цена заснована на скупу опција под називом Радно време ресурса</span><span class="sxs-lookup"><span data-stu-id="96f3d-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="96f3d-131">Креирање података за димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="96f3d-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="96f3d-132">Можете ручно креирати податке за димензије засноване на ентитетима или коришћењем Microsoft Excel позива за увоз или услуге.</span><span class="sxs-lookup"><span data-stu-id="96f3d-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="96f3d-133">Користите кораке из ове процедуре да бисте креирали две стандардне позиције, **Инжењер система** и **Виши инжењер система** из димензије засноване на ентитетима **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="96f3d-134">Ако је обим података које желите да креирате мали, као у следећем примеру, можете да користите стандардни образац.</span><span class="sxs-lookup"><span data-stu-id="96f3d-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="96f3d-135">У апликацији PSA, кликните на **Напредна претрага**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="96f3d-136">Изаберите ентитет **Стандардна позиција** а, а затим кликните на **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="96f3d-137">Биће приказани сви редови у ентитету **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="96f3d-138">Кликните на дугме **Ново**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-138">Click **New**.</span></span> <span data-ttu-id="96f3d-139">У поље **Назив** унесите „Инжењер система“, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="96f3d-140">Затворите образац.</span><span class="sxs-lookup"><span data-stu-id="96f3d-140">Close the form.</span></span> 
4. <span data-ttu-id="96f3d-141">Поновите кораке 1-3 да бисте креирали још једну стандардну позицији „Виши инжењер система“.</span><span class="sxs-lookup"><span data-stu-id="96f3d-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="96f3d-142">Пробни подаци за ентитет Стандардна позиција</span><span class="sxs-lookup"><span data-stu-id="96f3d-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="96f3d-143">Додајте све захтеване PSA ентитете и сродне компоненте у решење за димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="96f3d-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="96f3d-144">Мораћете да додате следеће Project Service ентитете у решење за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="96f3d-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="96f3d-145">Кораке у овој процедури користите да бисте направили неке важне промене шема у решењу за одређивање цена, тако да ентитети постану свесни нових димензија одређивања цена.</span><span class="sxs-lookup"><span data-stu-id="96f3d-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="96f3d-146">У апликацији PSA кликните на **Подешавања** > **Решења**, а затим двапут на **\<име организације > димензије одређивања цена**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="96f3d-147">У левом окну за навигацију истраживача решења изаберите **Додај постојеће** > **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="96f3d-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="96f3d-148">У дијалогу **Компоненте решења** изаберите следеће ентитете:</span><span class="sxs-lookup"><span data-stu-id="96f3d-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="96f3d-149">Стварно</span><span class="sxs-lookup"><span data-stu-id="96f3d-149">Actual</span></span>
- <span data-ttu-id="96f3d-150">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="96f3d-150">Bookable Resource</span></span>
- <span data-ttu-id="96f3d-151">Ставка процене</span><span class="sxs-lookup"><span data-stu-id="96f3d-151">Estimate Line</span></span>
- <span data-ttu-id="96f3d-152">Детаљ ставке фактуре</span><span class="sxs-lookup"><span data-stu-id="96f3d-152">Invoice Line Detail</span></span>
- <span data-ttu-id="96f3d-153">Ставка у главној књизи</span><span class="sxs-lookup"><span data-stu-id="96f3d-153">Journal Line</span></span>
- <span data-ttu-id="96f3d-154">Детаљ предмета уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="96f3d-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="96f3d-155">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="96f3d-155">Project Team Member</span></span>
- <span data-ttu-id="96f3d-156">Детаљ ставке понуде</span><span class="sxs-lookup"><span data-stu-id="96f3d-156">Quote Line Detail</span></span>
- <span data-ttu-id="96f3d-157">Провизија на цену улоге</span><span class="sxs-lookup"><span data-stu-id="96f3d-157">Role Price Markup</span></span>
- <span data-ttu-id="96f3d-158">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="96f3d-158">Role Price</span></span> 
- <span data-ttu-id="96f3d-159">Ставка времена</span><span class="sxs-lookup"><span data-stu-id="96f3d-159">Time Entry</span></span> 

> ![Додавање постојећих ентитета у решење за димензије одређивања цена](media/Existing-entities-to-PD-solution.png)

> ![Изаберите компоненте решења](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="96f3d-162">Обавезно укључите све обрасце и приказе за сваки од изабраних ентитета.</span><span class="sxs-lookup"><span data-stu-id="96f3d-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="96f3d-163">Кликните на **Не** када се од вас затражи да укључите зависне ентитете за гореизабране ентитете.</span><span class="sxs-lookup"><span data-stu-id="96f3d-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![Немојте да укључујете све повезане компоненте](media/Do-not-include-required.png)


