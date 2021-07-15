---
title: Коришћење API-ја за распоред пројеката за извођење операција са ентитетима распоређивања
description: Ова тема пружа информације и примере за коришћење API-ја распореда пројеката.
author: sigitac
ms.date: 06/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4915261c08a3271a919e04084e92a14b297c1b35
ms.sourcegitcommit: 2f16c2bc7c8350676a6a380c61fffa9958db6a0b
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/22/2021
ms.locfileid: "6293245"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="4d3af-103">Коришћење API-ја за распоред пројеката за извођење операција са ентитетима распоређивања</span><span class="sxs-lookup"><span data-stu-id="4d3af-103">Use Project schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="4d3af-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="4d3af-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="4d3af-105">Неке или све функционалности забележене у овој теми доступне су као део издања верзије за преглед.</span><span class="sxs-lookup"><span data-stu-id="4d3af-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="4d3af-106">Садржај и функционалност су подложни променама.</span><span class="sxs-lookup"><span data-stu-id="4d3af-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="4d3af-107">Ентитети планирања</span><span class="sxs-lookup"><span data-stu-id="4d3af-107">Scheduling entities</span></span>

<span data-ttu-id="4d3af-108">API-ји за распоред пројеката пружају могућност извршавања операција креирања, ажурирања и брисања помоћу **ентитета за заказивање**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-108">Project schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="4d3af-109">Тим ентитетима се управља путем механизма за распоређивање у апликацији Project за веб.</span><span class="sxs-lookup"><span data-stu-id="4d3af-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="4d3af-110">Креирање, ажурирање и брисање операција помоћу **ентитета планирања** били су ограничени у ранијим издањима услуге Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="4d3af-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="4d3af-111">Следећа табела даје потпуну листу ентитета за распоред пројеката.</span><span class="sxs-lookup"><span data-stu-id="4d3af-111">The following table provides a full list of the Project schedule entities.</span></span>

| <span data-ttu-id="4d3af-112">Назив ентитета</span><span class="sxs-lookup"><span data-stu-id="4d3af-112">Entity name</span></span>  | <span data-ttu-id="4d3af-113">Логичко име ентитета</span><span class="sxs-lookup"><span data-stu-id="4d3af-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="4d3af-114">Project</span><span class="sxs-lookup"><span data-stu-id="4d3af-114">Project</span></span> | <span data-ttu-id="4d3af-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="4d3af-115">msdyn_project</span></span> |
| <span data-ttu-id="4d3af-116">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="4d3af-116">Project Task</span></span>  | <span data-ttu-id="4d3af-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="4d3af-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="4d3af-118">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="4d3af-118">Project Task Dependency</span></span>  | <span data-ttu-id="4d3af-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="4d3af-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="4d3af-120">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="4d3af-120">Resource Assignment</span></span> | <span data-ttu-id="4d3af-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="4d3af-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="4d3af-122">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="4d3af-122">Project Bucket</span></span>  | <span data-ttu-id="4d3af-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="4d3af-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="4d3af-124">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="4d3af-124">Project Team Member</span></span> | <span data-ttu-id="4d3af-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="4d3af-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="4d3af-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="4d3af-126">OperationSet</span></span>

<span data-ttu-id="4d3af-127">Ентитет OperationSet је образац јединице рада који се може користити када се у трансакцији мора обрадити неколико захтева који утичу на распоред.</span><span class="sxs-lookup"><span data-stu-id="4d3af-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="project-schedule-apis"></a><span data-ttu-id="4d3af-128">API-ји за распоред пројеката</span><span class="sxs-lookup"><span data-stu-id="4d3af-128">Project schedule APIs</span></span>

<span data-ttu-id="4d3af-129">Следи листа актуелних API-ја за распоред пројеката.</span><span class="sxs-lookup"><span data-stu-id="4d3af-129">The following is a list of current Project schedule APIs.</span></span>

- <span data-ttu-id="4d3af-130">**msdyn_CreateProjectV1**: Овај API се може користити за креирање пројекта.</span><span class="sxs-lookup"><span data-stu-id="4d3af-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="4d3af-131">Пројекат и подразумевани контејнер пројекта креирају се одмах.</span><span class="sxs-lookup"><span data-stu-id="4d3af-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="4d3af-132">**msdyn_CreateTeamMemberV1**: Овај API се може користити за креирање члана пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="4d3af-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="4d3af-133">Евиденција члана тима креира се одмах.</span><span class="sxs-lookup"><span data-stu-id="4d3af-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="4d3af-134">**msdyn_CreateOperationSetV1**: Овај API се може користити за заказивање неколико захтева који се морају извршити у оквиру трансакције.</span><span class="sxs-lookup"><span data-stu-id="4d3af-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="4d3af-135">**msdyn_PSSCreateV1**: Овај API се може користити за креирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="4d3af-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="4d3af-136">Ентитет може бити било који ентитет распоређивања пројекта који подржава операцију креирања.</span><span class="sxs-lookup"><span data-stu-id="4d3af-136">The entity can be any of the Project scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="4d3af-137">**msdyn_PSSUpdateV1**: Овај API се може користити за ажурирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="4d3af-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="4d3af-138">Ентитет може бити било који ентитет распоређивања пројекта који подржава операцију ажурирања.</span><span class="sxs-lookup"><span data-stu-id="4d3af-138">The entity can be any of the Project scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="4d3af-139">**msdyn_PSSDeleteV1**: Овај API се може користити за брисање ентитета.</span><span class="sxs-lookup"><span data-stu-id="4d3af-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="4d3af-140">Ентитет може бити било који ентитет распоређивања пројекта који подржава операцију брисања.</span><span class="sxs-lookup"><span data-stu-id="4d3af-140">The entity can be any of the Project scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="4d3af-141">**msdyn_ExecuteOperationSetV1**: Овај API се користи за извршавање свих операција унутар датог скупа операција.</span><span class="sxs-lookup"><span data-stu-id="4d3af-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-project-schedule-apis-with-operationset"></a><span data-ttu-id="4d3af-142">Коришћење API-ја за распоред пројеката са ентитетом OperationSet</span><span class="sxs-lookup"><span data-stu-id="4d3af-142">Using Project schedule APIs with OperationSet</span></span>

