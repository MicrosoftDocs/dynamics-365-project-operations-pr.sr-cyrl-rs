---
title: Разматрања надоградње структурне анализе посла
description: Ова тема пружа информације о надоградњи структурне анализе посла из апликације Project Service Automation верзије 2.x у верзију 3.x.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: a067521410f0fe0d8f5d4c510a35f2a3b018dce3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281766"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="2ca7a-103">Разматрања надоградње структурне анализе посла</span><span class="sxs-lookup"><span data-stu-id="2ca7a-103">Upgrade considerations for the work breakdown structure</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2ca7a-104">Ова тема пружа информације о надоградњи структурне анализе посла из апликације Project Service Automation верзије 2.x у верзију 3.x.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="2ca7a-105">Ова тема дефинише исправно стање пројекта у апликацији Project Service Automation (PSA), потребно за успешну надоградњу.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="2ca7a-106">Постоје и информације о уобичајеним условима блокирања који ће довести до неуспешне надоградње.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="2ca7a-107">Више информација о дефинисању пројектних задатака и њиховим функцијама у оквиру распореда пројекта потражите у чланку [Распореди пројеката](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="2ca7a-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="2ca7a-108">Кључни ентитети</span><span class="sxs-lookup"><span data-stu-id="2ca7a-108">Key entities</span></span>
<span data-ttu-id="2ca7a-109">За исправну структурну анализу посла која је већ учитана са ресурсима, потребни су следећи ентитети:</span><span class="sxs-lookup"><span data-stu-id="2ca7a-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="2ca7a-110">Пројекат</span><span class="sxs-lookup"><span data-stu-id="2ca7a-110">Project</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="2ca7a-111">Пројектни тим</span><span class="sxs-lookup"><span data-stu-id="2ca7a-111">Project Team</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="2ca7a-112">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="2ca7a-112">Project Task</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="2ca7a-113">Доделе ресурса</span><span class="sxs-lookup"><span data-stu-id="2ca7a-113">Resource Assignments</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="2ca7a-114">Зависност пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="2ca7a-114">Project Task Dependency</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="2ca7a-115">Ресурси који могу да се резервишу</span><span class="sxs-lookup"><span data-stu-id="2ca7a-115">Bookable Resources</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="2ca7a-116">Да бисте дефинисали структурну анализу посла коју је учитао ресурс, морате да довршите следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="2ca7a-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="2ca7a-117">Креирајте нови пројекат.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-117">Create a new project.</span></span> <span data-ttu-id="2ca7a-118">За више информација о томе како да креирате нови пројекат, погледајте [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span><span class="sxs-lookup"><span data-stu-id="2ca7a-118">For more information about how to create a new project, see [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="2ca7a-119">Креирајте један или више задатака.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-119">Create one or more tasks.</span></span> <span data-ttu-id="2ca7a-120">За више информација о томе како да креирате нови задатак, погледајте [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span><span class="sxs-lookup"><span data-stu-id="2ca7a-120">For more information about how to create a task, see [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="2ca7a-121">Дефинишите зависне елементе задатка.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-121">Define the task dependencies.</span></span> <span data-ttu-id="2ca7a-122">За још информација погледајте [Зависност пројектног задатка](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span><span class="sxs-lookup"><span data-stu-id="2ca7a-122">For more information, see [Project Task Dependency](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="2ca7a-123">Доделите чланове пројектног тима пројекту.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-123">Assign project team members to the project.</span></span> <span data-ttu-id="2ca7a-124">За више информација, погледајте [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span><span class="sxs-lookup"><span data-stu-id="2ca7a-124">For more information, see [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="2ca7a-125">Доделите чланове пројектног тима задацима.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="2ca7a-126">За више информација, погледајте [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span><span class="sxs-lookup"><span data-stu-id="2ca7a-126">For more information, see [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="2ca7a-127">Односи унутар пројектног тима</span><span class="sxs-lookup"><span data-stu-id="2ca7a-127">Project team relationships</span></span>

<span data-ttu-id="2ca7a-128">Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:</span><span class="sxs-lookup"><span data-stu-id="2ca7a-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="2ca7a-129">Сви чланови пројектног тима морају бити повезани са ресурсом који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="2ca7a-130">Сви чланови пројектног тима морају бити повезани са истим пројектом.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="2ca7a-131">Односи у оквиру пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="2ca7a-131">Project task relationships</span></span>
<span data-ttu-id="2ca7a-132">Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:</span><span class="sxs-lookup"><span data-stu-id="2ca7a-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="2ca7a-133">Сви повезани задаци морају бити повезани са истим пројектом.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="2ca7a-134">Сваки задатак ставке мора имати надређени задатак.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="2ca7a-135">Сваки задатак мора имати надређени пројекат.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="2ca7a-136">Важећи услови</span><span class="sxs-lookup"><span data-stu-id="2ca7a-136">Valid conditions</span></span>

- <span data-ttu-id="2ca7a-137">Трајање сваког задатка мора бити дуже од сат времена или једнако том времену (>=) и краће од 1.800.000 минута (1250 дана).\*</span><span class="sxs-lookup"><span data-stu-id="2ca7a-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="2ca7a-138">Сви задаци морају имати датум почетка који није пре 1.1.2000.\*</span><span class="sxs-lookup"><span data-stu-id="2ca7a-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="2ca7a-139">Сви задаци морају имати датум почетка који је најдаље 17 година од данашњег дана.\*</span><span class="sxs-lookup"><span data-stu-id="2ca7a-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="2ca7a-140">Сви задаци морају да имају датум почетка који је пре датума завршетка или исти као тај датум.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="2ca7a-141">Све врсте трансакција за класификације (Трошкови, Материјал, Порез и Време) морају имати вредности за ставке **Подразумевана јединица** и **Група јединица**.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="2ca7a-142">Формате датума са словима треба избегавати.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="2ca7a-143">Потенцијални кораци за ублажавање</span><span class="sxs-lookup"><span data-stu-id="2ca7a-143">Potential mitigation steps</span></span>
- <span data-ttu-id="2ca7a-144">Користите напредну претрагу за идентификацију пројектних задатака који не садрже ID пројекта.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="2ca7a-145">Користите напредну претрагу да бисте идентификовали пројектне задатке где је заказано трајање дуже од > 1.800.000.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="2ca7a-146">Пре него што унесете било какве промене података, требало би да истражите сва прилагођавања повезана са ентитетом која су могла довести до тога да се подаци доведу у лош статус.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="2ca7a-147">Требало би да се позабавите са овим прилагођавањима пре него што наставите са било каквим исправкама које се односе на податке.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="2ca7a-148">За идентификоване задатке који су наслеђени, размотрите брисање ових задатака ако вам нису потребни или ако би требало бити повезани са исправних надређеним пројектом.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="2ca7a-149">За све задатке у којима је трајање дуже од 1250 дана, размотрите додавање више задатака како бисте представљали укупно трајање, ако је доступно.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="2ca7a-150">Ставке забележене звездицом (\*) имају ограничења због чињенице да управљање односима са клијентима (CRM) подржава само 7320 проширења понављања.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="2ca7a-151">Не смете да прекорачите ово ограничење.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="2ca7a-152">Односи између додела ресурса</span><span class="sxs-lookup"><span data-stu-id="2ca7a-152">Resource Assignment relationships</span></span>
<span data-ttu-id="2ca7a-153">Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:</span><span class="sxs-lookup"><span data-stu-id="2ca7a-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="2ca7a-154">Све доделе ресурса у структурној анализи посла морају бити повезане са истим пројектом.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="2ca7a-155">Све доделе ресурса у структурној анализи посла морају бити повезане са члановима пројектног тима у истом пројекту.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="2ca7a-156">Потенцијални кораци за ублажавање</span><span class="sxs-lookup"><span data-stu-id="2ca7a-156">Potential mitigation steps</span></span>
- <span data-ttu-id="2ca7a-157">Идентификујте све задатке који спадају ван гореописаних услова.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="2ca7a-158">Све доделе ресурса које више нису важеће би требало бити обрисане.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="2ca7a-159">Односи између зависних елемената пројектног задатка</span><span class="sxs-lookup"><span data-stu-id="2ca7a-159">Project task dependency relationships</span></span>
<span data-ttu-id="2ca7a-160">Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:</span><span class="sxs-lookup"><span data-stu-id="2ca7a-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="2ca7a-161">Сви зависни елементи задатка пројекта морају бити повезани са истим пројектом.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="2ca7a-162">Задатак не може да има исти зависни елемент на који се упућује више пута.</span><span class="sxs-lookup"><span data-stu-id="2ca7a-162">A task can't have the same dependency referenced more than once.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]