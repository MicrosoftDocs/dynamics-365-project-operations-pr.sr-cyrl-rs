---
title: Креирање пројектног тима
description: Ова тема пружа информације о томе како да креирате и управљате пројектним тимовима.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kdwns
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8d3d39aa28565692bf894ff8d4fc8f8c3c5542d4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006214"
---
# <a name="create-a-project-team"></a><span data-ttu-id="52c5b-103">Креирање пројектног тима</span><span class="sxs-lookup"><span data-stu-id="52c5b-103">Create a project team</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="52c5b-104">Да би користио улоге које су претходно постављене у пројекту, менаџер пројекта мора повезати улоге са пројектом.</span><span class="sxs-lookup"><span data-stu-id="52c5b-104">To use the roles that were previously set up in a project, a project manager must associate the roles with the project.</span></span> <span data-ttu-id="52c5b-105">За пројекат се може доделити више улога.</span><span class="sxs-lookup"><span data-stu-id="52c5b-105">Multiple roles can be assigned for a project.</span></span> <span data-ttu-id="52c5b-106">Да би се спречила забуна, ове улоге се аутоматски означавају током резервације.</span><span class="sxs-lookup"><span data-stu-id="52c5b-106">To prevent confusion, these roles are automatically labeled during reservation.</span></span> <span data-ttu-id="52c5b-107">На пример, ако менаџер пројекта захтева три софтверска инжењера, аутоматски се генеришу три улоге софтверског инжењера које имају ознаке **софтверски инжењер 1**, **софтверски инжењер 2** и **софтверски инжењер 3**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-107">For example, if the project manager requires three software engineers, three Software engineer roles that have **software engineer 1**, **software engineer 2**, and **software engineer 3** as their labels are automatically generated.</span></span> <span data-ttu-id="52c5b-108">Ако су карактеристике улоге претходно постављене за улогу, оне се примењују као филтер током претраживања ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c5b-108">If role characteristics were previously set for the role, they are applied as a filter during searches for a resource.</span></span> <span data-ttu-id="52c5b-109">Додатне карактеристике се могу додати по потреби за даље прецизирање претраге.</span><span class="sxs-lookup"><span data-stu-id="52c5b-109">Additional characteristics can be added as required to further refine the search.</span></span>

<span data-ttu-id="52c5b-110">Поставке приказа такође се могу прилагодити како би се добио бољи приказ доступности ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c5b-110">View settings can also be customized to give a better view of resource availability.</span></span> <span data-ttu-id="52c5b-111">Постоје опције за приказивање расположивости по сатима, дневно, недељно, месечно, квартално и годишње.</span><span class="sxs-lookup"><span data-stu-id="52c5b-111">There are options to show hourly, daily, weekly, monthly, quarterly, and annual availability.</span></span> <span data-ttu-id="52c5b-112">Такође постоји опција за приказ расположивог и преосталог капацитета ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c5b-112">There is also an option to show available and remaining capacity on resources.</span></span> <span data-ttu-id="52c5b-113">Ова опција је корисна за управљање временом када процењујете доступно време за активности или доступност ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c5b-113">This option is useful for time management, when you're estimating available time for activities or resource availability.</span></span>

<span data-ttu-id="52c5b-114">Менаџер пројекта може одабрати улогу на страници, а затим, ако постоји доступан ресурс који одговара захтевима, изаберите да резервишете ресурс за попуњавање улоге.</span><span class="sxs-lookup"><span data-stu-id="52c5b-114">The project manager can select a role on the page and then, if there is an available resource that fits the requirement, select to reserve a resource to fill the role.</span></span> <span data-ttu-id="52c5b-115">Имајте на уму да ресурси у овом тренутку не морају бити резервисани у фази планирања.</span><span class="sxs-lookup"><span data-stu-id="52c5b-115">Note that the resources don't have to be reserved at this point in the planning stage.</span></span> <span data-ttu-id="52c5b-116">Када креирате САП, можете заменити улоге ресурсима особља за пројекат.</span><span class="sxs-lookup"><span data-stu-id="52c5b-116">When you create a WBS, you can replace roles with staffed resources for the project.</span></span> <span data-ttu-id="52c5b-117">Ако се улоге замене ресурсима особља у САП-у, подешавање ресурса аутоматски ажурира списак и распоред пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="52c5b-117">If roles are replaced with staffed resources in the WBS, the resource setup automatically updates the project team listing and scheduling.</span></span>

