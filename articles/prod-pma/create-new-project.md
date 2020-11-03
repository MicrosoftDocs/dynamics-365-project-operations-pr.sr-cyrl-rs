---
title: Креирајте нови пројекат
description: Ова тема пружа информације о томе како да креирате нов пројекат.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 727d287c571b2a64bf10b2393a87567093a420d2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084107"
---
# <a name="create-a-new-project"></a><span data-ttu-id="f4067-103">Креирајте нови пројекат</span><span class="sxs-lookup"><span data-stu-id="f4067-103">Create a new project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f4067-104">Обавите следеће кораке да бисте креирали нови пројекат.</span><span class="sxs-lookup"><span data-stu-id="f4067-104">Complete the following steps to create a new project.</span></span>

1. <span data-ttu-id="f4067-105">На страници **Менаџмент пројекта** изаберите **Нови пројекат** и унесите следеће вредности:</span><span class="sxs-lookup"><span data-stu-id="f4067-105">On the **Project management** page, select **New project** , and enter the following values:</span></span>

    - <span data-ttu-id="f4067-106">**Тип пројекта:** Време и материјал</span><span class="sxs-lookup"><span data-stu-id="f4067-106">**Project type:** Time and material</span></span>
    - <span data-ttu-id="f4067-107">**Назив пројекта:** Надоградња XYZ фаза 2</span><span class="sxs-lookup"><span data-stu-id="f4067-107">**Project name:** XYZ Upgrade Phase 2</span></span>
    - <span data-ttu-id="f4067-108">**Група пројеката:** TM\_WIP</span><span class="sxs-lookup"><span data-stu-id="f4067-108">**Project group:** TM\_WIP</span></span>
    - <span data-ttu-id="f4067-109">**ID уговора о пројекту:** 00000002</span><span class="sxs-lookup"><span data-stu-id="f4067-109">**Project contract ID:** 00000002</span></span>

2. <span data-ttu-id="f4067-110">Изаберите **Креирајте пројекат**.</span><span class="sxs-lookup"><span data-stu-id="f4067-110">Select **Create project**.</span></span>

## <a name="assign-a-resource-to-a-project"></a><span data-ttu-id="f4067-111">Додељивање ресурса пројекту</span><span class="sxs-lookup"><span data-stu-id="f4067-111">Assign a resource to a project</span></span>

1. <span data-ttu-id="f4067-112">На страници **Радници** , на листи **Радници** , изаберите запис за радника за којег сте претходно подесили компетенције и отворите запис радника.</span><span class="sxs-lookup"><span data-stu-id="f4067-112">On the **Workers** page, in the **Workers** list, select the record for the worker that you previously set up competencies for, and open the worker record.</span></span>
2. <span data-ttu-id="f4067-113">У окну радњи, на картици **Пројекат** , у групи **Подешавање** изаберите **Додели пројекте**.</span><span class="sxs-lookup"><span data-stu-id="f4067-113">On the Action Pane, on the **Project** tab, in the **Setup** group, select **Assign projects**.</span></span>
3. <span data-ttu-id="f4067-114">На страници **Доделе пројеката за валидацију ресурса** , на картици **Пројекти** , у пољу **Додај пројекат изабраним пројектима** , филтрирајте према пројекту **Надоградња XYZ фаза 2**.</span><span class="sxs-lookup"><span data-stu-id="f4067-114">On the **Resource validation project assignments** page, on the **Projects** tab, in the **Add the project to selected projects** field, filter on the **XYZ Upgrade Phase 2** project.</span></span>
4. <span data-ttu-id="f4067-115">У окну **Преостали пројекти** , изаберите пројекат, а затим изаберите дугме са стрелицом да бисте га додали у окно **Изабрани пројекти**.</span><span class="sxs-lookup"><span data-stu-id="f4067-115">In the **Remaining projects** pane, select a project, and then select the arrow button to add it to the **Selected projects** pane.</span></span>

<span data-ttu-id="f4067-116">Такође можете да доделите категорије за ресурс по потреби.</span><span class="sxs-lookup"><span data-stu-id="f4067-116">You can also assign categories for a resource as you require.</span></span> <span data-ttu-id="f4067-117">Тип категорије је или **Трошак** или **Приход**.</span><span class="sxs-lookup"><span data-stu-id="f4067-117">The category type is either **Cost** or **Revenue**.</span></span> <span data-ttu-id="f4067-118">Тип категорије одређује ваша организација.</span><span class="sxs-lookup"><span data-stu-id="f4067-118">The category type is determined by your organization.</span></span> <span data-ttu-id="f4067-119">Ако за ресурс нису додељене категорије, Finance тражи подразумевану категорију цена по сату за трошкове и приход.</span><span class="sxs-lookup"><span data-stu-id="f4067-119">If no categories are assigned for a resource, Finance looks up the default category on hour prices for cost and revenue.</span></span>

