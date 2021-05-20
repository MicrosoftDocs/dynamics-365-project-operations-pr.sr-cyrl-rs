---
title: Коришћење API-ја за распоред за обављање операција са ентитетима планирања
description: Ова тема пружа информације и примере за коришћење API-ја за распоред.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950822"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="ad5d6-103">Коришћење API-ја за распоред за обављање операција са ентитетима планирања</span><span class="sxs-lookup"><span data-stu-id="ad5d6-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="ad5d6-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="ad5d6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="ad5d6-105">Неке или све функционалности забележене у овој теми доступне су као део издања верзије за преглед.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="ad5d6-106">Садржај и функционалност су подложни променама.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="ad5d6-107">Ентитети планирања</span><span class="sxs-lookup"><span data-stu-id="ad5d6-107">Scheduling entities</span></span>

<span data-ttu-id="ad5d6-108">API-ји за распоред пружају могућност извршавања операција креирања, ажурирања и брисања помоћу **ентитета планирања**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="ad5d6-109">Тим ентитетима се управља путем механизма за распоређивање у апликацији Project за веб.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="ad5d6-110">Креирање, ажурирање и брисање операција помоћу **ентитета планирања** били су ограничени у ранијим издањима услуге Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="ad5d6-111">Следећа табела даје потпуну листу **ентитета планирања**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="ad5d6-112">Назив ентитета</span><span class="sxs-lookup"><span data-stu-id="ad5d6-112">Entity name</span></span>  | <span data-ttu-id="ad5d6-113">Логичко име ентитета</span><span class="sxs-lookup"><span data-stu-id="ad5d6-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="ad5d6-114">Project</span><span class="sxs-lookup"><span data-stu-id="ad5d6-114">Project</span></span> | <span data-ttu-id="ad5d6-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="ad5d6-115">msdyn_project</span></span> |
| <span data-ttu-id="ad5d6-116">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="ad5d6-116">Project Task</span></span>  | <span data-ttu-id="ad5d6-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="ad5d6-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="ad5d6-118">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="ad5d6-118">Project Task Dependency</span></span>  | <span data-ttu-id="ad5d6-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="ad5d6-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="ad5d6-120">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="ad5d6-120">Resource Assignment</span></span> | <span data-ttu-id="ad5d6-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="ad5d6-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="ad5d6-122">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="ad5d6-122">Project Bucket</span></span>  | <span data-ttu-id="ad5d6-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="ad5d6-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="ad5d6-124">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="ad5d6-124">Project Team Member</span></span> | <span data-ttu-id="ad5d6-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="ad5d6-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="ad5d6-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="ad5d6-126">OperationSet</span></span>

<span data-ttu-id="ad5d6-127">Ентитет OperationSet је образац јединице рада који се може користити када се у трансакцији мора обрадити неколико захтева који утичу на распоред.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="ad5d6-128">API-ји за распоред</span><span class="sxs-lookup"><span data-stu-id="ad5d6-128">Schedule APIs</span></span>

<span data-ttu-id="ad5d6-129">Следи листа актуелних API-ја за распоред.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="ad5d6-130">**msdyn_CreateProjectV1**: Овај API се може користити за креирање пројекта.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="ad5d6-131">Пројекат и подразумевани контејнер пројекта креирају се одмах.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="ad5d6-132">**msdyn_CreateTeamMemberV1**: Овај API се може користити за креирање члана пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="ad5d6-133">Евиденција члана тима креира се одмах.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="ad5d6-134">**msdyn_CreateOperationSetV1**: Овај API се може користити за заказивање неколико захтева који се морају извршити у оквиру трансакције.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="ad5d6-135">**msdyn_PSSCreateV1**: Овај API се може користити за креирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="ad5d6-136">Ентитет може бити било који ентитет планирања који подржава операцију креирања.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="ad5d6-137">**msdyn_PSSUpdateV1**: Овај API се може користити за ажурирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="ad5d6-138">Ентитет може бити било који ентитет планирања који подржава операцију ажурирања.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="ad5d6-139">**msdyn_PSSDeleteV1**: Овај API се може користити за брисање ентитета.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="ad5d6-140">Ентитет може бити било који ентитет планирања који подржава операцију брисања.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="ad5d6-141">**msdyn_ExecuteOperationSetV1**: Овај API се користи за извршавање свих операција унутар датог скупа операција.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="ad5d6-142">Коришћење API-ја распореда са OperationSet ентитетом</span><span class="sxs-lookup"><span data-stu-id="ad5d6-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="ad5d6-143">Пошто се записи са **CreateProjectV1** и **CreateTeamMemberV1** креирају одмах, ови API-ји се не могу користити у **OperationSet ентитету** директно.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="ad5d6-144">Међутим, API можете користити за креирање потребних записа, креирајте **OperationSet ентитет**, а затим користите ове унапред креиране записе у **OperationSet ентитету**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="ad5d6-145">Подржане операције</span><span class="sxs-lookup"><span data-stu-id="ad5d6-145">Supported operations</span></span>

