---
title: Креирање прилагођених поља и ентитета као димензије за одређивање цена
description: Ова тема пружа информације о томе како да креирате прилагођене скупове опција или ентитете.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
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
ms.openlocfilehash: fc5917856b8f28d36dc55593a68eba7823a00b36
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642831"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="0c0cf-103">Креирање прилагођених поља и ентитета као димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="0c0cf-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="0c0cf-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="0c0cf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0c0cf-105">Обавите следеће кораке када желите да креирате прилагођени скуп опција или ентитет за коришћење као димензије одређивања цена.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="0c0cf-106">За више информација погледајте [Прегледу димензија одређивања цена](pricing-dimensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="0c0cf-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="0c0cf-107">Препоручује се да се све промене димензије прилагођене цене уносе у одвојеном решењу.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="0c0cf-108">Ова важна најбоља пракса пружа флексибилност у будућности за ажурирање или уклањање промена по потреби.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="0c0cf-109">Ово ће такође помоћи у поновној употреби вашег посла и олакшати пренос ових промена на другу инстанцу. Након што извршите све потребне промене, извезите ово решење као **Комплетно решење** и увезите га у друге инстанце да бисте поново користили подешавање цена.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="0c0cf-110">Креирање прилагођених поља и скупова опција у решењу за димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="0c0cf-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="0c0cf-111">Димензија одређивања цена може бити скуп опција или ентитет.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="0c0cf-112">И једно и друго морате да креирате у решењу за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="0c0cf-113">Кораци у овој процедури објашњавају како да креирате димензије засноване на ентитетима и димензије засноване на скупу опција.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="0c0cf-114">Димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="0c0cf-114">Entity-based dimensions</span></span>
<span data-ttu-id="0c0cf-115">Да бисте креирали димензије засноване на ентитетима, следите ове кораке:</span><span class="sxs-lookup"><span data-stu-id="0c0cf-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="0c0cf-116">Идите на **Подешавања** > **Решења**, а затим двапут кликните на **\<your organization name> димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="0c0cf-117">У левом окну за навигацију истраживача решења изаберите **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="0c0cf-118">Изаберите **Ново** да бисте креирали нови ентитет под називом **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="0c0cf-119">Унесите преостале потребне информације, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![Дефиниција стандардног ентитета назива](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="0c0cf-121">Димензије засноване на скупу опција</span><span class="sxs-lookup"><span data-stu-id="0c0cf-121">Option set-based dimensions</span></span> 
<span data-ttu-id="0c0cf-122">Можете креирати две димензије засноване на скуповима опција.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="0c0cf-123">Користите **Место рада ресурса** да бисте пратили цену за рад на локацији **Кућа** и за рад **На локацији**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="0c0cf-124">Користите **Радно време ресурса** са вредностима **Редовно** и **Прековремено** да бисте применили провизију када је посао завршен.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="0c0cf-125">Следећи графикон даје приказ димензије **Место рада ресурса**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![Димензија одређивања цена заснована на скупу опција под називом Радна локација ресурса](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="0c0cf-127">Следећи графикон даје приказ димензије **Радно време ресурса**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![Димензија одређивања цена заснована на скупу опција под називом Радно време ресурса](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="0c0cf-129">Идите на **Подешавања** > **Решења**, а затим двапут кликните на **\<your organization name> димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="0c0cf-130">У левом окну за навигацију истраживача решења изаберите **Скупови опција**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="0c0cf-131">Изаберите **Ново** да бисте креирали нови скуп опција, унесите преостале захтеване информације, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="0c0cf-132">Креирање података за димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="0c0cf-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="0c0cf-133">Можете ручно креирати податке за димензије засноване на ентитетима или коришћењем Microsoft Excel позива за увоз или услуге.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="0c0cf-134">Користите кораке из ове процедуре да бисте креирали две стандардне позиције, **Инжењер система** и **Виши инжењер система** из димензије засноване на ентитетима **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="0c0cf-135">Ако је обим података које желите да креирате мали, као у следећем примеру, можете да користите стандардни образац.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="0c0cf-136">Изаберите **Напредна претрага**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="0c0cf-137">Изаберите ентитет **Стандардна позиција** а, а затим изаберите **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="0c0cf-138">Биће приказани сви редови у ентитету **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="0c0cf-139">Изаберите **Ново**, а затим у поље **Име** унесите „Инжењер система“ и изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="0c0cf-140">Затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-140">Close the page.</span></span> 
5. <span data-ttu-id="0c0cf-141">Поновите кораке 1-3 да бисте креирали још једну стандардну позицији „Виши инжењер система“.</span><span class="sxs-lookup"><span data-stu-id="0c0cf-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![Пробни подаци за ентитет Стандардна позиција](media/ST-data.png)
