---
title: Промене у управљању ресурсима (Project Service Automation 3.x)
description: Ова тема пружа информације о променама у области управљања ресурсима.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 25fafd22-fe94-4865-8d4d-3e6582c999d5
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
ms.openlocfilehash: e00ce5a9604e25764567a3f9d38ec85aec4245d4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755393"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="2dc5d-103">Промене у управљању ресурсима (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="2dc5d-103">Resource management changes (Project Service Automation 3.x)</span></span>

<span data-ttu-id="2dc5d-104">Одељци ове теме пружају информације о променама које су извршене у области управљања ресурсима у услузи Dynamics 365 Project Service Automation верзије 3.x.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="2dc5d-105">Процене за пројекат</span><span class="sxs-lookup"><span data-stu-id="2dc5d-105">Project estimates</span></span>

<span data-ttu-id="2dc5d-106">Уместо да се заснива на ентитету **msdyn\_projecttask** (**Пројектни задатак**), процене пројеката се заснивају на ентитету **msdyn\_resourceassignment** (**Додела ресурса**).</span><span class="sxs-lookup"><span data-stu-id="2dc5d-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="2dc5d-107">Доделе ресурса су постале „извор истине“ за заказивање задатака и одређивање цена задатака.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="2dc5d-108">Задаци ставке</span><span class="sxs-lookup"><span data-stu-id="2dc5d-108">Line tasks</span></span>

<span data-ttu-id="2dc5d-109">У апликацији PSA 3.x, задаци ставке су застарели.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="2dc5d-110">Задаци сада указују на цео задатак уместо на задатке ставке.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="2dc5d-111">Следећи пример приказује како се задатак који се зове „Пробни задатак“ додељује А и Б члановима тима у старијим верзијама апликације PSA и апликацији PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="2dc5d-112">**Пре верзије апликације PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="2dc5d-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="2dc5d-113">Пробни задатак</span><span class="sxs-lookup"><span data-stu-id="2dc5d-113">Test task</span></span>

        - <span data-ttu-id="2dc5d-114">Пробни задатак – 1. задатак ставке</span><span class="sxs-lookup"><span data-stu-id="2dc5d-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="2dc5d-115">Додела члану А</span><span class="sxs-lookup"><span data-stu-id="2dc5d-115">Assignment to A</span></span>

        - <span data-ttu-id="2dc5d-116">Пробни задатак – 2. задатак ставке</span><span class="sxs-lookup"><span data-stu-id="2dc5d-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="2dc5d-117">Додела члану Б</span><span class="sxs-lookup"><span data-stu-id="2dc5d-117">Assignment to B</span></span>

- <span data-ttu-id="2dc5d-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="2dc5d-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="2dc5d-119">Пробни задатак</span><span class="sxs-lookup"><span data-stu-id="2dc5d-119">Test task</span></span>

        - <span data-ttu-id="2dc5d-120">Додела члану А</span><span class="sxs-lookup"><span data-stu-id="2dc5d-120">Assignment to A</span></span>
        - <span data-ttu-id="2dc5d-121">Додела члану Б</span><span class="sxs-lookup"><span data-stu-id="2dc5d-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="2dc5d-122">Неодељени задатак</span><span class="sxs-lookup"><span data-stu-id="2dc5d-122">Unassigned assignment</span></span>

