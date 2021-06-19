---
title: Коришћење API-ја за распоред за обављање операција са ентитетима планирања
description: Ова тема пружа информације и примере за коришћење API-ја за распоред.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4a032dc7bcbdf23fce3c3b2ca63c51d473bd8e26
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116815"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="d49f9-103">Коришћење API-ја за распоред за обављање операција са ентитетима планирања</span><span class="sxs-lookup"><span data-stu-id="d49f9-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="d49f9-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="d49f9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="d49f9-105">Неке или све функционалности забележене у овој теми доступне су као део издања верзије за преглед.</span><span class="sxs-lookup"><span data-stu-id="d49f9-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="d49f9-106">Садржај и функционалност су подложни променама.</span><span class="sxs-lookup"><span data-stu-id="d49f9-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="d49f9-107">Ентитети планирања</span><span class="sxs-lookup"><span data-stu-id="d49f9-107">Scheduling entities</span></span>

<span data-ttu-id="d49f9-108">API-ји за распоред пружају могућност извршавања операција креирања, ажурирања и брисања помоћу **ентитета планирања**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="d49f9-109">Тим ентитетима се управља путем механизма за распоређивање у апликацији Project за веб.</span><span class="sxs-lookup"><span data-stu-id="d49f9-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="d49f9-110">Креирање, ажурирање и брисање операција помоћу **ентитета планирања** били су ограничени у ранијим издањима услуге Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="d49f9-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="d49f9-111">Следећа табела даје потпуну листу **ентитета планирања**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="d49f9-112">Назив ентитета</span><span class="sxs-lookup"><span data-stu-id="d49f9-112">Entity name</span></span>  | <span data-ttu-id="d49f9-113">Логичко име ентитета</span><span class="sxs-lookup"><span data-stu-id="d49f9-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="d49f9-114">Project</span><span class="sxs-lookup"><span data-stu-id="d49f9-114">Project</span></span> | <span data-ttu-id="d49f9-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="d49f9-115">msdyn_project</span></span> |
| <span data-ttu-id="d49f9-116">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="d49f9-116">Project Task</span></span>  | <span data-ttu-id="d49f9-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="d49f9-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="d49f9-118">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="d49f9-118">Project Task Dependency</span></span>  | <span data-ttu-id="d49f9-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="d49f9-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="d49f9-120">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="d49f9-120">Resource Assignment</span></span> | <span data-ttu-id="d49f9-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="d49f9-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="d49f9-122">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="d49f9-122">Project Bucket</span></span>  | <span data-ttu-id="d49f9-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="d49f9-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="d49f9-124">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="d49f9-124">Project Team Member</span></span> | <span data-ttu-id="d49f9-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="d49f9-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="d49f9-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="d49f9-126">OperationSet</span></span>

<span data-ttu-id="d49f9-127">Ентитет OperationSet је образац јединице рада који се може користити када се у трансакцији мора обрадити неколико захтева који утичу на распоред.</span><span class="sxs-lookup"><span data-stu-id="d49f9-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="d49f9-128">API-ји за распоред</span><span class="sxs-lookup"><span data-stu-id="d49f9-128">Schedule APIs</span></span>

<span data-ttu-id="d49f9-129">Следи листа актуелних API-ја за распоред.</span><span class="sxs-lookup"><span data-stu-id="d49f9-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="d49f9-130">**msdyn_CreateProjectV1**: Овај API се може користити за креирање пројекта.</span><span class="sxs-lookup"><span data-stu-id="d49f9-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="d49f9-131">Пројекат и подразумевани контејнер пројекта креирају се одмах.</span><span class="sxs-lookup"><span data-stu-id="d49f9-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="d49f9-132">**msdyn_CreateTeamMemberV1**: Овај API се може користити за креирање члана пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="d49f9-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="d49f9-133">Евиденција члана тима креира се одмах.</span><span class="sxs-lookup"><span data-stu-id="d49f9-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="d49f9-134">**msdyn_CreateOperationSetV1**: Овај API се може користити за заказивање неколико захтева који се морају извршити у оквиру трансакције.</span><span class="sxs-lookup"><span data-stu-id="d49f9-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="d49f9-135">**msdyn_PSSCreateV1**: Овај API се може користити за креирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="d49f9-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="d49f9-136">Ентитет може бити било који ентитет планирања који подржава операцију креирања.</span><span class="sxs-lookup"><span data-stu-id="d49f9-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="d49f9-137">**msdyn_PSSUpdateV1**: Овај API се може користити за ажурирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="d49f9-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="d49f9-138">Ентитет може бити било који ентитет планирања који подржава операцију ажурирања.</span><span class="sxs-lookup"><span data-stu-id="d49f9-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="d49f9-139">**msdyn_PSSDeleteV1**: Овај API се може користити за брисање ентитета.</span><span class="sxs-lookup"><span data-stu-id="d49f9-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="d49f9-140">Ентитет може бити било који ентитет планирања који подржава операцију брисања.</span><span class="sxs-lookup"><span data-stu-id="d49f9-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="d49f9-141">**msdyn_ExecuteOperationSetV1**: Овај API се користи за извршавање свих операција унутар датог скупа операција.</span><span class="sxs-lookup"><span data-stu-id="d49f9-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="d49f9-142">Коришћење API-ја распореда са OperationSet ентитетом</span><span class="sxs-lookup"><span data-stu-id="d49f9-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="d49f9-143">Пошто се записи са **CreateProjectV1** и **CreateTeamMemberV1** креирају одмах, ови API-ји се не могу користити у **OperationSet ентитету** директно.</span><span class="sxs-lookup"><span data-stu-id="d49f9-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="d49f9-144">Међутим, API можете користити за креирање потребних записа, креирајте **OperationSet ентитет**, а затим користите ове унапред креиране записе у **OperationSet ентитету**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="d49f9-145">Подржане операције</span><span class="sxs-lookup"><span data-stu-id="d49f9-145">Supported operations</span></span>

