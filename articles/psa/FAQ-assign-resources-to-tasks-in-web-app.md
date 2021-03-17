---
title: Како да доделим ресурс који може да се резервише задатку у веб апликацији
description: Преглед начина на који можете доделити ресурсе које је могуће доделити.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: b4296837cabd4c6f7e2d2924079658e45ce8b87c
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286311"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="6b1a6-103">Како да додељујете ресурс који може да се резервише задатку у веб апликацији (апликација Project Service v2.x)?</span><span class="sxs-lookup"><span data-stu-id="6b1a6-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6b1a6-104">Постоје два начина доделе ресурса задатку у програму Project Service.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="6b1a6-105">Ресурс можете да резервишете као члан тима, а затим да га доделите задатку.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="6b1a6-106">Или можете да креирате генеричког члана тима преко доделе улога на задацима, генерисања тима, а затим попуњавањем захтева за прављење резервне копије са именованим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="6b1a6-107">Имајте у виду да ако желите да доделите ресурс који може да се резервише задатку, члан тима ресурса који може да се резервише мора да има довољно доступних резервација.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="6b1a6-108">Статус резервације мора да буде тип извршавања Фиксно резервиши и са статусом Извршено.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="6b1a6-109">Ако нема довољно резервација за ресурс, Project Service уклања задатак и приказује следећу поруку о грешци:</span><span class="sxs-lookup"><span data-stu-id="6b1a6-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="6b1a6-110">*Није могуће доделити ресурс задатку – Следеће ресурси немају довољно резервисаних радних сати за пројекат*</span><span class="sxs-lookup"><span data-stu-id="6b1a6-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="6b1a6-111">Резервишите ресурс као члан тима, а затим доделите ресурс задатку</span><span class="sxs-lookup"><span data-stu-id="6b1a6-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="6b1a6-112">Са овим методом додајете ресурс у пројектни тим, а затим додељујете задатке ресурсу у распореду пројекта.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="6b1a6-113">Ево како то да урадите:</span><span class="sxs-lookup"><span data-stu-id="6b1a6-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="6b1a6-114">У координатној мрежи члана тима додајте новог члана тима тако што ћете изабрати **Нови**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="6b1a6-115">На екрану брзог креирања члана тима, изаберите име ресурса који може да се резервише и подесите улогу.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="6b1a6-116">Изаберите датуме **Од** и **До**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="6b1a6-117">![Снимак екрана додавања члана тима](media/FAQ-Resources-to-Tasks2-1.png "Снимак екрана додавања члана тима")</span><span class="sxs-lookup"><span data-stu-id="6b1a6-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="6b1a6-118">Изаберите један од следећих начина доделе за резервацију ресурса:</span><span class="sxs-lookup"><span data-stu-id="6b1a6-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="6b1a6-119">**Пун капацитет** резервише пуни капацитет ресурса за наведене почетне и крајње датуме.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="6b1a6-120">**Проценат капацитета** резервише одређени проценат капацитета ресурса за наведене датуме почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="6b1a6-121">**По сатима – Равномерно распоређивање** резервише ресурс за одређени број часова, равномерно их распоређујући по дану током наведених датума почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="6b1a6-122">**По сатима – Почетно оптерећење** резервише ресурс за одређени број часова, распоређујући часове рада по дану на прве дане током наведених датума почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="6b1a6-123">Немојте изабрати **Ниједно** јер он додаје ресурс тиму, али не креира ниједну резервацију која троши капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="6b1a6-124">Изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-124">Select **Save**.</span></span>

    <span data-ttu-id="6b1a6-125">Имајте у виду да сати резервације морају да буду довољни да покрију часове ангажовања и периоде датума задатака којима додељујете овај ресурс.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="6b1a6-126">Ако они нису усклађени, не можете доделити ресурс задатку.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="6b1a6-127">На структурној анализи посла (САП) за задатак, кликните на падајући мени ћелија ресурса.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="6b1a6-128">Затим:</span><span class="sxs-lookup"><span data-stu-id="6b1a6-128">Then:</span></span> 

    1. <span data-ttu-id="6b1a6-129">Изаберите **Додај**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-129">Select **Add**.</span></span>
    2. <span data-ttu-id="6b1a6-130">Изаберите падајући мени у оквиру опције **Ресурси** и изаберите члана тима којег сте додали изнад.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="6b1a6-131">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-131">Select **OK**.</span></span> <span data-ttu-id="6b1a6-132">Члан тима је сада додељен задатку.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="6b1a6-133">![Снимак екрана додавања ресурса помоћу САП-а](media/FAQ-Resources-to-Tasks2-2.png "Снимак екрана додавања ресурса помоћу САП-а")</span><span class="sxs-lookup"><span data-stu-id="6b1a6-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="6b1a6-134">У координатној мрежи члана тима, у оквиру ставке Додељени часови видећете агрегиране додељене радне сате ресурса.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="6b1a6-135">То ће бити мање или једнако резервисаним часовима за ресурс.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="6b1a6-136">![Снимак екрана додељених часова ресурсу](media/FAQ-Resources-to-Tasks2-3.png "Снимак екрана додељених часова ресурсу")</span><span class="sxs-lookup"><span data-stu-id="6b1a6-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="6b1a6-137">Ако задатак који покушавате да доделите ресурсу почиње након датума завршетка резервација ресурса, ресурс се неће појавити на падајућој листи.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="6b1a6-138">Имајте у виду да ресурсу можете да доделите више часова него што су његови резервисани часови ако ресурс има преостали недодељени капацитет.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="6b1a6-139">У том случају, ресурс ће бити само делимично додељен до његових резервација.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="6b1a6-140">Те преостале недодељене сате можете да видите додавањем колоне Часови без ресурса у структурну анализу посла.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="6b1a6-141">Ако су ресурси додељени својим резервисаним часовима (њихови резервисани часови су једнаки њиховим додељеним часовима), видећете следећу поруку о грешци када покушате да им доделите још задатака:</span><span class="sxs-lookup"><span data-stu-id="6b1a6-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="6b1a6-142">*Није могуће доделити ресурс задатку – Следеће ресурси немају довољно резервисаних радних сати за пројекат.*</span><span class="sxs-lookup"><span data-stu-id="6b1a6-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="6b1a6-143">Осим тога, подразумевани члан тима менаџера пројекта који је додат у тим када сте креирали пројекат се додаје без икаквих резервација и није му могуће доделити ниједан задатак.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="6b1a6-144">Он се неће приказивати у падајућој листи ресурса за задатак.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="6b1a6-145">Ако желите да доделите овај ресурс, потребно је да га уклоните из тима, а затим поново да га додате са начином доделе који није Ниједно.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="6b1a6-146">Разлог због ког се додају тиму када се пројекат креира јесте да би пројекат имао бар једну подразумевану особу која одобрава пројекат.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="6b1a6-147">Креирање генеричког члана тима преко доделе улога за задатке</span><span class="sxs-lookup"><span data-stu-id="6b1a6-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="6b1a6-148">Овај метод осигурава да ресурси имају довољно резервација за задатке.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="6b1a6-149">Као прво, креирате чувар места или генерички ресурс који описује карактеристике именованог ресурса за којег напослетку желите да ради на задацима генерисањем тима након доделе улога задацима.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="6b1a6-150">Ево како то да урадите:</span><span class="sxs-lookup"><span data-stu-id="6b1a6-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="6b1a6-151">На структурној анализи посла, изаберите задатак.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="6b1a6-152">Изаберите икону падајућег листе **Додељена улога** у ћелији ресурса.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="6b1a6-153">Изаберите падајућу листу **Улога** и изаберите улогу за генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="6b1a6-154">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="6b1a6-155">![Снимак екрана коришћења САП-а за додавање ресурса](media/FAQ-Resources-to-Tasks2-4.png "Снимак екрана коришћења САП-а за додавање ресурса")</span><span class="sxs-lookup"><span data-stu-id="6b1a6-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="6b1a6-156">Након што сте довршили додељивање улога задацима у САП-у, изаберите **Генерисање пројектног тима**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="6b1a6-157">Project Service креира минимални број генеричких чланова тима на основу улога, јединица за одређивање ресурса организације и календара пројекта агрегирањем додела задатка.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="6b1a6-158">![Снимак екрана генерисања пројектног тима](media/FAQ-Resources-to-Tasks2-5.png "Снимак екрана генерисања пројектног тима")</span><span class="sxs-lookup"><span data-stu-id="6b1a6-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="6b1a6-159">На координатној мрежи члана тима видећете ресурсе типа Генерички ресурс са улогом и именом положаја.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="6b1a6-160">Ако су потребна два ресурса за улогу како бисте довршили рад, функција Генерисање тима креира два члана тима и користи име положаја како би их разликовала.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="6b1a6-161">![Снимак екрана додавања два генеричка ресурса](media/FAQ-Resources-to-Tasks2-6.png "Снимак екрана додавања два генеричка ресурса")</span><span class="sxs-lookup"><span data-stu-id="6b1a6-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="6b1a6-162">Можете отворити захтев за прављење резервне копије ресурса за генеричког члана тима тако што ћете изабрати везу у оквиру опције Захтев за ресурс.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="6b1a6-163">![Снимак екрана отварања захтева за прављење резервне копије ресурса](media/FAQ-Resources-to-Tasks2-7.png "Снимак екрана отварања захтева за прављење резервне копије ресурса")</span><span class="sxs-lookup"><span data-stu-id="6b1a6-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="6b1a6-164">Изаберите ставку **Резервиши** за генерички ресурс, а затим можете да користите табелу распореда да бисте пронашли и резервисали стварни ресурс.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="6b1a6-165">Можете у да проследите захтев за испуњење по менаџеру ресурса тако што ћете изабрати **Проследи захтев**.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="6b1a6-166">Када генерички ресурс буде испуњен именованим ресурсом, генерички ресурс се уклања из тима, а доделе задатка из генеричког ресурса се додељују именованом ресурсу који је испунио захтев за ресурсом генеричког ресурса.</span><span class="sxs-lookup"><span data-stu-id="6b1a6-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 



[!INCLUDE[footer-include](../includes/footer-banner.md)]