| <span data-ttu-id="ad5d6-146">Ентитет планирања</span><span class="sxs-lookup"><span data-stu-id="ad5d6-146">Scheduling entity</span></span> | <span data-ttu-id="ad5d6-147">Направи</span><span class="sxs-lookup"><span data-stu-id="ad5d6-147">Create</span></span> | <span data-ttu-id="ad5d6-148">Ажурирање</span><span class="sxs-lookup"><span data-stu-id="ad5d6-148">Update</span></span> | <span data-ttu-id="ad5d6-149">Delete</span><span class="sxs-lookup"><span data-stu-id="ad5d6-149">Delete</span></span> | <span data-ttu-id="ad5d6-150">Важна разматрања</span><span class="sxs-lookup"><span data-stu-id="ad5d6-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="ad5d6-151">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="ad5d6-151">Project task</span></span> | <span data-ttu-id="ad5d6-152">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-152">Yes</span></span> | <span data-ttu-id="ad5d6-153">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-153">Yes</span></span> | <span data-ttu-id="ad5d6-154">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-154">Yes</span></span> | <span data-ttu-id="ad5d6-155">Ниједно</span><span class="sxs-lookup"><span data-stu-id="ad5d6-155">None</span></span> |
| <span data-ttu-id="ad5d6-156">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="ad5d6-156">Project task dependency</span></span> | <span data-ttu-id="ad5d6-157">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-157">Yes</span></span> | <span data-ttu-id="ad5d6-158">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-158">Yes</span></span> | | <span data-ttu-id="ad5d6-159">Записи зависности пројектних задатака се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="ad5d6-160">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="ad5d6-161">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="ad5d6-161">Resource assignment</span></span> | <span data-ttu-id="ad5d6-162">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-162">Yes</span></span> | <span data-ttu-id="ad5d6-163">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-163">Yes</span></span> | | <span data-ttu-id="ad5d6-164">Нису подржане операције са следећим пољима: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="ad5d6-165">Записи о додели ресурса се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="ad5d6-166">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="ad5d6-167">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="ad5d6-167">Project bucket</span></span> | <span data-ttu-id="ad5d6-168">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="ad5d6-168">N/A</span></span> | <span data-ttu-id="ad5d6-169">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="ad5d6-169">N/A</span></span> | <span data-ttu-id="ad5d6-170">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="ad5d6-170">N/A</span></span> | <span data-ttu-id="ad5d6-171">Подразумевани контејнер се креира се помоћу API-ја **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="ad5d6-172">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="ad5d6-172">Project team member</span></span> | <span data-ttu-id="ad5d6-173">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-173">Yes</span></span> | <span data-ttu-id="ad5d6-174">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-174">Yes</span></span> | <span data-ttu-id="ad5d6-175">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-175">Yes</span></span> | <span data-ttu-id="ad5d6-176">За операцију креирања користите API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="ad5d6-177">Project</span><span class="sxs-lookup"><span data-stu-id="ad5d6-177">Project</span></span> | <span data-ttu-id="ad5d6-178">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-178">Yes</span></span> | <span data-ttu-id="ad5d6-179">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-179">Yes</span></span> | <span data-ttu-id="ad5d6-180">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="ad5d6-180">N/A</span></span> | <span data-ttu-id="ad5d6-181">Нису подржане операције са следећим пољима: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="ad5d6-182">Ови API-ји се могу позивати са објектима ентитета који укључују прилагођена поља.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="ad5d6-183">Својство ID је опционално.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-183">The ID property is optional.</span></span> <span data-ttu-id="ad5d6-184">Ако је обезбеђено, систем покушава да га користи и избацује изузетак ако не може да га користи.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="ad5d6-185">Ако није обезбеђено, систем ће га генерисати.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="ad5d6-186">Ограничена поља</span><span class="sxs-lookup"><span data-stu-id="ad5d6-186">Restricted fields</span></span>

<span data-ttu-id="ad5d6-187">Следеће табеле дефинишу поља за која је ограничено **Креирај** и **Уреди.**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="ad5d6-188">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="ad5d6-188">Project task</span></span>