| <span data-ttu-id="d49f9-146">Ентитет планирања</span><span class="sxs-lookup"><span data-stu-id="d49f9-146">Scheduling entity</span></span> | <span data-ttu-id="d49f9-147">Направи</span><span class="sxs-lookup"><span data-stu-id="d49f9-147">Create</span></span> | <span data-ttu-id="d49f9-148">Ажурирање</span><span class="sxs-lookup"><span data-stu-id="d49f9-148">Update</span></span> | <span data-ttu-id="d49f9-149">Delete</span><span class="sxs-lookup"><span data-stu-id="d49f9-149">Delete</span></span> | <span data-ttu-id="d49f9-150">Важна разматрања</span><span class="sxs-lookup"><span data-stu-id="d49f9-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="d49f9-151">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="d49f9-151">Project task</span></span> | <span data-ttu-id="d49f9-152">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-152">Yes</span></span> | <span data-ttu-id="d49f9-153">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-153">Yes</span></span> | <span data-ttu-id="d49f9-154">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-154">Yes</span></span> | <span data-ttu-id="d49f9-155">Ниједно</span><span class="sxs-lookup"><span data-stu-id="d49f9-155">None</span></span> |
| <span data-ttu-id="d49f9-156">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="d49f9-156">Project task dependency</span></span> | <span data-ttu-id="d49f9-157">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-157">Yes</span></span> | <span data-ttu-id="d49f9-158">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-158">Yes</span></span> | | <span data-ttu-id="d49f9-159">Записи зависности пројектних задатака се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="d49f9-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="d49f9-160">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="d49f9-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="d49f9-161">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="d49f9-161">Resource assignment</span></span> | <span data-ttu-id="d49f9-162">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-162">Yes</span></span> | <span data-ttu-id="d49f9-163">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-163">Yes</span></span> | | <span data-ttu-id="d49f9-164">Нису подржане операције са следећим пољима: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="d49f9-165">Записи о додели ресурса се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="d49f9-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="d49f9-166">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="d49f9-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="d49f9-167">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="d49f9-167">Project bucket</span></span> | <span data-ttu-id="d49f9-168">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="d49f9-168">N/A</span></span> | <span data-ttu-id="d49f9-169">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="d49f9-169">N/A</span></span> | <span data-ttu-id="d49f9-170">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="d49f9-170">N/A</span></span> | <span data-ttu-id="d49f9-171">Подразумевани контејнер се креира се помоћу API-ја **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="d49f9-172">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="d49f9-172">Project team member</span></span> | <span data-ttu-id="d49f9-173">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-173">Yes</span></span> | <span data-ttu-id="d49f9-174">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-174">Yes</span></span> | <span data-ttu-id="d49f9-175">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-175">Yes</span></span> | <span data-ttu-id="d49f9-176">За операцију креирања користите API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="d49f9-177">Project</span><span class="sxs-lookup"><span data-stu-id="d49f9-177">Project</span></span> | <span data-ttu-id="d49f9-178">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-178">Yes</span></span> | <span data-ttu-id="d49f9-179">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-179">Yes</span></span> | <span data-ttu-id="d49f9-180">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="d49f9-180">N/A</span></span> | <span data-ttu-id="d49f9-181">Нису подржане операције са следећим пољима: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="d49f9-182">Ови API-ји се могу позивати са објектима ентитета који укључују прилагођена поља.</span><span class="sxs-lookup"><span data-stu-id="d49f9-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="d49f9-183">Својство ID је опционално.</span><span class="sxs-lookup"><span data-stu-id="d49f9-183">The ID property is optional.</span></span> <span data-ttu-id="d49f9-184">Ако је обезбеђено, систем покушава да га користи и избацује изузетак ако не може да га користи.</span><span class="sxs-lookup"><span data-stu-id="d49f9-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="d49f9-185">Ако није обезбеђено, систем ће га генерисати.</span><span class="sxs-lookup"><span data-stu-id="d49f9-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="d49f9-186">Ограничена поља</span><span class="sxs-lookup"><span data-stu-id="d49f9-186">Restricted fields</span></span>

<span data-ttu-id="d49f9-187">Следеће табеле дефинишу поља за која је ограничено **Креирај** и **Уреди.**</span><span class="sxs-lookup"><span data-stu-id="d49f9-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="d49f9-188">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="d49f9-188">Project task</span></span>

