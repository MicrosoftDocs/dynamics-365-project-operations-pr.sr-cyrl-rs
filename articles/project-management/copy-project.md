---
title: Копирање пројекта
description: Ова тема пружа информације о копирању пројеката у услузи Dynamics 365 Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 02/22/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: af1942e81691d9e13fdcbbf68599c1a8a4004582
ms.sourcegitcommit: 24528bb9c0ef8898077cb3bc672daa211c0e73aa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "5479537"
---
# <a name="copy-a-project"></a><span data-ttu-id="e4e30-103">Копирање пројекта</span><span class="sxs-lookup"><span data-stu-id="e4e30-103">Copy a project</span></span>

<span data-ttu-id="e4e30-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="e4e30-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e4e30-105">Уз Dynamics 365 Project Operations, можете брзо да правите нове пројекте избором опције **Копирај пројекат** у обрасцу **Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="e4e30-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="e4e30-106">Да бисте копирали пројекат, отворите пројекат који желите да копирате, а затим изаберите **Копирај пројекат**.</span><span class="sxs-lookup"><span data-stu-id="e4e30-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="e4e30-107">Радња ће копирати:</span><span class="sxs-lookup"><span data-stu-id="e4e30-107">The action will copy:</span></span>

- <span data-ttu-id="e4e30-108">Својства пројекта (процењени датум почетка се копира из изворног пројекта)</span><span class="sxs-lookup"><span data-stu-id="e4e30-108">Project properties (The estimated start date is copied from the source project)</span></span>
- <span data-ttu-id="e4e30-109">Структурну анализу посла</span><span class="sxs-lookup"><span data-stu-id="e4e30-109">The Work breakdown structure</span></span>
- <span data-ttu-id="e4e30-110">Чланови пројектног тима</span><span class="sxs-lookup"><span data-stu-id="e4e30-110">Project team members</span></span>
- <span data-ttu-id="e4e30-111">Процене за пројекат</span><span class="sxs-lookup"><span data-stu-id="e4e30-111">Project estimates</span></span>
- <span data-ttu-id="e4e30-112">Процене трошкова пројекта</span><span class="sxs-lookup"><span data-stu-id="e4e30-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="e4e30-113">Својства пројекта</span><span class="sxs-lookup"><span data-stu-id="e4e30-113">Project properties</span></span>

<span data-ttu-id="e4e30-114">Када се пројекат копира, копирају се вредности у следећим пољима:</span><span class="sxs-lookup"><span data-stu-id="e4e30-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="e4e30-115">Име</span><span class="sxs-lookup"><span data-stu-id="e4e30-115">Name</span></span>
- <span data-ttu-id="e4e30-116">Опис</span><span class="sxs-lookup"><span data-stu-id="e4e30-116">Description</span></span>
- <span data-ttu-id="e4e30-117">Клијент</span><span class="sxs-lookup"><span data-stu-id="e4e30-117">Customer</span></span>
- <span data-ttu-id="e4e30-118">Предложак календара</span><span class="sxs-lookup"><span data-stu-id="e4e30-118">Calendar Template</span></span>
- <span data-ttu-id="e4e30-119">Валута</span><span class="sxs-lookup"><span data-stu-id="e4e30-119">Currency</span></span>
- <span data-ttu-id="e4e30-120">Јединица уговарања</span><span class="sxs-lookup"><span data-stu-id="e4e30-120">Contracting Unit</span></span>
- <span data-ttu-id="e4e30-121">Менаџер пројекта</span><span class="sxs-lookup"><span data-stu-id="e4e30-121">Project Manager</span></span>
- <span data-ttu-id="e4e30-122">Статус</span><span class="sxs-lookup"><span data-stu-id="e4e30-122">Status</span></span>
- <span data-ttu-id="e4e30-123">Укупан статус пројекта</span><span class="sxs-lookup"><span data-stu-id="e4e30-123">Overall Project Status</span></span>
- <span data-ttu-id="e4e30-124">Коментари</span><span class="sxs-lookup"><span data-stu-id="e4e30-124">Comments</span></span>
- <span data-ttu-id="e4e30-125">Процене</span><span class="sxs-lookup"><span data-stu-id="e4e30-125">Estimates</span></span>
- <span data-ttu-id="e4e30-126">Процењени датум почетка</span><span class="sxs-lookup"><span data-stu-id="e4e30-126">Estimated Start Date</span></span>
- <span data-ttu-id="e4e30-127">Датум завршетка</span><span class="sxs-lookup"><span data-stu-id="e4e30-127">Finish Date</span></span>
- <span data-ttu-id="e4e30-128">Ангажовање (часови)</span><span class="sxs-lookup"><span data-stu-id="e4e30-128">Effort (Hours)</span></span>
- <span data-ttu-id="e4e30-129">Процењени трошкови рада</span><span class="sxs-lookup"><span data-stu-id="e4e30-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="e4e30-130">Процењени износ трошкова</span><span class="sxs-lookup"><span data-stu-id="e4e30-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="e4e30-131">Структурна анализа посла</span><span class="sxs-lookup"><span data-stu-id="e4e30-131">Work breakdown structure</span></span>

<span data-ttu-id="e4e30-132">Када се пројекат копира, копира се целокупна структурна анализа посла учитаног ресурса.</span><span class="sxs-lookup"><span data-stu-id="e4e30-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="e4e30-133">Именовани ресурс замењује генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e4e30-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="e4e30-134">Ако именовани ресурси немају исто радно време као генерички ресурс, распоред ће се поново израчунати и трајање задатка се може променити.</span><span class="sxs-lookup"><span data-stu-id="e4e30-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="e4e30-135">Чланови пројектног тима</span><span class="sxs-lookup"><span data-stu-id="e4e30-135">Project team members</span></span>

<span data-ttu-id="e4e30-136">Када се пројектни тим копира из изворног пројекта, копирају се генерички ресурси.</span><span class="sxs-lookup"><span data-stu-id="e4e30-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="e4e30-137">Доделе генеричких ресурса такође се одржавају као у изворном пројекту.</span><span class="sxs-lookup"><span data-stu-id="e4e30-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="e4e30-138">Именовани ресурси ће се претворити у генеричке чланове тима.</span><span class="sxs-lookup"><span data-stu-id="e4e30-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="e4e30-139">Процене</span><span class="sxs-lookup"><span data-stu-id="e4e30-139">Estimates</span></span>

<span data-ttu-id="e4e30-140">Када се пројекат копира, из изворног пројекта се копирају и ставке процене ресурса и трошкова.</span><span class="sxs-lookup"><span data-stu-id="e4e30-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="e4e30-141">За информације о томе како програмски приступити опцији Копирај пројекат, погледајте [Развијајте предлошке пројеката помоћу опције Копирај пројекат](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="e4e30-141">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
