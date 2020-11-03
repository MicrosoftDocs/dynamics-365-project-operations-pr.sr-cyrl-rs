---
title: Подешавања пројекта
description: Ова тема пружа информације о подешавањима управљања пројектима.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: c9b8659f3b7ee81d2e21ef52743debd521fa9bb9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084135"
---
# <a name="project-settings"></a><span data-ttu-id="81c67-103">Подешавања пројекта</span><span class="sxs-lookup"><span data-stu-id="81c67-103">Project settings</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="81c67-104">За приступ функцијама планирања пројеката користите следећа подешавања.</span><span class="sxs-lookup"><span data-stu-id="81c67-104">Use the following settings to access the project planning features.</span></span>

## <a name="work-template"></a><span data-ttu-id="81c67-105">Радни предложак</span><span class="sxs-lookup"><span data-stu-id="81c67-105">Work template</span></span>

<span data-ttu-id="81c67-106">Да бисте креирали распоред пројекта, креирајте предложак календара пројекта који дефинише број радних сати по дану и све прекиде пословних активности.</span><span class="sxs-lookup"><span data-stu-id="81c67-106">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="81c67-107">Да бисте креирали предложак календара пројекта, радни предложак повезујете са пољем **Предложак календара** за пројекат.</span><span class="sxs-lookup"><span data-stu-id="81c67-107">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="81c67-108">Следите ове кораке за креирање радног предлошка.</span><span class="sxs-lookup"><span data-stu-id="81c67-108">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="81c67-109">У апликацији PSA, у левом навигационом окну, кликните на **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="81c67-109">In PSA, in the left navigation pane, click **Resources**.</span></span> 
2. <span data-ttu-id="81c67-110">На страници листе **Ресурси** отворите запис корисника, а затим изаберите **Прикажи радно време**.</span><span class="sxs-lookup"><span data-stu-id="81c67-110">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="81c67-111">Обавезно дозволите искачуће прозоре на страници прегледача.</span><span class="sxs-lookup"><span data-stu-id="81c67-111">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="81c67-112">Ово вам омогућава да видите радно време подешено за ресурс.</span><span class="sxs-lookup"><span data-stu-id="81c67-112">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="81c67-113">На картици **Месечни приказ** кликните на **Подешавање**.</span><span class="sxs-lookup"><span data-stu-id="81c67-113">On the **Monthly View** tab, click **Set Up**.</span></span> <span data-ttu-id="81c67-114">Појавиће се листа са три опције:</span><span class="sxs-lookup"><span data-stu-id="81c67-114">A list of three options appears:</span></span> 

  - <span data-ttu-id="81c67-115">Нови седмични распоред</span><span class="sxs-lookup"><span data-stu-id="81c67-115">New Weekly Schedule</span></span>
  - <span data-ttu-id="81c67-116">Распоред посла за један дан</span><span class="sxs-lookup"><span data-stu-id="81c67-116">Work Schedule for One Day</span></span>
  - <span data-ttu-id="81c67-117">Одступање у времену</span><span class="sxs-lookup"><span data-stu-id="81c67-117">Time Off</span></span>

> ![Подешавање опција](media/project-13.png)

4. <span data-ttu-id="81c67-119">Изаберите **Нови седмични распоред** , а затим подесите опције за овај распоред ресурса.</span><span class="sxs-lookup"><span data-stu-id="81c67-119">Select **New Weekly Schedule** , and then set the options for this resource schedule.</span></span> <span data-ttu-id="81c67-120">Можете подесити периодични седмични распоред, параметре сата у дану, прекид пословних активности и још много тога.</span><span class="sxs-lookup"><span data-stu-id="81c67-120">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="81c67-121">Подесите опсег датума, изаберите **Сачувај** , а затим кликните на **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="81c67-121">Set the date range, select **Save** , and then click **Close**.</span></span> 
6. <span data-ttu-id="81c67-122">Вратите се на страницу листе **Ресурси** и одаберите ресурс за који сте одредили радно време.</span><span class="sxs-lookup"><span data-stu-id="81c67-122">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="81c67-123">Изаберите **Подесите календар као** да подесили радни предложак.</span><span class="sxs-lookup"><span data-stu-id="81c67-123">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="81c67-124">У дијалог **Радни предложак** унесите име радног предлошка, а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="81c67-124">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="81c67-125">Сада можете повезати радни предложак са предлошком календара пројекта.</span><span class="sxs-lookup"><span data-stu-id="81c67-125">You can now associate the work template with a project calendar template.</span></span>