| <span data-ttu-id="d49f9-189">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="d49f9-189">**Logical name**</span></span>                       | <span data-ttu-id="d49f9-190">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="d49f9-190">**Can create**</span></span> | <span data-ttu-id="d49f9-191">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="d49f9-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="d49f9-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="d49f9-193">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-193">no</span></span>             | <span data-ttu-id="d49f9-194">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-194">no</span></span>               |
| <span data-ttu-id="d49f9-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="d49f9-196">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-196">no</span></span>             | <span data-ttu-id="d49f9-197">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-197">no</span></span>               |
| <span data-ttu-id="d49f9-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="d49f9-198">msdyn_actualend</span></span>                        | <span data-ttu-id="d49f9-199">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-199">no</span></span>             | <span data-ttu-id="d49f9-200">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-200">no</span></span>               |
| <span data-ttu-id="d49f9-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="d49f9-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="d49f9-202">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-202">no</span></span>             | <span data-ttu-id="d49f9-203">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-203">no</span></span>               |
| <span data-ttu-id="d49f9-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="d49f9-205">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-205">no</span></span>             | <span data-ttu-id="d49f9-206">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-206">no</span></span>               |
| <span data-ttu-id="d49f9-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="d49f9-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="d49f9-208">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-208">no</span></span>             | <span data-ttu-id="d49f9-209">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-209">no</span></span>               |
| <span data-ttu-id="d49f9-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="d49f9-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="d49f9-211">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-211">no</span></span>             | <span data-ttu-id="d49f9-212">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-212">no</span></span>               |
| <span data-ttu-id="d49f9-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="d49f9-214">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-214">no</span></span>             | <span data-ttu-id="d49f9-215">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-215">no</span></span>               |
| <span data-ttu-id="d49f9-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="d49f9-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="d49f9-217">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-217">no</span></span>             | <span data-ttu-id="d49f9-218">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-218">no</span></span>               |
| <span data-ttu-id="d49f9-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="d49f9-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="d49f9-220">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-220">no</span></span>             | <span data-ttu-id="d49f9-221">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-221">no</span></span>               |
| <span data-ttu-id="d49f9-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="d49f9-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="d49f9-223">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-223">no</span></span>             | <span data-ttu-id="d49f9-224">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-224">no</span></span>               |
| <span data-ttu-id="d49f9-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="d49f9-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="d49f9-226">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-226">no</span></span>             | <span data-ttu-id="d49f9-227">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-227">no</span></span>               |
| <span data-ttu-id="d49f9-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="d49f9-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="d49f9-229">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-229">no</span></span>             | <span data-ttu-id="d49f9-230">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-230">no</span></span>               |
| <span data-ttu-id="d49f9-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="d49f9-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="d49f9-232">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-232">no</span></span>             | <span data-ttu-id="d49f9-233">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-233">no</span></span>               |
| <span data-ttu-id="d49f9-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="d49f9-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="d49f9-235">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-235">no</span></span>             | <span data-ttu-id="d49f9-236">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-236">no</span></span>               |
| <span data-ttu-id="d49f9-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="d49f9-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="d49f9-238">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-238">no</span></span>             | <span data-ttu-id="d49f9-239">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-239">no</span></span>               |
| <span data-ttu-id="d49f9-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="d49f9-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="d49f9-241">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-241">no</span></span>             | <span data-ttu-id="d49f9-242">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-242">no</span></span>               |
| <span data-ttu-id="d49f9-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="d49f9-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="d49f9-244">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-244">no</span></span>             | <span data-ttu-id="d49f9-245">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-245">no</span></span>               |
| <span data-ttu-id="d49f9-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="d49f9-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="d49f9-247">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-247">no</span></span>             | <span data-ttu-id="d49f9-248">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-248">no</span></span>               |
| <span data-ttu-id="d49f9-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="d49f9-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="d49f9-250">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-250">no</span></span>             | <span data-ttu-id="d49f9-251">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-251">no</span></span>               |
| <span data-ttu-id="d49f9-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="d49f9-253">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-253">no</span></span>             | <span data-ttu-id="d49f9-254">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-254">no</span></span>               |
| <span data-ttu-id="d49f9-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="d49f9-256">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-256">no</span></span>             | <span data-ttu-id="d49f9-257">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-257">no</span></span>               |
| <span data-ttu-id="d49f9-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="d49f9-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="d49f9-259">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-259">no</span></span>             | <span data-ttu-id="d49f9-260">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-260">no</span></span>               |
| <span data-ttu-id="d49f9-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="d49f9-262">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-262">no</span></span>             | <span data-ttu-id="d49f9-263">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-263">no</span></span>               |
| <span data-ttu-id="d49f9-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="d49f9-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="d49f9-265">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-265">no</span></span>             | <span data-ttu-id="d49f9-266">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-266">no</span></span>               |
| <span data-ttu-id="d49f9-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="d49f9-267">msdyn_progress</span></span>                         | <span data-ttu-id="d49f9-268">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-268">no</span></span>             | <span data-ttu-id="d49f9-269">не (да за P4W)</span><span class="sxs-lookup"><span data-stu-id="d49f9-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="d49f9-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="d49f9-271">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-271">no</span></span>             | <span data-ttu-id="d49f9-272">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-272">no</span></span>               |
| <span data-ttu-id="d49f9-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="d49f9-274">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-274">no</span></span>             | <span data-ttu-id="d49f9-275">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-275">no</span></span>               |
| <span data-ttu-id="d49f9-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="d49f9-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="d49f9-277">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-277">no</span></span>             | <span data-ttu-id="d49f9-278">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-278">no</span></span>               |
| <span data-ttu-id="d49f9-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="d49f9-280">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-280">no</span></span>             | <span data-ttu-id="d49f9-281">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-281">no</span></span>               |
| <span data-ttu-id="d49f9-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="d49f9-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="d49f9-283">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-283">no</span></span>             | <span data-ttu-id="d49f9-284">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-284">no</span></span>               |
| <span data-ttu-id="d49f9-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="d49f9-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="d49f9-286">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-286">no</span></span>             | <span data-ttu-id="d49f9-287">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-287">no</span></span>               |
| <span data-ttu-id="d49f9-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="d49f9-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="d49f9-289">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-289">no</span></span>             | <span data-ttu-id="d49f9-290">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-290">no</span></span>               |
| <span data-ttu-id="d49f9-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="d49f9-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="d49f9-292">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-292">no</span></span>             | <span data-ttu-id="d49f9-293">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-293">no</span></span>               |
| <span data-ttu-id="d49f9-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="d49f9-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="d49f9-295">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-295">no</span></span>             | <span data-ttu-id="d49f9-296">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-296">no</span></span>               |
| <span data-ttu-id="d49f9-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="d49f9-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="d49f9-298">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-298">no</span></span>             | <span data-ttu-id="d49f9-299">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-299">no</span></span>               |
| <span data-ttu-id="d49f9-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="d49f9-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="d49f9-301">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-301">no</span></span>             | <span data-ttu-id="d49f9-302">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-302">no</span></span>               |
| <span data-ttu-id="d49f9-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="d49f9-304">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-304">no</span></span>             | <span data-ttu-id="d49f9-305">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-305">no</span></span>               |
| <span data-ttu-id="d49f9-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="d49f9-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="d49f9-307">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-307">no</span></span>             | <span data-ttu-id="d49f9-308">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-308">no</span></span>               |
| <span data-ttu-id="d49f9-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="d49f9-310">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-310">no</span></span>             | <span data-ttu-id="d49f9-311">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-311">no</span></span>               |
| <span data-ttu-id="d49f9-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="d49f9-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="d49f9-313">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-313">no</span></span>             | <span data-ttu-id="d49f9-314">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-314">no</span></span>               |
| <span data-ttu-id="d49f9-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="d49f9-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="d49f9-316">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-316">no</span></span>             | <span data-ttu-id="d49f9-317">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-317">no</span></span>               |
| <span data-ttu-id="d49f9-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="d49f9-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="d49f9-319">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-319">no</span></span>             | <span data-ttu-id="d49f9-320">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-320">no</span></span>               |
| <span data-ttu-id="d49f9-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="d49f9-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="d49f9-322">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-322">no</span></span>             | <span data-ttu-id="d49f9-323">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-323">no</span></span>               |
| <span data-ttu-id="d49f9-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="d49f9-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="d49f9-325">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-325">no</span></span>             | <span data-ttu-id="d49f9-326">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-326">no</span></span>               |
| <span data-ttu-id="d49f9-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="d49f9-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="d49f9-328">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-328">no</span></span>             | <span data-ttu-id="d49f9-329">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-329">no</span></span>               |
| <span data-ttu-id="d49f9-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="d49f9-330">msdyn_summary</span></span>                          | <span data-ttu-id="d49f9-331">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-331">no</span></span>             | <span data-ttu-id="d49f9-332">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-332">no</span></span>               |
| <span data-ttu-id="d49f9-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="d49f9-334">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-334">no</span></span>             | <span data-ttu-id="d49f9-335">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-335">no</span></span>               |
| <span data-ttu-id="d49f9-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="d49f9-337">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-337">no</span></span>             | <span data-ttu-id="d49f9-338">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="d49f9-339">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="d49f9-339">Project task dependency</span></span>

