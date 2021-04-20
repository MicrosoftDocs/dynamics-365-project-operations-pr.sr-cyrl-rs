---
title: Коришћење API-ја за распоред за обављање операција са ентитетима планирања
description: Ова тема пружа информације и примере за коришћење API-ја за распоред.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868147"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="55e12-103">Коришћење API-ја за распоред за обављање операција са ентитетима планирања</span><span class="sxs-lookup"><span data-stu-id="55e12-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="55e12-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="55e12-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="55e12-105">Неке или све функционалности забележене у овој теми доступне су као део издања верзије за преглед.</span><span class="sxs-lookup"><span data-stu-id="55e12-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="55e12-106">Садржај и функционалност су подложни променама.</span><span class="sxs-lookup"><span data-stu-id="55e12-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="55e12-107">Ентитети планирања</span><span class="sxs-lookup"><span data-stu-id="55e12-107">Scheduling entities</span></span>

<span data-ttu-id="55e12-108">API-ји за распоред пружају могућност извршавања операција креирања, ажурирања и брисања помоћу **ентитета планирања**.</span><span class="sxs-lookup"><span data-stu-id="55e12-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="55e12-109">Тим ентитетима се управља путем механизма за распоређивање у апликацији Project за веб.</span><span class="sxs-lookup"><span data-stu-id="55e12-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="55e12-110">Креирање, ажурирање и брисање операција помоћу **ентитета планирања** били су ограничени у ранијим издањима услуге Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="55e12-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="55e12-111">Следећа табела даје потпуну листу **ентитета планирања**.</span><span class="sxs-lookup"><span data-stu-id="55e12-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="55e12-112">Назив ентитета</span><span class="sxs-lookup"><span data-stu-id="55e12-112">Entity name</span></span>  | <span data-ttu-id="55e12-113">Логичко име ентитета</span><span class="sxs-lookup"><span data-stu-id="55e12-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="55e12-114">Project</span><span class="sxs-lookup"><span data-stu-id="55e12-114">Project</span></span> | <span data-ttu-id="55e12-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="55e12-115">msdyn_project</span></span> |
| <span data-ttu-id="55e12-116">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="55e12-116">Project Task</span></span>  | <span data-ttu-id="55e12-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="55e12-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="55e12-118">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="55e12-118">Project Task Dependency</span></span>  | <span data-ttu-id="55e12-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="55e12-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="55e12-120">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="55e12-120">Resource Assignment</span></span> | <span data-ttu-id="55e12-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="55e12-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="55e12-122">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="55e12-122">Project Bucket</span></span>  | <span data-ttu-id="55e12-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="55e12-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="55e12-124">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="55e12-124">Project Team Member</span></span> | <span data-ttu-id="55e12-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="55e12-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="55e12-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="55e12-126">OperationSet</span></span>

<span data-ttu-id="55e12-127">Ентитет OperationSet је образац јединице рада који се може користити када се у трансакцији мора обрадити неколико захтева који утичу на распоред.</span><span class="sxs-lookup"><span data-stu-id="55e12-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="55e12-128">API-ји за распоред</span><span class="sxs-lookup"><span data-stu-id="55e12-128">Schedule APIs</span></span>

