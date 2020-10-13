---
title: Управљање временским зонама
description: Када се пројекат креира, његова временска зона заснива се на временској зони дефинисаној у предлошку радног сата који се примењује.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27f58f0dacc3404119a719547ad374629c740740
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961942"
---
# <a name="manage-time-zones"></a><span data-ttu-id="89fc0-103">Управљање временским зонама</span><span class="sxs-lookup"><span data-stu-id="89fc0-103">Manage time zones</span></span>

<span data-ttu-id="89fc0-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="89fc0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="89fc0-105">Пројекти</span><span class="sxs-lookup"><span data-stu-id="89fc0-105">Projects</span></span>

<span data-ttu-id="89fc0-106">Када се пројекат креира, његова временска зона се заснива на временској зони дефинисаној у предлошку радног сата који се примењује.</span><span class="sxs-lookup"><span data-stu-id="89fc0-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="89fc0-107">На обрасцу **Пројекат**, датуми су увек релативни у односу на временску зону корисника који је пријављен на свакој картици, осим картице **Задатак**. Када прегледате структурне анализе посла, датуми ће се увек приказивати у временској зони пројекта.</span><span class="sxs-lookup"><span data-stu-id="89fc0-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="89fc0-108">Задаци</span><span class="sxs-lookup"><span data-stu-id="89fc0-108">Tasks</span></span>

<span data-ttu-id="89fc0-109">Када се задатак креира, време почетка, време завршетка и број сати на дан контролишу се радним временом пројекта.</span><span class="sxs-lookup"><span data-stu-id="89fc0-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="89fc0-110">На пример, ако се задатак креира са пројектом чија је временска зона -8 PST и има радно време од 9:00 до 17:00 од понедељка до петка, сваки задатак креиран без доделе поштоваће време почетка и време завршетка календара пројекта.</span><span class="sxs-lookup"><span data-stu-id="89fc0-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="89fc0-111">Управљање ресурсима помоћу временских зона</span><span class="sxs-lookup"><span data-stu-id="89fc0-111">Manage resources with time zones</span></span>

<span data-ttu-id="89fc0-112">За тачне и предвидљиве резултате приликом употребе **продужења резервације**, постоје два кључна предуслова која морају бити испуњена:</span><span class="sxs-lookup"><span data-stu-id="89fc0-112">For accurate and predictable results when using **Extend Booking**, there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="89fc0-113">Корисник мора да конфигурише временску зону свог уређаја тако да одговара временској зони дефинисаној у системским **подешавањима персонализације**.</span><span class="sxs-lookup"><span data-stu-id="89fc0-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![Подешавања временске зоне у оперативном систему Windows 10](media/reconcile-assignments-03.png)

  ![Подешавања временске зоне у подешавањима персонализације](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="89fc0-116">Ресурс који може да се резервише мора имати најмање један минут радног времена који се преклапа са контурама које се користе за дефинисање траженог додатка.</span><span class="sxs-lookup"><span data-stu-id="89fc0-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="89fc0-117">На пример, следећи ресурси са радним временом које пада између 9:00 и 19:00.</span><span class="sxs-lookup"><span data-stu-id="89fc0-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![Поређење контура ресурса](media/reconcile-assignments-05.png)

<span data-ttu-id="89fc0-119">Следећа табела приказује:</span><span class="sxs-lookup"><span data-stu-id="89fc0-119">The following table shows:</span></span>

- <span data-ttu-id="89fc0-120">Предложак календара пројекта</span><span class="sxs-lookup"><span data-stu-id="89fc0-120">A project calendar template</span></span>
- <span data-ttu-id="89fc0-121">Ресурс А: овај ресурс има исти календар и налази се у истој временској зони као и пројекат.</span><span class="sxs-lookup"><span data-stu-id="89fc0-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="89fc0-122">Почетно време резервације ће бити у 9:00.</span><span class="sxs-lookup"><span data-stu-id="89fc0-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="89fc0-123">Ресурс Б: Овај ресурс се налази у другој временској зони у односу на пројекат и почиње у 7:00 у својој временској зони.</span><span class="sxs-lookup"><span data-stu-id="89fc0-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="89fc0-124">Међутим, резервације ће почети у 9:00, јер је то најраније време почетка контуре задатка.</span><span class="sxs-lookup"><span data-stu-id="89fc0-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="89fc0-125">Ресурси Ц и Д: Ресурси се налазе у различитим временским зонама, различитим међусобно и у односу на пројекат, а њихове резервације започињу најраније од одговарајућег расположивог времена почетка.</span><span class="sxs-lookup"><span data-stu-id="89fc0-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="89fc0-126">Ентитет</span><span class="sxs-lookup"><span data-stu-id="89fc0-126">Entity</span></span>  |<span data-ttu-id="89fc0-127">Календар</span><span class="sxs-lookup"><span data-stu-id="89fc0-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="89fc0-128">Предложак календара пројекта</span><span class="sxs-lookup"><span data-stu-id="89fc0-128">Project calendar template</span></span>   | ![календар пројекта](media/reconcile-assignments-06.png) |
|<span data-ttu-id="89fc0-130">Ресурс А</span><span class="sxs-lookup"><span data-stu-id="89fc0-130">Resource A</span></span>  | ![Календар ресурса А](media/reconcile-assignments-06.png) |
|<span data-ttu-id="89fc0-132">Ресурс Б</span><span class="sxs-lookup"><span data-stu-id="89fc0-132">Resource B</span></span>  |  ![Календар ресурса Б](media/reconcile-assignments-07.png) |
|<span data-ttu-id="89fc0-134">Ресурс Ц</span><span class="sxs-lookup"><span data-stu-id="89fc0-134">Resource C</span></span>  |  ![Календар ресурса Ц](media/reconcile-assignments-08.png) |
|<span data-ttu-id="89fc0-136">Ресурс Д</span><span class="sxs-lookup"><span data-stu-id="89fc0-136">Resource D</span></span>  | ![Календар ресурса Д](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="89fc0-138">Када одете на приказ **Усаглашавање**, приказују се доделе ресурса и придружени недостаци резервација.</span><span class="sxs-lookup"><span data-stu-id="89fc0-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![Приказ усклађивања пре продужетка](media/reconcile-assignments-10.png)

<span data-ttu-id="89fc0-140">Када се за сваки ресурс користи функција проширеног резервисања, резервације се успешно продужавају за сваки ресурс, јер се радно време сваког ресурса преклапа са контурама недостатка.</span><span class="sxs-lookup"><span data-stu-id="89fc0-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![Приказ усклађивања након продужења резервације](media/reconcile-assignments-11.png) 

<span data-ttu-id="89fc0-142">Приметите да бољи увид у детаље резервације показује разлике у времену почетка резервација.</span><span class="sxs-lookup"><span data-stu-id="89fc0-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="89fc0-143">Резервације почињу не раније од времена почетка контуре доделе и не раније од расположивог времена почетка ресурса.</span><span class="sxs-lookup"><span data-stu-id="89fc0-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![Нове резервације ресурса на табели распореда](media/reconcile-assignments-12.png)