| <span data-ttu-id="d49f9-340">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="d49f9-340">**Logical name**</span></span>              | <span data-ttu-id="d49f9-341">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="d49f9-341">**Can create**</span></span> | <span data-ttu-id="d49f9-342">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="d49f9-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="d49f9-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="d49f9-343">msdyn_linktype</span></span>                | <span data-ttu-id="d49f9-344">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-344">no</span></span>             | <span data-ttu-id="d49f9-345">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-345">no</span></span>           |
| <span data-ttu-id="d49f9-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="d49f9-346">msdyn_linktypename</span></span>            | <span data-ttu-id="d49f9-347">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-347">no</span></span>             | <span data-ttu-id="d49f9-348">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-348">no</span></span>           |
| <span data-ttu-id="d49f9-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="d49f9-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="d49f9-350">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-350">yes</span></span>            | <span data-ttu-id="d49f9-351">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-351">no</span></span>           |
| <span data-ttu-id="d49f9-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="d49f9-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="d49f9-353">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-353">yes</span></span>            | <span data-ttu-id="d49f9-354">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-354">no</span></span>           |
| <span data-ttu-id="d49f9-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="d49f9-355">msdyn_project</span></span>                 | <span data-ttu-id="d49f9-356">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-356">yes</span></span>            | <span data-ttu-id="d49f9-357">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-357">no</span></span>           |
| <span data-ttu-id="d49f9-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="d49f9-358">msdyn_projectname</span></span>             | <span data-ttu-id="d49f9-359">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-359">yes</span></span>            | <span data-ttu-id="d49f9-360">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-360">no</span></span>           |
| <span data-ttu-id="d49f9-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="d49f9-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="d49f9-362">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-362">yes</span></span>            | <span data-ttu-id="d49f9-363">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-363">no</span></span>           |
| <span data-ttu-id="d49f9-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="d49f9-364">msdyn_successortask</span></span>           | <span data-ttu-id="d49f9-365">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-365">yes</span></span>            | <span data-ttu-id="d49f9-366">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-366">no</span></span>           |
| <span data-ttu-id="d49f9-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="d49f9-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="d49f9-368">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-368">yes</span></span>            | <span data-ttu-id="d49f9-369">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="d49f9-370">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="d49f9-370">Resource assignment</span></span>