<span data-ttu-id="4d3af-143">Пошто се записи са **CreateProjectV1** и **CreateTeamMemberV1** креирају одмах, ови API-ји се не могу користити у **OperationSet ентитету** директно.</span><span class="sxs-lookup"><span data-stu-id="4d3af-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="4d3af-144">Међутим, API можете користити за креирање потребних записа, креирајте **OperationSet ентитет**, а затим користите ове унапред креиране записе у **OperationSet ентитету**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="4d3af-145">Подржане операције</span><span class="sxs-lookup"><span data-stu-id="4d3af-145">Supported operations</span></span>

| <span data-ttu-id="4d3af-146">Ентитет планирања</span><span class="sxs-lookup"><span data-stu-id="4d3af-146">Scheduling entity</span></span> | <span data-ttu-id="4d3af-147">Направи</span><span class="sxs-lookup"><span data-stu-id="4d3af-147">Create</span></span> | <span data-ttu-id="4d3af-148">Ажурирање</span><span class="sxs-lookup"><span data-stu-id="4d3af-148">Update</span></span> | <span data-ttu-id="4d3af-149">Delete</span><span class="sxs-lookup"><span data-stu-id="4d3af-149">Delete</span></span> | <span data-ttu-id="4d3af-150">Важна разматрања</span><span class="sxs-lookup"><span data-stu-id="4d3af-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="4d3af-151">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="4d3af-151">Project task</span></span> | <span data-ttu-id="4d3af-152">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-152">Yes</span></span> | <span data-ttu-id="4d3af-153">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-153">Yes</span></span> | <span data-ttu-id="4d3af-154">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-154">Yes</span></span> | <span data-ttu-id="4d3af-155">Ниједно</span><span class="sxs-lookup"><span data-stu-id="4d3af-155">None</span></span> |
| <span data-ttu-id="4d3af-156">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="4d3af-156">Project task dependency</span></span> | <span data-ttu-id="4d3af-157">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-157">Yes</span></span> | <span data-ttu-id="4d3af-158">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-158">Yes</span></span> | | <span data-ttu-id="4d3af-159">Записи зависности пројектних задатака се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="4d3af-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="4d3af-160">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="4d3af-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="4d3af-161">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="4d3af-161">Resource assignment</span></span> | <span data-ttu-id="4d3af-162">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-162">Yes</span></span> | <span data-ttu-id="4d3af-163">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-163">Yes</span></span> | | <span data-ttu-id="4d3af-164">Нису подржане операције са следећим пољима: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="4d3af-165">Записи о додели ресурса се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="4d3af-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="4d3af-166">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="4d3af-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="4d3af-167">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="4d3af-167">Project bucket</span></span> | <span data-ttu-id="4d3af-168">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="4d3af-168">N/A</span></span> | <span data-ttu-id="4d3af-169">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="4d3af-169">N/A</span></span> | <span data-ttu-id="4d3af-170">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="4d3af-170">N/A</span></span> | <span data-ttu-id="4d3af-171">Подразумевани контејнер се креира се помоћу API-ја **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="4d3af-172">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="4d3af-172">Project team member</span></span> | <span data-ttu-id="4d3af-173">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-173">Yes</span></span> | <span data-ttu-id="4d3af-174">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-174">Yes</span></span> | <span data-ttu-id="4d3af-175">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-175">Yes</span></span> | <span data-ttu-id="4d3af-176">За операцију креирања користите API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="4d3af-177">Project</span><span class="sxs-lookup"><span data-stu-id="4d3af-177">Project</span></span> | <span data-ttu-id="4d3af-178">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-178">Yes</span></span> | <span data-ttu-id="4d3af-179">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-179">Yes</span></span> | <span data-ttu-id="4d3af-180">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="4d3af-180">N/A</span></span> | <span data-ttu-id="4d3af-181">Нису подржане операције са следећим пољима: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="4d3af-182">Ови API-ји се могу позивати са објектима ентитета који укључују прилагођена поља.</span><span class="sxs-lookup"><span data-stu-id="4d3af-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="4d3af-183">Својство ID је опционално.</span><span class="sxs-lookup"><span data-stu-id="4d3af-183">The ID property is optional.</span></span> <span data-ttu-id="4d3af-184">Ако је обезбеђено, систем покушава да га користи и избацује изузетак ако не може да га користи.</span><span class="sxs-lookup"><span data-stu-id="4d3af-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="4d3af-185">Ако није обезбеђено, систем ће га генерисати.</span><span class="sxs-lookup"><span data-stu-id="4d3af-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="4d3af-186">Ограничена поља</span><span class="sxs-lookup"><span data-stu-id="4d3af-186">Restricted fields</span></span>

<span data-ttu-id="4d3af-187">Следеће табеле дефинишу поља за која је ограничено **Креирај** и **Уреди.**</span><span class="sxs-lookup"><span data-stu-id="4d3af-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="4d3af-188">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="4d3af-188">Project task</span></span>