## <a name="set-up-project-resource-and-role-characteristics"></a><span data-ttu-id="f4067-120">Подешавање карактеристика и улога ресурса пројекта</span><span class="sxs-lookup"><span data-stu-id="f4067-120">Set up project resource and role characteristics</span></span>

<span data-ttu-id="f4067-121">Менаџер пројекта може користити функционалност ресурса за пројекат да би креирао улоге потребне за пројекат.</span><span class="sxs-lookup"><span data-stu-id="f4067-121">A project manager can use the project resourcing functionality to create the roles that are required for the project.</span></span> <span data-ttu-id="f4067-122">Улоге се могу користити ако су потврђени ресурси и даље непознати када се ресурси резервишу.</span><span class="sxs-lookup"><span data-stu-id="f4067-122">Roles can be used if confirmed resources are still unknown when resources are being reserved.</span></span> <span data-ttu-id="f4067-123">Улоге се могу привремено резервисати као планирани ресурси, тако да можете наставити фазе планирања пројекта.</span><span class="sxs-lookup"><span data-stu-id="f4067-123">Roles can be temporarily reserved as planned resources, so that you can continue the project planning stages.</span></span>

<span data-ttu-id="f4067-124">[![Пример улоге](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span><span class="sxs-lookup"><span data-stu-id="f4067-124">[![Example of a role](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span></span> 

<span data-ttu-id="f4067-125">**Сценарио:** Contoso је ангажован да заврши пројекат Време и материјал који има одобрену повељу пројекта.</span><span class="sxs-lookup"><span data-stu-id="f4067-125">**Scenario:** Contoso was hired to complete a Time and material project that has an approved project charter.</span></span> <span data-ttu-id="f4067-126">Млађи менаџер пројекта још увек довршава опсег пројекта.</span><span class="sxs-lookup"><span data-stu-id="f4067-126">The junior project manager is still completing the scope of the project.</span></span> <span data-ttu-id="f4067-127">Менаџер ресурса тренутно идентификује одређене ресурсе који ће бити резервисани за рад на новом пројекту.</span><span class="sxs-lookup"><span data-stu-id="f4067-127">The resource manager is currently identifying specific resources that will be reserved to work on the new project.</span></span> <span data-ttu-id="f4067-128">Због критичне природе пројекта, спонзор пројекта затражио је старијег менаџера пројекта као једну од улога.</span><span class="sxs-lookup"><span data-stu-id="f4067-128">Because of the critical nature of the project, the project sponsor requested Senior project manager as one of the roles.</span></span> <span data-ttu-id="f4067-129">Менаџер ресурса мора набавити нови ресурс и дефинисати улогу у систему у случају да млађи менаџер пројекта захтева информације о ресурсима током планирања пројекта.</span><span class="sxs-lookup"><span data-stu-id="f4067-129">The resource manager must acquire the new resource and define the role in the system in case the junior project manager requires the resource information during project planning.</span></span>

<span data-ttu-id="f4067-130">Следећи кораци показују како менаџер ресурса може да постави улогу вишег менаџера пројекта и повеже карактеристике ресурса са њом.</span><span class="sxs-lookup"><span data-stu-id="f4067-130">The following steps show how the resource manager can set up the Senior project manager role and associate resource characteristics with it.</span></span> <span data-ttu-id="f4067-131">Касније се улога може користити за тражење доступних ресурса који одговарају траженим компетенцијама ресурса.</span><span class="sxs-lookup"><span data-stu-id="f4067-131">Later, the role can be used to search for available resources that match the required resource competencies.</span></span>

1. <span data-ttu-id="f4067-132">На страници **Подешавање улога** изаберите **Нова** и унесите следеће вредности:</span><span class="sxs-lookup"><span data-stu-id="f4067-132">On the **Setup roles** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="f4067-133">**ID улоге:** Виши менаџер пројекта</span><span class="sxs-lookup"><span data-stu-id="f4067-133">**Role ID:** Senior Project Manager</span></span>
    - <span data-ttu-id="f4067-134">**Опис:** Виши менаџер пројекта</span><span class="sxs-lookup"><span data-stu-id="f4067-134">**Description:** Senior Project Manager</span></span>

2. <span data-ttu-id="f4067-135">Изаберите **Креирај**.</span><span class="sxs-lookup"><span data-stu-id="f4067-135">Select **Create**.</span></span>
3. <span data-ttu-id="f4067-136">Изаберите улогу **Виши менаџер пројекта** , а затим изаберите **Конфигуриши карактеристике**.</span><span class="sxs-lookup"><span data-stu-id="f4067-136">Select the **Senior Project Manager** role, and then select **Configure characteristics**.</span></span>
4. <span data-ttu-id="f4067-137">У пољу **Тип карактеристике** , изаберите **Вештина**.</span><span class="sxs-lookup"><span data-stu-id="f4067-137">In the **Characteristics type** field, select **Skill**.</span></span>
5. <span data-ttu-id="f4067-138">У пољу **Доступне карактеристике** , унесите вештину за тражење.</span><span class="sxs-lookup"><span data-stu-id="f4067-138">In the **Available characteristics** field, enter the skill to search for.</span></span>
6. <span data-ttu-id="f4067-139">У пољу **Тип карактеристике** , изаберите **Цертификат**.</span><span class="sxs-lookup"><span data-stu-id="f4067-139">In the **Characteristic type** field, select **Certificate**.</span></span>
7. <span data-ttu-id="f4067-140">У пољу **Доступне карактеристике** , унесите тип цертификата за тражење.</span><span class="sxs-lookup"><span data-stu-id="f4067-140">In the **Available characteristics** field, enter the certificate type to search for.</span></span>

## <a name="assign-a-project-resource-to-a-project"></a><span data-ttu-id="f4067-141">Додељивање ресурса пројекту</span><span class="sxs-lookup"><span data-stu-id="f4067-141">Assign a project resource to a project</span></span>

1. <span data-ttu-id="f4067-142">На страници **Сви пројекти** изаберите пројекат **Надоградња XYZ фаза 2**.</span><span class="sxs-lookup"><span data-stu-id="f4067-142">On the **All projects** page, select the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="f4067-143">На картици **Пројектни тим и распоређивање** , изаберите **Додај**.</span><span class="sxs-lookup"><span data-stu-id="f4067-143">On the **Project team and scheduling** tab, select **Add**.</span></span>
3. <span data-ttu-id="f4067-144">У пољу **Улога** изаберите **Члан тима**.</span><span class="sxs-lookup"><span data-stu-id="f4067-144">In the **Role** field, select **Team member**.</span></span>
4. <span data-ttu-id="f4067-145">Изаберите **Резервиши из календара**.</span><span class="sxs-lookup"><span data-stu-id="f4067-145">Select **Book from calendar**.</span></span>
5. <span data-ttu-id="f4067-146">На страници **Доступност ресурса** изаберите **Погледајте подешавања**.</span><span class="sxs-lookup"><span data-stu-id="f4067-146">On the **Resource availability** page, select **View settings**.</span></span>
6. <span data-ttu-id="f4067-147">На страници **Прилагодите поставке приказа** , унесите следеће вредности:</span><span class="sxs-lookup"><span data-stu-id="f4067-147">On the **Adjust view settings** page, enter the following values:</span></span>

    - <span data-ttu-id="f4067-148">**Формат за приказ опсега датума:** Дан</span><span class="sxs-lookup"><span data-stu-id="f4067-148">**Format for date range view:** Day</span></span>
    - <span data-ttu-id="f4067-149">**Прикажи описе доступности:** Да</span><span class="sxs-lookup"><span data-stu-id="f4067-149">**Display availability descriptions:** Yes</span></span>
    - <span data-ttu-id="f4067-150">**Прикажи преостали капацитет:** Да</span><span class="sxs-lookup"><span data-stu-id="f4067-150">**Display remaining capacity:** Yes</span></span>

7. <span data-ttu-id="f4067-151">Изаберите ресурс у листи ресурса.</span><span class="sxs-lookup"><span data-stu-id="f4067-151">In the list of resources, select a resource.</span></span>
8. <span data-ttu-id="f4067-152">Изаберите **Фиксна резервација** и **Пуни капацитет**.</span><span class="sxs-lookup"><span data-stu-id="f4067-152">Select **Hard book** and **Full capacity**.</span></span>

## <a name="assign-a-resource-to-a-default-role"></a><span data-ttu-id="f4067-153">Додељивање ресурса подразумеваној улози</span><span class="sxs-lookup"><span data-stu-id="f4067-153">Assign a resource to a default role</span></span>

<span data-ttu-id="f4067-154">Да би помогли менаџерима пројеката или ресурса да даље дубински претражују ресурсе који могу бити резервисани за пројекат.</span><span class="sxs-lookup"><span data-stu-id="f4067-154">To help project or resource managers can drill down further on the resources that can be reserved for a project.</span></span> <span data-ttu-id="f4067-155">Подразумевану улогу можете повезати са постојећим или новостеченим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="f4067-155">You can associate a default role with an existing resource or a newly acquired resource.</span></span> <span data-ttu-id="f4067-156">На пример, када је Данијел запослен, имао је искуство и вештине да попуни улогу пословног аналитичара.</span><span class="sxs-lookup"><span data-stu-id="f4067-156">For example, when Daniel was hired, he had the experience and skills to fill the Business analyst role.</span></span> <span data-ttu-id="f4067-157">Менаџер ресурса доделио је ову улогу Данијелу као подразумевану.</span><span class="sxs-lookup"><span data-stu-id="f4067-157">The resource manager assigned this role as Daniel's default role.</span></span> <span data-ttu-id="f4067-158">Стога је менаџер ресурса додао Данијела у скуп пословних аналитичара који су доступни за рад на пројектима.</span><span class="sxs-lookup"><span data-stu-id="f4067-158">Therefore, the resource manager added Daniel to a pool of business analysts who are available to work on projects.</span></span>

<span data-ttu-id="f4067-159">Током резервације ресурса, менаџери пројеката могу филтрирати ресурсе улога који су доступни за рад на пројектима.</span><span class="sxs-lookup"><span data-stu-id="f4067-159">During resource reservation, project managers can filter the role resources that are available to work on projects.</span></span> <span data-ttu-id="f4067-160">Ове информације могу да користе као један критеријум када обављају анализу одлука према више критеријума током попуњавања ресурса.</span><span class="sxs-lookup"><span data-stu-id="f4067-160">They can use this information as one criterion when they perform multi-criteria decision analysis during resource fulfillment.</span></span> <span data-ttu-id="f4067-161">Они такође могу да додају друге карактеристике ресурса у филтер за тражење ресурса који имају специфичне вештине, образовање и искуство за дати пројекат.</span><span class="sxs-lookup"><span data-stu-id="f4067-161">They can also add other resource characteristics to the filter to search for resources that have specific skills, education, and experience for a given project.</span></span>

<span data-ttu-id="f4067-162">**Сценарио:** Одобрени пројекат је започео, а улога вишег менаџера пројекта била је резервисана као планирани ресурс током фазе планирања пројекта.</span><span class="sxs-lookup"><span data-stu-id="f4067-162">**Scenario:** An approved project has started, and the Senior project manager role was reserved as a planned resource during the project planning stage.</span></span> <span data-ttu-id="f4067-163">Менаџер ресурса је сада набавио ресурс за испуњавање улоге вишег менаџера пројекта.</span><span class="sxs-lookup"><span data-stu-id="f4067-163">The resource manager has now acquired a resource to fulfill the Senior project manager role.</span></span>

1. <span data-ttu-id="f4067-164">На страници **Листа ресурса** , изаберите **Данијел Голдшмит**.</span><span class="sxs-lookup"><span data-stu-id="f4067-164">On the **Resources list** page, select **Daniel Goldschmidt**.</span></span>
2. <span data-ttu-id="f4067-165">На страници **Улога ресурса** изаберите **Нова** и унесите следеће вредности:</span><span class="sxs-lookup"><span data-stu-id="f4067-165">On the **Resource role** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="f4067-166">**Ступа на снагу:** Унесите тренутни датум.</span><span class="sxs-lookup"><span data-stu-id="f4067-166">**Effective:** Enter the current date.</span></span>
    - <span data-ttu-id="f4067-167">**Истицање:** Унесите **Никад**.</span><span class="sxs-lookup"><span data-stu-id="f4067-167">**Expiration:** Enter **Never**.</span></span>
    - <span data-ttu-id="f4067-168">**Улога:** Унесите **Виши менаџер пројекта**.</span><span class="sxs-lookup"><span data-stu-id="f4067-168">**Role:** Enter **Senior Project Manager**.</span></span>

3. <span data-ttu-id="f4067-169">Изаберите **Сачувај** , а затим затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="f4067-169">Select **Save** , and then close the page.</span></span>
4. <span data-ttu-id="f4067-170">На картици **Компетенције** , додајте вештину **Менаџмент пројекта** и **PMP** цертификат.</span><span class="sxs-lookup"><span data-stu-id="f4067-170">On the **Competencies** tab, add the **ProjectMgmt** skill and the **PMP** certificate.</span></span>