| <span data-ttu-id="ad5d6-189">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-189">**Logical name**</span></span>                       | <span data-ttu-id="ad5d6-190">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-190">**Can create**</span></span> | <span data-ttu-id="ad5d6-191">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="ad5d6-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="ad5d6-193">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-193">no</span></span>             | <span data-ttu-id="ad5d6-194">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-194">no</span></span>               |
| <span data-ttu-id="ad5d6-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="ad5d6-196">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-196">no</span></span>             | <span data-ttu-id="ad5d6-197">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-197">no</span></span>               |
| <span data-ttu-id="ad5d6-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="ad5d6-198">msdyn_actualend</span></span>                        | <span data-ttu-id="ad5d6-199">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-199">no</span></span>             | <span data-ttu-id="ad5d6-200">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-200">no</span></span>               |
| <span data-ttu-id="ad5d6-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="ad5d6-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="ad5d6-202">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-202">no</span></span>             | <span data-ttu-id="ad5d6-203">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-203">no</span></span>               |
| <span data-ttu-id="ad5d6-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="ad5d6-205">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-205">no</span></span>             | <span data-ttu-id="ad5d6-206">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-206">no</span></span>               |
| <span data-ttu-id="ad5d6-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="ad5d6-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="ad5d6-208">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-208">no</span></span>             | <span data-ttu-id="ad5d6-209">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-209">no</span></span>               |
| <span data-ttu-id="ad5d6-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="ad5d6-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="ad5d6-211">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-211">no</span></span>             | <span data-ttu-id="ad5d6-212">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-212">no</span></span>               |
| <span data-ttu-id="ad5d6-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="ad5d6-214">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-214">no</span></span>             | <span data-ttu-id="ad5d6-215">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-215">no</span></span>               |
| <span data-ttu-id="ad5d6-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="ad5d6-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="ad5d6-217">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-217">no</span></span>             | <span data-ttu-id="ad5d6-218">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-218">no</span></span>               |
| <span data-ttu-id="ad5d6-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ad5d6-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="ad5d6-220">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-220">no</span></span>             | <span data-ttu-id="ad5d6-221">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-221">no</span></span>               |
| <span data-ttu-id="ad5d6-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="ad5d6-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="ad5d6-223">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-223">no</span></span>             | <span data-ttu-id="ad5d6-224">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-224">no</span></span>               |
| <span data-ttu-id="ad5d6-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="ad5d6-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="ad5d6-226">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-226">no</span></span>             | <span data-ttu-id="ad5d6-227">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-227">no</span></span>               |
| <span data-ttu-id="ad5d6-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="ad5d6-229">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-229">no</span></span>             | <span data-ttu-id="ad5d6-230">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-230">no</span></span>               |
| <span data-ttu-id="ad5d6-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="ad5d6-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="ad5d6-232">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-232">no</span></span>             | <span data-ttu-id="ad5d6-233">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-233">no</span></span>               |
| <span data-ttu-id="ad5d6-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="ad5d6-235">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-235">no</span></span>             | <span data-ttu-id="ad5d6-236">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-236">no</span></span>               |
| <span data-ttu-id="ad5d6-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="ad5d6-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="ad5d6-238">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-238">no</span></span>             | <span data-ttu-id="ad5d6-239">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-239">no</span></span>               |
| <span data-ttu-id="ad5d6-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="ad5d6-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="ad5d6-241">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-241">no</span></span>             | <span data-ttu-id="ad5d6-242">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-242">no</span></span>               |
| <span data-ttu-id="ad5d6-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="ad5d6-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="ad5d6-244">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-244">no</span></span>             | <span data-ttu-id="ad5d6-245">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-245">no</span></span>               |
| <span data-ttu-id="ad5d6-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="ad5d6-247">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-247">no</span></span>             | <span data-ttu-id="ad5d6-248">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-248">no</span></span>               |
| <span data-ttu-id="ad5d6-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="ad5d6-250">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-250">no</span></span>             | <span data-ttu-id="ad5d6-251">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-251">no</span></span>               |
| <span data-ttu-id="ad5d6-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="ad5d6-253">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-253">no</span></span>             | <span data-ttu-id="ad5d6-254">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-254">no</span></span>               |
| <span data-ttu-id="ad5d6-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="ad5d6-256">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-256">no</span></span>             | <span data-ttu-id="ad5d6-257">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-257">no</span></span>               |
| <span data-ttu-id="ad5d6-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="ad5d6-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="ad5d6-259">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-259">no</span></span>             | <span data-ttu-id="ad5d6-260">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-260">no</span></span>               |
| <span data-ttu-id="ad5d6-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="ad5d6-262">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-262">no</span></span>             | <span data-ttu-id="ad5d6-263">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-263">no</span></span>               |
| <span data-ttu-id="ad5d6-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="ad5d6-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="ad5d6-265">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-265">no</span></span>             | <span data-ttu-id="ad5d6-266">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-266">no</span></span>               |
| <span data-ttu-id="ad5d6-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="ad5d6-267">msdyn_progress</span></span>                         | <span data-ttu-id="ad5d6-268">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-268">no</span></span>             | <span data-ttu-id="ad5d6-269">не (да за P4W)</span><span class="sxs-lookup"><span data-stu-id="ad5d6-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="ad5d6-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="ad5d6-271">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-271">no</span></span>             | <span data-ttu-id="ad5d6-272">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-272">no</span></span>               |
| <span data-ttu-id="ad5d6-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="ad5d6-274">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-274">no</span></span>             | <span data-ttu-id="ad5d6-275">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-275">no</span></span>               |
| <span data-ttu-id="ad5d6-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="ad5d6-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="ad5d6-277">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-277">no</span></span>             | <span data-ttu-id="ad5d6-278">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-278">no</span></span>               |
| <span data-ttu-id="ad5d6-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="ad5d6-280">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-280">no</span></span>             | <span data-ttu-id="ad5d6-281">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-281">no</span></span>               |
| <span data-ttu-id="ad5d6-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="ad5d6-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="ad5d6-283">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-283">no</span></span>             | <span data-ttu-id="ad5d6-284">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-284">no</span></span>               |
| <span data-ttu-id="ad5d6-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="ad5d6-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="ad5d6-286">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-286">no</span></span>             | <span data-ttu-id="ad5d6-287">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-287">no</span></span>               |
| <span data-ttu-id="ad5d6-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="ad5d6-289">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-289">no</span></span>             | <span data-ttu-id="ad5d6-290">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-290">no</span></span>               |
| <span data-ttu-id="ad5d6-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="ad5d6-292">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-292">no</span></span>             | <span data-ttu-id="ad5d6-293">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-293">no</span></span>               |
| <span data-ttu-id="ad5d6-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="ad5d6-295">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-295">no</span></span>             | <span data-ttu-id="ad5d6-296">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-296">no</span></span>               |
| <span data-ttu-id="ad5d6-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="ad5d6-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="ad5d6-298">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-298">no</span></span>             | <span data-ttu-id="ad5d6-299">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-299">no</span></span>               |
| <span data-ttu-id="ad5d6-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="ad5d6-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="ad5d6-301">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-301">no</span></span>             | <span data-ttu-id="ad5d6-302">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-302">no</span></span>               |
| <span data-ttu-id="ad5d6-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="ad5d6-304">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-304">no</span></span>             | <span data-ttu-id="ad5d6-305">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-305">no</span></span>               |
| <span data-ttu-id="ad5d6-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="ad5d6-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="ad5d6-307">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-307">no</span></span>             | <span data-ttu-id="ad5d6-308">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-308">no</span></span>               |
| <span data-ttu-id="ad5d6-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="ad5d6-310">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-310">no</span></span>             | <span data-ttu-id="ad5d6-311">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-311">no</span></span>               |
| <span data-ttu-id="ad5d6-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="ad5d6-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="ad5d6-313">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-313">no</span></span>             | <span data-ttu-id="ad5d6-314">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-314">no</span></span>               |
| <span data-ttu-id="ad5d6-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="ad5d6-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="ad5d6-316">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-316">no</span></span>             | <span data-ttu-id="ad5d6-317">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-317">no</span></span>               |
| <span data-ttu-id="ad5d6-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="ad5d6-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="ad5d6-319">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-319">no</span></span>             | <span data-ttu-id="ad5d6-320">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-320">no</span></span>               |
| <span data-ttu-id="ad5d6-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="ad5d6-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="ad5d6-322">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-322">no</span></span>             | <span data-ttu-id="ad5d6-323">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-323">no</span></span>               |
| <span data-ttu-id="ad5d6-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="ad5d6-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="ad5d6-325">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-325">no</span></span>             | <span data-ttu-id="ad5d6-326">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-326">no</span></span>               |
| <span data-ttu-id="ad5d6-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="ad5d6-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="ad5d6-328">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-328">no</span></span>             | <span data-ttu-id="ad5d6-329">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-329">no</span></span>               |
| <span data-ttu-id="ad5d6-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="ad5d6-330">msdyn_summary</span></span>                          | <span data-ttu-id="ad5d6-331">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-331">no</span></span>             | <span data-ttu-id="ad5d6-332">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-332">no</span></span>               |
| <span data-ttu-id="ad5d6-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="ad5d6-334">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-334">no</span></span>             | <span data-ttu-id="ad5d6-335">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-335">no</span></span>               |
| <span data-ttu-id="ad5d6-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="ad5d6-337">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-337">no</span></span>             | <span data-ttu-id="ad5d6-338">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="ad5d6-339">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="ad5d6-339">Project task dependency</span></span>