| <span data-ttu-id="4d3af-189">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="4d3af-189">**Logical name**</span></span>                       | <span data-ttu-id="4d3af-190">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="4d3af-190">**Can create**</span></span> | <span data-ttu-id="4d3af-191">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="4d3af-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="4d3af-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="4d3af-193">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-193">no</span></span>             | <span data-ttu-id="4d3af-194">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-194">no</span></span>               |
| <span data-ttu-id="4d3af-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="4d3af-196">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-196">no</span></span>             | <span data-ttu-id="4d3af-197">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-197">no</span></span>               |
| <span data-ttu-id="4d3af-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="4d3af-198">msdyn_actualend</span></span>                        | <span data-ttu-id="4d3af-199">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-199">no</span></span>             | <span data-ttu-id="4d3af-200">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-200">no</span></span>               |
| <span data-ttu-id="4d3af-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="4d3af-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="4d3af-202">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-202">no</span></span>             | <span data-ttu-id="4d3af-203">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-203">no</span></span>               |
| <span data-ttu-id="4d3af-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="4d3af-205">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-205">no</span></span>             | <span data-ttu-id="4d3af-206">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-206">no</span></span>               |
| <span data-ttu-id="4d3af-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="4d3af-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="4d3af-208">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-208">no</span></span>             | <span data-ttu-id="4d3af-209">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-209">no</span></span>               |
| <span data-ttu-id="4d3af-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="4d3af-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="4d3af-211">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-211">no</span></span>             | <span data-ttu-id="4d3af-212">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-212">no</span></span>               |
| <span data-ttu-id="4d3af-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="4d3af-214">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-214">no</span></span>             | <span data-ttu-id="4d3af-215">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-215">no</span></span>               |
| <span data-ttu-id="4d3af-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="4d3af-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="4d3af-217">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-217">no</span></span>             | <span data-ttu-id="4d3af-218">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-218">no</span></span>               |
| <span data-ttu-id="4d3af-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4d3af-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="4d3af-220">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-220">no</span></span>             | <span data-ttu-id="4d3af-221">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-221">no</span></span>               |
| <span data-ttu-id="4d3af-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="4d3af-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="4d3af-223">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-223">no</span></span>             | <span data-ttu-id="4d3af-224">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-224">no</span></span>               |
| <span data-ttu-id="4d3af-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="4d3af-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="4d3af-226">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-226">no</span></span>             | <span data-ttu-id="4d3af-227">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-227">no</span></span>               |
| <span data-ttu-id="4d3af-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="4d3af-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="4d3af-229">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-229">no</span></span>             | <span data-ttu-id="4d3af-230">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-230">no</span></span>               |
| <span data-ttu-id="4d3af-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="4d3af-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="4d3af-232">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-232">no</span></span>             | <span data-ttu-id="4d3af-233">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-233">no</span></span>               |
| <span data-ttu-id="4d3af-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="4d3af-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="4d3af-235">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-235">no</span></span>             | <span data-ttu-id="4d3af-236">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-236">no</span></span>               |
| <span data-ttu-id="4d3af-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="4d3af-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="4d3af-238">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-238">no</span></span>             | <span data-ttu-id="4d3af-239">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-239">no</span></span>               |
| <span data-ttu-id="4d3af-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="4d3af-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="4d3af-241">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-241">no</span></span>             | <span data-ttu-id="4d3af-242">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-242">no</span></span>               |
| <span data-ttu-id="4d3af-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="4d3af-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="4d3af-244">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-244">no</span></span>             | <span data-ttu-id="4d3af-245">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-245">no</span></span>               |
| <span data-ttu-id="4d3af-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="4d3af-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="4d3af-247">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-247">no</span></span>             | <span data-ttu-id="4d3af-248">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-248">no</span></span>               |
| <span data-ttu-id="4d3af-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="4d3af-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="4d3af-250">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-250">no</span></span>             | <span data-ttu-id="4d3af-251">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-251">no</span></span>               |
| <span data-ttu-id="4d3af-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="4d3af-253">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-253">no</span></span>             | <span data-ttu-id="4d3af-254">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-254">no</span></span>               |
| <span data-ttu-id="4d3af-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="4d3af-256">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-256">no</span></span>             | <span data-ttu-id="4d3af-257">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-257">no</span></span>               |
| <span data-ttu-id="4d3af-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4d3af-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="4d3af-259">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-259">no</span></span>             | <span data-ttu-id="4d3af-260">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-260">no</span></span>               |
| <span data-ttu-id="4d3af-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="4d3af-262">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-262">no</span></span>             | <span data-ttu-id="4d3af-263">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-263">no</span></span>               |
| <span data-ttu-id="4d3af-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="4d3af-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="4d3af-265">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-265">no</span></span>             | <span data-ttu-id="4d3af-266">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-266">no</span></span>               |
| <span data-ttu-id="4d3af-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="4d3af-267">msdyn_progress</span></span>                         | <span data-ttu-id="4d3af-268">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-268">no</span></span>             | <span data-ttu-id="4d3af-269">не (да за P4W)</span><span class="sxs-lookup"><span data-stu-id="4d3af-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="4d3af-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="4d3af-271">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-271">no</span></span>             | <span data-ttu-id="4d3af-272">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-272">no</span></span>               |
| <span data-ttu-id="4d3af-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="4d3af-274">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-274">no</span></span>             | <span data-ttu-id="4d3af-275">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-275">no</span></span>               |
| <span data-ttu-id="4d3af-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="4d3af-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="4d3af-277">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-277">no</span></span>             | <span data-ttu-id="4d3af-278">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-278">no</span></span>               |
| <span data-ttu-id="4d3af-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="4d3af-280">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-280">no</span></span>             | <span data-ttu-id="4d3af-281">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-281">no</span></span>               |
| <span data-ttu-id="4d3af-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="4d3af-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="4d3af-283">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-283">no</span></span>             | <span data-ttu-id="4d3af-284">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-284">no</span></span>               |
| <span data-ttu-id="4d3af-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="4d3af-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="4d3af-286">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-286">no</span></span>             | <span data-ttu-id="4d3af-287">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-287">no</span></span>               |
| <span data-ttu-id="4d3af-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="4d3af-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="4d3af-289">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-289">no</span></span>             | <span data-ttu-id="4d3af-290">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-290">no</span></span>               |
| <span data-ttu-id="4d3af-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="4d3af-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="4d3af-292">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-292">no</span></span>             | <span data-ttu-id="4d3af-293">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-293">no</span></span>               |
| <span data-ttu-id="4d3af-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="4d3af-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="4d3af-295">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-295">no</span></span>             | <span data-ttu-id="4d3af-296">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-296">no</span></span>               |
| <span data-ttu-id="4d3af-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="4d3af-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="4d3af-298">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-298">no</span></span>             | <span data-ttu-id="4d3af-299">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-299">no</span></span>               |
| <span data-ttu-id="4d3af-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="4d3af-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="4d3af-301">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-301">no</span></span>             | <span data-ttu-id="4d3af-302">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-302">no</span></span>               |
| <span data-ttu-id="4d3af-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="4d3af-304">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-304">no</span></span>             | <span data-ttu-id="4d3af-305">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-305">no</span></span>               |
| <span data-ttu-id="4d3af-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="4d3af-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="4d3af-307">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-307">no</span></span>             | <span data-ttu-id="4d3af-308">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-308">no</span></span>               |
| <span data-ttu-id="4d3af-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="4d3af-310">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-310">no</span></span>             | <span data-ttu-id="4d3af-311">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-311">no</span></span>               |
| <span data-ttu-id="4d3af-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="4d3af-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="4d3af-313">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-313">no</span></span>             | <span data-ttu-id="4d3af-314">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-314">no</span></span>               |
| <span data-ttu-id="4d3af-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="4d3af-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="4d3af-316">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-316">no</span></span>             | <span data-ttu-id="4d3af-317">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-317">no</span></span>               |
| <span data-ttu-id="4d3af-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="4d3af-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="4d3af-319">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-319">no</span></span>             | <span data-ttu-id="4d3af-320">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-320">no</span></span>               |
| <span data-ttu-id="4d3af-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="4d3af-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="4d3af-322">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-322">no</span></span>             | <span data-ttu-id="4d3af-323">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-323">no</span></span>               |
| <span data-ttu-id="4d3af-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="4d3af-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="4d3af-325">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-325">no</span></span>             | <span data-ttu-id="4d3af-326">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-326">no</span></span>               |
| <span data-ttu-id="4d3af-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="4d3af-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="4d3af-328">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-328">no</span></span>             | <span data-ttu-id="4d3af-329">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-329">no</span></span>               |
| <span data-ttu-id="4d3af-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="4d3af-330">msdyn_summary</span></span>                          | <span data-ttu-id="4d3af-331">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-331">no</span></span>             | <span data-ttu-id="4d3af-332">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-332">no</span></span>               |
| <span data-ttu-id="4d3af-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="4d3af-334">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-334">no</span></span>             | <span data-ttu-id="4d3af-335">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-335">no</span></span>               |
| <span data-ttu-id="4d3af-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="4d3af-337">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-337">no</span></span>             | <span data-ttu-id="4d3af-338">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="4d3af-339">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="4d3af-339">Project task dependency</span></span>

