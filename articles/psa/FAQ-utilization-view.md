---
title: Приказ наплативе укупне искоришћености ресурса
description: Ова тема пружа информације о приказу укупне искоришћености ресурса.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a1d1db532c65b2a13f3cf4e1281a5987490b96df
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122181"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="90c6a-103">Приказ наплативе укупне искоришћености ресурса</span><span class="sxs-lookup"><span data-stu-id="90c6a-103">View chargeable utilization for resources</span></span>
 
<span data-ttu-id="90c6a-104">**Приказ укупне искоришћености** на страници **Укупна искоришћеност ресурса у апликацији Project Service** приказује наплативу укупну искоришћеност сваког ресурса који може да се резервише.</span><span class="sxs-lookup"><span data-stu-id="90c6a-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="90c6a-105">Пошто је приказ заснован на табели распореда, пронаћићете доста истих функција.</span><span class="sxs-lookup"><span data-stu-id="90c6a-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![Снимак екрана приказа укупне искоришћености](media/FAQ-utilization-1.png)
 

<span data-ttu-id="90c6a-107">Израчунавање наплативе укупне искоришћености функционише на следећи начин:</span><span class="sxs-lookup"><span data-stu-id="90c6a-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="90c6a-108">Наплатива укупна искоришћеност = (наплативи стварни сати) / (капацитет ресурса).</span><span class="sxs-lookup"><span data-stu-id="90c6a-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="90c6a-109">Ћелије представљају израчунату наплативу укупну искоришћеност за изабрани период (дани, седмице или месеци).</span><span class="sxs-lookup"><span data-stu-id="90c6a-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="90c6a-110">Боје у свакој ћелији приказују наплативу укупну искоришћеност за ресурс у поређењу са његовом циљном наплативом укупном искоришћеношћу.</span><span class="sxs-lookup"><span data-stu-id="90c6a-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="90c6a-111">Циљна укупна искоришћеност може бити подешена за подразумевану улогу ресурса или за самог појединачног ресурса.</span><span class="sxs-lookup"><span data-stu-id="90c6a-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="90c6a-112">Израчунавање прво гледа појединца за циљ, а затим подразумевану улогу ресурса.</span><span class="sxs-lookup"><span data-stu-id="90c6a-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="90c6a-113">Подешавање циља уа ресурс</span><span class="sxs-lookup"><span data-stu-id="90c6a-113">Set target on a resource</span></span>