| <span data-ttu-id="ad5d6-340">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-340">**Logical name**</span></span>              | <span data-ttu-id="ad5d6-341">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-341">**Can create**</span></span> | <span data-ttu-id="ad5d6-342">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="ad5d6-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="ad5d6-343">msdyn_linktype</span></span>                | <span data-ttu-id="ad5d6-344">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-344">no</span></span>             | <span data-ttu-id="ad5d6-345">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-345">no</span></span>           |
| <span data-ttu-id="ad5d6-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="ad5d6-346">msdyn_linktypename</span></span>            | <span data-ttu-id="ad5d6-347">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-347">no</span></span>             | <span data-ttu-id="ad5d6-348">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-348">no</span></span>           |
| <span data-ttu-id="ad5d6-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="ad5d6-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="ad5d6-350">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-350">yes</span></span>            | <span data-ttu-id="ad5d6-351">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-351">no</span></span>           |
| <span data-ttu-id="ad5d6-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="ad5d6-353">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-353">yes</span></span>            | <span data-ttu-id="ad5d6-354">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-354">no</span></span>           |
| <span data-ttu-id="ad5d6-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="ad5d6-355">msdyn_project</span></span>                 | <span data-ttu-id="ad5d6-356">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-356">yes</span></span>            | <span data-ttu-id="ad5d6-357">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-357">no</span></span>           |
| <span data-ttu-id="ad5d6-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-358">msdyn_projectname</span></span>             | <span data-ttu-id="ad5d6-359">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-359">yes</span></span>            | <span data-ttu-id="ad5d6-360">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-360">no</span></span>           |
| <span data-ttu-id="ad5d6-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="ad5d6-362">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-362">yes</span></span>            | <span data-ttu-id="ad5d6-363">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-363">no</span></span>           |
| <span data-ttu-id="ad5d6-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="ad5d6-364">msdyn_successortask</span></span>           | <span data-ttu-id="ad5d6-365">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-365">yes</span></span>            | <span data-ttu-id="ad5d6-366">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-366">no</span></span>           |
| <span data-ttu-id="ad5d6-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="ad5d6-368">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-368">yes</span></span>            | <span data-ttu-id="ad5d6-369">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="ad5d6-370">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="ad5d6-370">Resource assignment</span></span>