| <span data-ttu-id="4d3af-340">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="4d3af-340">**Logical name**</span></span>              | <span data-ttu-id="4d3af-341">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="4d3af-341">**Can create**</span></span> | <span data-ttu-id="4d3af-342">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="4d3af-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="4d3af-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="4d3af-343">msdyn_linktype</span></span>                | <span data-ttu-id="4d3af-344">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-344">no</span></span>             | <span data-ttu-id="4d3af-345">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-345">no</span></span>           |
| <span data-ttu-id="4d3af-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="4d3af-346">msdyn_linktypename</span></span>            | <span data-ttu-id="4d3af-347">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-347">no</span></span>             | <span data-ttu-id="4d3af-348">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-348">no</span></span>           |
| <span data-ttu-id="4d3af-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="4d3af-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="4d3af-350">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-350">yes</span></span>            | <span data-ttu-id="4d3af-351">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-351">no</span></span>           |
| <span data-ttu-id="4d3af-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="4d3af-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="4d3af-353">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-353">yes</span></span>            | <span data-ttu-id="4d3af-354">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-354">no</span></span>           |
| <span data-ttu-id="4d3af-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="4d3af-355">msdyn_project</span></span>                 | <span data-ttu-id="4d3af-356">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-356">yes</span></span>            | <span data-ttu-id="4d3af-357">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-357">no</span></span>           |
| <span data-ttu-id="4d3af-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="4d3af-358">msdyn_projectname</span></span>             | <span data-ttu-id="4d3af-359">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-359">yes</span></span>            | <span data-ttu-id="4d3af-360">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-360">no</span></span>           |
| <span data-ttu-id="4d3af-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="4d3af-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="4d3af-362">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-362">yes</span></span>            | <span data-ttu-id="4d3af-363">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-363">no</span></span>           |
| <span data-ttu-id="4d3af-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="4d3af-364">msdyn_successortask</span></span>           | <span data-ttu-id="4d3af-365">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-365">yes</span></span>            | <span data-ttu-id="4d3af-366">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-366">no</span></span>           |
| <span data-ttu-id="4d3af-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="4d3af-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="4d3af-368">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-368">yes</span></span>            | <span data-ttu-id="4d3af-369">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="4d3af-370">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="4d3af-370">Resource assignment</span></span>

