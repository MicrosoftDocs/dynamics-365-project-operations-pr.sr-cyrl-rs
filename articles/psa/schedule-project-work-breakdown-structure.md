---
title: Закажите пројекат са структурном анализом посла
description: Како да планирате пројекат са структурном анализом посла у апликацији Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: a00e39f78890426721a49cd569ba8ce4accb30a9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282711"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="dd451-103">Планирајте пројекат са структурном анализом посла (Project Service)</span><span class="sxs-lookup"><span data-stu-id="dd451-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="dd451-104">Распоред пројекта наводи који посао треба да се обави, који ресурси ће извршити посао и временски оквир у ком посао треба да се доврши.</span><span class="sxs-lookup"><span data-stu-id="dd451-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="dd451-105">Распоред пројекта одражава сав посао повезан са завршавањем пројекта на време.</span><span class="sxs-lookup"><span data-stu-id="dd451-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="dd451-106">Један од првих корака у почетној фази пројекта је да се направи распоред пројекта.</span><span class="sxs-lookup"><span data-stu-id="dd451-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="dd451-107">Да бисте успоставили распоред пројекта, потребно је да креирате структурну анализу посла.</span><span class="sxs-lookup"><span data-stu-id="dd451-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="dd451-108">Креирање пројектне структуре са структурном анализом посла која вам помаже да:</span><span class="sxs-lookup"><span data-stu-id="dd451-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="dd451-109">Поделите посао у задатке којима је лако управљати</span><span class="sxs-lookup"><span data-stu-id="dd451-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="dd451-110">Процените време потребно за довршење задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="dd451-111">Подесите зависности и трајање задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="dd451-112">Одредите улоге које су потребне за довршавање сваког задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="dd451-113">Распоред пројекта структурној анализи посла има познати изглед и осећај, заједно са интерактивним Gantt графиконом.</span><span class="sxs-lookup"><span data-stu-id="dd451-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="dd451-114">Креирање структурне анализе посла за пројекат</span><span class="sxs-lookup"><span data-stu-id="dd451-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="dd451-115">Креирање структурне анализе посла за представљање редослед задатака у пројекту</span><span class="sxs-lookup"><span data-stu-id="dd451-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="dd451-116">Структурна анализа посла укључује задатке, захтеве за сваки задатак и информације о приходима и трошковима.</span><span class="sxs-lookup"><span data-stu-id="dd451-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="dd451-117">У структурну анализу посла можете додати:</span><span class="sxs-lookup"><span data-stu-id="dd451-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="dd451-118">Редослед задатака у хијерархији</span><span class="sxs-lookup"><span data-stu-id="dd451-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="dd451-119">Друге задатке, ако их има, који морају бити довршени пре него што можете покренути задатак</span><span class="sxs-lookup"><span data-stu-id="dd451-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="dd451-120">Почетни датум, датум престанка и трајање задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="dd451-121">Број часова потребних за задатак</span><span class="sxs-lookup"><span data-stu-id="dd451-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="dd451-122">Све потребне вештине и образовање за раднике</span><span class="sxs-lookup"><span data-stu-id="dd451-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="dd451-123">Запослени који су постављени на задатак</span><span class="sxs-lookup"><span data-stu-id="dd451-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="dd451-124">Процењени приход и трошкови</span><span class="sxs-lookup"><span data-stu-id="dd451-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="dd451-125">Типови задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-125">Task types</span></span>  
<span data-ttu-id="dd451-126">Видећете следеће врсте задатака приликом креирања структурне анализе посла:</span><span class="sxs-lookup"><span data-stu-id="dd451-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="dd451-127">**Основни чвор пројекта**.</span><span class="sxs-lookup"><span data-stu-id="dd451-127">**Project root node**</span></span> | <span data-ttu-id="dd451-128">Сажетак највишег нивоа за задатак пројекта.</span><span class="sxs-lookup"><span data-stu-id="dd451-128">The top-level summary task for the project.</span></span> <span data-ttu-id="dd451-129">Сви други пројектни задаци се креирају у оквиру њега.</span><span class="sxs-lookup"><span data-stu-id="dd451-129">All other project tasks are created under it.</span></span> <span data-ttu-id="dd451-130">Име основног задатка је име пројекта.</span><span class="sxs-lookup"><span data-stu-id="dd451-130">The name of the root task is the project name.</span></span> <span data-ttu-id="dd451-131">Труд, датуми и трајање коренског чвора се заснивају на вредностима хијерархије испод њега.</span><span class="sxs-lookup"><span data-stu-id="dd451-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="dd451-132">Није могуће уредити својства коренског чвора или избришите коренски чвор.</span><span class="sxs-lookup"><span data-stu-id="dd451-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="dd451-133">**Резиме или задаци спремишта**</span><span class="sxs-lookup"><span data-stu-id="dd451-133">**Summary or container tasks**</span></span> | <span data-ttu-id="dd451-134">Задатак сажетка је задатак који има подзадатке.</span><span class="sxs-lookup"><span data-stu-id="dd451-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="dd451-135">Задатак сажетка нема самостални труд или трошак.</span><span class="sxs-lookup"><span data-stu-id="dd451-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="dd451-136">Његов труд и трошак су збирне вредности његових подзадатака.</span><span class="sxs-lookup"><span data-stu-id="dd451-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="dd451-137">Можете променити име задатка сажетка али не можете променити труд, датуме или време трајања, зато што се они аутоматски израчунавају.</span><span class="sxs-lookup"><span data-stu-id="dd451-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="dd451-138">Брисањем задатка сажетка брише задатак и све његове подзадатке.</span><span class="sxs-lookup"><span data-stu-id="dd451-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="dd451-139">**Задаци чвора листа**</span><span class="sxs-lookup"><span data-stu-id="dd451-139">**Leaf node tasks**</span></span> | <span data-ttu-id="dd451-140">Задатак чвор листа представља најдетаљнији посао на пројекту.</span><span class="sxs-lookup"><span data-stu-id="dd451-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="dd451-141">Садржи процењени труд, планирани број ресурса, планиране датуме почетка и завршетка и трајање.</span><span class="sxs-lookup"><span data-stu-id="dd451-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="dd451-142">Хијерархија задатака</span><span class="sxs-lookup"><span data-stu-id="dd451-142">Task hierarchy</span></span>  
 <span data-ttu-id="dd451-143">Имате следеће опције приликом креирања хијерархије задатака:</span><span class="sxs-lookup"><span data-stu-id="dd451-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="dd451-144">**Додај задатак**.</span><span class="sxs-lookup"><span data-stu-id="dd451-144">**Add task**.</span></span>   <span data-ttu-id="dd451-145">Можете да додате задатак у положај који одаберете у хијерархији задатака.</span><span class="sxs-lookup"><span data-stu-id="dd451-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="dd451-146">Ако не одаберете положај, нови задатак се појављује на крају.</span><span class="sxs-lookup"><span data-stu-id="dd451-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="dd451-147">**Увлачење задатка**.</span><span class="sxs-lookup"><span data-stu-id="dd451-147">**Indent task**.</span></span>   <span data-ttu-id="dd451-148">Увлачењем задатка га чините подређеним задатку директно изнад њега.</span><span class="sxs-lookup"><span data-stu-id="dd451-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="dd451-149">**Извлачење задатка**.</span><span class="sxs-lookup"><span data-stu-id="dd451-149">**Outdent task**.</span></span>   <span data-ttu-id="dd451-150">Извуците задатак да бисте га учинили тако да није више подзадатак његовог првобитно надређеног задатка.</span><span class="sxs-lookup"><span data-stu-id="dd451-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="dd451-151">**Премести нагоре и Премести надоле**.</span><span class="sxs-lookup"><span data-stu-id="dd451-151">**Move up and Move down**.</span></span>   <span data-ttu-id="dd451-152">Померање задатака нагоре и надоле у хијерархији његовог надређеног задатка.</span><span class="sxs-lookup"><span data-stu-id="dd451-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="dd451-153">Премештање задатка нагоре или надоле нема утицаја на његов труд, трошак, датуме или трајање.</span><span class="sxs-lookup"><span data-stu-id="dd451-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="dd451-154">Атрибути задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-154">Task attributes</span></span>  
 <span data-ttu-id="dd451-155">Име задатка описује посао који треба да се доврши.</span><span class="sxs-lookup"><span data-stu-id="dd451-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="dd451-156">Користите различите атрибуте задатка да бисте описали распоред и захтеве запослених на задатку.</span><span class="sxs-lookup"><span data-stu-id="dd451-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="dd451-157">Заказивање атрибута</span><span class="sxs-lookup"><span data-stu-id="dd451-157">Schedule attributes</span></span>

 - <span data-ttu-id="dd451-158">Вредности које доделите за **Часове труда**, **Број ресурса**, **Датум Почетка**, **Датум Завршетка**, и **Трајање** за одређивање распореда задатака.</span><span class="sxs-lookup"><span data-stu-id="dd451-158">Assign values to **Effort hours**, **Number of resources**, **Start date**, **End date**, and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="dd451-159">**Труд** је процена часова потребних за довршавање задатка.</span><span class="sxs-lookup"><span data-stu-id="dd451-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="dd451-160">**Број ресурса** је процена која менаџера пројекта ставља у задатак како би се пронашао најбољи могући распоред.</span><span class="sxs-lookup"><span data-stu-id="dd451-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="dd451-161">**Трајање** (у данима) означава број радних дана који ће бити потребни за довршавање задатка.</span><span class="sxs-lookup"><span data-stu-id="dd451-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="dd451-162">Атрибути запослених</span><span class="sxs-lookup"><span data-stu-id="dd451-162">Staffing attributes</span></span>

 - <span data-ttu-id="dd451-163">**Улога**, **Ресурса организационе јединице**, **Број ресурса**, и **Ресурса** за описивање захтева запосленима за задатак.</span><span class="sxs-lookup"><span data-stu-id="dd451-163">**Role**, **Resource organizational unit**, **Number of resources**, and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="dd451-164">**Улога** описује врсту ресурса потребног за обављање задатка.</span><span class="sxs-lookup"><span data-stu-id="dd451-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="dd451-165">**Ресурс организационе јединице** означава организациону јединицу из које су људски ресурси за тај задатак; ово такође утиче на трошкове и процену продаје задатка, пошто се ово рачуна за одређивање цене продаје по јединици за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="dd451-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="dd451-166">**Ресурси** садрже генеричке ресурсе или назване ресурсе када је један пронађен.</span><span class="sxs-lookup"><span data-stu-id="dd451-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="dd451-167">Зависности задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-167">Task dependencies</span></span>  
 <span data-ttu-id="dd451-168">Можете да креирате претходне односе између једног или више задатака у структурној анализи посла.</span><span class="sxs-lookup"><span data-stu-id="dd451-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="dd451-169">Можете поставити једну или више вредности за поље претходник на задацима да бисте указали на задатке од којих ће зависити.</span><span class="sxs-lookup"><span data-stu-id="dd451-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="dd451-170">Када доделите претходну вредност задатку, задатак можете да покренете једино када довршите све претходне задатке.</span><span class="sxs-lookup"><span data-stu-id="dd451-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="dd451-171">Подешавање ове зависности задатка довешће до поновног прерачунавања датума планиране почетка задатка као најновији крај свих његових претходника.</span><span class="sxs-lookup"><span data-stu-id="dd451-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="dd451-172">Повезани утицај претходника на распоред није ограничен режимом задатка дефинисаног у задатку.</span><span class="sxs-lookup"><span data-stu-id="dd451-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="dd451-173">Режим задатка</span><span class="sxs-lookup"><span data-stu-id="dd451-173">Task mode</span></span>  
 <span data-ttu-id="dd451-174">Режим задатка је једна од важних чинилаца који одређују заказивање задатака чвора листа.</span><span class="sxs-lookup"><span data-stu-id="dd451-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="dd451-175">Постоје два режима задатака за сваки задатак: режим аутоматског заказивања и режим ручног заказивања.</span><span class="sxs-lookup"><span data-stu-id="dd451-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="dd451-176">**Аутоматско заказивање**.</span><span class="sxs-lookup"><span data-stu-id="dd451-176">**Auto scheduling**.</span></span>   <span data-ttu-id="dd451-177">Када подесите режим задатка на Аутоматско заказивање, механизам за заказивање задатака користи правила о праћењу атрибута задатака ради утврђивања распореда за задатак:</span><span class="sxs-lookup"><span data-stu-id="dd451-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="dd451-178">Претходни задаци</span><span class="sxs-lookup"><span data-stu-id="dd451-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="dd451-179">Ангажовање</span><span class="sxs-lookup"><span data-stu-id="dd451-179">Effort</span></span>  
  
    -   <span data-ttu-id="dd451-180">Број ресурса</span><span class="sxs-lookup"><span data-stu-id="dd451-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="dd451-181">Датуми почетка и завршетка</span><span class="sxs-lookup"><span data-stu-id="dd451-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="dd451-182">**Правила планирања**.</span><span class="sxs-lookup"><span data-stu-id="dd451-182">**Scheduling rules**.</span></span>   <span data-ttu-id="dd451-183">Датум почетка задатка чвора листа који нема претходних задатака подразумевано је заказан за почетак пројекта.</span><span class="sxs-lookup"><span data-stu-id="dd451-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="dd451-184">Трајање задатка чвора листа се увек израчунава као број радних дана између његовог почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="dd451-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="dd451-185">Када се задатак аутоматски заказује, механизам за планирање прати правила испод:</span><span class="sxs-lookup"><span data-stu-id="dd451-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="dd451-186">Датуми почетка и завршетка задатка увек морају бити радни дани у складу са календаром за планирање пројекта</span><span class="sxs-lookup"><span data-stu-id="dd451-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="dd451-187">Датум почетка задатка који има претходне задатке је подразумевано последњи датум завршетка претходних задатака</span><span class="sxs-lookup"><span data-stu-id="dd451-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="dd451-188">Труд = Број особа \* Трајање \* часова у стандардном радном дану календара пројекта</span><span class="sxs-lookup"><span data-stu-id="dd451-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="dd451-189">**Ручно планирање**.</span><span class="sxs-lookup"><span data-stu-id="dd451-189">**Manual scheduling**.</span></span>   <span data-ttu-id="dd451-190">У неким случајевима, можда ћете желети да одступите од ових правила.</span><span class="sxs-lookup"><span data-stu-id="dd451-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="dd451-191">У овим случајевима, можете поставити режим задатака на ручно заказивање задатака.</span><span class="sxs-lookup"><span data-stu-id="dd451-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="dd451-192">Зауставља механизам за планирање из израчунавања вредности за друге атрибуте заказивања.</span><span class="sxs-lookup"><span data-stu-id="dd451-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="dd451-193">Подешавање претходних задатака на задатке увек утиче на датум почетка зависног задатка.</span><span class="sxs-lookup"><span data-stu-id="dd451-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="dd451-194">Креирање структурне анализе посла</span><span class="sxs-lookup"><span data-stu-id="dd451-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="dd451-195">Идите на **Project Service > Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="dd451-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="dd451-196">Кликните на пројекат на коме желите да радите.</span><span class="sxs-lookup"><span data-stu-id="dd451-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="dd451-197">На траци у врху екрана изаберите стрелицу надоле поред назива пројекта, а затим кликните на Структурну анализу посла.</span><span class="sxs-lookup"><span data-stu-id="dd451-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="dd451-198">Да бисте додали задатак, кликните на дугме **Додај Задатак**.</span><span class="sxs-lookup"><span data-stu-id="dd451-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="dd451-199">Попуните поља за задатак, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="dd451-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="dd451-200">Наставите додавање задатака док се не заврши структурна анализа посла.</span><span class="sxs-lookup"><span data-stu-id="dd451-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="dd451-201">Приликом креирања структурне анализе посла, можете урадити следеће да бисте организовали своје задатке:</span><span class="sxs-lookup"><span data-stu-id="dd451-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="dd451-202">Изаберите задатак и кликните на дугме **Увуци** да бисте га преместили у други задатак или Извуци да бисте преместили изван нивоа.</span><span class="sxs-lookup"><span data-stu-id="dd451-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="dd451-203">Изаберите задатак и кликните на дугме **Премести нагоре** или **Премести надоле** да бисте га преместили нагоре или надоле на листи.</span><span class="sxs-lookup"><span data-stu-id="dd451-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="dd451-204">Кликните на дугме **Сакриј гантограм** да бисте сакрили гантограм и кликните на дугме **Прикажи гантограм** да бисте га поново приказали.</span><span class="sxs-lookup"><span data-stu-id="dd451-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="dd451-205">Изаберите други период времена за гантограм у опцији **Временска скала**.</span><span class="sxs-lookup"><span data-stu-id="dd451-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="dd451-206">Да бисте додали улоге које сте навели у вашу структурну анализу посла за чланове тима вашег пројекта, кликните на дугме **Генерисање тима за пројекат**.</span><span class="sxs-lookup"><span data-stu-id="dd451-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="dd451-207">Кликните на дугме **Сачувај** у доњем десном углу екрана када завршите са уношењем измена.</span><span class="sxs-lookup"><span data-stu-id="dd451-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="dd451-208">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="dd451-208">See Also</span></span>  
 [<span data-ttu-id="dd451-209">Водич за менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="dd451-209">Project manager guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]