## <a name="resource-roles"></a><span data-ttu-id="81c67-126">Улоге ресурса</span><span class="sxs-lookup"><span data-stu-id="81c67-126">Resource roles</span></span>

<span data-ttu-id="81c67-127">Термин *улога ресурса* односи се на скуп вештина, компетенција и цертификације које особа мора имати да би могла да обавља одређени скуп задатака у пројекту.</span><span class="sxs-lookup"><span data-stu-id="81c67-127">The term *resource role* refers to the set of skills, competencies, and certifications that a person must have to perform a specific set of tasks on a project.</span></span> <span data-ttu-id="81c67-128">PSA вам омогућава да одредите трошкове и наплатите време ресурса на основу улоге са којом је ресурс повезан.</span><span class="sxs-lookup"><span data-stu-id="81c67-128">PSA lets you cost and bill a resource's time based on the role that the resource is associated with.</span></span> <span data-ttu-id="81c67-129">Свака организација мора подесити ове улоге користећи леву навигацију у менију **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="81c67-129">Every organization must set up these roles by using the left navigation on the **Project Service** menu.</span></span>

<span data-ttu-id="81c67-130">Свака организација мора подесити ове улоге на страници **Активне категорије ресурса**.</span><span class="sxs-lookup"><span data-stu-id="81c67-130">Every organization must set up these roles on the **Active Resource Categories** page.</span></span> <span data-ttu-id="81c67-131">Да бисте отворили ову страницу, у левом навигационом окну изаберите **Улоге ресурса**.</span><span class="sxs-lookup"><span data-stu-id="81c67-131">To open this page, in the left navigation pane, select **Resource Roles**.</span></span>

## <a name="price-lists"></a><span data-ttu-id="81c67-132">Ценовници</span><span class="sxs-lookup"><span data-stu-id="81c67-132">Price lists</span></span>

<span data-ttu-id="81c67-133">Ценовници вам омогућавају да подесите цене коштања и продајне цене за улоге ресурса, категорије трошкова, производе и друге елементе у организацији.</span><span class="sxs-lookup"><span data-stu-id="81c67-133">Price lists let you set cost and sales prices for resource roles, expense categories, products, and other elements in an organization.</span></span> <span data-ttu-id="81c67-134">Да бисте могли да подесите финансијске процене за посао који мора да се обави за пројекат, треба да креирате одговарајућу листу трошкова и ценовник продаје.</span><span class="sxs-lookup"><span data-stu-id="81c67-134">Before you set financial estimates for the work that must be delivered for a project, you should create a backing cost and sales price list.</span></span> <span data-ttu-id="81c67-135">У одељку са параметрима треба да подесите и подразумевани ценовник трошкова и продајни ценовник који се односи на све пројекте креиране у организацији.</span><span class="sxs-lookup"><span data-stu-id="81c67-135">In the parameters section, you should also set up a default cost and sales price list that applies to all projects that are created in the organization.</span></span> <span data-ttu-id="81c67-136">На страници **Активни параметри пројекта** проверите да ли сте подесили подразумевани ценовник трошкова и продајни ценовник.</span><span class="sxs-lookup"><span data-stu-id="81c67-136">On the **Active Project Parameters** page, make sure that you set up a default cost and sales price list.</span></span>
