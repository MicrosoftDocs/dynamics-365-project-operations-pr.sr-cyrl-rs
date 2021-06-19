---
title: Промене у управљању ресурсима (Project Service Automation 3.x)
description: Ова тема пружа информације о променама у области управљања ресурсима.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: e888d55b93c40e08e51bd4480853fec37f2b6333
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007834"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="46fdd-103">Промене у управљању ресурсима (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="46fdd-103">Resource management changes (Project Service Automation 3.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

<span data-ttu-id="46fdd-104">Одељци ове теме пружају информације о променама које су извршене у области управљања ресурсима у услузи Dynamics 365 Project Service Automation верзије 3.x.</span><span class="sxs-lookup"><span data-stu-id="46fdd-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="46fdd-105">Процене за пројекат</span><span class="sxs-lookup"><span data-stu-id="46fdd-105">Project estimates</span></span>

<span data-ttu-id="46fdd-106">Уместо да се заснива на ентитету **msdyn\_projecttask** (**Пројектни задатак**), процене пројеката се заснивају на ентитету **msdyn\_resourceassignment** (**Додела ресурса**).</span><span class="sxs-lookup"><span data-stu-id="46fdd-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="46fdd-107">Доделе ресурса су постале „извор истине“ за заказивање задатака и одређивање цена задатака.</span><span class="sxs-lookup"><span data-stu-id="46fdd-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="46fdd-108">Задаци ставке</span><span class="sxs-lookup"><span data-stu-id="46fdd-108">Line tasks</span></span>

<span data-ttu-id="46fdd-109">У апликацији PSA 3.x, задаци ставке су застарели.</span><span class="sxs-lookup"><span data-stu-id="46fdd-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="46fdd-110">Задаци сада указују на цео задатак уместо на задатке ставке.</span><span class="sxs-lookup"><span data-stu-id="46fdd-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="46fdd-111">Следећи пример приказује како се задатак који се зове „Пробни задатак“ додељује А и Б члановима тима у старијим верзијама апликације PSA и апликацији PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="46fdd-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="46fdd-112">**Пре верзије апликације PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="46fdd-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="46fdd-113">Пробни задатак</span><span class="sxs-lookup"><span data-stu-id="46fdd-113">Test task</span></span>

        - <span data-ttu-id="46fdd-114">Пробни задатак – 1. задатак ставке</span><span class="sxs-lookup"><span data-stu-id="46fdd-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="46fdd-115">Додела члану А</span><span class="sxs-lookup"><span data-stu-id="46fdd-115">Assignment to A</span></span>

        - <span data-ttu-id="46fdd-116">Пробни задатак – 2. задатак ставке</span><span class="sxs-lookup"><span data-stu-id="46fdd-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="46fdd-117">Додела члану Б</span><span class="sxs-lookup"><span data-stu-id="46fdd-117">Assignment to B</span></span>

- <span data-ttu-id="46fdd-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="46fdd-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="46fdd-119">Пробни задатак</span><span class="sxs-lookup"><span data-stu-id="46fdd-119">Test task</span></span>

        - <span data-ttu-id="46fdd-120">Додела члану А</span><span class="sxs-lookup"><span data-stu-id="46fdd-120">Assignment to A</span></span>
        - <span data-ttu-id="46fdd-121">Додела члану Б</span><span class="sxs-lookup"><span data-stu-id="46fdd-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="46fdd-122">Неодељени задатак</span><span class="sxs-lookup"><span data-stu-id="46fdd-122">Unassigned assignment</span></span>