| <span data-ttu-id="d49f9-371">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="d49f9-371">**Logical name**</span></span>             | <span data-ttu-id="d49f9-372">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="d49f9-372">**Can create**</span></span> | <span data-ttu-id="d49f9-373">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="d49f9-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="d49f9-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="d49f9-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="d49f9-375">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-375">yes</span></span>            | <span data-ttu-id="d49f9-376">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-376">no</span></span>           |
| <span data-ttu-id="d49f9-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="d49f9-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="d49f9-378">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-378">yes</span></span>            | <span data-ttu-id="d49f9-379">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-379">no</span></span>           |
| <span data-ttu-id="d49f9-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="d49f9-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="d49f9-381">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-381">no</span></span>             | <span data-ttu-id="d49f9-382">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-382">no</span></span>           |
| <span data-ttu-id="d49f9-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="d49f9-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="d49f9-384">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-384">no</span></span>             | <span data-ttu-id="d49f9-385">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-385">no</span></span>           |
| <span data-ttu-id="d49f9-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="d49f9-386">msdyn_committype</span></span>             | <span data-ttu-id="d49f9-387">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-387">no</span></span>             | <span data-ttu-id="d49f9-388">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-388">no</span></span>           |
| <span data-ttu-id="d49f9-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="d49f9-389">msdyn_committypename</span></span>         | <span data-ttu-id="d49f9-390">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-390">no</span></span>             | <span data-ttu-id="d49f9-391">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-391">no</span></span>           |
| <span data-ttu-id="d49f9-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="d49f9-392">msdyn_effort</span></span>                 | <span data-ttu-id="d49f9-393">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-393">no</span></span>             | <span data-ttu-id="d49f9-394">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-394">no</span></span>           |
| <span data-ttu-id="d49f9-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="d49f9-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="d49f9-396">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-396">no</span></span>             | <span data-ttu-id="d49f9-397">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-397">no</span></span>           |
| <span data-ttu-id="d49f9-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="d49f9-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="d49f9-399">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-399">no</span></span>             | <span data-ttu-id="d49f9-400">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-400">no</span></span>           |
| <span data-ttu-id="d49f9-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="d49f9-401">msdyn_finish</span></span>                 | <span data-ttu-id="d49f9-402">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-402">no</span></span>             | <span data-ttu-id="d49f9-403">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-403">no</span></span>           |
| <span data-ttu-id="d49f9-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="d49f9-405">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-405">no</span></span>             | <span data-ttu-id="d49f9-406">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-406">no</span></span>           |
| <span data-ttu-id="d49f9-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="d49f9-408">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-408">no</span></span>             | <span data-ttu-id="d49f9-409">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-409">no</span></span>           |
| <span data-ttu-id="d49f9-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="d49f9-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="d49f9-411">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-411">no</span></span>             | <span data-ttu-id="d49f9-412">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-412">no</span></span>           |
| <span data-ttu-id="d49f9-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="d49f9-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="d49f9-414">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-414">no</span></span>             | <span data-ttu-id="d49f9-415">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-415">no</span></span>           |
| <span data-ttu-id="d49f9-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="d49f9-417">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-417">no</span></span>             | <span data-ttu-id="d49f9-418">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-418">no</span></span>           |
| <span data-ttu-id="d49f9-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="d49f9-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="d49f9-420">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-420">no</span></span>             | <span data-ttu-id="d49f9-421">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-421">no</span></span>           |
| <span data-ttu-id="d49f9-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="d49f9-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="d49f9-423">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-423">no</span></span>             | <span data-ttu-id="d49f9-424">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-424">no</span></span>           |
| <span data-ttu-id="d49f9-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="d49f9-425">msdyn_projectid</span></span>              | <span data-ttu-id="d49f9-426">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-426">yes</span></span>            | <span data-ttu-id="d49f9-427">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-427">no</span></span>           |
| <span data-ttu-id="d49f9-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="d49f9-428">msdyn_projectidname</span></span>          | <span data-ttu-id="d49f9-429">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-429">no</span></span>             | <span data-ttu-id="d49f9-430">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-430">no</span></span>           |
| <span data-ttu-id="d49f9-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="d49f9-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="d49f9-432">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-432">no</span></span>             | <span data-ttu-id="d49f9-433">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-433">no</span></span>           |
| <span data-ttu-id="d49f9-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="d49f9-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="d49f9-435">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-435">no</span></span>             | <span data-ttu-id="d49f9-436">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-436">no</span></span>           |
| <span data-ttu-id="d49f9-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="d49f9-437">msdyn_start</span></span>                  | <span data-ttu-id="d49f9-438">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-438">no</span></span>             | <span data-ttu-id="d49f9-439">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-439">no</span></span>           |
| <span data-ttu-id="d49f9-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="d49f9-440">msdyn_taskid</span></span>                 | <span data-ttu-id="d49f9-441">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-441">no</span></span>             | <span data-ttu-id="d49f9-442">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-442">no</span></span>           |
| <span data-ttu-id="d49f9-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="d49f9-443">msdyn_taskidname</span></span>             | <span data-ttu-id="d49f9-444">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-444">no</span></span>             | <span data-ttu-id="d49f9-445">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-445">no</span></span>           |
| <span data-ttu-id="d49f9-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="d49f9-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="d49f9-447">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-447">no</span></span>             | <span data-ttu-id="d49f9-448">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="d49f9-449">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="d49f9-449">Project team member</span></span>