1. <span data-ttu-id="90c6a-114">Идите на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="90c6a-115">Изаберите ресурс да бисте отворили запис.</span><span class="sxs-lookup"><span data-stu-id="90c6a-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="90c6a-116">На картици **Project Service** можете подесити циљну укупну искоришћеност ресурса.</span><span class="sxs-lookup"><span data-stu-id="90c6a-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![Снимак екрана коришћења картице Project Service за подешавање циљне укупне искоришћености](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="90c6a-118">Подешавање циљне укупне искоришћености за улогу</span><span class="sxs-lookup"><span data-stu-id="90c6a-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="90c6a-119">Идите на **Ресурси** \> **Улоге ресурса**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="90c6a-120">Изаберите улогу и отворите запис.</span><span class="sxs-lookup"><span data-stu-id="90c6a-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="90c6a-121">Подесите циљну укупну искоришћеност за улогу.</span><span class="sxs-lookup"><span data-stu-id="90c6a-121">Set the target utilization for the role.</span></span>

> ![Снимак екрана коришћења улога ресурса за подешавање циљне укупне искоришћености](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="90c6a-123">Израчунавање наплативе укупне искоришћености ресурса</span><span class="sxs-lookup"><span data-stu-id="90c6a-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="90c6a-124">Да бисте израчунали наплативу укупну искоришћеност за ресурс, потребно је да испуните неке предуслове.</span><span class="sxs-lookup"><span data-stu-id="90c6a-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="90c6a-125">Подешавање подразумеване улоге за појединачни ресурс</span><span class="sxs-lookup"><span data-stu-id="90c6a-125">Set default role for individual resource</span></span>

<span data-ttu-id="90c6a-126">Прво, циљна укупна искоришћеност мора бити подешена за улогу појединачног ресурса или за улогу ресурса.</span><span class="sxs-lookup"><span data-stu-id="90c6a-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="90c6a-127">Ако користите улоге ресурса за циљеве, сваки појединачни ресурс мора да има подразумевану улогу.</span><span class="sxs-lookup"><span data-stu-id="90c6a-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="90c6a-128">Да бисте то подесили, идите на ставку **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="90c6a-129">Изаберите ресурс, отворите запис, а затим изаберите картицу **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="90c6a-130">У мрежи **Улога ресурса**, уверите се да постоји једна улога за ресурс и да је **Is Default** подешен на **Да**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="90c6a-131">Промена типа наплате за улогу ресурса</span><span class="sxs-lookup"><span data-stu-id="90c6a-131">Change billing type for resource role</span></span>

<span data-ttu-id="90c6a-132">Улоге ресурса морају бити подешене тако да имају тип наплате **Наплатив**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="90c6a-133">Идите на **Ресурси** \> **Улоге ресурса**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="90c6a-134">Отворите запис који желите да ажурирате, а затим подесите подразумевани тип наплате на **Наплативо**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="90c6a-135">Подешавање радног времена за улогу ресурса</span><span class="sxs-lookup"><span data-stu-id="90c6a-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="90c6a-136">Ресурс мора да има радно време за израчунавање капацитета.</span><span class="sxs-lookup"><span data-stu-id="90c6a-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="90c6a-137">Идите на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="90c6a-138">Изаберите ресурс да бисте отворили запис, а затим изаберите **Прикажи радно време**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="90c6a-139">Можете масовно да исправите листу ресурса применом **предлошка за радно време** са приказа **листе ресурса**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="90c6a-140">Решавање проблема са наплатним стварним сатима</span><span class="sxs-lookup"><span data-stu-id="90c6a-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="90c6a-141">Извор наплативих стварних сати је ентитет **Стварне вредности**.</span><span class="sxs-lookup"><span data-stu-id="90c6a-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="90c6a-142">Стварне вредности чији је тип наплате **Наплативо** су обухваћени у израчунавање и зато морате да имате пројекте у којима су стварне вредности наплативе.</span><span class="sxs-lookup"><span data-stu-id="90c6a-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="90c6a-143">Ако не видите наплативу укупну искоришћеност, ево неких ствари које можете да проверите:</span><span class="sxs-lookup"><span data-stu-id="90c6a-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="90c6a-144">Ресурс има радне часове који су дефинисани за капацитет.</span><span class="sxs-lookup"><span data-stu-id="90c6a-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="90c6a-145">Ресурс има појединачно дефинисани циљ укупне искоришћености или му је додељена подразумевана улога.</span><span class="sxs-lookup"><span data-stu-id="90c6a-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="90c6a-146">За улогу је дефинисан циљ укупне искоришћености.</span><span class="sxs-lookup"><span data-stu-id="90c6a-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="90c6a-147">Стварне вредности имају тип наплате **Наплативо** за период за који очекујете израчунавање укупне искоришћености.</span><span class="sxs-lookup"><span data-stu-id="90c6a-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="90c6a-148">Проверите следеће ствари ако видите стварне вредности чији типови наплате нису наплативи:</span><span class="sxs-lookup"><span data-stu-id="90c6a-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="90c6a-149">Улога коришћена за стварне трошкове има подразумевани тип наплате који се разликује од типа „Наплативо“.</span><span class="sxs-lookup"><span data-stu-id="90c6a-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="90c6a-150">Улоге за предмет уговора за пројекат који подржава пројекат је подешена на ненаплативо.</span><span class="sxs-lookup"><span data-stu-id="90c6a-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="90c6a-151">Пројекат нема повезани предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="90c6a-151">The project does not have an associated contract line.</span></span>