<span data-ttu-id="46fdd-123">У апликацији PSA 3.x, недодељени задатак је задатак који је додељен члану тима који има нулту вредност (**NULL**) и ресурсу са нултом вредношћу (**NULL**).</span><span class="sxs-lookup"><span data-stu-id="46fdd-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="46fdd-124">Недодељени задаци могу се појавити у неколико сценарија:</span><span class="sxs-lookup"><span data-stu-id="46fdd-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="46fdd-125">Ако је задатак креиран, али још увек није додељен ниједном члану тима, увек се креира недодељени задатак.</span><span class="sxs-lookup"><span data-stu-id="46fdd-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="46fdd-126">Ако се уклоне сви додељени корисници из задатка, за тај задатак се поново креира недодељени задатак.</span><span class="sxs-lookup"><span data-stu-id="46fdd-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="46fdd-127">Поља за заказивање у ентитету Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="46fdd-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="46fdd-128">Поља у ентитету **msdyn\_projecttask** су застарела или премештена у ентитет **msdyn\_resourceassignment** или се сада наводе у ентитету **msdyn\_projectteam** (**Члан пројектног тима**).</span><span class="sxs-lookup"><span data-stu-id="46fdd-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="46fdd-129">Застарело поље у ентитету msdyn\_projecttask (пројектни задатак)</span><span class="sxs-lookup"><span data-stu-id="46fdd-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="46fdd-130">Ново поље у ентитету msdyn\_resourceassignment (додела ресурса)</span><span class="sxs-lookup"><span data-stu-id="46fdd-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="46fdd-131">Коментар</span><span class="sxs-lookup"><span data-stu-id="46fdd-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="46fdd-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="46fdd-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="46fdd-133">ниједно</span><span class="sxs-lookup"><span data-stu-id="46fdd-133">None</span></span> | |
| <span data-ttu-id="46fdd-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="46fdd-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="46fdd-135">ниједно</span><span class="sxs-lookup"><span data-stu-id="46fdd-135">None</span></span> | |
| <span data-ttu-id="46fdd-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="46fdd-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="46fdd-137">ниједно</span><span class="sxs-lookup"><span data-stu-id="46fdd-137">None</span></span> | |
| <span data-ttu-id="46fdd-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="46fdd-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="46fdd-139">ниједно</span><span class="sxs-lookup"><span data-stu-id="46fdd-139">None</span></span> | |
| <span data-ttu-id="46fdd-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="46fdd-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="46fdd-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="46fdd-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="46fdd-142">Формат структуре података JSON (JavaScript Object Notation) која се чува у пољу је промењен.</span><span class="sxs-lookup"><span data-stu-id="46fdd-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="46fdd-143">Заказивање скице</span><span class="sxs-lookup"><span data-stu-id="46fdd-143">Schedule contour</span></span>

<span data-ttu-id="46fdd-144">Скица распореда се чува у пољу **Планирани рад** (**msdyn\_plannedwork**) сваког ентитета **Додела ресурса** (**msdyn\_resourceassignment**).</span><span class="sxs-lookup"><span data-stu-id="46fdd-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="46fdd-145">Структура</span><span class="sxs-lookup"><span data-stu-id="46fdd-145">Structure</span></span>

<span data-ttu-id="46fdd-146">Нова структура скице распореда састоји се од флексибилних делића времена који су дефинисани за сваки дан распореда.</span><span class="sxs-lookup"><span data-stu-id="46fdd-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="46fdd-147">Сваки делић времена има следећа својства:</span><span class="sxs-lookup"><span data-stu-id="46fdd-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="46fdd-148">**Почетак** - Почетак радног времена за дан, према календару пројекта.</span><span class="sxs-lookup"><span data-stu-id="46fdd-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="46fdd-149">**Крај** - Крај радног времена за дан, према календару пројекта.</span><span class="sxs-lookup"><span data-stu-id="46fdd-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="46fdd-150">**Радно време** - Број сати који су додељени у дану.</span><span class="sxs-lookup"><span data-stu-id="46fdd-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="46fdd-151">**Пример**</span><span class="sxs-lookup"><span data-stu-id="46fdd-151">**Example**</span></span>

<span data-ttu-id="46fdd-152">Овај пример користи календар пројекта где је радни дан од 9:00 до 17:00 у временској зони UTC-8.</span><span class="sxs-lookup"><span data-stu-id="46fdd-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="46fdd-153">Аутоматско заказивање и ручно заказивање</span><span class="sxs-lookup"><span data-stu-id="46fdd-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="46fdd-154">Ако је задатак аутоматски заказан, сати се учитавају унапред, а трајање задатка може бити смањено.</span><span class="sxs-lookup"><span data-stu-id="46fdd-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="46fdd-155">**Пример**</span><span class="sxs-lookup"><span data-stu-id="46fdd-155">**Example**</span></span>

<span data-ttu-id="46fdd-156">Следећи задатак је аутоматски заказан за 18 сати током три дана (од 3. до 5. децембра 2018. године).</span><span class="sxs-lookup"><span data-stu-id="46fdd-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="46fdd-157">Ако је задатак ручно заказан, сати су равномерно распоређени на све датуме.</span><span class="sxs-lookup"><span data-stu-id="46fdd-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="46fdd-158">**Пример**</span><span class="sxs-lookup"><span data-stu-id="46fdd-158">**Example**</span></span>