| <span data-ttu-id="4d3af-371">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="4d3af-371">**Logical name**</span></span>             | <span data-ttu-id="4d3af-372">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="4d3af-372">**Can create**</span></span> | <span data-ttu-id="4d3af-373">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="4d3af-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="4d3af-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="4d3af-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="4d3af-375">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-375">yes</span></span>            | <span data-ttu-id="4d3af-376">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-376">no</span></span>           |
| <span data-ttu-id="4d3af-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="4d3af-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="4d3af-378">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-378">yes</span></span>            | <span data-ttu-id="4d3af-379">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-379">no</span></span>           |
| <span data-ttu-id="4d3af-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="4d3af-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="4d3af-381">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-381">no</span></span>             | <span data-ttu-id="4d3af-382">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-382">no</span></span>           |
| <span data-ttu-id="4d3af-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="4d3af-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="4d3af-384">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-384">no</span></span>             | <span data-ttu-id="4d3af-385">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-385">no</span></span>           |
| <span data-ttu-id="4d3af-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="4d3af-386">msdyn_committype</span></span>             | <span data-ttu-id="4d3af-387">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-387">no</span></span>             | <span data-ttu-id="4d3af-388">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-388">no</span></span>           |
| <span data-ttu-id="4d3af-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="4d3af-389">msdyn_committypename</span></span>         | <span data-ttu-id="4d3af-390">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-390">no</span></span>             | <span data-ttu-id="4d3af-391">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-391">no</span></span>           |
| <span data-ttu-id="4d3af-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="4d3af-392">msdyn_effort</span></span>                 | <span data-ttu-id="4d3af-393">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-393">no</span></span>             | <span data-ttu-id="4d3af-394">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-394">no</span></span>           |
| <span data-ttu-id="4d3af-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4d3af-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="4d3af-396">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-396">no</span></span>             | <span data-ttu-id="4d3af-397">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-397">no</span></span>           |
| <span data-ttu-id="4d3af-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="4d3af-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="4d3af-399">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-399">no</span></span>             | <span data-ttu-id="4d3af-400">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-400">no</span></span>           |
| <span data-ttu-id="4d3af-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="4d3af-401">msdyn_finish</span></span>                 | <span data-ttu-id="4d3af-402">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-402">no</span></span>             | <span data-ttu-id="4d3af-403">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-403">no</span></span>           |
| <span data-ttu-id="4d3af-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="4d3af-405">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-405">no</span></span>             | <span data-ttu-id="4d3af-406">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-406">no</span></span>           |
| <span data-ttu-id="4d3af-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="4d3af-408">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-408">no</span></span>             | <span data-ttu-id="4d3af-409">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-409">no</span></span>           |
| <span data-ttu-id="4d3af-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="4d3af-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="4d3af-411">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-411">no</span></span>             | <span data-ttu-id="4d3af-412">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-412">no</span></span>           |
| <span data-ttu-id="4d3af-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4d3af-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="4d3af-414">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-414">no</span></span>             | <span data-ttu-id="4d3af-415">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-415">no</span></span>           |
| <span data-ttu-id="4d3af-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="4d3af-417">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-417">no</span></span>             | <span data-ttu-id="4d3af-418">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-418">no</span></span>           |
| <span data-ttu-id="4d3af-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="4d3af-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="4d3af-420">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-420">no</span></span>             | <span data-ttu-id="4d3af-421">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-421">no</span></span>           |
| <span data-ttu-id="4d3af-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="4d3af-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="4d3af-423">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-423">no</span></span>             | <span data-ttu-id="4d3af-424">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-424">no</span></span>           |
| <span data-ttu-id="4d3af-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="4d3af-425">msdyn_projectid</span></span>              | <span data-ttu-id="4d3af-426">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-426">yes</span></span>            | <span data-ttu-id="4d3af-427">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-427">no</span></span>           |
| <span data-ttu-id="4d3af-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="4d3af-428">msdyn_projectidname</span></span>          | <span data-ttu-id="4d3af-429">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-429">no</span></span>             | <span data-ttu-id="4d3af-430">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-430">no</span></span>           |
| <span data-ttu-id="4d3af-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="4d3af-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="4d3af-432">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-432">no</span></span>             | <span data-ttu-id="4d3af-433">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-433">no</span></span>           |
| <span data-ttu-id="4d3af-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="4d3af-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="4d3af-435">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-435">no</span></span>             | <span data-ttu-id="4d3af-436">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-436">no</span></span>           |
| <span data-ttu-id="4d3af-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="4d3af-437">msdyn_start</span></span>                  | <span data-ttu-id="4d3af-438">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-438">no</span></span>             | <span data-ttu-id="4d3af-439">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-439">no</span></span>           |
| <span data-ttu-id="4d3af-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="4d3af-440">msdyn_taskid</span></span>                 | <span data-ttu-id="4d3af-441">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-441">no</span></span>             | <span data-ttu-id="4d3af-442">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-442">no</span></span>           |
| <span data-ttu-id="4d3af-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="4d3af-443">msdyn_taskidname</span></span>             | <span data-ttu-id="4d3af-444">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-444">no</span></span>             | <span data-ttu-id="4d3af-445">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-445">no</span></span>           |
| <span data-ttu-id="4d3af-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="4d3af-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="4d3af-447">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-447">no</span></span>             | <span data-ttu-id="4d3af-448">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="4d3af-449">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="4d3af-449">Project team member</span></span>