<span data-ttu-id="55e12-129">Следи листа актуелних API-ја за распоред.</span><span class="sxs-lookup"><span data-stu-id="55e12-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="55e12-130">**msdyn_CreateProjectV1**: Овај API се може користити за креирање пројекта.</span><span class="sxs-lookup"><span data-stu-id="55e12-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="55e12-131">Пројекат и подразумевани контејнер пројекта креирају се одмах.</span><span class="sxs-lookup"><span data-stu-id="55e12-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="55e12-132">**msdyn_CreateTeamMemberV1**: Овај API се може користити за креирање члана пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="55e12-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="55e12-133">Евиденција члана тима креира се одмах.</span><span class="sxs-lookup"><span data-stu-id="55e12-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="55e12-134">**msdyn_CreateOperationSetV1**: Овај API се може користити за заказивање неколико захтева који се морају извршити у оквиру трансакције.</span><span class="sxs-lookup"><span data-stu-id="55e12-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="55e12-135">**msdyn_PSSCreateV1**: Овај API се може користити за креирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="55e12-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="55e12-136">Ентитет може бити било који ентитет планирања који подржава операцију креирања.</span><span class="sxs-lookup"><span data-stu-id="55e12-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="55e12-137">**msdyn_PSSUpdateV1**: Овај API се може користити за ажурирање ентитета.</span><span class="sxs-lookup"><span data-stu-id="55e12-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="55e12-138">Ентитет може бити било који ентитет планирања који подржава операцију ажурирања.</span><span class="sxs-lookup"><span data-stu-id="55e12-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="55e12-139">**msdyn_PSSDeleteV1**: Овај API се може користити за брисање ентитета.</span><span class="sxs-lookup"><span data-stu-id="55e12-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="55e12-140">Ентитет може бити било који ентитет планирања који подржава операцију брисања.</span><span class="sxs-lookup"><span data-stu-id="55e12-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="55e12-141">**msdyn_ExecuteOperationSetV1**: Овај API се користи за извршавање свих операција унутар датог скупа операција.</span><span class="sxs-lookup"><span data-stu-id="55e12-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="55e12-142">Коришћење API-ја распореда са OperationSet ентитетом</span><span class="sxs-lookup"><span data-stu-id="55e12-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="55e12-143">Пошто се записи са **CreateProjectV1** и **CreateTeamMemberV1** креирају одмах, ови API-ји се не могу користити у **OperationSet ентитету** директно.</span><span class="sxs-lookup"><span data-stu-id="55e12-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="55e12-144">Међутим, API можете користити за креирање потребних записа, креирајте **OperationSet ентитет**, а затим користите ове унапред креиране записе у **OperationSet ентитету**.</span><span class="sxs-lookup"><span data-stu-id="55e12-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="55e12-145">Подржане операције</span><span class="sxs-lookup"><span data-stu-id="55e12-145">Supported operations</span></span>

| <span data-ttu-id="55e12-146">Ентитет планирања</span><span class="sxs-lookup"><span data-stu-id="55e12-146">Scheduling entity</span></span> | <span data-ttu-id="55e12-147">Направи</span><span class="sxs-lookup"><span data-stu-id="55e12-147">Create</span></span> | <span data-ttu-id="55e12-148">Ажурирање</span><span class="sxs-lookup"><span data-stu-id="55e12-148">Update</span></span> | <span data-ttu-id="55e12-149">Delete</span><span class="sxs-lookup"><span data-stu-id="55e12-149">Delete</span></span> | <span data-ttu-id="55e12-150">Важна разматрања</span><span class="sxs-lookup"><span data-stu-id="55e12-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="55e12-151">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="55e12-151">Project task</span></span> | <span data-ttu-id="55e12-152">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-152">Yes</span></span> | <span data-ttu-id="55e12-153">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-153">Yes</span></span> | <span data-ttu-id="55e12-154">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-154">Yes</span></span> | <span data-ttu-id="55e12-155">Ниједно</span><span class="sxs-lookup"><span data-stu-id="55e12-155">None</span></span> |
| <span data-ttu-id="55e12-156">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="55e12-156">Project task dependency</span></span> | <span data-ttu-id="55e12-157">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-157">Yes</span></span> | <span data-ttu-id="55e12-158">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-158">Yes</span></span> | | <span data-ttu-id="55e12-159">Записи зависности пројектних задатака се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="55e12-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="55e12-160">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="55e12-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="55e12-161">Додела ресурса</span><span class="sxs-lookup"><span data-stu-id="55e12-161">Resource assignment</span></span> | <span data-ttu-id="55e12-162">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-162">Yes</span></span> | <span data-ttu-id="55e12-163">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-163">Yes</span></span> | | <span data-ttu-id="55e12-164">Нису подржане операције са следећим пољима: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="55e12-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="55e12-165">Записи о додели ресурса се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="55e12-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="55e12-166">Уместо тога, стари запис може да се избрише и може да се креира нови запис.</span><span class="sxs-lookup"><span data-stu-id="55e12-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="55e12-167">Контејнер пројекта</span><span class="sxs-lookup"><span data-stu-id="55e12-167">Project bucket</span></span> | <span data-ttu-id="55e12-168">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="55e12-168">N/A</span></span> | <span data-ttu-id="55e12-169">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="55e12-169">N/A</span></span> | <span data-ttu-id="55e12-170">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="55e12-170">N/A</span></span> | <span data-ttu-id="55e12-171">Подразумевани контејнер се креира се помоћу API-ја **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="55e12-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="55e12-172">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="55e12-172">Project team member</span></span> | <span data-ttu-id="55e12-173">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-173">Yes</span></span> | <span data-ttu-id="55e12-174">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-174">Yes</span></span> | <span data-ttu-id="55e12-175">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-175">Yes</span></span> | <span data-ttu-id="55e12-176">За операцију креирања користите API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="55e12-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="55e12-177">Project</span><span class="sxs-lookup"><span data-stu-id="55e12-177">Project</span></span> | <span data-ttu-id="55e12-178">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-178">Yes</span></span> | <span data-ttu-id="55e12-179">Да</span><span class="sxs-lookup"><span data-stu-id="55e12-179">Yes</span></span> | <span data-ttu-id="55e12-180">Није применљиво</span><span class="sxs-lookup"><span data-stu-id="55e12-180">N/A</span></span> | <span data-ttu-id="55e12-181">Нису подржане операције са следећим пољима: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.</span><span class="sxs-lookup"><span data-stu-id="55e12-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="55e12-182">Ови API-ји се могу позивати са објектима ентитета који укључују прилагођена поља.</span><span class="sxs-lookup"><span data-stu-id="55e12-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="55e12-183">Својство ID је опционално.</span><span class="sxs-lookup"><span data-stu-id="55e12-183">The ID property is optional.</span></span> <span data-ttu-id="55e12-184">Ако је обезбеђено, систем покушава да га користи и избацује изузетак ако не може да га користи.</span><span class="sxs-lookup"><span data-stu-id="55e12-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="55e12-185">Ако није обезбеђено, систем ће га генерисати.</span><span class="sxs-lookup"><span data-stu-id="55e12-185">If it isn't provided, the system will generate it.</span></span>