<span data-ttu-id="2dc5d-123">У апликацији PSA 3.x, недодељени задатак је задатак који је додељен члану тима који има нулту вредност (**NULL**) и ресурсу са нултом вредношћу (**NULL**).</span><span class="sxs-lookup"><span data-stu-id="2dc5d-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="2dc5d-124">Недодељени задаци могу се појавити у неколико сценарија:</span><span class="sxs-lookup"><span data-stu-id="2dc5d-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="2dc5d-125">Ако је задатак креиран, али још увек није додељен ниједном члану тима, увек се креира недодељени задатак.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="2dc5d-126">Ако се уклоне сви додељени корисници из задатка, за тај задатак се поново креира недодељени задатак.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="2dc5d-127">Поља за заказивање у ентитету Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="2dc5d-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="2dc5d-128">Поља у ентитету **msdyn\_projecttask** су застарела или премештена у ентитет **msdyn\_resourceassignment** или се сада наводе у ентитету **msdyn\_projectteam** (**Члан пројектног тима**).</span><span class="sxs-lookup"><span data-stu-id="2dc5d-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="2dc5d-129">Застарело поље у ентитету msdyn\_projecttask (пројектни задатак)</span><span class="sxs-lookup"><span data-stu-id="2dc5d-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="2dc5d-130">Ново поље у ентитету msdyn\_resourceassignment (додела ресурса)</span><span class="sxs-lookup"><span data-stu-id="2dc5d-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="2dc5d-131">Коментар</span><span class="sxs-lookup"><span data-stu-id="2dc5d-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="2dc5d-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="2dc5d-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="2dc5d-133">ниједно</span><span class="sxs-lookup"><span data-stu-id="2dc5d-133">None</span></span> | |
| <span data-ttu-id="2dc5d-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="2dc5d-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="2dc5d-135">ниједно</span><span class="sxs-lookup"><span data-stu-id="2dc5d-135">None</span></span> | |
| <span data-ttu-id="2dc5d-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="2dc5d-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="2dc5d-137">ниједно</span><span class="sxs-lookup"><span data-stu-id="2dc5d-137">None</span></span> | |
| <span data-ttu-id="2dc5d-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="2dc5d-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="2dc5d-139">ниједно</span><span class="sxs-lookup"><span data-stu-id="2dc5d-139">None</span></span> | |
| <span data-ttu-id="2dc5d-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="2dc5d-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="2dc5d-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="2dc5d-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="2dc5d-142">Формат структуре података JSON (JavaScript Object Notation) која се чува у пољу је промењен.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="2dc5d-143">Заказивање скице</span><span class="sxs-lookup"><span data-stu-id="2dc5d-143">Schedule contour</span></span>

<span data-ttu-id="2dc5d-144">Скица распореда се чува у пољу **Планирани рад** (**msdyn\_plannedwork**) сваког ентитета **Додела ресурса** (**msdyn\_resourceassignment**).</span><span class="sxs-lookup"><span data-stu-id="2dc5d-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="2dc5d-145">Структура</span><span class="sxs-lookup"><span data-stu-id="2dc5d-145">Structure</span></span>

<span data-ttu-id="2dc5d-146">Нова структура скице распореда састоји се од флексибилних делића времена који су дефинисани за сваки дан распореда.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="2dc5d-147">Сваки делић времена има следећа својства:</span><span class="sxs-lookup"><span data-stu-id="2dc5d-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="2dc5d-148">**Почетак** - Почетак радног времена за дан, према календару пројекта.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="2dc5d-149">**Крај** - Крај радног времена за дан, према календару пројекта.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="2dc5d-150">**Радно време** - Број сати који су додељени у дану.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="2dc5d-151">**Пример**</span><span class="sxs-lookup"><span data-stu-id="2dc5d-151">**Example**</span></span>

<span data-ttu-id="2dc5d-152">Овај пример користи календар пројекта где је радни дан од 9:00 до 17:00 у временској зони UTC-8.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="2dc5d-153">Аутоматско заказивање и ручно заказивање</span><span class="sxs-lookup"><span data-stu-id="2dc5d-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="2dc5d-154">Ако је задатак аутоматски заказан, сати се учитавају унапред, а трајање задатка може бити смањено.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="2dc5d-155">**Пример**</span><span class="sxs-lookup"><span data-stu-id="2dc5d-155">**Example**</span></span>

<span data-ttu-id="2dc5d-156">Следећи задатак је аутоматски заказан за 18 сати током три дана (од 3. до 5. децембра 2018. године).</span><span class="sxs-lookup"><span data-stu-id="2dc5d-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="2dc5d-157">Ако је задатак ручно заказан, сати су равномерно распоређени на све датуме.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="2dc5d-158">**Пример**</span><span class="sxs-lookup"><span data-stu-id="2dc5d-158">**Example**</span></span>