| <span data-ttu-id="ad5d6-371">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-371">**Logical name**</span></span>             | <span data-ttu-id="ad5d6-372">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-372">**Can create**</span></span> | <span data-ttu-id="ad5d6-373">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="ad5d6-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="ad5d6-375">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-375">yes</span></span>            | <span data-ttu-id="ad5d6-376">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-376">no</span></span>           |
| <span data-ttu-id="ad5d6-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="ad5d6-378">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-378">yes</span></span>            | <span data-ttu-id="ad5d6-379">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-379">no</span></span>           |
| <span data-ttu-id="ad5d6-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="ad5d6-381">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-381">no</span></span>             | <span data-ttu-id="ad5d6-382">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-382">no</span></span>           |
| <span data-ttu-id="ad5d6-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="ad5d6-384">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-384">no</span></span>             | <span data-ttu-id="ad5d6-385">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-385">no</span></span>           |
| <span data-ttu-id="ad5d6-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="ad5d6-386">msdyn_committype</span></span>             | <span data-ttu-id="ad5d6-387">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-387">no</span></span>             | <span data-ttu-id="ad5d6-388">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-388">no</span></span>           |
| <span data-ttu-id="ad5d6-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="ad5d6-389">msdyn_committypename</span></span>         | <span data-ttu-id="ad5d6-390">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-390">no</span></span>             | <span data-ttu-id="ad5d6-391">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-391">no</span></span>           |
| <span data-ttu-id="ad5d6-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="ad5d6-392">msdyn_effort</span></span>                 | <span data-ttu-id="ad5d6-393">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-393">no</span></span>             | <span data-ttu-id="ad5d6-394">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-394">no</span></span>           |
| <span data-ttu-id="ad5d6-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ad5d6-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="ad5d6-396">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-396">no</span></span>             | <span data-ttu-id="ad5d6-397">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-397">no</span></span>           |
| <span data-ttu-id="ad5d6-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="ad5d6-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="ad5d6-399">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-399">no</span></span>             | <span data-ttu-id="ad5d6-400">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-400">no</span></span>           |
| <span data-ttu-id="ad5d6-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="ad5d6-401">msdyn_finish</span></span>                 | <span data-ttu-id="ad5d6-402">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-402">no</span></span>             | <span data-ttu-id="ad5d6-403">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-403">no</span></span>           |
| <span data-ttu-id="ad5d6-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="ad5d6-405">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-405">no</span></span>             | <span data-ttu-id="ad5d6-406">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-406">no</span></span>           |
| <span data-ttu-id="ad5d6-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="ad5d6-408">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-408">no</span></span>             | <span data-ttu-id="ad5d6-409">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-409">no</span></span>           |
| <span data-ttu-id="ad5d6-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="ad5d6-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="ad5d6-411">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-411">no</span></span>             | <span data-ttu-id="ad5d6-412">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-412">no</span></span>           |
| <span data-ttu-id="ad5d6-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="ad5d6-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="ad5d6-414">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-414">no</span></span>             | <span data-ttu-id="ad5d6-415">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-415">no</span></span>           |
| <span data-ttu-id="ad5d6-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="ad5d6-417">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-417">no</span></span>             | <span data-ttu-id="ad5d6-418">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-418">no</span></span>           |
| <span data-ttu-id="ad5d6-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="ad5d6-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="ad5d6-420">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-420">no</span></span>             | <span data-ttu-id="ad5d6-421">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-421">no</span></span>           |
| <span data-ttu-id="ad5d6-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="ad5d6-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="ad5d6-423">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-423">no</span></span>             | <span data-ttu-id="ad5d6-424">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-424">no</span></span>           |
| <span data-ttu-id="ad5d6-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-425">msdyn_projectid</span></span>              | <span data-ttu-id="ad5d6-426">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-426">yes</span></span>            | <span data-ttu-id="ad5d6-427">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-427">no</span></span>           |
| <span data-ttu-id="ad5d6-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-428">msdyn_projectidname</span></span>          | <span data-ttu-id="ad5d6-429">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-429">no</span></span>             | <span data-ttu-id="ad5d6-430">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-430">no</span></span>           |
| <span data-ttu-id="ad5d6-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="ad5d6-432">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-432">no</span></span>             | <span data-ttu-id="ad5d6-433">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-433">no</span></span>           |
| <span data-ttu-id="ad5d6-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="ad5d6-435">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-435">no</span></span>             | <span data-ttu-id="ad5d6-436">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-436">no</span></span>           |
| <span data-ttu-id="ad5d6-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="ad5d6-437">msdyn_start</span></span>                  | <span data-ttu-id="ad5d6-438">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-438">no</span></span>             | <span data-ttu-id="ad5d6-439">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-439">no</span></span>           |
| <span data-ttu-id="ad5d6-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-440">msdyn_taskid</span></span>                 | <span data-ttu-id="ad5d6-441">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-441">no</span></span>             | <span data-ttu-id="ad5d6-442">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-442">no</span></span>           |
| <span data-ttu-id="ad5d6-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-443">msdyn_taskidname</span></span>             | <span data-ttu-id="ad5d6-444">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-444">no</span></span>             | <span data-ttu-id="ad5d6-445">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-445">no</span></span>           |
| <span data-ttu-id="ad5d6-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="ad5d6-447">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-447">no</span></span>             | <span data-ttu-id="ad5d6-448">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="ad5d6-449">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="ad5d6-449">Project team member</span></span>