<span data-ttu-id="52c5b-118">[![Списак пројектног тима који укључује и улоге и стварне ресурсе](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span><span class="sxs-lookup"><span data-stu-id="52c5b-118">[![Project team listing that includes both roles and actual resources](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span></span> 

<span data-ttu-id="52c5b-119">Менаџер пројекта има разне могућности за резервацију ресурса за пројекат, као што су **Преостали капацитет**, **Пун капацитет**, **Проценат капацитета** и **Наведите радно време**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-119">The project manager has various options for booking a resource for a project, such as **Remaining capacity**, **Full capacity**, **Capacity percentage**, and **Specify hours**.</span></span> <span data-ttu-id="52c5b-120">Ове опције резервације могу се отказати у било ком тренутку ако се промене додељивања ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c5b-120">These booking options can be canceled at any time if resource assignments change.</span></span> <span data-ttu-id="52c5b-121">Подржане су две врсте резервација:</span><span class="sxs-lookup"><span data-stu-id="52c5b-121">Two types of booking are supported:</span></span>

- <span data-ttu-id="52c5b-122">**Фиксна резервација** – Резервација ресурса је одобрена и потврђена за рад на ангажовању током одређеног времена.</span><span class="sxs-lookup"><span data-stu-id="52c5b-122">**Hard Book** – The resource reservation was approved and confirmed to work on the engagement for the specified duration.</span></span>
- <span data-ttu-id="52c5b-123">**Условна резервација** – Резервације ресурса су условно подешене за рад на ангажовању током одређеног времена.</span><span class="sxs-lookup"><span data-stu-id="52c5b-123">**Soft book** – The resource reservations was tentatively set to work on the engagement for the specified duration.</span></span>

<span data-ttu-id="52c5b-124">Следећа процедура објашњава како да креирате пројектни тим.</span><span class="sxs-lookup"><span data-stu-id="52c5b-124">The following procedure explains how to create a project team.</span></span>

## <a name="create-a-project-team"></a><span data-ttu-id="52c5b-125">Креирање пројектног тима</span><span class="sxs-lookup"><span data-stu-id="52c5b-125">Create a project team</span></span>

1. <span data-ttu-id="52c5b-126">На страници листе **Сви пројекти** изаберите пројекат, а затим изаберите **Уреди**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-126">On the **All projects** list page, select a project, and then select **Edit**.</span></span>
2. <span data-ttu-id="52c5b-127">На картици **Пројектни тим и распоређивање**, у поље **Датум завршетка распореда** унесите датум почетка распореда увећан за један месец.</span><span class="sxs-lookup"><span data-stu-id="52c5b-127">On the **Project team and scheduling** tab, in the **Schedule end date** field, enter the schedule start date plus one month.</span></span> <span data-ttu-id="52c5b-128">На пример, ако је датум почетка распореда 24. јун 2017. (24.6.2017), Унесите **24.07.2017**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-128">For example, if the schedule start date is June 24, 2017 (24/06/2017), enter **24/07/2017**.</span></span>
3. <span data-ttu-id="52c5b-129">Изаберите **Додај**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-129">Select **Add**.</span></span>
4. <span data-ttu-id="52c5b-130">У окну **Додавање улога у пројекат**, у пољу **Улога** изаберите **Виши менаџер пројекта**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-130">In the **Add roles to the project** pane, in the **Role** field, select **Senior Project Manager**.</span></span>
5. <span data-ttu-id="52c5b-131">Изаберите **Потребне компетенције**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-131">Select **Required competencies**.</span></span>
6. <span data-ttu-id="52c5b-132">На страници **Одаберите карактеристике**, карактеристике које сте претходно поставили за улогу вишег менаџера пројекта су подразумевано изабране.</span><span class="sxs-lookup"><span data-stu-id="52c5b-132">On the **Choose characteristics** page, the characteristics that you previously set for the Senior project manager role are selected by default.</span></span> <span data-ttu-id="52c5b-133">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-133">Select **OK**.</span></span>
7. <span data-ttu-id="52c5b-134">На страници **Додавање улоге пројекту**, у пољу **Број ресурса** унесите **1**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-134">On the **Add roles to project** page, in the **Number of resources** field, enter **1**.</span></span>
8. <span data-ttu-id="52c5b-135">У пољу **Ресурс**, преглед приказује све ресурсе који имају потребне компетенције.</span><span class="sxs-lookup"><span data-stu-id="52c5b-135">In the **Resource** field, the lookup shows all resources that have the required competencies.</span></span> <span data-ttu-id="52c5b-136">Изаберите **Данијел Голдшмит**, а затим изаберите **Креирај**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-136">Select **Daniel Goldschmidt**, and then select **Create**.</span></span>
9. <span data-ttu-id="52c5b-137">На страници **Пројекат** изаберите **Додај**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-137">On the **Project** page, select **Add**.</span></span>
10. <span data-ttu-id="52c5b-138">У окну **Додавање улога у пројекат**, у пољу **Улога** изаберите **Члан тима**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-138">In the **Add roles to the project** pane, in the **Role** field, select **Team member**.</span></span> <span data-ttu-id="52c5b-139">У поље **Број ресурса** унесите **5**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-139">In the **Number of resources** field, enter **5**.</span></span>
11. <span data-ttu-id="52c5b-140">Изаберите **Креирај**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-140">Select **Create**.</span></span>
12. <span data-ttu-id="52c5b-141">На страници **Пројекти**, изаберите **Попуни ресурс**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-141">On the **Projects** page, select **Fulfill resource**.</span></span>

## <a name="monitor-project-teams"></a><span data-ttu-id="52c5b-142">Надгледајте пројектне тимове</span><span class="sxs-lookup"><span data-stu-id="52c5b-142">Monitor project teams</span></span>
1. <span data-ttu-id="52c5b-143">На страници **Сви пројекти**, изаберите везу **ID пројекта** за пројекат **Надоградња XYZ фаза 2**.</span><span class="sxs-lookup"><span data-stu-id="52c5b-143">On the **All projects** page, select the **Project ID** link for the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="52c5b-144">На брзој картици **Пројектни тим и заказивање**, уверите се да су наведени ресурси пројекта тачни.</span><span class="sxs-lookup"><span data-stu-id="52c5b-144">On the **Project team and scheduling** FastTab, verify that the project resources that are listed are correct.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]