<span data-ttu-id="2dc5d-159">Следећи задатак је ручно заказан за 18 сати током три дана (од 3. до 5. децембра 2018. године).</span><span class="sxs-lookup"><span data-stu-id="2dc5d-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="2dc5d-160">Јединица доделе</span><span class="sxs-lookup"><span data-stu-id="2dc5d-160">Assignment unit</span></span>

<span data-ttu-id="2dc5d-161">Јединица доделе застарела је у апликацији PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="2dc5d-162">Сати ангажовања на задатку сада су равномерно подељени, по дану, на све додељене ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="2dc5d-163">**Пример**</span><span class="sxs-lookup"><span data-stu-id="2dc5d-163">**Example**</span></span>

<span data-ttu-id="2dc5d-164">У овом примеру, задатак је додељен на два ресурса и аутоматски је заказан за 36 сати током три дана (од 3. до 5. децембра 2018. године).</span><span class="sxs-lookup"><span data-stu-id="2dc5d-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="2dc5d-165">1. додела:</span><span class="sxs-lookup"><span data-stu-id="2dc5d-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="2dc5d-166">2. додела:</span><span class="sxs-lookup"><span data-stu-id="2dc5d-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="2dc5d-167">Димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="2dc5d-167">Pricing dimensions</span></span>

<span data-ttu-id="2dc5d-168">У апликацији PSA 3.x, поља димензија за одређивање цена, специфична за ресурсе (као што су **Улога** и **Организациона јединица**) су уклоњени из ентитета **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="2dc5d-169">Ова поља се сада могу преузети од одговарајућег члана пројектног тима (**msdyn\_projectteam**) за доделу ресурса (**msdyn\_resourceassignment**) када се генеришу процене пројеката.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="2dc5d-170">Ново поље, **msdyn\_organizationalunit**, је додато у ентитет **msdyn\_projectteam**.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="2dc5d-171">Застарело поље у ентитету msdyn\_projecttask (пројектни задатак)</span><span class="sxs-lookup"><span data-stu-id="2dc5d-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="2dc5d-172">Поље у ентитету msdyn\_projectteam (члан пројектног тима) које се користи уместо тога</span><span class="sxs-lookup"><span data-stu-id="2dc5d-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="2dc5d-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="2dc5d-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="2dc5d-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="2dc5d-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="2dc5d-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="2dc5d-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="2dc5d-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="2dc5d-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="2dc5d-177">Скицирања</span><span class="sxs-lookup"><span data-stu-id="2dc5d-177">Contours</span></span>

<span data-ttu-id="2dc5d-178">Поља са скицама за одређивање цена и процене су застарела у ентитету **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="2dc5d-179">Премештена су у ентитет **msdyn\_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="2dc5d-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="2dc5d-180">Застарело поље у ентитету msdyn\_projecttask (пројектни задатак)</span><span class="sxs-lookup"><span data-stu-id="2dc5d-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="2dc5d-181">Ново поље у ентитету msdyn\_resourceassignment (додела ресурса)</span><span class="sxs-lookup"><span data-stu-id="2dc5d-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="2dc5d-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="2dc5d-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="2dc5d-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="2dc5d-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="2dc5d-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="2dc5d-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="2dc5d-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="2dc5d-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="2dc5d-186">Следећа поља су додата у ентитет **msdyn\_resourceassignment**:</span><span class="sxs-lookup"><span data-stu-id="2dc5d-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="2dc5d-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="2dc5d-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="2dc5d-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="2dc5d-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="2dc5d-189">Следећа поља за планиране, стварне и преостале трошкове и продају непромењена су у ентитету **msdyn\_projecttask**:</span><span class="sxs-lookup"><span data-stu-id="2dc5d-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="2dc5d-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="2dc5d-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="2dc5d-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="2dc5d-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="2dc5d-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="2dc5d-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="2dc5d-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="2dc5d-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="2dc5d-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="2dc5d-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="2dc5d-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="2dc5d-195">msdyn\_remainingsales</span></span>