| <span data-ttu-id="4d3af-450">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="4d3af-450">**Logical name**</span></span>                                 | <span data-ttu-id="4d3af-451">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="4d3af-451">**Can create**</span></span> | <span data-ttu-id="4d3af-452">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="4d3af-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="4d3af-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="4d3af-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="4d3af-454">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-454">no</span></span>             | <span data-ttu-id="4d3af-455">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-455">no</span></span>           |
| <span data-ttu-id="4d3af-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="4d3af-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="4d3af-457">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-457">no</span></span>             | <span data-ttu-id="4d3af-458">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-458">no</span></span>           |
| <span data-ttu-id="4d3af-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="4d3af-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="4d3af-460">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-460">no</span></span>             | <span data-ttu-id="4d3af-461">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-461">no</span></span>           |
| <span data-ttu-id="4d3af-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="4d3af-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="4d3af-463">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-463">no</span></span>             | <span data-ttu-id="4d3af-464">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-464">no</span></span>           |
| <span data-ttu-id="4d3af-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="4d3af-465">msdyn_effort</span></span>                                     | <span data-ttu-id="4d3af-466">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-466">no</span></span>             | <span data-ttu-id="4d3af-467">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-467">no</span></span>           |
| <span data-ttu-id="4d3af-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4d3af-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="4d3af-469">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-469">no</span></span>             | <span data-ttu-id="4d3af-470">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-470">no</span></span>           |
| <span data-ttu-id="4d3af-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="4d3af-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="4d3af-472">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-472">no</span></span>             | <span data-ttu-id="4d3af-473">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-473">no</span></span>           |
| <span data-ttu-id="4d3af-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="4d3af-474">msdyn_finish</span></span>                                     | <span data-ttu-id="4d3af-475">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-475">no</span></span>             | <span data-ttu-id="4d3af-476">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-476">no</span></span>           |
| <span data-ttu-id="4d3af-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="4d3af-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="4d3af-478">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-478">no</span></span>             | <span data-ttu-id="4d3af-479">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-479">no</span></span>           |
| <span data-ttu-id="4d3af-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="4d3af-480">msdyn_hours</span></span>                                      | <span data-ttu-id="4d3af-481">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-481">no</span></span>             | <span data-ttu-id="4d3af-482">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-482">no</span></span>           |
| <span data-ttu-id="4d3af-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="4d3af-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="4d3af-484">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-484">no</span></span>             | <span data-ttu-id="4d3af-485">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-485">no</span></span>           |
| <span data-ttu-id="4d3af-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="4d3af-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="4d3af-487">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-487">no</span></span>             | <span data-ttu-id="4d3af-488">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-488">no</span></span>           |
| <span data-ttu-id="4d3af-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="4d3af-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="4d3af-490">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-490">no</span></span>             | <span data-ttu-id="4d3af-491">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-491">no</span></span>           |
| <span data-ttu-id="4d3af-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="4d3af-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="4d3af-493">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-493">no</span></span>             | <span data-ttu-id="4d3af-494">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-494">no</span></span>           |
| <span data-ttu-id="4d3af-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="4d3af-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="4d3af-496">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-496">no</span></span>             | <span data-ttu-id="4d3af-497">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-497">no</span></span>           |
| <span data-ttu-id="4d3af-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="4d3af-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="4d3af-499">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-499">no</span></span>             | <span data-ttu-id="4d3af-500">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-500">no</span></span>           |
| <span data-ttu-id="4d3af-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="4d3af-501">msdyn_start</span></span>                                      | <span data-ttu-id="4d3af-502">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-502">no</span></span>             | <span data-ttu-id="4d3af-503">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="4d3af-504">Project</span><span class="sxs-lookup"><span data-stu-id="4d3af-504">Project</span></span>