| <span data-ttu-id="d49f9-450">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="d49f9-450">**Logical name**</span></span>                                 | <span data-ttu-id="d49f9-451">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="d49f9-451">**Can create**</span></span> | <span data-ttu-id="d49f9-452">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="d49f9-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="d49f9-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="d49f9-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="d49f9-454">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-454">no</span></span>             | <span data-ttu-id="d49f9-455">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-455">no</span></span>           |
| <span data-ttu-id="d49f9-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="d49f9-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="d49f9-457">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-457">no</span></span>             | <span data-ttu-id="d49f9-458">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-458">no</span></span>           |
| <span data-ttu-id="d49f9-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="d49f9-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="d49f9-460">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-460">no</span></span>             | <span data-ttu-id="d49f9-461">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-461">no</span></span>           |
| <span data-ttu-id="d49f9-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="d49f9-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="d49f9-463">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-463">no</span></span>             | <span data-ttu-id="d49f9-464">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-464">no</span></span>           |
| <span data-ttu-id="d49f9-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="d49f9-465">msdyn_effort</span></span>                                     | <span data-ttu-id="d49f9-466">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-466">no</span></span>             | <span data-ttu-id="d49f9-467">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-467">no</span></span>           |
| <span data-ttu-id="d49f9-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="d49f9-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="d49f9-469">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-469">no</span></span>             | <span data-ttu-id="d49f9-470">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-470">no</span></span>           |
| <span data-ttu-id="d49f9-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="d49f9-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="d49f9-472">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-472">no</span></span>             | <span data-ttu-id="d49f9-473">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-473">no</span></span>           |
| <span data-ttu-id="d49f9-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="d49f9-474">msdyn_finish</span></span>                                     | <span data-ttu-id="d49f9-475">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-475">no</span></span>             | <span data-ttu-id="d49f9-476">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-476">no</span></span>           |
| <span data-ttu-id="d49f9-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="d49f9-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="d49f9-478">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-478">no</span></span>             | <span data-ttu-id="d49f9-479">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-479">no</span></span>           |
| <span data-ttu-id="d49f9-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="d49f9-480">msdyn_hours</span></span>                                      | <span data-ttu-id="d49f9-481">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-481">no</span></span>             | <span data-ttu-id="d49f9-482">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-482">no</span></span>           |
| <span data-ttu-id="d49f9-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="d49f9-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="d49f9-484">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-484">no</span></span>             | <span data-ttu-id="d49f9-485">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-485">no</span></span>           |
| <span data-ttu-id="d49f9-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="d49f9-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="d49f9-487">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-487">no</span></span>             | <span data-ttu-id="d49f9-488">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-488">no</span></span>           |
| <span data-ttu-id="d49f9-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="d49f9-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="d49f9-490">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-490">no</span></span>             | <span data-ttu-id="d49f9-491">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-491">no</span></span>           |
| <span data-ttu-id="d49f9-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="d49f9-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="d49f9-493">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-493">no</span></span>             | <span data-ttu-id="d49f9-494">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-494">no</span></span>           |
| <span data-ttu-id="d49f9-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="d49f9-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="d49f9-496">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-496">no</span></span>             | <span data-ttu-id="d49f9-497">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-497">no</span></span>           |
| <span data-ttu-id="d49f9-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="d49f9-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="d49f9-499">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-499">no</span></span>             | <span data-ttu-id="d49f9-500">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-500">no</span></span>           |
| <span data-ttu-id="d49f9-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="d49f9-501">msdyn_start</span></span>                                      | <span data-ttu-id="d49f9-502">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-502">no</span></span>             | <span data-ttu-id="d49f9-503">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="d49f9-504">Project</span><span class="sxs-lookup"><span data-stu-id="d49f9-504">Project</span></span>

