---
title: Копирање пројекта
description: Ова тема пружа информације о копирању пројеката у услузи Dynamics 365 Project Operations.
author: ruhercul
ms.date: 05/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c3055ab5b8c07faa2bc9167956d283e2a66029dd
ms.sourcegitcommit: 173f2b1f4e063c440a5f78d76d456c62aadbd89e
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/24/2021
ms.locfileid: "6091272"
---
# <a name="copy-a-project"></a><span data-ttu-id="fec46-103">Копирање пројекта</span><span class="sxs-lookup"><span data-stu-id="fec46-103">Copy a project</span></span>

<span data-ttu-id="fec46-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="fec46-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="fec46-105">Уз Dynamics 365 Project Operations, можете брзо да правите нове пројекте избором опције **Копирај пројекат** у обрасцу **Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="fec46-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="fec46-106">Да бисте копирали пројекат, отворите пројекат који желите да копирате, а затим изаберите **Копирај пројекат**.</span><span class="sxs-lookup"><span data-stu-id="fec46-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="fec46-107">Радња ће копирати следеће:</span><span class="sxs-lookup"><span data-stu-id="fec46-107">The action will copy the following:</span></span>

- <span data-ttu-id="fec46-108">Својства пројекта</span><span class="sxs-lookup"><span data-stu-id="fec46-108">Project properties</span></span> 
- <span data-ttu-id="fec46-109">Структурна анализа посла</span><span class="sxs-lookup"><span data-stu-id="fec46-109">Work breakdown structure</span></span>
- <span data-ttu-id="fec46-110">Чланови пројектног тима</span><span class="sxs-lookup"><span data-stu-id="fec46-110">Project team members</span></span>
- <span data-ttu-id="fec46-111">Процене за пројекат</span><span class="sxs-lookup"><span data-stu-id="fec46-111">Project estimates</span></span>
- <span data-ttu-id="fec46-112">Процене трошкова пројекта</span><span class="sxs-lookup"><span data-stu-id="fec46-112">Project expense estimates</span></span>
- <span data-ttu-id="fec46-113">Процене материјала за пројекат</span><span class="sxs-lookup"><span data-stu-id="fec46-113">Project material estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="fec46-114">Својства пројекта</span><span class="sxs-lookup"><span data-stu-id="fec46-114">Project properties</span></span>

<span data-ttu-id="fec46-115">Када се пројекат копира, копирају се вредности у следећим пољима:</span><span class="sxs-lookup"><span data-stu-id="fec46-115">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="fec46-116">Име</span><span class="sxs-lookup"><span data-stu-id="fec46-116">Name</span></span>
- <span data-ttu-id="fec46-117">Опис</span><span class="sxs-lookup"><span data-stu-id="fec46-117">Description</span></span>
- <span data-ttu-id="fec46-118">Клијент</span><span class="sxs-lookup"><span data-stu-id="fec46-118">Customer</span></span>
- <span data-ttu-id="fec46-119">Предложак календара</span><span class="sxs-lookup"><span data-stu-id="fec46-119">Calendar Template</span></span>
- <span data-ttu-id="fec46-120">Валута</span><span class="sxs-lookup"><span data-stu-id="fec46-120">Currency</span></span>
- <span data-ttu-id="fec46-121">Јединица уговарања</span><span class="sxs-lookup"><span data-stu-id="fec46-121">Contracting Unit</span></span>
- <span data-ttu-id="fec46-122">Менаџер пројекта</span><span class="sxs-lookup"><span data-stu-id="fec46-122">Project Manager</span></span>
- <span data-ttu-id="fec46-123">Статус</span><span class="sxs-lookup"><span data-stu-id="fec46-123">Status</span></span>
- <span data-ttu-id="fec46-124">Укупан статус пројекта</span><span class="sxs-lookup"><span data-stu-id="fec46-124">Overall Project Status</span></span>
- <span data-ttu-id="fec46-125">Коментари</span><span class="sxs-lookup"><span data-stu-id="fec46-125">Comments</span></span>
- <span data-ttu-id="fec46-126">Процене</span><span class="sxs-lookup"><span data-stu-id="fec46-126">Estimates</span></span>
- <span data-ttu-id="fec46-127">Процењени датум почетка: Ово је датум када се пројекат креира из копије.</span><span class="sxs-lookup"><span data-stu-id="fec46-127">Estimated Start Date: This is the date that the project is created from the copy.</span></span>
- <span data-ttu-id="fec46-128">Процењени датум завршетка: Овај датум се прилагођава на основу датума почетка новог пројекта који је направљен из копије.</span><span class="sxs-lookup"><span data-stu-id="fec46-128">Estimated Finish Date: This date is adjusted based on the start date of the new project that was made from the copy.</span></span>
- <span data-ttu-id="fec46-129">Ангажовање (часови)</span><span class="sxs-lookup"><span data-stu-id="fec46-129">Effort (Hours)</span></span>
- <span data-ttu-id="fec46-130">Процењени трошкови рада</span><span class="sxs-lookup"><span data-stu-id="fec46-130">Estimated Labor Cost</span></span>
- <span data-ttu-id="fec46-131">Процењени износ трошкова</span><span class="sxs-lookup"><span data-stu-id="fec46-131">Estimated Expense Cost</span></span>
- <span data-ttu-id="fec46-132">Износ процењених трошкова материјала</span><span class="sxs-lookup"><span data-stu-id="fec46-132">Estimated Material Cost</span></span>

