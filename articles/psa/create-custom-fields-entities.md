---
title: Креирање прилагођених поља и ентитета
description: Ова тема објашњава како се креирају скупови опција и ентитети у решењу платформе Power Apps.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 442ff9cf2206bec307cea7ff30b9266502d8f77b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084041"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="e4e14-103">Креирање прилагођених поља и ентитета</span><span class="sxs-lookup"><span data-stu-id="e4e14-103">Create custom fields and entities</span></span> 

<span data-ttu-id="e4e14-104">Обавите следеће кораке када желите да креирате прилагођени скуп опција или ентитет на Power Apps платформи.</span><span class="sxs-lookup"><span data-stu-id="e4e14-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="e4e14-105">Процедуре у овој теми би требало да буду завршене коришћењем веб интерфејса апликације Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="e4e14-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e4e14-106">Препоручује се да се све промене димензије прилагођене цене уносе у одвојеном решењу.</span><span class="sxs-lookup"><span data-stu-id="e4e14-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="e4e14-107">Ова важна најбоља пракса пружа флексибилност у будућности за ажурирање или уклањање промена по потреби, помоћи ће при поновној употреби посла и олакшава прилагођавање ових промена другој инстанци.</span><span class="sxs-lookup"><span data-stu-id="e4e14-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="e4e14-108">Након што унесете све потребне промене, извезите ово решење као **Комплетно решење** и увезите га у друге инстанце да бисте поново користили подешавање цена.</span><span class="sxs-lookup"><span data-stu-id="e4e14-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="e4e14-109">Креирање прилагођених поља и скупова опција у решењу за димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="e4e14-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="e4e14-110">Димензија одређивања цена може бити скуп опција или ентитет.</span><span class="sxs-lookup"><span data-stu-id="e4e14-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="e4e14-111">И једно и друго морате да креирате у решењу за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="e4e14-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="e4e14-112">Кораци у овој процедури објашњавају како да креирате димензије засноване на ентитетима и димензије засноване на скупу опција.</span><span class="sxs-lookup"><span data-stu-id="e4e14-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="e4e14-113">Димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="e4e14-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="e4e14-114">У PSA кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-114">In PSA, click **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="e4e14-115">У левом окну за навигацију истраживача решења изаберите **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="e4e14-116">Кликните на **Нови** да бисте креирали нови ентитет под називом **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="e4e14-117">Унесите преостале потребне информације, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![Дефиниција стандардног ентитета назива](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="e4e14-119">Димензије засноване на скупу опција</span><span class="sxs-lookup"><span data-stu-id="e4e14-119">Option set-based dimensions</span></span> 
<span data-ttu-id="e4e14-120">Можете креирати две димензије засноване на скуповима опција.</span><span class="sxs-lookup"><span data-stu-id="e4e14-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="e4e14-121">Помоћу поља **Радна локација ресурса** пратите цену радне локације **Код куће** и **На локацији** и користите **Радно време ресурса** са вредностима **Стандардно** и **Прековремено** да бисте применили провизију када се посао заврши.</span><span class="sxs-lookup"><span data-stu-id="e4e14-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="e4e14-122">У PSA кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-122">In PSA, click **Settings** > **Solutions** , and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="e4e14-123">У левом окну за навигацију истраживача решења изаберите **Скупови опција**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="e4e14-124">Кликните на **Ново** да бисте креирали нови скуп опција, унесите преостале захтеване информације, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="e4e14-125">Димензија одређивања цена заснована на скупу опција под називом Радна локација ресурса</span><span class="sxs-lookup"><span data-stu-id="e4e14-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="e4e14-126">Димензија одређивања цена заснована на скупу опција под називом Радно време ресурса</span><span class="sxs-lookup"><span data-stu-id="e4e14-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="e4e14-127">Креирање података за димензије засноване на ентитетима</span><span class="sxs-lookup"><span data-stu-id="e4e14-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="e4e14-128">Можете ручно креирати податке за димензије засноване на ентитетима или коришћењем Microsoft Excel позива за увоз или услуге.</span><span class="sxs-lookup"><span data-stu-id="e4e14-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="e4e14-129">Користите кораке из ове процедуре да бисте креирали две стандардне позиције, **Инжењер система** и **Виши инжењер система** из димензије засноване на ентитетима **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="e4e14-130">Ако је обим података које желите да креирате мали, као у следећем примеру, можете да користите стандардни образац.</span><span class="sxs-lookup"><span data-stu-id="e4e14-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="e4e14-131">У апликацији PSA, кликните на **Напредна претрага**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="e4e14-132">Изаберите ентитет **Стандардна позиција** а, а затим кликните на **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="e4e14-133">Биће приказани сви редови у ентитету **Стандардна позиција**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="e4e14-134">Кликните на дугме **Ново**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-134">Click **New**.</span></span> <span data-ttu-id="e4e14-135">У поље **Назив** унесите „Инжењер система“, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="e4e14-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="e4e14-136">Затворите образац.</span><span class="sxs-lookup"><span data-stu-id="e4e14-136">Close the form.</span></span> 
4. <span data-ttu-id="e4e14-137">Поновите кораке 1-3 да бисте креирали још једну стандардну позицији „Виши инжењер система“.</span><span class="sxs-lookup"><span data-stu-id="e4e14-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="e4e14-138">Пробни подаци за ентитет Стандардна позиција</span><span class="sxs-lookup"><span data-stu-id="e4e14-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)