| <span data-ttu-id="d49f9-505">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="d49f9-505">**Logical name**</span></span>                       | <span data-ttu-id="d49f9-506">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="d49f9-506">**Can create**</span></span> | <span data-ttu-id="d49f9-507">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="d49f9-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="d49f9-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="d49f9-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="d49f9-509">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-509">no</span></span>             | <span data-ttu-id="d49f9-510">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-510">no</span></span>           |
| <span data-ttu-id="d49f9-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="d49f9-512">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-512">no</span></span>             | <span data-ttu-id="d49f9-513">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-513">no</span></span>           |
| <span data-ttu-id="d49f9-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="d49f9-515">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-515">no</span></span>             | <span data-ttu-id="d49f9-516">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-516">no</span></span>           |
| <span data-ttu-id="d49f9-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="d49f9-518">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-518">no</span></span>             | <span data-ttu-id="d49f9-519">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-519">no</span></span>           |
| <span data-ttu-id="d49f9-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="d49f9-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="d49f9-521">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-521">no</span></span>             | <span data-ttu-id="d49f9-522">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-522">no</span></span>           |
| <span data-ttu-id="d49f9-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="d49f9-524">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-524">no</span></span>             | <span data-ttu-id="d49f9-525">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-525">no</span></span>           |
| <span data-ttu-id="d49f9-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="d49f9-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="d49f9-527">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-527">yes</span></span>            | <span data-ttu-id="d49f9-528">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-528">no</span></span>           |
| <span data-ttu-id="d49f9-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="d49f9-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="d49f9-530">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-530">yes</span></span>            | <span data-ttu-id="d49f9-531">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-531">no</span></span>           |
| <span data-ttu-id="d49f9-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="d49f9-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="d49f9-533">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-533">yes</span></span>            | <span data-ttu-id="d49f9-534">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-534">no</span></span>           |
| <span data-ttu-id="d49f9-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="d49f9-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="d49f9-536">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-536">no</span></span>             | <span data-ttu-id="d49f9-537">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-537">no</span></span>           |
| <span data-ttu-id="d49f9-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="d49f9-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="d49f9-539">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-539">no</span></span>             | <span data-ttu-id="d49f9-540">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-540">no</span></span>           |
| <span data-ttu-id="d49f9-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="d49f9-542">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-542">no</span></span>             | <span data-ttu-id="d49f9-543">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-543">no</span></span>           |
| <span data-ttu-id="d49f9-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="d49f9-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="d49f9-545">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-545">no</span></span>             | <span data-ttu-id="d49f9-546">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-546">no</span></span>           |
| <span data-ttu-id="d49f9-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="d49f9-548">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-548">no</span></span>             | <span data-ttu-id="d49f9-549">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-549">no</span></span>           |
| <span data-ttu-id="d49f9-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="d49f9-550">msdyn_duration</span></span>                         | <span data-ttu-id="d49f9-551">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-551">no</span></span>             | <span data-ttu-id="d49f9-552">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-552">no</span></span>           |
| <span data-ttu-id="d49f9-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="d49f9-553">msdyn_effort</span></span>                           | <span data-ttu-id="d49f9-554">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-554">no</span></span>             | <span data-ttu-id="d49f9-555">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-555">no</span></span>           |
| <span data-ttu-id="d49f9-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="d49f9-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="d49f9-557">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-557">no</span></span>             | <span data-ttu-id="d49f9-558">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-558">no</span></span>           |
| <span data-ttu-id="d49f9-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="d49f9-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="d49f9-560">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-560">no</span></span>             | <span data-ttu-id="d49f9-561">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-561">no</span></span>           |
| <span data-ttu-id="d49f9-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="d49f9-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="d49f9-563">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-563">no</span></span>             | <span data-ttu-id="d49f9-564">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-564">no</span></span>           |
| <span data-ttu-id="d49f9-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="d49f9-565">msdyn_finish</span></span>                           | <span data-ttu-id="d49f9-566">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-566">yes</span></span>            | <span data-ttu-id="d49f9-567">Да</span><span class="sxs-lookup"><span data-stu-id="d49f9-567">yes</span></span>          |
| <span data-ttu-id="d49f9-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="d49f9-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="d49f9-569">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-569">no</span></span>             | <span data-ttu-id="d49f9-570">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-570">no</span></span>           |
| <span data-ttu-id="d49f9-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="d49f9-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="d49f9-572">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-572">no</span></span>             | <span data-ttu-id="d49f9-573">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-573">no</span></span>           |
| <span data-ttu-id="d49f9-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="d49f9-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="d49f9-575">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-575">no</span></span>             | <span data-ttu-id="d49f9-576">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-576">no</span></span>           |
| <span data-ttu-id="d49f9-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="d49f9-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="d49f9-578">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-578">no</span></span>             | <span data-ttu-id="d49f9-579">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-579">no</span></span>           |
| <span data-ttu-id="d49f9-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="d49f9-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="d49f9-581">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-581">no</span></span>             | <span data-ttu-id="d49f9-582">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-582">no</span></span>           |
| <span data-ttu-id="d49f9-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="d49f9-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="d49f9-584">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-584">no</span></span>             | <span data-ttu-id="d49f9-585">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-585">no</span></span>           |
| <span data-ttu-id="d49f9-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="d49f9-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="d49f9-587">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-587">no</span></span>             | <span data-ttu-id="d49f9-588">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-588">no</span></span>           |
| <span data-ttu-id="d49f9-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="d49f9-590">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-590">no</span></span>             | <span data-ttu-id="d49f9-591">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-591">no</span></span>           |
| <span data-ttu-id="d49f9-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="d49f9-593">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-593">no</span></span>             | <span data-ttu-id="d49f9-594">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-594">no</span></span>           |
| <span data-ttu-id="d49f9-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="d49f9-596">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-596">no</span></span>             | <span data-ttu-id="d49f9-597">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-597">no</span></span>           |
| <span data-ttu-id="d49f9-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="d49f9-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="d49f9-599">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-599">no</span></span>             | <span data-ttu-id="d49f9-600">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-600">no</span></span>           |
| <span data-ttu-id="d49f9-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="d49f9-602">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-602">no</span></span>             | <span data-ttu-id="d49f9-603">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-603">no</span></span>           |
| <span data-ttu-id="d49f9-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="d49f9-604">msdyn_progress</span></span>                         | <span data-ttu-id="d49f9-605">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-605">no</span></span>             | <span data-ttu-id="d49f9-606">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-606">no</span></span>           |
| <span data-ttu-id="d49f9-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="d49f9-608">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-608">no</span></span>             | <span data-ttu-id="d49f9-609">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-609">no</span></span>           |
| <span data-ttu-id="d49f9-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="d49f9-611">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-611">no</span></span>             | <span data-ttu-id="d49f9-612">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-612">no</span></span>           |
| <span data-ttu-id="d49f9-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="d49f9-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="d49f9-614">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-614">no</span></span>             | <span data-ttu-id="d49f9-615">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-615">no</span></span>           |
| <span data-ttu-id="d49f9-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="d49f9-617">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-617">no</span></span>             | <span data-ttu-id="d49f9-618">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-618">no</span></span>           |
| <span data-ttu-id="d49f9-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="d49f9-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="d49f9-620">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-620">no</span></span>             | <span data-ttu-id="d49f9-621">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-621">no</span></span>           |
| <span data-ttu-id="d49f9-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="d49f9-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="d49f9-623">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-623">no</span></span>             | <span data-ttu-id="d49f9-624">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-624">no</span></span>           |
| <span data-ttu-id="d49f9-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="d49f9-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="d49f9-626">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-626">no</span></span>             | <span data-ttu-id="d49f9-627">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-627">no</span></span>           |
| <span data-ttu-id="d49f9-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="d49f9-629">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-629">no</span></span>             | <span data-ttu-id="d49f9-630">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-630">no</span></span>           |
| <span data-ttu-id="d49f9-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="d49f9-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="d49f9-632">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-632">no</span></span>             | <span data-ttu-id="d49f9-633">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-633">no</span></span>           |
| <span data-ttu-id="d49f9-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="d49f9-635">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-635">no</span></span>             | <span data-ttu-id="d49f9-636">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-636">no</span></span>           |
| <span data-ttu-id="d49f9-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="d49f9-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="d49f9-638">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-638">no</span></span>             | <span data-ttu-id="d49f9-639">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-639">no</span></span>           |
| <span data-ttu-id="d49f9-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="d49f9-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="d49f9-641">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-641">no</span></span>             | <span data-ttu-id="d49f9-642">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-642">no</span></span>           |
| <span data-ttu-id="d49f9-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="d49f9-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="d49f9-644">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-644">no</span></span>             | <span data-ttu-id="d49f9-645">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-645">no</span></span>           |
| <span data-ttu-id="d49f9-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="d49f9-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="d49f9-647">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-647">no</span></span>             | <span data-ttu-id="d49f9-648">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-648">no</span></span>           |
| <span data-ttu-id="d49f9-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="d49f9-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="d49f9-650">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-650">no</span></span>             | <span data-ttu-id="d49f9-651">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-651">no</span></span>           |
| <span data-ttu-id="d49f9-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="d49f9-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="d49f9-653">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-653">no</span></span>             | <span data-ttu-id="d49f9-654">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-654">no</span></span>           |
| <span data-ttu-id="d49f9-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="d49f9-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="d49f9-656">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-656">no</span></span>             | <span data-ttu-id="d49f9-657">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-657">no</span></span>           |
| <span data-ttu-id="d49f9-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="d49f9-659">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-659">no</span></span>             | <span data-ttu-id="d49f9-660">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-660">no</span></span>           |
| <span data-ttu-id="d49f9-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="d49f9-662">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-662">no</span></span>             | <span data-ttu-id="d49f9-663">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-663">no</span></span>           |
| <span data-ttu-id="d49f9-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="d49f9-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="d49f9-665">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-665">no</span></span>             | <span data-ttu-id="d49f9-666">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-666">no</span></span>           |
| <span data-ttu-id="d49f9-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="d49f9-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="d49f9-668">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-668">no</span></span>             | <span data-ttu-id="d49f9-669">не</span><span class="sxs-lookup"><span data-stu-id="d49f9-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="d49f9-670">Ограничења и познати проблеми</span><span class="sxs-lookup"><span data-stu-id="d49f9-670">Limitations and known issues</span></span>
<span data-ttu-id="d49f9-671">Следи листа ограничења и познатих проблема:</span><span class="sxs-lookup"><span data-stu-id="d49f9-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="d49f9-672">API-је за распоред могу да користе само **корисници са лиценцом за Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="d49f9-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="d49f9-673">Не могу их користити:</span><span class="sxs-lookup"><span data-stu-id="d49f9-673">They can't be used by:</span></span>
    - <span data-ttu-id="d49f9-674">Корисници апликације</span><span class="sxs-lookup"><span data-stu-id="d49f9-674">Application users</span></span>
    - <span data-ttu-id="d49f9-675">Корисници система</span><span class="sxs-lookup"><span data-stu-id="d49f9-675">System users</span></span>
    - <span data-ttu-id="d49f9-676">Корисници интеграције</span><span class="sxs-lookup"><span data-stu-id="d49f9-676">Integration users</span></span>
    - <span data-ttu-id="d49f9-677">Остали корисници који немају потребну лиценцу</span><span class="sxs-lookup"><span data-stu-id="d49f9-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="d49f9-678">Сваки **OperationSet ентитет** може да има највише 100 операција.</span><span class="sxs-lookup"><span data-stu-id="d49f9-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="d49f9-679">Сваки корисник може да има највише 10 отворених **OperationSet ентитета**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="d49f9-680">Project Operations тренутно подржава максимално 500 укупних задатака на пројекту.</span><span class="sxs-lookup"><span data-stu-id="d49f9-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="d49f9-681">Статус грешке и евиденције грешака **OperationSet ентитета** тренутно нису доступне.</span><span class="sxs-lookup"><span data-stu-id="d49f9-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="d49f9-682">Ограничења и границе пројеката и задатака</span><span class="sxs-lookup"><span data-stu-id="d49f9-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="d49f9-683">Руковање грешкама</span><span class="sxs-lookup"><span data-stu-id="d49f9-683">Error handling</span></span>

   - <span data-ttu-id="d49f9-684">Да бисте прегледали грешке генерисане из скупова операција, идите на **Подешавања** \> **Закажи интеграцију** \> **Скупови операција**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="d49f9-685">Да бисте прегледали грешке генерисане услугом планирања пројеката, идите на **Подешавања** \> **Закажи интеграцију** \> **Дневници грешака PSS-а**.</span><span class="sxs-lookup"><span data-stu-id="d49f9-685">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="d49f9-686">Пример сценарија</span><span class="sxs-lookup"><span data-stu-id="d49f9-686">Sample scenario</span></span>

<span data-ttu-id="d49f9-687">У овом сценарију, креираћете пројекат, члана тима, четири задатка и два задатка ресурса.</span><span class="sxs-lookup"><span data-stu-id="d49f9-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="d49f9-688">Затим ћете ажурирати један задатак, ажурирати пројекат, избрисати један задатак, избрисати једну доделу ресурса и креирати зависност задатка.</span><span class="sxs-lookup"><span data-stu-id="d49f9-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="d49f9-689">Додатни примери</span><span class="sxs-lookup"><span data-stu-id="d49f9-689">Additional samples</span></span>

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
