---
title: Процена продају и трошкова пројекта када ресурс који може да се резервише испуњава више улога у пројекту
description: У овој теми се пружају информације о томе како се димензије цене могу користити за подршку одређивању цена и трошкова за ресурс који испуњава више улога у пројекту.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 8ddc827a4170c5576c0a4350b51e6a119094ac50
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084024"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-mulitple-roles-on-a-project"></a><span data-ttu-id="181a3-103">Процена продају и трошкова пројекта када ресурс који може да се резервише испуњава више улога у пројекту</span><span class="sxs-lookup"><span data-stu-id="181a3-103">Estimate project sales and costs when a bookable resource fills mulitple roles on a project</span></span> 

<span data-ttu-id="181a3-104">Компаније засноване на пројекту често имају потребу да један ресурсом обавља више улога на пројекту.</span><span class="sxs-lookup"><span data-stu-id="181a3-104">Project-based companies often have the need for one resource to perform mulitple roles on a project.</span></span> <span data-ttu-id="181a3-105">Цене и трошкови за сваку од ових улога могу се различито одредити, што значи да време истог ресурса на пројекту може добити различиту финансијску процену у зависности од наплате и стопе трошкова за сваку од улога.</span><span class="sxs-lookup"><span data-stu-id="181a3-105">Each of these roles could be priced and costed differently which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="181a3-106">Project Service Automation омогућава подешавање вредности у запису члана тима за именовани ресурс и омогућава различите замене за сваки од задатака којима је додељен члан тима.</span><span class="sxs-lookup"><span data-stu-id="181a3-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="181a3-107">Следећи пример објашњава како једноставна измена ове вредности омогућава ресурсу да има више улога у пројекту са различитим трошковима и стопама наплате.</span><span class="sxs-lookup"><span data-stu-id="181a3-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="181a3-108">Креирање задатака</span><span class="sxs-lookup"><span data-stu-id="181a3-108">Create tasks</span></span>
<span data-ttu-id="181a3-109">Направите два пројектна задатка по 40 сати, задатак А и задатак Б. Изаберите задатак А као претходника задатка Б.</span><span class="sxs-lookup"><span data-stu-id="181a3-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="181a3-110">Подешавање улоге и организационе јединице за генеричког члана пројектног тима</span><span class="sxs-lookup"><span data-stu-id="181a3-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="181a3-111">На страници **Распоред** изаберите ред **Задатак** за задатак А.</span><span class="sxs-lookup"><span data-stu-id="181a3-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="181a3-112">У пољу **Ресурси** изаберите **Креирај** у падајућој листи.</span><span class="sxs-lookup"><span data-stu-id="181a3-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="181a3-113">На страници **Брзо креирање члана тима** , наведите атрибуте генеричког члана тима који може да изврши овај задатак.</span><span class="sxs-lookup"><span data-stu-id="181a3-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="181a3-114">Изаберите одговарајућу улогу и организациону јединицу, а затим изаберите **Сачувај и затвори**.</span><span class="sxs-lookup"><span data-stu-id="181a3-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="181a3-115">Генерички члан тима се креира и додељује овом задатку.</span><span class="sxs-lookup"><span data-stu-id="181a3-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="181a3-116">Поновите ове кораке за задатак Б и уверите се да се улога и организациона јединица генеричког члана тима креираног за задатак Б разликује од задатка А.</span><span class="sxs-lookup"><span data-stu-id="181a3-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="181a3-117">Подешавање улоге и организационе јединице за пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="181a3-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="181a3-118">Када креирате задатак А, изаберите задатак, а затим изаберите **Уређуј задатак**.</span><span class="sxs-lookup"><span data-stu-id="181a3-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="181a3-119">На страници **Детаљи задатка** пронађите поља **Улога** и **Организациона јединица** , додајте вредности потребне за ресурс који би извршио овај задатак.</span><span class="sxs-lookup"><span data-stu-id="181a3-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="181a3-120">Ако довршавате ове сценарије користећи Project Service Automation демо податке, изаберите **Вођа консултаната** за улогу и **Fabrikam US** као организациону јединицу.</span><span class="sxs-lookup"><span data-stu-id="181a3-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="181a3-121">Изаберите задатак Б, а затим изаберите **Уреди задатак**.</span><span class="sxs-lookup"><span data-stu-id="181a3-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="181a3-122">На страници **Детаљи задатка** пронађите поља **Улога** и **Организациона јединица** , додајте вредности потребне за ресурс који би извршио овај задатак.</span><span class="sxs-lookup"><span data-stu-id="181a3-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="181a3-123">Уверите се да се вредности у пољима **Улога** и **Организациона јединица** за задатак Б разликују од оних за задатак А.</span><span class="sxs-lookup"><span data-stu-id="181a3-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from those for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="181a3-124">Ако довршавате ове сценарије користећи Project Service Automation демо податке, изаберите **Техничар мреже** за улогу и **Fabrikam US** као организациону јединицу.</span><span class="sxs-lookup"><span data-stu-id="181a3-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="181a3-125">Сачувајте и затворите страницу **Детаљи задатка**.</span><span class="sxs-lookup"><span data-stu-id="181a3-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behaviour"></a><span data-ttu-id="181a3-126">Члан тима и процена понашања</span><span class="sxs-lookup"><span data-stu-id="181a3-126">Team member and estimates behaviour</span></span> 

