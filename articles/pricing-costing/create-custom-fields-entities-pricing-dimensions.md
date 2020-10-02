---
title: Креирање прилагођених поља и ентитета као димензије за одређивање цена
description: Ова тема пружа информације о томе како да креирате прилагођене скупове опција или ентитете.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 2000f7e710267560fe2bd52b0e33024617d108ea
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898279"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="320c5-103">Креирање прилагођених поља и ентитета као димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="320c5-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="320c5-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="320c5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="320c5-105">Обавите следеће кораке када желите да креирате прилагођени скуп опција или ентитет.</span><span class="sxs-lookup"><span data-stu-id="320c5-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="320c5-106">Препоручује се да се све промене димензије прилагођене цене уносе у одвојеном решењу.</span><span class="sxs-lookup"><span data-stu-id="320c5-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="320c5-107">Ова важна најбоља пракса пружа флексибилност у будућности за ажурирање или уклањање промена по потреби, помоћи ће при поновној употреби посла и олакшава прилагођавање ових промена другој инстанци.</span><span class="sxs-lookup"><span data-stu-id="320c5-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="320c5-108">Након што унесете све потребне промене, извезите ово решење као **Комплетно решење** и увезите га у друге инстанце да бисте поново користили подешавање цена.</span><span class="sxs-lookup"><span data-stu-id="320c5-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="320c5-109">Креирање прилагођеног решења за димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="320c5-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="320c5-110">Идите на **Подешавања** > **Решења**, а затим изаберите **Ново** да бисте креирали ново решење.</span><span class="sxs-lookup"><span data-stu-id="320c5-110">Go to **Settings** > **Solutions**, and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="320c5-111">Именујте решење, **\<your organization name> димензије за одређивање цена**, унесите преостале захтеване информације, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="320c5-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="320c5-112">Креирање прилагођених поља и скупова опција у решењу за димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="320c5-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="320c5-113">Димензија одређивања цена може бити скуп опција или ентитет.</span><span class="sxs-lookup"><span data-stu-id="320c5-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="320c5-114">И једно и друго морате да креирате у решењу за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="320c5-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="320c5-115">Кораци у овој процедури објашњавају како да креирате димензије засноване на ентитетима и димензије засноване на скупу опција.</span><span class="sxs-lookup"><span data-stu-id="320c5-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="320c5-116">Димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="320c5-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="320c5-117">Идите на **Подешавања** > **Решења**, а затим двапут кликните на **\<your organization name> димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="320c5-117">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="320c5-118">У левом окну за навигацију истраживача решења изаберите **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="320c5-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="320c5-119">Изаберите **Ново** да бисте креирали нови ентитет под називом **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="320c5-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="320c5-120">Унесите преостале потребне информације, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="320c5-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="320c5-121">Димензије засноване на скупу опција</span><span class="sxs-lookup"><span data-stu-id="320c5-121">Option set-based dimensions</span></span> 
<span data-ttu-id="320c5-122">Можете креирати две димензије засноване на скуповима опција.</span><span class="sxs-lookup"><span data-stu-id="320c5-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="320c5-123">Помоћу поља **Радна локација ресурса** пратите цену радне локације **Код куће** и **На локацији** и користите **Радно време ресурса** са вредностима **Стандардно** и **Прековремено** да бисте применили провизију када се посао заврши.</span><span class="sxs-lookup"><span data-stu-id="320c5-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="320c5-124">Идите на **Подешавања** > **Решења**, а затим двапут кликните на **\<your organization name> димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="320c5-124">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="320c5-125">У левом окну за навигацију истраживача решења изаберите **Скупови опција**.</span><span class="sxs-lookup"><span data-stu-id="320c5-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="320c5-126">Изаберите **Ново** да бисте креирали нови скуп опција, унесите преостале захтеване информације, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="320c5-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="320c5-127">Креирање података за димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="320c5-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="320c5-128">Можете ручно креирати податке за димензије засноване на ентитетима или коришћењем Microsoft Excel позива за увоз или услуге.</span><span class="sxs-lookup"><span data-stu-id="320c5-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="320c5-129">Користите кораке из ове процедуре да бисте креирали две стандардне позиције, **Инжењер система** и **Виши инжењер система** из димензије засноване на ентитетима **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="320c5-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="320c5-130">Ако је обим података које желите да креирате мали, као у следећем примеру, можете да користите стандардни образац.</span><span class="sxs-lookup"><span data-stu-id="320c5-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="320c5-131">Изаберите **Напредна претрага**, изаберите ентитет **Стандардни наслов**, а затим изаберите **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="320c5-131">Select **Advanced Find**, select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="320c5-132">Биће приказани сви редови у ентитету **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="320c5-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="320c5-133">Изаберите **Ново**, а затим у поље **Име** унесите „Инжењер система“ и изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="320c5-133">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="320c5-134">Затворите образац.</span><span class="sxs-lookup"><span data-stu-id="320c5-134">Close the form.</span></span> 
4. <span data-ttu-id="320c5-135">Поновите кораке 1-3 да бисте креирали још једну стандардну позицији „Виши инжењер система“.</span><span class="sxs-lookup"><span data-stu-id="320c5-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="320c5-136">Додајте све захтеване ентитете и сродне компоненте у решење за димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="320c5-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="320c5-137">Мораћете да додате следеће ентитете у решење за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="320c5-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="320c5-138">Кораке у овој процедури користите да бисте направили неке важне промене шема у решењу за одређивање цена, тако да ентитети постану свесни нових димензија одређивања цена.</span><span class="sxs-lookup"><span data-stu-id="320c5-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="320c5-139">Изаберите **Подешавања** > **Решења**, а затим двапут кликните на **\<your organization name> димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="320c5-139">Select **Settings** > **Solutions**, and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="320c5-140">У левом окну за навигацију истраживача решења изаберите **Додај постојеће** > **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="320c5-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="320c5-141">У дијалогу **Компоненте решења** изаберите следеће ентитете:</span><span class="sxs-lookup"><span data-stu-id="320c5-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="320c5-142">Стварно</span><span class="sxs-lookup"><span data-stu-id="320c5-142">Actual</span></span>
  - <span data-ttu-id="320c5-143">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="320c5-143">Bookable Resource</span></span>
  - <span data-ttu-id="320c5-144">Ставка процене</span><span class="sxs-lookup"><span data-stu-id="320c5-144">Estimate Line</span></span>
  - <span data-ttu-id="320c5-145">Детаљ ставке фактуре</span><span class="sxs-lookup"><span data-stu-id="320c5-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="320c5-146">Ставка у главној књизи</span><span class="sxs-lookup"><span data-stu-id="320c5-146">Journal Line</span></span>
  - <span data-ttu-id="320c5-147">Детаљ предмета уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="320c5-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="320c5-148">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="320c5-148">Project Team Member</span></span>
  - <span data-ttu-id="320c5-149">Детаљ ставке понуде</span><span class="sxs-lookup"><span data-stu-id="320c5-149">Quote Line Detail</span></span>
  - <span data-ttu-id="320c5-150">Провизија на цену улоге</span><span class="sxs-lookup"><span data-stu-id="320c5-150">Role Price Markup</span></span>
  - <span data-ttu-id="320c5-151">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="320c5-151">Role Price</span></span> 
  - <span data-ttu-id="320c5-152">Ставка времена</span><span class="sxs-lookup"><span data-stu-id="320c5-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="320c5-153">Обавезно укључите све обрасце и приказе за сваки од изабраних ентитета.</span><span class="sxs-lookup"><span data-stu-id="320c5-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="320c5-154">Изаберите **Не** када се од вас затражи да укључите зависне ентитете за гореизабране ентитете.</span><span class="sxs-lookup"><span data-stu-id="320c5-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

