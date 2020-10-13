---
title: Ажурирање пројекта
description: Ова тема пружа информације о ажурирању пројеката у услузи Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 5c9cd0c7c6886bd454c5f2ef2ae7f20d1707293f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897830"
---
# <a name="update-a-project"></a><span data-ttu-id="d39fd-103">Ажурирање пројекта</span><span class="sxs-lookup"><span data-stu-id="d39fd-103">Update a project</span></span>

<span data-ttu-id="d39fd-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="d39fd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d39fd-105">У наставку се налази резиме поља која се могу ажурирати у пројекту након креирања и све применљиве импликације ажурирања.</span><span class="sxs-lookup"><span data-stu-id="d39fd-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="d39fd-106">Поља детаља о пројекту</span><span class="sxs-lookup"><span data-stu-id="d39fd-106">Project detail fields</span></span>

- <span data-ttu-id="d39fd-107">**Назив**: Наслов пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="d39fd-108">**Опис**: Преглед пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="d39fd-109">**Клијент**: Предузеће којем ће пројекат бити испоручен.</span><span class="sxs-lookup"><span data-stu-id="d39fd-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="d39fd-110">**Предложак календара**: Радно време пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="d39fd-111">Када се поље промени, цео распоред се прерачунава.</span><span class="sxs-lookup"><span data-stu-id="d39fd-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="d39fd-112">**Валута**: Валута пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="d39fd-113">Ово поље се подразумевано заснива на валути дефинисаној у уговорној јединици.</span><span class="sxs-lookup"><span data-stu-id="d39fd-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="d39fd-114">Када се уговорна јединица ажурира, поље се такође ажурира.</span><span class="sxs-lookup"><span data-stu-id="d39fd-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="d39fd-115">**Уговорна јединица**: Организациона јединица која представља групу или одељење предузећа које је првенствено одговорно за повећање продаје и управљање испоруком посла и услуга клијенту.</span><span class="sxs-lookup"><span data-stu-id="d39fd-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="d39fd-116">**Менаџер пројекта**: Члан пројектног тима који има овлашћење да прегледа и одобри ставке времена и трошкове.</span><span class="sxs-lookup"><span data-stu-id="d39fd-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="d39fd-117">Поља за процену</span><span class="sxs-lookup"><span data-stu-id="d39fd-117">Estimate fields</span></span>

- <span data-ttu-id="d39fd-118">**Процењени датум почетка**: Датум почетка пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="d39fd-119">Када се ово поље ажурира, сви задаци на пројекту помериће свој почетак сразмерно новом датуму почетка.</span><span class="sxs-lookup"><span data-stu-id="d39fd-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="d39fd-120">**Датум завршетка**: Датум за када је планиран завршетак пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="d39fd-121">**Ангажовање**: Процењено ангажовање у пројекту.</span><span class="sxs-lookup"><span data-stu-id="d39fd-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="d39fd-122">Када се задаци додају у пројекат, ово поље више није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="d39fd-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="d39fd-123">**Процењена цена рада**: Процењена цена рада на пројекту.</span><span class="sxs-lookup"><span data-stu-id="d39fd-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="d39fd-124">Када се цене рада додају у пројекат, ово поље више није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="d39fd-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="d39fd-125">**Процењени трошкови**: Процењени трошкови пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="d39fd-126">Када се трошкови додају у пројекат, ово поље више није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="d39fd-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="d39fd-127">Поља стварних вредности пројекта</span><span class="sxs-lookup"><span data-stu-id="d39fd-127">Project actual fields</span></span>
- <span data-ttu-id="d39fd-128">**Стварни почетак**: Датум када је пројекат започет.</span><span class="sxs-lookup"><span data-stu-id="d39fd-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="d39fd-129">**Стварни завршетак**: Биће ажуриран када се пројекат заврши.</span><span class="sxs-lookup"><span data-stu-id="d39fd-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="d39fd-130">Поља статуса пројекта</span><span class="sxs-lookup"><span data-stu-id="d39fd-130">Project status fields</span></span>

- <span data-ttu-id="d39fd-131">**Свеукупни статус пројекта**: Свеукупна исправност пројекта коју обезбеђује менаџер пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="d39fd-132">**Коментари**: Описивање тренутне исправности пројекта коју је обезбедио менаџер пројекта.</span><span class="sxs-lookup"><span data-stu-id="d39fd-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>