| <span data-ttu-id="4d3af-505">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="4d3af-505">**Logical name**</span></span>                       | <span data-ttu-id="4d3af-506">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="4d3af-506">**Can create**</span></span> | <span data-ttu-id="4d3af-507">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="4d3af-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="4d3af-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="4d3af-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="4d3af-509">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-509">no</span></span>             | <span data-ttu-id="4d3af-510">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-510">no</span></span>           |
| <span data-ttu-id="4d3af-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="4d3af-512">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-512">no</span></span>             | <span data-ttu-id="4d3af-513">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-513">no</span></span>           |
| <span data-ttu-id="4d3af-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="4d3af-515">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-515">no</span></span>             | <span data-ttu-id="4d3af-516">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-516">no</span></span>           |
| <span data-ttu-id="4d3af-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="4d3af-518">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-518">no</span></span>             | <span data-ttu-id="4d3af-519">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-519">no</span></span>           |
| <span data-ttu-id="4d3af-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="4d3af-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="4d3af-521">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-521">no</span></span>             | <span data-ttu-id="4d3af-522">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-522">no</span></span>           |
| <span data-ttu-id="4d3af-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="4d3af-524">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-524">no</span></span>             | <span data-ttu-id="4d3af-525">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-525">no</span></span>           |
| <span data-ttu-id="4d3af-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="4d3af-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="4d3af-527">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-527">yes</span></span>            | <span data-ttu-id="4d3af-528">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-528">no</span></span>           |
| <span data-ttu-id="4d3af-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="4d3af-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="4d3af-530">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-530">yes</span></span>            | <span data-ttu-id="4d3af-531">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-531">no</span></span>           |
| <span data-ttu-id="4d3af-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="4d3af-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="4d3af-533">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-533">yes</span></span>            | <span data-ttu-id="4d3af-534">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-534">no</span></span>           |
| <span data-ttu-id="4d3af-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="4d3af-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="4d3af-536">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-536">no</span></span>             | <span data-ttu-id="4d3af-537">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-537">no</span></span>           |
| <span data-ttu-id="4d3af-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="4d3af-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="4d3af-539">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-539">no</span></span>             | <span data-ttu-id="4d3af-540">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-540">no</span></span>           |
| <span data-ttu-id="4d3af-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="4d3af-542">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-542">no</span></span>             | <span data-ttu-id="4d3af-543">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-543">no</span></span>           |
| <span data-ttu-id="4d3af-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="4d3af-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="4d3af-545">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-545">no</span></span>             | <span data-ttu-id="4d3af-546">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-546">no</span></span>           |
| <span data-ttu-id="4d3af-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="4d3af-548">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-548">no</span></span>             | <span data-ttu-id="4d3af-549">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-549">no</span></span>           |
| <span data-ttu-id="4d3af-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="4d3af-550">msdyn_duration</span></span>                         | <span data-ttu-id="4d3af-551">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-551">no</span></span>             | <span data-ttu-id="4d3af-552">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-552">no</span></span>           |
| <span data-ttu-id="4d3af-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="4d3af-553">msdyn_effort</span></span>                           | <span data-ttu-id="4d3af-554">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-554">no</span></span>             | <span data-ttu-id="4d3af-555">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-555">no</span></span>           |
| <span data-ttu-id="4d3af-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4d3af-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="4d3af-557">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-557">no</span></span>             | <span data-ttu-id="4d3af-558">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-558">no</span></span>           |
| <span data-ttu-id="4d3af-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="4d3af-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="4d3af-560">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-560">no</span></span>             | <span data-ttu-id="4d3af-561">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-561">no</span></span>           |
| <span data-ttu-id="4d3af-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="4d3af-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="4d3af-563">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-563">no</span></span>             | <span data-ttu-id="4d3af-564">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-564">no</span></span>           |
| <span data-ttu-id="4d3af-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="4d3af-565">msdyn_finish</span></span>                           | <span data-ttu-id="4d3af-566">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-566">yes</span></span>            | <span data-ttu-id="4d3af-567">Да</span><span class="sxs-lookup"><span data-stu-id="4d3af-567">yes</span></span>          |
| <span data-ttu-id="4d3af-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="4d3af-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="4d3af-569">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-569">no</span></span>             | <span data-ttu-id="4d3af-570">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-570">no</span></span>           |
| <span data-ttu-id="4d3af-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="4d3af-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="4d3af-572">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-572">no</span></span>             | <span data-ttu-id="4d3af-573">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-573">no</span></span>           |
| <span data-ttu-id="4d3af-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="4d3af-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="4d3af-575">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-575">no</span></span>             | <span data-ttu-id="4d3af-576">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-576">no</span></span>           |
| <span data-ttu-id="4d3af-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="4d3af-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="4d3af-578">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-578">no</span></span>             | <span data-ttu-id="4d3af-579">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-579">no</span></span>           |
| <span data-ttu-id="4d3af-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="4d3af-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="4d3af-581">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-581">no</span></span>             | <span data-ttu-id="4d3af-582">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-582">no</span></span>           |
| <span data-ttu-id="4d3af-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="4d3af-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="4d3af-584">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-584">no</span></span>             | <span data-ttu-id="4d3af-585">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-585">no</span></span>           |
| <span data-ttu-id="4d3af-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="4d3af-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="4d3af-587">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-587">no</span></span>             | <span data-ttu-id="4d3af-588">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-588">no</span></span>           |
| <span data-ttu-id="4d3af-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="4d3af-590">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-590">no</span></span>             | <span data-ttu-id="4d3af-591">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-591">no</span></span>           |
| <span data-ttu-id="4d3af-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="4d3af-593">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-593">no</span></span>             | <span data-ttu-id="4d3af-594">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-594">no</span></span>           |
| <span data-ttu-id="4d3af-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="4d3af-596">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-596">no</span></span>             | <span data-ttu-id="4d3af-597">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-597">no</span></span>           |
| <span data-ttu-id="4d3af-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4d3af-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="4d3af-599">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-599">no</span></span>             | <span data-ttu-id="4d3af-600">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-600">no</span></span>           |
| <span data-ttu-id="4d3af-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="4d3af-602">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-602">no</span></span>             | <span data-ttu-id="4d3af-603">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-603">no</span></span>           |
| <span data-ttu-id="4d3af-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="4d3af-604">msdyn_progress</span></span>                         | <span data-ttu-id="4d3af-605">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-605">no</span></span>             | <span data-ttu-id="4d3af-606">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-606">no</span></span>           |
| <span data-ttu-id="4d3af-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="4d3af-608">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-608">no</span></span>             | <span data-ttu-id="4d3af-609">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-609">no</span></span>           |
| <span data-ttu-id="4d3af-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="4d3af-611">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-611">no</span></span>             | <span data-ttu-id="4d3af-612">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-612">no</span></span>           |
| <span data-ttu-id="4d3af-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="4d3af-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="4d3af-614">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-614">no</span></span>             | <span data-ttu-id="4d3af-615">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-615">no</span></span>           |
| <span data-ttu-id="4d3af-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="4d3af-617">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-617">no</span></span>             | <span data-ttu-id="4d3af-618">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-618">no</span></span>           |
| <span data-ttu-id="4d3af-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="4d3af-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="4d3af-620">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-620">no</span></span>             | <span data-ttu-id="4d3af-621">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-621">no</span></span>           |
| <span data-ttu-id="4d3af-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="4d3af-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="4d3af-623">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-623">no</span></span>             | <span data-ttu-id="4d3af-624">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-624">no</span></span>           |
| <span data-ttu-id="4d3af-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="4d3af-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="4d3af-626">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-626">no</span></span>             | <span data-ttu-id="4d3af-627">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-627">no</span></span>           |
| <span data-ttu-id="4d3af-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="4d3af-629">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-629">no</span></span>             | <span data-ttu-id="4d3af-630">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-630">no</span></span>           |
| <span data-ttu-id="4d3af-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="4d3af-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="4d3af-632">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-632">no</span></span>             | <span data-ttu-id="4d3af-633">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-633">no</span></span>           |
| <span data-ttu-id="4d3af-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="4d3af-635">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-635">no</span></span>             | <span data-ttu-id="4d3af-636">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-636">no</span></span>           |
| <span data-ttu-id="4d3af-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="4d3af-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="4d3af-638">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-638">no</span></span>             | <span data-ttu-id="4d3af-639">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-639">no</span></span>           |
| <span data-ttu-id="4d3af-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="4d3af-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="4d3af-641">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-641">no</span></span>             | <span data-ttu-id="4d3af-642">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-642">no</span></span>           |
| <span data-ttu-id="4d3af-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="4d3af-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="4d3af-644">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-644">no</span></span>             | <span data-ttu-id="4d3af-645">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-645">no</span></span>           |
| <span data-ttu-id="4d3af-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="4d3af-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="4d3af-647">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-647">no</span></span>             | <span data-ttu-id="4d3af-648">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-648">no</span></span>           |
| <span data-ttu-id="4d3af-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="4d3af-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="4d3af-650">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-650">no</span></span>             | <span data-ttu-id="4d3af-651">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-651">no</span></span>           |
| <span data-ttu-id="4d3af-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="4d3af-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="4d3af-653">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-653">no</span></span>             | <span data-ttu-id="4d3af-654">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-654">no</span></span>           |
| <span data-ttu-id="4d3af-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="4d3af-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="4d3af-656">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-656">no</span></span>             | <span data-ttu-id="4d3af-657">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-657">no</span></span>           |
| <span data-ttu-id="4d3af-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="4d3af-659">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-659">no</span></span>             | <span data-ttu-id="4d3af-660">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-660">no</span></span>           |
| <span data-ttu-id="4d3af-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="4d3af-662">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-662">no</span></span>             | <span data-ttu-id="4d3af-663">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-663">no</span></span>           |
| <span data-ttu-id="4d3af-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="4d3af-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="4d3af-665">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-665">no</span></span>             | <span data-ttu-id="4d3af-666">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-666">no</span></span>           |
| <span data-ttu-id="4d3af-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="4d3af-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="4d3af-668">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-668">no</span></span>             | <span data-ttu-id="4d3af-669">не</span><span class="sxs-lookup"><span data-stu-id="4d3af-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="4d3af-670">Ограничења и познати проблеми</span><span class="sxs-lookup"><span data-stu-id="4d3af-670">Limitations and known issues</span></span>
<span data-ttu-id="4d3af-671">Следи листа ограничења и познатих проблема:</span><span class="sxs-lookup"><span data-stu-id="4d3af-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="4d3af-672">API-је за распоред пројеката могу да користе само **Корисници са лиценцом за Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="4d3af-672">Project Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="4d3af-673">Не могу их користити:</span><span class="sxs-lookup"><span data-stu-id="4d3af-673">They can't be used by:</span></span>
    - <span data-ttu-id="4d3af-674">Корисници апликације</span><span class="sxs-lookup"><span data-stu-id="4d3af-674">Application users</span></span>
    - <span data-ttu-id="4d3af-675">Корисници система</span><span class="sxs-lookup"><span data-stu-id="4d3af-675">System users</span></span>
    - <span data-ttu-id="4d3af-676">Корисници интеграције</span><span class="sxs-lookup"><span data-stu-id="4d3af-676">Integration users</span></span>
    - <span data-ttu-id="4d3af-677">Остали корисници који немају потребну лиценцу</span><span class="sxs-lookup"><span data-stu-id="4d3af-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="4d3af-678">Сваки **OperationSet ентитет** може да има највише 100 операција.</span><span class="sxs-lookup"><span data-stu-id="4d3af-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="4d3af-679">Сваки корисник може да има највише 10 отворених **OperationSet ентитета**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="4d3af-680">Project Operations тренутно подржава максимално 500 укупних задатака на пројекту.</span><span class="sxs-lookup"><span data-stu-id="4d3af-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="4d3af-681">Статус грешке и евиденције грешака **OperationSet ентитета** тренутно нису доступне.</span><span class="sxs-lookup"><span data-stu-id="4d3af-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="4d3af-682">Ограничења и границе пројеката и задатака</span><span class="sxs-lookup"><span data-stu-id="4d3af-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="4d3af-683">Руковање грешкама</span><span class="sxs-lookup"><span data-stu-id="4d3af-683">Error handling</span></span>

   - <span data-ttu-id="4d3af-684">Да бисте прегледали грешке генерисане из скупова операција, идите на **Подешавања** \> **Закажи интеграцију** \> **Скупови операција**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="4d3af-685">Да бисте прегледали грешке које је генерисала услуга распореда пројеката, идите на **Подешавања** \> **Интеграција распореда** \> **PSS евиденције грешака**.</span><span class="sxs-lookup"><span data-stu-id="4d3af-685">To review errors generated from the Project schedule Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="4d3af-686">Пример сценарија</span><span class="sxs-lookup"><span data-stu-id="4d3af-686">Sample scenario</span></span>

<span data-ttu-id="4d3af-687">У овом сценарију, креираћете пројекат, члана тима, четири задатка и два задатка ресурса.</span><span class="sxs-lookup"><span data-stu-id="4d3af-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="4d3af-688">Затим ћете ажурирати један задатак, ажурирати пројекат, избрисати један задатак, избрисати једну доделу ресурса и креирати зависност задатка.</span><span class="sxs-lookup"><span data-stu-id="4d3af-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="4d3af-689">Додатни примери</span><span class="sxs-lookup"><span data-stu-id="4d3af-689">Additional samples</span></span>

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