<span data-ttu-id="46fdd-159">Следећи задатак је ручно заказан за 18 сати током три дана (од 3. до 5. децембра 2018. године).</span><span class="sxs-lookup"><span data-stu-id="46fdd-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="46fdd-160">Јединица доделе</span><span class="sxs-lookup"><span data-stu-id="46fdd-160">Assignment unit</span></span>

<span data-ttu-id="46fdd-161">Јединица доделе застарела је у апликацији PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="46fdd-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="46fdd-162">Сати ангажовања на задатку сада су равномерно подељени, по дану, на све додељене ресурсе.</span><span class="sxs-lookup"><span data-stu-id="46fdd-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="46fdd-163">**Пример**</span><span class="sxs-lookup"><span data-stu-id="46fdd-163">**Example**</span></span>

<span data-ttu-id="46fdd-164">У овом примеру, задатак је додељен на два ресурса и аутоматски је заказан за 36 сати током три дана (од 3. до 5. децембра 2018. године).</span><span class="sxs-lookup"><span data-stu-id="46fdd-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="46fdd-165">1. додела:</span><span class="sxs-lookup"><span data-stu-id="46fdd-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="46fdd-166">2. додела:</span><span class="sxs-lookup"><span data-stu-id="46fdd-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="46fdd-167">Димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="46fdd-167">Pricing dimensions</span></span>

<span data-ttu-id="46fdd-168">У апликацији PSA 3.x, поља димензија за одређивање цена, специфична за ресурсе (као што су **Улога** и **Организациона јединица**) су уклоњени из ентитета **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="46fdd-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="46fdd-169">Ова поља се сада могу преузети од одговарајућег члана пројектног тима (**msdyn\_projectteam**) за доделу ресурса (**msdyn\_resourceassignment**) када се генеришу процене пројеката.</span><span class="sxs-lookup"><span data-stu-id="46fdd-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="46fdd-170">Ново поље, **msdyn\_organizationalunit**, је додато у ентитет **msdyn\_projectteam**.</span><span class="sxs-lookup"><span data-stu-id="46fdd-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="46fdd-171">Застарело поље у ентитету msdyn\_projecttask (пројектни задатак)</span><span class="sxs-lookup"><span data-stu-id="46fdd-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="46fdd-172">Поље у ентитету msdyn\_projectteam (члан пројектног тима) које се користи уместо тога</span><span class="sxs-lookup"><span data-stu-id="46fdd-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="46fdd-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="46fdd-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="46fdd-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="46fdd-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="46fdd-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="46fdd-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="46fdd-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="46fdd-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="46fdd-177">Скицирања</span><span class="sxs-lookup"><span data-stu-id="46fdd-177">Contours</span></span>

<span data-ttu-id="46fdd-178">Поља са скицама за одређивање цена и процене су застарела у ентитету **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="46fdd-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="46fdd-179">Премештена су у ентитет **msdyn\_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="46fdd-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="46fdd-180">Застарело поље у ентитету msdyn\_projecttask (пројектни задатак)</span><span class="sxs-lookup"><span data-stu-id="46fdd-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="46fdd-181">Ново поље у ентитету msdyn\_resourceassignment (додела ресурса)</span><span class="sxs-lookup"><span data-stu-id="46fdd-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="46fdd-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="46fdd-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="46fdd-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="46fdd-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="46fdd-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="46fdd-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="46fdd-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="46fdd-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="46fdd-186">Следећа поља су додата у ентитет **msdyn\_resourceassignment**:</span><span class="sxs-lookup"><span data-stu-id="46fdd-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="46fdd-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="46fdd-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="46fdd-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="46fdd-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="46fdd-189">Следећа поља за планиране, стварне и преостале трошкове и продају непромењена су у ентитету **msdyn\_projecttask**:</span><span class="sxs-lookup"><span data-stu-id="46fdd-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="46fdd-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="46fdd-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="46fdd-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="46fdd-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="46fdd-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="46fdd-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="46fdd-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="46fdd-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="46fdd-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="46fdd-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="46fdd-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="46fdd-195">msdyn\_remainingsales</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]