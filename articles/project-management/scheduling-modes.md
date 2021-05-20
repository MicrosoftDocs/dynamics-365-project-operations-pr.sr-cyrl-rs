---
title: Режими планирања
description: Ова тема пружа информације о режимима планирања.
author: ruhercul
manager: AnnBe
ms.date: 05/04/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fe54944999617b248ff925148a78601dd4be7aca
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981453"
---
# <a name="scheduling-modes"></a><span data-ttu-id="39794-103">Режими планирања</span><span class="sxs-lookup"><span data-stu-id="39794-103">Scheduling modes</span></span>

<span data-ttu-id="39794-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="39794-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="39794-105">Dynamics 365 Project Operations пружа могућност организацијама да дефинишу како управљају променама кључних променљивих у задацима унутар структуре расподеле рада.</span><span class="sxs-lookup"><span data-stu-id="39794-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="39794-106">На основу специфичних потреба организације, пројект менаџери могу да изврше промене у начину распоређивања када се пројекат креира.</span><span class="sxs-lookup"><span data-stu-id="39794-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="39794-107">У Project Operations доступна су три начина распоређивања:</span><span class="sxs-lookup"><span data-stu-id="39794-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="39794-108">Фиксно трајање (ово је подразумевани режим)</span><span class="sxs-lookup"><span data-stu-id="39794-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="39794-109">Фиксни рад</span><span class="sxs-lookup"><span data-stu-id="39794-109">Fixed work</span></span>
  - <span data-ttu-id="39794-110">Фиксне јединице</span><span class="sxs-lookup"><span data-stu-id="39794-110">Fixed units</span></span>

<span data-ttu-id="39794-111">Вредности на које утиче дефиниција одређеног режима распореда одређују се следећом формулом:</span><span class="sxs-lookup"><span data-stu-id="39794-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="39794-112">Напор (*Посао*) = Трајање x Јединице</span><span class="sxs-lookup"><span data-stu-id="39794-112">Effort (*Work*) = Duration x Units</span></span>

<span data-ttu-id="39794-113">Када дефинишете режим заказивања пројекта, постављате једну од ових вредности, које се потом не могу променити.</span><span class="sxs-lookup"><span data-stu-id="39794-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="39794-114">Држање ове вредности као константе ставља приоритет на ту вредност, што обавештава систем да је не мења када се промене друге две вредности.</span><span class="sxs-lookup"><span data-stu-id="39794-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="39794-115">Следећа табела пружа информације о утицајима избора одређеног режима.</span><span class="sxs-lookup"><span data-stu-id="39794-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="39794-116">**У овом задатку**</span><span class="sxs-lookup"><span data-stu-id="39794-116">**In this task**</span></span>             | <span data-ttu-id="39794-117">**Ако ревидирате јединице**</span><span class="sxs-lookup"><span data-stu-id="39794-117">**If you revise units**</span></span>   | <span data-ttu-id="39794-118">**Ако ревидирате трајање**</span><span class="sxs-lookup"><span data-stu-id="39794-118">**If you revise duration**</span></span> | <span data-ttu-id="39794-119">**Ако ревидирате напор**</span><span class="sxs-lookup"><span data-stu-id="39794-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="39794-120">Задатак са фиксним јединицама</span><span class="sxs-lookup"><span data-stu-id="39794-120">Fixed units task</span></span>     | <span data-ttu-id="39794-121">Трајање је прерачунато.</span><span class="sxs-lookup"><span data-stu-id="39794-121">Duration is recalculated.</span></span> | <span data-ttu-id="39794-122">Напор се прерачунава.</span><span class="sxs-lookup"><span data-stu-id="39794-122">Effort is recalculated.</span></span>    | <span data-ttu-id="39794-123">Трајање је прерачунато.</span><span class="sxs-lookup"><span data-stu-id="39794-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="39794-124">Задатак фиксног ангажовања</span><span class="sxs-lookup"><span data-stu-id="39794-124">Fixed effort task</span></span>    | <span data-ttu-id="39794-125">Трајање је прерачунато.</span><span class="sxs-lookup"><span data-stu-id="39794-125">Duration is recalculated.</span></span> | <span data-ttu-id="39794-126">Јединице се прерачунавају.</span><span class="sxs-lookup"><span data-stu-id="39794-126">Units are recalculated.</span></span>    | <span data-ttu-id="39794-127">Трајање је прерачунато.</span><span class="sxs-lookup"><span data-stu-id="39794-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="39794-128">Задатак фиксног трајања</span><span class="sxs-lookup"><span data-stu-id="39794-128">Fixed duration task</span></span>  | <span data-ttu-id="39794-129">Напор се прерачунава.</span><span class="sxs-lookup"><span data-stu-id="39794-129">Effort is recalculated.</span></span>   | <span data-ttu-id="39794-130">Напор се прерачунава.</span><span class="sxs-lookup"><span data-stu-id="39794-130">Effort is recalculated.</span></span>    | <span data-ttu-id="39794-131">Јединице се прерачунавају.</span><span class="sxs-lookup"><span data-stu-id="39794-131">Units are recalculated.</span></span>   |

<span data-ttu-id="39794-132">За више информација о импликацијама датог режима погледајте [Промените тип задатка за тачније распоређивање](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="39794-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="39794-133">У теми се појам **Посао** користи уместо **Напор**.</span><span class="sxs-lookup"><span data-stu-id="39794-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="39794-134">Промените режим заказивања организације</span><span class="sxs-lookup"><span data-stu-id="39794-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="39794-135">Довршите следеће кораке да бисте дефинисали режим заказивања организације.</span><span class="sxs-lookup"><span data-stu-id="39794-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="39794-136">Идите на **Подешавања** \> **Општа** \> **Параметри**, а затим изаберите параметар пројекта.</span><span class="sxs-lookup"><span data-stu-id="39794-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="39794-137">На страници **Параметри пројекта** изаберите подразумевани режим заказивања за организацију, а затим дефинишите способност да менаџер пројекта замени поставку приликом креирања новог пројекта.</span><span class="sxs-lookup"><span data-stu-id="39794-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="39794-138">Промените поставку режима заказивања на пројекту</span><span class="sxs-lookup"><span data-stu-id="39794-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="39794-139">Ако организација дозволи менаџеру пројекта да замени задати режим распоређивања, менаџер пројекта може то променити када креира нови пројекат.</span><span class="sxs-lookup"><span data-stu-id="39794-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="39794-140">Међутим, након што је пројекат сачуван, режим заказивања не може се променити.</span><span class="sxs-lookup"><span data-stu-id="39794-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="39794-141">Копирани пројекти</span><span class="sxs-lookup"><span data-stu-id="39794-141">Copied projects</span></span>

<span data-ttu-id="39794-142">Будући да се пројекат креира када се предузме акција копирања, менаџер пројекта не може да постави режим заказивања.</span><span class="sxs-lookup"><span data-stu-id="39794-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="39794-143">Одредишни пројекат ће се увек подразумевати за режим дефинисан на организационом нивоу.</span><span class="sxs-lookup"><span data-stu-id="39794-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="39794-144">Копирани задаци</span><span class="sxs-lookup"><span data-stu-id="39794-144">Copied tasks</span></span>

<span data-ttu-id="39794-145">Када се задатак копира из једног пројекта у други, задатак наслеђује режим распореда одредишног пројекта.</span><span class="sxs-lookup"><span data-stu-id="39794-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
