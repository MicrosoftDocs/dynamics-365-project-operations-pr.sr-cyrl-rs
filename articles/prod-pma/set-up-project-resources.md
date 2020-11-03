---
title: Подешавање ресурса пројекта
description: Ова тема пружа информације о подешавању или захтевању ресурса пројекта.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 7eec8ad5d78019219b2e04ca75eeaa5a3c8a748f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084144"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="b4fe6-103">Подешавање ресурса пројекта</span><span class="sxs-lookup"><span data-stu-id="b4fe6-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b4fe6-104">Морате поставити календар и повезати га са запосленим или радником.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="b4fe6-105">Календар се користи за планирање пројекта и радно време ресурса који су резервисани за пројекат.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="b4fe6-106">Током подешавања календара, менаџери пројеката могу извршити нивелисање ресурса као део оптимизације ресурса.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="b4fe6-107">На основу календарског распореда, ресурси се могу ограничити.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="b4fe6-108">Календар можете подесити на страници **Календари**.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="b4fe6-109">Када радника поставите као ресурс пројекта, можете да бирате између радника који раде у компанији за коју постављате ресурсе.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="b4fe6-110">Алтернативно, можете да изаберете раднике из других компанија у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="b4fe6-111">Ти радници су познати као међукомпанијски ресурси.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="b4fe6-112">Следећи поступци објашњавају како да поставите радника као ресурс пројекта у вашој компанији и како да поставите међукомпанијски ресурс пројекта.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="b4fe6-113">Поставите радника као ресурс пројекта</span><span class="sxs-lookup"><span data-stu-id="b4fe6-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="b4fe6-114">На страници **Радници** , на листи **Радници** , изаберите радника којег додајете као ресурс пројекта и отворите запис радника.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="b4fe6-115">У окну радњи изаберите **Пројекат** &gt; **Подешавање** &gt; **Подешавање пројекта**.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="b4fe6-116">Изаберите календар, а затим затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="b4fe6-117">Такође можете одредити подразумеване пројекте за ресурс као врсту претходног додељивања.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="b4fe6-118">Претходна додељивања се могу користити када менаџер ресурса или менаџер пројеката унапред зна на којим пројектима ће ресурс радити.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="b4fe6-119">Претходна додељивања се такође могу заснивати на захтеву спонзора пројекта или клијента.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="b4fe6-120">Да бисте унапред доделили пројекат, на страници **Додела пројеката** , на картици **Пројекти** , у листи **Преостали пројекти** изаберите одговарајући пројекат.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="b4fe6-121">Подесите међукомпанијски ресурс</span><span class="sxs-lookup"><span data-stu-id="b4fe6-121">Set up an intercompany resource</span></span>

<span data-ttu-id="b4fe6-122">Када радника поставите као међукомпанијски ресурс, морате довршити подешавање и у компанији зајмодавцу и у компанији зајмопримцу.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="b4fe6-123">У компанији зајмодавцу</span><span class="sxs-lookup"><span data-stu-id="b4fe6-123">In the lending company</span></span>

1. <span data-ttu-id="b4fe6-124">У услузи Finance проверите да ли је изабрана компанија зајмодавац, а затим довршите поступак у претходном одељку „Постављање радника као ресурса пројекта“.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="b4fe6-125">На страници **Међукомпанијско рачуноводство** , изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="b4fe6-126">У пољу **ID правног лица** изаберите компанију зајмодавца.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="b4fe6-127">Попуните преостала поља на одговарајући начин, а затим изаберите опцију **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="b4fe6-128">На страници **Цена трансфера** , изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="b4fe6-129">У пољу **Правно лице зајмопримац** изаберите одговарајућу компанију.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="b4fe6-130">Да бисте позајмљивали компанији зајмопримцу само оне ресурсе које сте креирали на почетку овог одељка, у пољу **Ресурс** изаберите име ресурса који сте креирали.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="b4fe6-131">Да бисте учинили све ресурсе у компанији доступним компанији зајмопримцу, оставите поље **Ресурс** празно.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="b4fe6-132">На страници **Параметри управљања пројектом и рачуноводственом** , на картици **Међукомпанијско** подесите опцију **Омогући међукомпанијско распоређивање ресурса временске распореде** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="b4fe6-133">У компанији зајмопримцу</span><span class="sxs-lookup"><span data-stu-id="b4fe6-133">In the borrowing company</span></span>

- <span data-ttu-id="b4fe6-134">На страници **Листа ресурса** , у филтер за претрагу унесите име ресурса који сте креирали за компанију зајмодавца, да бисте проверили да ли је име укључено у листу ресурса за компанију зајмопримца.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="b4fe6-135">Захтевање ресурса пројекта</span><span class="sxs-lookup"><span data-stu-id="b4fe6-135">Request project resources</span></span>
<span data-ttu-id="b4fe6-136">Функционалност за распоређивање ресурса пројекта омогућава да само менаџери ресурса распоређују ресурсе особља на ангажовања или пројекте.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="b4fe6-137">Да бисте омогућили ову функционалност, извршите следеће задатке или проверите да ли су завршени:</span><span class="sxs-lookup"><span data-stu-id="b4fe6-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="b4fe6-138">Подесите секвенце бројева.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-138">Set up number sequences.</span></span>
- <span data-ttu-id="b4fe6-139">Подесите токове посла управљања пројектима и рачуноводством.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="b4fe6-140">Омогућите токове посла захтева за ресурсима.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-140">Enable resource request workflows.</span></span>

<span data-ttu-id="b4fe6-141">Након завршетка претходних задатака, можете извршити следеће задатке по потреби:</span><span class="sxs-lookup"><span data-stu-id="b4fe6-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="b4fe6-142">Креирајте захтев за ресурсом из условно резервисаног ресурса особља.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="b4fe6-143">Надгледајте захтеве за ресурсима.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-143">Monitor resource requests.</span></span>
- <span data-ttu-id="b4fe6-144">Испуните захтеве за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="b4fe6-145">Затражите ресурсе особља из САП.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="b4fe6-146">Резервишите ресурсе за пројекат без захтева за ресурсима особља.</span><span class="sxs-lookup"><span data-stu-id="b4fe6-146">Book resources to a project without having a request for a staffed resource.</span></span>