> [!NOTE]
> <span data-ttu-id="fec46-133">Копирање пројекта је дуготрајна операција.</span><span class="sxs-lookup"><span data-stu-id="fec46-133">Copy project is a long running operation.</span></span> <span data-ttu-id="fec46-134">Копирају се и записи пројекта, њихови релевантни атрибути и многи повезани ентитети.</span><span class="sxs-lookup"><span data-stu-id="fec46-134">Project records, their relevant attributes, and many related entities are also copied.</span></span> <span data-ttu-id="fec46-135">Због дуготрајне природе операције, након започињања копирања, циљна страница пројекта се закључава за уређивање док се операција копирања не доврши.</span><span class="sxs-lookup"><span data-stu-id="fec46-135">Because of the long running nature of the operation, after the copy starts, the target project page is locked for editing until the copy operation is complete.</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="fec46-136">Структурна анализа посла</span><span class="sxs-lookup"><span data-stu-id="fec46-136">Work breakdown structure</span></span>

<span data-ttu-id="fec46-137">Када се пројекат копира, копира се целокупна структурна анализа посла учитаног ресурса.</span><span class="sxs-lookup"><span data-stu-id="fec46-137">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="fec46-138">Именовани ресурс замењује генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fec46-138">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="fec46-139">Ако именовани ресурси немају исто радно време као генерички ресурс, распоред ће се поново израчунати и трајање задатка се може променити.</span><span class="sxs-lookup"><span data-stu-id="fec46-139">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="fec46-140">Чланови пројектног тима</span><span class="sxs-lookup"><span data-stu-id="fec46-140">Project team members</span></span>

<span data-ttu-id="fec46-141">Када се пројектни тим копира из изворног пројекта, копирају се генерички ресурси.</span><span class="sxs-lookup"><span data-stu-id="fec46-141">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="fec46-142">Доделе генеричких ресурса такође се одржавају као у изворном пројекту.</span><span class="sxs-lookup"><span data-stu-id="fec46-142">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="fec46-143">Именовани ресурси ће се претворити у генеричке чланове тима.</span><span class="sxs-lookup"><span data-stu-id="fec46-143">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="fec46-144">Процене</span><span class="sxs-lookup"><span data-stu-id="fec46-144">Estimates</span></span>

<span data-ttu-id="fec46-145">Када се пројекат копира, ставке ресурса, трошкова и процене материјала копирају се из изворног пројекта.</span><span class="sxs-lookup"><span data-stu-id="fec46-145">When the project is copied, resource, expense and material estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="fec46-146">За информације о томе како програмски приступити опцији Копирај пројекат, погледајте [Развијајте предлошке пројеката помоћу опције Копирај пројекат](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="fec46-146">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