## <a name="limitations-and-known-issues"></a><span data-ttu-id="55e12-186">Ограничења и познати проблеми</span><span class="sxs-lookup"><span data-stu-id="55e12-186">Limitations and known issues</span></span>
<span data-ttu-id="55e12-187">Следи листа ограничења и познатих проблема:</span><span class="sxs-lookup"><span data-stu-id="55e12-187">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="55e12-188">API-је за распоред могу да користе само **корисници са лиценцом за Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="55e12-188">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="55e12-189">Не могу их користити:</span><span class="sxs-lookup"><span data-stu-id="55e12-189">They can't be used by:</span></span>
    - <span data-ttu-id="55e12-190">Корисници апликације</span><span class="sxs-lookup"><span data-stu-id="55e12-190">Application users</span></span>
    - <span data-ttu-id="55e12-191">Корисници система</span><span class="sxs-lookup"><span data-stu-id="55e12-191">System users</span></span>
    - <span data-ttu-id="55e12-192">Корисници интеграције</span><span class="sxs-lookup"><span data-stu-id="55e12-192">Integration users</span></span>
    - <span data-ttu-id="55e12-193">Остали корисници који немају потребну лиценцу</span><span class="sxs-lookup"><span data-stu-id="55e12-193">Other users that don't have the required license</span></span>
- <span data-ttu-id="55e12-194">Сваки **OperationSet ентитет** може да има највише 100 операција.</span><span class="sxs-lookup"><span data-stu-id="55e12-194">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="55e12-195">Сваки корисник може да има највише 10 отворених **OperationSet ентитета**.</span><span class="sxs-lookup"><span data-stu-id="55e12-195">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="55e12-196">Project Operations тренутно подржава максимално 500 укупних задатака на пројекту.</span><span class="sxs-lookup"><span data-stu-id="55e12-196">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="55e12-197">Статус грешке и евиденције грешака **OperationSet ентитета** тренутно нису доступне.</span><span class="sxs-lookup"><span data-stu-id="55e12-197">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="55e12-198">API-ји за распоред су у верзији за јавни преглед.</span><span class="sxs-lookup"><span data-stu-id="55e12-198">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="55e12-199">Microsoft не подржава употребу ових API-ја у производном окружењу.</span><span class="sxs-lookup"><span data-stu-id="55e12-199">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="55e12-200">Пример сценарија</span><span class="sxs-lookup"><span data-stu-id="55e12-200">Sample scenario</span></span>

<span data-ttu-id="55e12-201">У овом сценарију, креираћете пројекат, члана тима, четири задатка и два задатка ресурса.</span><span class="sxs-lookup"><span data-stu-id="55e12-201">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="55e12-202">Затим ћете ажурирати један задатак, ажурирати пројекат, избрисати један задатак, избрисати једну доделу ресурса и креирати зависност задатка.</span><span class="sxs-lookup"><span data-stu-id="55e12-202">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="55e12-203">Додатни примери</span><span class="sxs-lookup"><span data-stu-id="55e12-203">Additional samples</span></span>

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