1. <span data-ttu-id="181a3-127">На страници **Детаљи задатка** , у одељку **Члан тима** , изаберите два члана генеричког тима, а затим изаберите **Генериши захтеве**.</span><span class="sxs-lookup"><span data-stu-id="181a3-127">On the **Task Details** page, on the **Team Member** , select the two generic team Members and then select **Generate Requirements**.</span></span> <span data-ttu-id="181a3-128">Тако ћете генерисати захтеве за ресурсима.</span><span class="sxs-lookup"><span data-stu-id="181a3-128">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="181a3-129">Изаберите ред члана тима за **Вођа консултаната** , а затим изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="181a3-129">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="181a3-130">Табела распореда се отвара и резервише ресурс за тај захтев.</span><span class="sxs-lookup"><span data-stu-id="181a3-130">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="181a3-131">Изаберите ред члана тима за **Техничар мреже** , а затим изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="181a3-131">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="181a3-132">Табела распореда се отвара и резервише исти ресурс за тај захтев.</span><span class="sxs-lookup"><span data-stu-id="181a3-132">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="181a3-133">Мрежа члана тима</span><span class="sxs-lookup"><span data-stu-id="181a3-133">Team Member grid</span></span> 
<span data-ttu-id="181a3-134">На мрежи **Члан тима** , уочите да су два генеричка записа чланова тима избрисана и да су замењена једним ресурсом.</span><span class="sxs-lookup"><span data-stu-id="181a3-134">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="181a3-135">Постоји један скуп вредности за тај ресурс који приказује задати скуп вредности за **улогу** и **организациону јединицу**.</span><span class="sxs-lookup"><span data-stu-id="181a3-135">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="181a3-136">Када проширите ред тог записа члана тима, на запису члана тима можете видети различите задатке за оба та задатка.</span><span class="sxs-lookup"><span data-stu-id="181a3-136">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="181a3-137">Сваки ред задатка има вредности специфичне за задатак за **улогу** и **организациону јединицу**.</span><span class="sxs-lookup"><span data-stu-id="181a3-137">Each assignment row has task specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="181a3-138">Мрежа процена</span><span class="sxs-lookup"><span data-stu-id="181a3-138">Estimates grid</span></span> 
<span data-ttu-id="181a3-139">Када одете на мрежу **Процене** , приметићете да обе доделе за исти ресурс имају различито одређене цене.</span><span class="sxs-lookup"><span data-stu-id="181a3-139">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="181a3-140">Цена доделе ресурса задатку А одређује се коришћењем вредности атрибута **Улога** за **вођу консултаната**.</span><span class="sxs-lookup"><span data-stu-id="181a3-140">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="181a3-141">Цена доделе истог ресурса задатку Б одређује се коришћењем вредности атрибута **Улога** за **техничара мреже**.</span><span class="sxs-lookup"><span data-stu-id="181a3-141">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>