| <span data-ttu-id="ad5d6-450">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-450">**Logical name**</span></span>                                 | <span data-ttu-id="ad5d6-451">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-451">**Can create**</span></span> | <span data-ttu-id="ad5d6-452">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="ad5d6-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="ad5d6-454">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-454">no</span></span>             | <span data-ttu-id="ad5d6-455">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-455">no</span></span>           |
| <span data-ttu-id="ad5d6-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="ad5d6-457">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-457">no</span></span>             | <span data-ttu-id="ad5d6-458">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-458">no</span></span>           |
| <span data-ttu-id="ad5d6-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="ad5d6-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="ad5d6-460">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-460">no</span></span>             | <span data-ttu-id="ad5d6-461">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-461">no</span></span>           |
| <span data-ttu-id="ad5d6-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="ad5d6-463">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-463">no</span></span>             | <span data-ttu-id="ad5d6-464">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-464">no</span></span>           |
| <span data-ttu-id="ad5d6-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="ad5d6-465">msdyn_effort</span></span>                                     | <span data-ttu-id="ad5d6-466">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-466">no</span></span>             | <span data-ttu-id="ad5d6-467">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-467">no</span></span>           |
| <span data-ttu-id="ad5d6-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ad5d6-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="ad5d6-469">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-469">no</span></span>             | <span data-ttu-id="ad5d6-470">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-470">no</span></span>           |
| <span data-ttu-id="ad5d6-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="ad5d6-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="ad5d6-472">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-472">no</span></span>             | <span data-ttu-id="ad5d6-473">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-473">no</span></span>           |
| <span data-ttu-id="ad5d6-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="ad5d6-474">msdyn_finish</span></span>                                     | <span data-ttu-id="ad5d6-475">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-475">no</span></span>             | <span data-ttu-id="ad5d6-476">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-476">no</span></span>           |
| <span data-ttu-id="ad5d6-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="ad5d6-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="ad5d6-478">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-478">no</span></span>             | <span data-ttu-id="ad5d6-479">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-479">no</span></span>           |
| <span data-ttu-id="ad5d6-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="ad5d6-480">msdyn_hours</span></span>                                      | <span data-ttu-id="ad5d6-481">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-481">no</span></span>             | <span data-ttu-id="ad5d6-482">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-482">no</span></span>           |
| <span data-ttu-id="ad5d6-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="ad5d6-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="ad5d6-484">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-484">no</span></span>             | <span data-ttu-id="ad5d6-485">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-485">no</span></span>           |
| <span data-ttu-id="ad5d6-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="ad5d6-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="ad5d6-487">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-487">no</span></span>             | <span data-ttu-id="ad5d6-488">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-488">no</span></span>           |
| <span data-ttu-id="ad5d6-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="ad5d6-490">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-490">no</span></span>             | <span data-ttu-id="ad5d6-491">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-491">no</span></span>           |
| <span data-ttu-id="ad5d6-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="ad5d6-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="ad5d6-493">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-493">no</span></span>             | <span data-ttu-id="ad5d6-494">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-494">no</span></span>           |
| <span data-ttu-id="ad5d6-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="ad5d6-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="ad5d6-496">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-496">no</span></span>             | <span data-ttu-id="ad5d6-497">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-497">no</span></span>           |
| <span data-ttu-id="ad5d6-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="ad5d6-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="ad5d6-499">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-499">no</span></span>             | <span data-ttu-id="ad5d6-500">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-500">no</span></span>           |
| <span data-ttu-id="ad5d6-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="ad5d6-501">msdyn_start</span></span>                                      | <span data-ttu-id="ad5d6-502">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-502">no</span></span>             | <span data-ttu-id="ad5d6-503">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="ad5d6-504">Project</span><span class="sxs-lookup"><span data-stu-id="ad5d6-504">Project</span></span>

