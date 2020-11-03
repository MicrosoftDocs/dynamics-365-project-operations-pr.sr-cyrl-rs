---
title: Водич за менаџера ресурса
description: Водич за управљање ресурсима у апликацији Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 4a26a384dfaf6b974ed35105434152e655ff6444
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084180"
---
# <a name="resource-manager-guide-project-service"></a><span data-ttu-id="5a8a0-103">Водич за менаџера ресурса (Project Service)</span><span class="sxs-lookup"><span data-stu-id="5a8a0-103">Resource manager guide (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="5a8a0-104">Могућности [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у систему [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] вам помажу да пронађете праве ресурсе у право време за прави пројекат и да се постарате да се сви ресурси ефикасно користе.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-104">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] help you find the right resources at the right time for the right project and make sure all resources are utilized efficiently.</span></span>  
  
 <span data-ttu-id="5a8a0-105">Примените консултанте предузећа ефикасно са резултатима уз [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="5a8a0-105">Deploy your company’s consultants efficiently and effectively with the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="5a8a0-106">Оне вам пружају алатке које су вам потребне да испланирате ресурса на основу захтева и распореда пројеката и вештина и доступности саветника.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-106">These provide you with the tools you need to schedule resources based on the requirements and schedules of consulting projects and on the skills and availability of your consultants.</span></span> <span data-ttu-id="5a8a0-107">Брзо можете да пронађете највише квалификоване саветнике који су доступни за рад на пројектима и лако можете да видите како да их боље планирате током сваког пројекта.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-107">You can quickly find the most qualified consultants who are available to work on projects, and you can easily see how to better schedule them during the course of each project.</span></span>  
  
 <span data-ttu-id="5a8a0-108">Планирање ресурса вам помаже да урадите следеће:</span><span class="sxs-lookup"><span data-stu-id="5a8a0-108">Resource scheduling helps you do the following:</span></span>  
  
- <span data-ttu-id="5a8a0-109">Спојите ресурсе са пројектима, на основу тога како њихове вештине и нивои стручности одговарају захтевима пројекта за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-109">Match resources to projects, based on how well their skills and proficiency levels match the project resource requirements.</span></span>  
  
- <span data-ttu-id="5a8a0-110">Спајање распореда ресурса са календаром пројекта, на основу њихове доступности и планираног слободног времена.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-110">Match a resource’s schedule to a project calendar, based on their availability and scheduled time off.</span></span> <span data-ttu-id="5a8a0-111">Календар означен бојама пружа визуелни приказ доступности ресурса.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-111">The color-coded calendar gives you visual cues about resource availability.</span></span>  
  
- <span data-ttu-id="5a8a0-112">Прегледајте капацитет сваког саветника и одредите начин на који се који капацитет тренутно користи.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-112">Review the capacity of each consultant and determine how that capacity is currently used.</span></span> <span data-ttu-id="5a8a0-113">Ово вам може помоћи да пронађете где је консултант можда у премало или превише искоришћен или ради у оквиру свог капацитета.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-113">This can help you find where a consultant might be under- or over-utilized, or if they’re working at capacity.</span></span>  
  
- <span data-ttu-id="5a8a0-114">Доделите проценат или одређени број часова за капацитет радника за пројекат.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-114">Assign a percentage or a specific number of hours for a worker’s capacity to a project.</span></span>  
  
- <span data-ttu-id="5a8a0-115">Правите групне резервације ресурса.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-115">Make group resource bookings.</span></span>  
  
- <span data-ttu-id="5a8a0-116">Условно и фиксно резервисање ресурса и конвертовање условно резервисаних сата у фиксно резервисане сате у једном кораку.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-116">Soft book or hard book resources, and convert soft-booked hours into hard-booked hours in one step.</span></span>  
  
- <span data-ttu-id="5a8a0-117">Аутоматски формирајте тим за пројекат на основу ресурса дефинисаних у структурној анализи посла за пројекат.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-117">Automatically form a project team based on resources defined in a work breakdown structure for a project.</span></span>  
  
- <span data-ttu-id="5a8a0-118">Испуните захтеве за ресурсе (резервишите, предлажите, нађите заменске ресурсе).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-118">Fulfill resource requests (book, propose, find substitute resources).</span></span>  
  
- <span data-ttu-id="5a8a0-119">Додељујте ресурсе у складу са централним (менаџер ресурса додељује) или хибридним моделом (менаџер ресурса и други менаџери могу да доделе).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-119">Assign resources according to a central (resource manager assigns) or hybrid model (resource manager and other managers can assign).</span></span> <span data-ttu-id="5a8a0-120">Више информација о подешавању централног модела управљања ресурсима наспрам хибридног потражите у чланку [Конфигурисање подешавања додатних параметара (Project Service)](../psa/configure-additional-parameters-settings.md).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-120">For more information about setting a central versus hybrid resource management model, see [Configure additional parameters settings (Project Service)](../psa/configure-additional-parameters-settings.md).</span></span>  
  
  <span data-ttu-id="5a8a0-121">Можете да управљате ресурсима ефикасно у разним пројектима и уверите се да су пројектима додељени ресурси на одговарајући начин.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-121">You can manage resources efficiently across projects and ensure that projects are staffed appropriately.</span></span> <span data-ttu-id="5a8a0-122">Мораћете да извршите следеће задатке:</span><span class="sxs-lookup"><span data-stu-id="5a8a0-122">You’ll need to perform the following tasks:</span></span>  
  
- <span data-ttu-id="5a8a0-123">[Управљање захтевима за ресурсе](../psa/manage-resource-requests.md).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-123">[Manage resource requests](../psa/manage-resource-requests.md).</span></span> <span data-ttu-id="5a8a0-124">Спојите вештине и стручност саветника са одговарајућим пројектима.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-124">Match the skills and proficiencies of your consultants to the right projects.</span></span>  
  
- <span data-ttu-id="5a8a0-125">[Приказ доступности ресурса](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-125">[View resource availability](../psa/view-resource-availability.md).</span></span> <span data-ttu-id="5a8a0-126">Проверите доступност саветника у приказу календара.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-126">Check consultants’ availability in a calendar view.</span></span>  
  
- <span data-ttu-id="5a8a0-127">[Приказ укупне искоришћености ресурса](../psa/view-resource-utilization.md).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-127">[View resource utilization](../psa/view-resource-utilization.md).</span></span> <span data-ttu-id="5a8a0-128">Погледајте проценат времена за које су ваши саветници тренутно резервисани.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-128">See the percentage of time that your consultants are currently booked.</span></span>  
  
- <span data-ttu-id="5a8a0-129">[Планирајте ресурсе за пројекат](../psa/schedule-resources-project.md).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-129">[Schedule resources for a project](../psa/schedule-resources-project.md).</span></span> <span data-ttu-id="5a8a0-130">Планирајте консултанте за пројекат.</span><span class="sxs-lookup"><span data-stu-id="5a8a0-130">Schedule consultants for a project.</span></span>  
  
  <span data-ttu-id="5a8a0-131">Више информација о прослеђивању захтева за ресурсе за појединачне пројекте потражите у чланку [Подношење захтева за ресурсе](../psa/submit-resource-requests.md).</span><span class="sxs-lookup"><span data-stu-id="5a8a0-131">For more information about submitting resource requests for individual projects, see [Submit resource requests](../psa/submit-resource-requests.md).</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="5a8a0-132">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="5a8a0-132">See Also</span></span>  
 <span data-ttu-id="5a8a0-133">[Преглед услуге Project Service](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="5a8a0-133">[Overview of Project Service](../psa/overview.md) </span></span>  
 <span data-ttu-id="5a8a0-134">[Водич за администраторе](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5a8a0-134">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="5a8a0-135">[Водич за менаџера за пословне контакте](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5a8a0-135">[Account Manager Guiden](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="5a8a0-136">[Водич за менаџера пројекта](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5a8a0-136">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 [<span data-ttu-id="5a8a0-137">Водич за време, трошак и сарадњу</span><span class="sxs-lookup"><span data-stu-id="5a8a0-137">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)
