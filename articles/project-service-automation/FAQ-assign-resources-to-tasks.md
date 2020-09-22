---
title: Додељивање ресурса задатку
description: Ова тема пружа информације о томе како доделити ресурсе задацима.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
ms.topic: article
ms.prod: Project Service
ms.technology: Dynamics 365 Project Service Automation 3.x
ms.assetid: 3ea9516c-0276-4e30-b308-f792f64d608b
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 509f7a4464b2e810900b31a78219ba696192a18b
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755477"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="65d7c-103">Додељивање ресурса задатку</span><span class="sxs-lookup"><span data-stu-id="65d7c-103">Assign a resource to a task</span></span>

<span data-ttu-id="65d7c-104">Постоје три начина доделе ресурса задатку у апликацији Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="65d7c-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="65d7c-105">Резервисање ресурса као члана тима и додела ресурса задатку</span><span class="sxs-lookup"><span data-stu-id="65d7c-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="65d7c-106">Ресурс можете да додате у пројектни тим, а затим да додељујете ресурс задацима у распореду пројекта.</span><span class="sxs-lookup"><span data-stu-id="65d7c-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="65d7c-107">На картици **Члан тима** додајте новог члана тима тако што ћете изабрати **Нови**.</span><span class="sxs-lookup"><span data-stu-id="65d7c-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="65d7c-108">Отвара се табла за **брзо креирање члана тима**, где можете да изаберете име ресурса који може да се резервише и подесите улогу.</span><span class="sxs-lookup"><span data-stu-id="65d7c-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="65d7c-109">Изаберите један од следећих начина доделе за резервацију ресурса:</span><span class="sxs-lookup"><span data-stu-id="65d7c-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="65d7c-110">**Пун капацитет** резервише пуни капацитет ресурса за наведене почетне и крајње датуме.</span><span class="sxs-lookup"><span data-stu-id="65d7c-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="65d7c-111">**Проценат капацитета** резервише одређени проценат капацитета ресурса за наведене датуме почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="65d7c-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="65d7c-112">**Равномерно распоређивање по сатима** резервише ресурс за одређени број часова, равномерно их распоређујући по дану током наведених датума почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="65d7c-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="65d7c-113">**По сатима – Почетно оптерећење** резервише ресурс за одређени број часова, распоређујући часове рада по дану на прве дане током наведених датума почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="65d7c-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="65d7c-114">**Ниједно** додаје ресурс тиму, али не креира ниједну резервацију која троши њихов капацитет.</span><span class="sxs-lookup"><span data-stu-id="65d7c-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="65d7c-115">На мрежи **Распоред** за задатак, изаберите икону **Ресурс** у ћелији ресурса, а затим у делу **Чланови тима** изаберите члана тима којег сте управо додали.</span><span class="sxs-lookup"><span data-stu-id="65d7c-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members**, select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="65d7c-116">Ресурс приказује резервисане и додељене часове и на картицама **Члан тима** и **Усаглашеност**.</span><span class="sxs-lookup"><span data-stu-id="65d7c-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="65d7c-117">Сати би требало да буду исти, али то није неопходно јер резервације и доделе нису чврсто повезане.</span><span class="sxs-lookup"><span data-stu-id="65d7c-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="65d7c-118">Картица **Усаглашеност** вам даје детаље када се разликују, као када доделите ресурсу више часова него што сте резервисали.</span><span class="sxs-lookup"><span data-stu-id="65d7c-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="65d7c-119">По потреби можете да исправите информације проширивањем резервације ресурса или променом доделе.</span><span class="sxs-lookup"><span data-stu-id="65d7c-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="65d7c-120">Креирање генеричког члана тима преко доделе задатка</span><span class="sxs-lookup"><span data-stu-id="65d7c-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="65d7c-121">Када креирате генеричког члана тима преко доделе задатка, креирате чувар места или генерички ресурс који описује карактеристике именованог ресурса за којег напослетку желите да ради на задацима.</span><span class="sxs-lookup"><span data-stu-id="65d7c-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="65d7c-122">Затим генеришете услов (или прослеђујете захтев коришћењем захтева) који се користи за претрагу и резервацију именованог ресурса.</span><span class="sxs-lookup"><span data-stu-id="65d7c-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="65d7c-123">На мрежи **Распоред** за задатак, изаберите икону **ресурса** у ћелији Ресурс.</span><span class="sxs-lookup"><span data-stu-id="65d7c-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="65d7c-124">Унесите име које ће служити као име чувара места ресурса.</span><span class="sxs-lookup"><span data-stu-id="65d7c-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="65d7c-125">На пример, Менаџер програма.</span><span class="sxs-lookup"><span data-stu-id="65d7c-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="65d7c-126">Изаберите **Креирај**, па у пољу **Брзо креирање члана пројектног тима** подесите улогу за генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="65d7c-126">Select **Create**, and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="65d7c-127">Можете да наставите са доделом задатака у овај ресурс чувара места избором ресурса у **бирачу ресурса** за задатак.</span><span class="sxs-lookup"><span data-stu-id="65d7c-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="65d7c-128">Они су наведени у оквиру опције **Чланови тима**.</span><span class="sxs-lookup"><span data-stu-id="65d7c-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="65d7c-129">Када завршите са додељивањем генеричког ресурса, изаберите генерички ресурс на картици **Тим**, а затим изаберите **Генериши потребу** да бисте креирали потребу за ресурсом за генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="65d7c-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="65d7c-130">Изаберите опцију **Резервиши** за генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="65d7c-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="65d7c-131">Затим можете да користите табелу распореда да бисте пронашли и резервисали прави ресурс.</span><span class="sxs-lookup"><span data-stu-id="65d7c-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="65d7c-132">Можете и да проследите захтев за испуњење од стране менаџера ресурса.</span><span class="sxs-lookup"><span data-stu-id="65d7c-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="65d7c-133">Када генерички ресурс буде испуњен именованим ресурсом, генерички ресурс се уклања из тима, а доделе задатка из генеричког ресурса се додељују именованом ресурсу који је испунио захтев за ресурсом генеричког ресурса.</span><span class="sxs-lookup"><span data-stu-id="65d7c-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="65d7c-134">Додела именованог ресурса са листе свих ресурса који могу да се резервишу</span><span class="sxs-lookup"><span data-stu-id="65d7c-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="65d7c-135">Можете да користите поље за претрагу у **бирачу ресурса** да бисте претраживали све ресурсе који могу да се резервишу и да их доделите задатку.</span><span class="sxs-lookup"><span data-stu-id="65d7c-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="65d7c-136">Ресурси додељени на овај начин додају се у тим без икаквих резервација.</span><span class="sxs-lookup"><span data-stu-id="65d7c-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="65d7c-137">То је слично додавању члана тима и одлуци да не изаберете ниједну методу доделе.</span><span class="sxs-lookup"><span data-stu-id="65d7c-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="65d7c-138">Ресурс се приказују на картицама **Тим** и **Усаглашеност** као ресурс само са доделама и са недостатком резервације.</span><span class="sxs-lookup"><span data-stu-id="65d7c-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="65d7c-139">Резервишете их ако желите да користите њихову доступност.</span><span class="sxs-lookup"><span data-stu-id="65d7c-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="65d7c-140">На мрежи **Распоред** за задатак, изаберите икону **ресурса** у ћелији Ресурс.</span><span class="sxs-lookup"><span data-stu-id="65d7c-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="65d7c-141">Започните унос имена.</span><span class="sxs-lookup"><span data-stu-id="65d7c-141">Start typing a name.</span></span> <span data-ttu-id="65d7c-142">Приказују се резултати претраге за име у **бирачу ресурса** у оквиру опције **Други ресурси**.</span><span class="sxs-lookup"><span data-stu-id="65d7c-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="65d7c-143">Изаберите ресурс који желите да доделите задатку.</span><span class="sxs-lookup"><span data-stu-id="65d7c-143">Select the resource that you want to assign to the task.</span></span>

