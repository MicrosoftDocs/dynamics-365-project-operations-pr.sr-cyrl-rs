---
title: Ажурирање пројекта
description: Ова тема пружа информације о ажурирању пројеката у услузи Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c07542444b970430d8143a60aad6970305769b22
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993389"
---
# <a name="update-a-project"></a><span data-ttu-id="18d39-103">Ажурирање пројекта</span><span class="sxs-lookup"><span data-stu-id="18d39-103">Update a project</span></span>

<span data-ttu-id="18d39-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="18d39-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="18d39-105">У наставку се налази резиме поља која се могу ажурирати у пројекту након креирања и све применљиве импликације ажурирања.</span><span class="sxs-lookup"><span data-stu-id="18d39-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="18d39-106">Поља детаља о пројекту</span><span class="sxs-lookup"><span data-stu-id="18d39-106">Project detail fields</span></span>

- <span data-ttu-id="18d39-107">**Назив**: Наслов пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="18d39-108">**Опис**: Преглед пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="18d39-109">**Клијент**: Предузеће којем ће пројекат бити испоручен.</span><span class="sxs-lookup"><span data-stu-id="18d39-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="18d39-110">**Предложак календара**: Радно време пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="18d39-111">Када се поље промени, цео распоред се прерачунава.</span><span class="sxs-lookup"><span data-stu-id="18d39-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="18d39-112">**Валута**: Валута пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="18d39-113">Ово поље се подразумевано заснива на валути дефинисаној у уговорној јединици.</span><span class="sxs-lookup"><span data-stu-id="18d39-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="18d39-114">Када се уговорна јединица ажурира, поље се такође ажурира.</span><span class="sxs-lookup"><span data-stu-id="18d39-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="18d39-115">**Уговорна јединица**: Организациона јединица која представља групу или одељење предузећа које је првенствено одговорно за повећање продаје и управљање испоруком посла и услуга клијенту.</span><span class="sxs-lookup"><span data-stu-id="18d39-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="18d39-116">**Менаџер пројекта**: Члан пројектног тима који има овлашћење да прегледа и одобри ставке времена и трошкове.</span><span class="sxs-lookup"><span data-stu-id="18d39-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="18d39-117">Поља за процену</span><span class="sxs-lookup"><span data-stu-id="18d39-117">Estimate fields</span></span>

- <span data-ttu-id="18d39-118">**Процењени датум почетка**: Датум почетка пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="18d39-119">Када се ово поље ажурира, сви задаци на пројекту помериће свој почетак сразмерно новом датуму почетка.</span><span class="sxs-lookup"><span data-stu-id="18d39-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="18d39-120">**Датум завршетка**: Датум за када је планиран завршетак пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="18d39-121">**Ангажовање**: Процењено ангажовање у пројекту.</span><span class="sxs-lookup"><span data-stu-id="18d39-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="18d39-122">Када се задаци додају у пројекат, ово поље више није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="18d39-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="18d39-123">**Процењена цена рада**: Процењена цена рада на пројекту.</span><span class="sxs-lookup"><span data-stu-id="18d39-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="18d39-124">Када се цене рада додају у пројекат, ово поље више није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="18d39-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="18d39-125">**Процењени трошкови**: Процењени трошкови пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="18d39-126">Када се трошкови додају у пројекат, ово поље више није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="18d39-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="18d39-127">Поља стварних вредности пројекта</span><span class="sxs-lookup"><span data-stu-id="18d39-127">Project actual fields</span></span>
- <span data-ttu-id="18d39-128">**Стварни почетак**: Датум када је пројекат започет.</span><span class="sxs-lookup"><span data-stu-id="18d39-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="18d39-129">**Стварни завршетак**: Биће ажуриран када се пројекат заврши.</span><span class="sxs-lookup"><span data-stu-id="18d39-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="18d39-130">Поља статуса пројекта</span><span class="sxs-lookup"><span data-stu-id="18d39-130">Project status fields</span></span>

- <span data-ttu-id="18d39-131">**Свеукупни статус пројекта**: Свеукупна исправност пројекта коју обезбеђује менаџер пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="18d39-132">**Коментари**: Описивање тренутне исправности пројекта коју је обезбедио менаџер пројекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]