| <span data-ttu-id="ad5d6-505">**Логичко име**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-505">**Logical name**</span></span>                       | <span data-ttu-id="ad5d6-506">**Може да креира**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-506">**Can create**</span></span> | <span data-ttu-id="ad5d6-507">**Може да мења**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="ad5d6-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="ad5d6-509">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-509">no</span></span>             | <span data-ttu-id="ad5d6-510">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-510">no</span></span>           |
| <span data-ttu-id="ad5d6-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="ad5d6-512">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-512">no</span></span>             | <span data-ttu-id="ad5d6-513">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-513">no</span></span>           |
| <span data-ttu-id="ad5d6-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="ad5d6-515">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-515">no</span></span>             | <span data-ttu-id="ad5d6-516">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-516">no</span></span>           |
| <span data-ttu-id="ad5d6-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="ad5d6-518">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-518">no</span></span>             | <span data-ttu-id="ad5d6-519">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-519">no</span></span>           |
| <span data-ttu-id="ad5d6-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="ad5d6-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="ad5d6-521">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-521">no</span></span>             | <span data-ttu-id="ad5d6-522">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-522">no</span></span>           |
| <span data-ttu-id="ad5d6-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="ad5d6-524">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-524">no</span></span>             | <span data-ttu-id="ad5d6-525">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-525">no</span></span>           |
| <span data-ttu-id="ad5d6-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="ad5d6-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="ad5d6-527">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-527">yes</span></span>            | <span data-ttu-id="ad5d6-528">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-528">no</span></span>           |
| <span data-ttu-id="ad5d6-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="ad5d6-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="ad5d6-530">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-530">yes</span></span>            | <span data-ttu-id="ad5d6-531">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-531">no</span></span>           |
| <span data-ttu-id="ad5d6-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="ad5d6-533">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-533">yes</span></span>            | <span data-ttu-id="ad5d6-534">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-534">no</span></span>           |
| <span data-ttu-id="ad5d6-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="ad5d6-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="ad5d6-536">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-536">no</span></span>             | <span data-ttu-id="ad5d6-537">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-537">no</span></span>           |
| <span data-ttu-id="ad5d6-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="ad5d6-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="ad5d6-539">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-539">no</span></span>             | <span data-ttu-id="ad5d6-540">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-540">no</span></span>           |
| <span data-ttu-id="ad5d6-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="ad5d6-542">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-542">no</span></span>             | <span data-ttu-id="ad5d6-543">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-543">no</span></span>           |
| <span data-ttu-id="ad5d6-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="ad5d6-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="ad5d6-545">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-545">no</span></span>             | <span data-ttu-id="ad5d6-546">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-546">no</span></span>           |
| <span data-ttu-id="ad5d6-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="ad5d6-548">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-548">no</span></span>             | <span data-ttu-id="ad5d6-549">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-549">no</span></span>           |
| <span data-ttu-id="ad5d6-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="ad5d6-550">msdyn_duration</span></span>                         | <span data-ttu-id="ad5d6-551">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-551">no</span></span>             | <span data-ttu-id="ad5d6-552">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-552">no</span></span>           |
| <span data-ttu-id="ad5d6-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="ad5d6-553">msdyn_effort</span></span>                           | <span data-ttu-id="ad5d6-554">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-554">no</span></span>             | <span data-ttu-id="ad5d6-555">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-555">no</span></span>           |
| <span data-ttu-id="ad5d6-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ad5d6-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="ad5d6-557">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-557">no</span></span>             | <span data-ttu-id="ad5d6-558">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-558">no</span></span>           |
| <span data-ttu-id="ad5d6-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="ad5d6-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="ad5d6-560">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-560">no</span></span>             | <span data-ttu-id="ad5d6-561">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-561">no</span></span>           |
| <span data-ttu-id="ad5d6-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="ad5d6-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="ad5d6-563">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-563">no</span></span>             | <span data-ttu-id="ad5d6-564">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-564">no</span></span>           |
| <span data-ttu-id="ad5d6-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="ad5d6-565">msdyn_finish</span></span>                           | <span data-ttu-id="ad5d6-566">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-566">yes</span></span>            | <span data-ttu-id="ad5d6-567">Да</span><span class="sxs-lookup"><span data-stu-id="ad5d6-567">yes</span></span>          |
| <span data-ttu-id="ad5d6-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="ad5d6-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="ad5d6-569">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-569">no</span></span>             | <span data-ttu-id="ad5d6-570">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-570">no</span></span>           |
| <span data-ttu-id="ad5d6-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="ad5d6-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="ad5d6-572">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-572">no</span></span>             | <span data-ttu-id="ad5d6-573">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-573">no</span></span>           |
| <span data-ttu-id="ad5d6-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="ad5d6-575">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-575">no</span></span>             | <span data-ttu-id="ad5d6-576">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-576">no</span></span>           |
| <span data-ttu-id="ad5d6-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="ad5d6-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="ad5d6-578">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-578">no</span></span>             | <span data-ttu-id="ad5d6-579">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-579">no</span></span>           |
| <span data-ttu-id="ad5d6-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="ad5d6-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="ad5d6-581">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-581">no</span></span>             | <span data-ttu-id="ad5d6-582">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-582">no</span></span>           |
| <span data-ttu-id="ad5d6-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="ad5d6-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="ad5d6-584">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-584">no</span></span>             | <span data-ttu-id="ad5d6-585">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-585">no</span></span>           |
| <span data-ttu-id="ad5d6-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="ad5d6-587">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-587">no</span></span>             | <span data-ttu-id="ad5d6-588">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-588">no</span></span>           |
| <span data-ttu-id="ad5d6-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="ad5d6-590">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-590">no</span></span>             | <span data-ttu-id="ad5d6-591">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-591">no</span></span>           |
| <span data-ttu-id="ad5d6-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="ad5d6-593">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-593">no</span></span>             | <span data-ttu-id="ad5d6-594">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-594">no</span></span>           |
| <span data-ttu-id="ad5d6-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="ad5d6-596">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-596">no</span></span>             | <span data-ttu-id="ad5d6-597">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-597">no</span></span>           |
| <span data-ttu-id="ad5d6-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="ad5d6-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="ad5d6-599">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-599">no</span></span>             | <span data-ttu-id="ad5d6-600">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-600">no</span></span>           |
| <span data-ttu-id="ad5d6-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="ad5d6-602">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-602">no</span></span>             | <span data-ttu-id="ad5d6-603">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-603">no</span></span>           |
| <span data-ttu-id="ad5d6-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="ad5d6-604">msdyn_progress</span></span>                         | <span data-ttu-id="ad5d6-605">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-605">no</span></span>             | <span data-ttu-id="ad5d6-606">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-606">no</span></span>           |
| <span data-ttu-id="ad5d6-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="ad5d6-608">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-608">no</span></span>             | <span data-ttu-id="ad5d6-609">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-609">no</span></span>           |
| <span data-ttu-id="ad5d6-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="ad5d6-611">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-611">no</span></span>             | <span data-ttu-id="ad5d6-612">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-612">no</span></span>           |
| <span data-ttu-id="ad5d6-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="ad5d6-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="ad5d6-614">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-614">no</span></span>             | <span data-ttu-id="ad5d6-615">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-615">no</span></span>           |
| <span data-ttu-id="ad5d6-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="ad5d6-617">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-617">no</span></span>             | <span data-ttu-id="ad5d6-618">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-618">no</span></span>           |
| <span data-ttu-id="ad5d6-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="ad5d6-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="ad5d6-620">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-620">no</span></span>             | <span data-ttu-id="ad5d6-621">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-621">no</span></span>           |
| <span data-ttu-id="ad5d6-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="ad5d6-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="ad5d6-623">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-623">no</span></span>             | <span data-ttu-id="ad5d6-624">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-624">no</span></span>           |
| <span data-ttu-id="ad5d6-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="ad5d6-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="ad5d6-626">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-626">no</span></span>             | <span data-ttu-id="ad5d6-627">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-627">no</span></span>           |
| <span data-ttu-id="ad5d6-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="ad5d6-629">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-629">no</span></span>             | <span data-ttu-id="ad5d6-630">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-630">no</span></span>           |
| <span data-ttu-id="ad5d6-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="ad5d6-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="ad5d6-632">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-632">no</span></span>             | <span data-ttu-id="ad5d6-633">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-633">no</span></span>           |
| <span data-ttu-id="ad5d6-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="ad5d6-635">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-635">no</span></span>             | <span data-ttu-id="ad5d6-636">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-636">no</span></span>           |
| <span data-ttu-id="ad5d6-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="ad5d6-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="ad5d6-638">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-638">no</span></span>             | <span data-ttu-id="ad5d6-639">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-639">no</span></span>           |
| <span data-ttu-id="ad5d6-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="ad5d6-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="ad5d6-641">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-641">no</span></span>             | <span data-ttu-id="ad5d6-642">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-642">no</span></span>           |
| <span data-ttu-id="ad5d6-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="ad5d6-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="ad5d6-644">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-644">no</span></span>             | <span data-ttu-id="ad5d6-645">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-645">no</span></span>           |
| <span data-ttu-id="ad5d6-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="ad5d6-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="ad5d6-647">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-647">no</span></span>             | <span data-ttu-id="ad5d6-648">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-648">no</span></span>           |
| <span data-ttu-id="ad5d6-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="ad5d6-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="ad5d6-650">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-650">no</span></span>             | <span data-ttu-id="ad5d6-651">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-651">no</span></span>           |
| <span data-ttu-id="ad5d6-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="ad5d6-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="ad5d6-653">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-653">no</span></span>             | <span data-ttu-id="ad5d6-654">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-654">no</span></span>           |
| <span data-ttu-id="ad5d6-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="ad5d6-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="ad5d6-656">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-656">no</span></span>             | <span data-ttu-id="ad5d6-657">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-657">no</span></span>           |
| <span data-ttu-id="ad5d6-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="ad5d6-659">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-659">no</span></span>             | <span data-ttu-id="ad5d6-660">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-660">no</span></span>           |
| <span data-ttu-id="ad5d6-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="ad5d6-662">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-662">no</span></span>             | <span data-ttu-id="ad5d6-663">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-663">no</span></span>           |
| <span data-ttu-id="ad5d6-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="ad5d6-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="ad5d6-665">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-665">no</span></span>             | <span data-ttu-id="ad5d6-666">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-666">no</span></span>           |
| <span data-ttu-id="ad5d6-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="ad5d6-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="ad5d6-668">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-668">no</span></span>             | <span data-ttu-id="ad5d6-669">не</span><span class="sxs-lookup"><span data-stu-id="ad5d6-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="ad5d6-670">Ограничења и познати проблеми</span><span class="sxs-lookup"><span data-stu-id="ad5d6-670">Limitations and known issues</span></span>
<span data-ttu-id="ad5d6-671">Следи листа ограничења и познатих проблема:</span><span class="sxs-lookup"><span data-stu-id="ad5d6-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="ad5d6-672">API-је за распоред могу да користе само **корисници са лиценцом за Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="ad5d6-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="ad5d6-673">Не могу их користити:</span><span class="sxs-lookup"><span data-stu-id="ad5d6-673">They can't be used by:</span></span>
    - <span data-ttu-id="ad5d6-674">Корисници апликације</span><span class="sxs-lookup"><span data-stu-id="ad5d6-674">Application users</span></span>
    - <span data-ttu-id="ad5d6-675">Корисници система</span><span class="sxs-lookup"><span data-stu-id="ad5d6-675">System users</span></span>
    - <span data-ttu-id="ad5d6-676">Корисници интеграције</span><span class="sxs-lookup"><span data-stu-id="ad5d6-676">Integration users</span></span>
    - <span data-ttu-id="ad5d6-677">Остали корисници који немају потребну лиценцу</span><span class="sxs-lookup"><span data-stu-id="ad5d6-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="ad5d6-678">Сваки **OperationSet ентитет** може да има највише 100 операција.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="ad5d6-679">Сваки корисник може да има највише 10 отворених **OperationSet ентитета**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="ad5d6-680">Project Operations тренутно подржава максимално 500 укупних задатака на пројекту.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="ad5d6-681">Статус грешке и евиденције грешака **OperationSet ентитета** тренутно нису доступне.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="ad5d6-682">API-ји за распоред су у верзији за јавни преглед.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="ad5d6-683">Microsoft не подржава употребу ових API-ја у производном окружењу.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="ad5d6-684">Ограничења и границе пројеката и задатака</span><span class="sxs-lookup"><span data-stu-id="ad5d6-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="ad5d6-685">Руковање грешкама</span><span class="sxs-lookup"><span data-stu-id="ad5d6-685">Error handling</span></span>

   - <span data-ttu-id="ad5d6-686">Да бисте прегледали грешке генерисане из скупова операција, идите на **Подешавања** \> **Закажи интеграцију** \> **Скупови операција**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="ad5d6-687">Да бисте прегледали грешке генерисане услугом планирања пројеката, идите на **Подешавања** \> **Закажи интеграцију** \> **Дневници грешака PSS-а**.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="ad5d6-688">Пример сценарија</span><span class="sxs-lookup"><span data-stu-id="ad5d6-688">Sample scenario</span></span>

<span data-ttu-id="ad5d6-689">У овом сценарију, креираћете пројекат, члана тима, четири задатка и два задатка ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="ad5d6-690">Затим ћете ажурирати један задатак, ажурирати пројекат, избрисати један задатак, избрисати једну доделу ресурса и креирати зависност задатка.</span><span class="sxs-lookup"><span data-stu-id="ad5d6-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="ad5d6-691">Додатни примери</span><span class="sxs-lookup"><span data-stu-id="ad5d6-691">Additional samples</span></span>

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
