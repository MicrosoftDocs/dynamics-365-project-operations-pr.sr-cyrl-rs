---
title: Како да „услово резервишете“ ресурсе у апликацији у верзији 2.x?
description: У овом чланку описано је како да условно резервишете чланове пројектног тима уз помоћ програма Project Service.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 18a1176c131e233f62f74dc0dd8a6aa3ee561da5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286041"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="f92c7-103">Како да „условно резервишем“ ресурсе у веб апликацији (апликација Project Service у верзији v2.x)?</span><span class="sxs-lookup"><span data-stu-id="f92c7-103">How do I "soft book" resources in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="f92c7-104">Условно можете да распоредите или „условно резервишете“ ресурс у пројектни тим како бисте приказали да намеравате да доделите ресурс пројекту.</span><span class="sxs-lookup"><span data-stu-id="f92c7-104">You can tentatively schedule or "soft book" a resource onto a project team to show you plan to assign the resource to a project.</span></span> <span data-ttu-id="f92c7-105">Условне резервације не троше доступни капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="f92c7-105">Soft bookings don’t consume a resource’s available capacity.</span></span> <span data-ttu-id="f92c7-106">Условно резервисани чланови тима не могу бити додељени пројектним задацима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-106">Soft-booked team members can’t be assigned to project tasks.</span></span> <span data-ttu-id="f92c7-107">Само ресурси који имају статус Фиксно резервисани и тип примене Примењено могу бити додељени задацима (под претпоставком да имају довољно фиксно резервисаних радних часова да покрију ангажовање за доделу).</span><span class="sxs-lookup"><span data-stu-id="f92c7-107">Only resources with the Status Hard Booked and Commit Type Committed can be assigned to tasks (assuming they have enough hard booking hours to cover the assignment effort).</span></span>

<span data-ttu-id="f92c7-108">Условно резервисани чланови тима се приказују у координатној мрежи Члан тима са условно резервисаним часовима приказаним у колони Условно резервисање.</span><span class="sxs-lookup"><span data-stu-id="f92c7-108">Soft-booked project team members show up in the Team Member grid with their soft-booked hours shown in the Soft Book column.</span></span> <span data-ttu-id="f92c7-109">Приказују се и на табели распореда.</span><span class="sxs-lookup"><span data-stu-id="f92c7-109">They also show up on the schedule board.</span></span> <span data-ttu-id="f92c7-110">Поново, они не означавају никакво коришћење капацитета, јер условно резервисање не користи капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="f92c7-110">Again, they don’t indicate any consumption of capacity as soft-booking doesn’t consume capacity of a resource.</span></span>

<span data-ttu-id="f92c7-111">Постоје три начина да условно резервишете члана тима за пројекат помоћу програма Project Service у верзији 2.x.</span><span class="sxs-lookup"><span data-stu-id="f92c7-111">There are three ways to soft-book a team member onto a project with Project Service version 2.x.</span></span> <span data-ttu-id="f92c7-112">Можете условно да резервишете са табелом распореда, да користите функцију Одржавање резервација или да креирате генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="f92c7-112">You can soft-book with the schedule board, use the Maintain Bookings feature, or by creating a generic resource.</span></span> <span data-ttu-id="f92c7-113">Ови начини су описани у наставку.</span><span class="sxs-lookup"><span data-stu-id="f92c7-113">These methods are described below.</span></span>

## <a name="soft-book-with-the-schedule-board"></a><span data-ttu-id="f92c7-114">Условно резервисање са табелом распореда</span><span class="sxs-lookup"><span data-stu-id="f92c7-114">Soft-book with the schedule board</span></span>

<span data-ttu-id="f92c7-115">Да бисте условно резервисали помоћу табеле распореда, пратите ову процедуру:</span><span class="sxs-lookup"><span data-stu-id="f92c7-115">To soft-book with the schedule board, follow this procedure:</span></span> 
1. <span data-ttu-id="f92c7-116">Отвори табелу распореда.</span><span class="sxs-lookup"><span data-stu-id="f92c7-116">Open the schedule board.</span></span>
2. <span data-ttu-id="f92c7-117">Изаберите картицу Пројекат на дну табле Захтеви за резервацију у оквиру табле распореда.</span><span class="sxs-lookup"><span data-stu-id="f92c7-117">Select the Project tab on the bottom Booking Requirements panel of the schedule board.</span></span>
3. <span data-ttu-id="f92c7-118">Пронађите пројекат за који желите да условно резервишете ресурс.</span><span class="sxs-lookup"><span data-stu-id="f92c7-118">Find the project you wish to soft-book a resource on.</span></span> <span data-ttu-id="f92c7-119">Ако имате више пројеката, кликните на заглавље колоне Пројекат, а затим пронађите свој пројекат помоћу филтера.</span><span class="sxs-lookup"><span data-stu-id="f92c7-119">If you have many projects, click on the Project column header and then use the filter to find your project.</span></span>
4. <span data-ttu-id="f92c7-120">Кликните на пројекат, а затим га превуците на координатну мрежу времена ресурса.</span><span class="sxs-lookup"><span data-stu-id="f92c7-120">Click on the project, then drag and drop it on the resource’s time grid.</span></span>
5. <span data-ttu-id="f92c7-121">То отвара таблу Креирање резервације ресурса са десне стране.</span><span class="sxs-lookup"><span data-stu-id="f92c7-121">This opens the Create Resource Booking panel on the right.</span></span> <span data-ttu-id="f92c7-122">Подесите датуме почетка и завршетка, изаберите Статус резервације као Условно и подесите часове.</span><span class="sxs-lookup"><span data-stu-id="f92c7-122">Adjust the start and end date, select the Booking Status as Soft and set the hours.</span></span> 
6. <span data-ttu-id="f92c7-123">Кликните на Резервиши.</span><span class="sxs-lookup"><span data-stu-id="f92c7-123">Click Book.</span></span>
7. <span data-ttu-id="f92c7-124">Натраг на пројекту, ресурс ће се сада приказивати као члан тима са условно резервисаним часовима у колони Условно резервисање.</span><span class="sxs-lookup"><span data-stu-id="f92c7-124">Back on the project, the resource will now show as a team member with the soft booked hours in the Soft Book column.</span></span>

<span data-ttu-id="f92c7-125">Имајте на уму да не можете да их доделите задацима у структурној анализи посла (САП) јер ресурси морају да буду фиксно резервисани за тим да би били додељени.</span><span class="sxs-lookup"><span data-stu-id="f92c7-125">Note that you can’t assign them to tasks on the work breakdown structure (WBS) as resources must be hard booked on the team to be assigned.</span></span>

## <a name="soft-book-using-the-maintain-bookings-feature"></a><span data-ttu-id="f92c7-126">Условно резервисање коришћењем функције Одржавање резервација</span><span class="sxs-lookup"><span data-stu-id="f92c7-126">Soft-book using the Maintain Bookings feature</span></span>

<span data-ttu-id="f92c7-127">Да бисте условно резервисали помоћу Одржавања резервација, пратите ову процедуру:</span><span class="sxs-lookup"><span data-stu-id="f92c7-127">To soft-book with Maintain Bookings follow this procedure:</span></span>
1. <span data-ttu-id="f92c7-128">Са мреже члана тима, кликните на Нови.</span><span class="sxs-lookup"><span data-stu-id="f92c7-128">From the team member grid, Click New.</span></span>
2. <span data-ttu-id="f92c7-129">Изаберите ресурс који је могуће резервисати, улогу, од/до.</span><span class="sxs-lookup"><span data-stu-id="f92c7-129">Select the bookable resource, role, from/to.</span></span>
3. <span data-ttu-id="f92c7-130">Изаберите начин доделе који није Ниједно:</span><span class="sxs-lookup"><span data-stu-id="f92c7-130">Select an allocation method other than None:</span></span>
- <span data-ttu-id="f92c7-131">Пуни капацитет</span><span class="sxs-lookup"><span data-stu-id="f92c7-131">Full Capacity</span></span>
- <span data-ttu-id="f92c7-132">Капацитет у процентима</span><span class="sxs-lookup"><span data-stu-id="f92c7-132">Percentage Capacity</span></span>
- <span data-ttu-id="f92c7-133">Равномерно распоређивање по сатима</span><span class="sxs-lookup"><span data-stu-id="f92c7-133">By Hours Distribute Evenly</span></span>
- <span data-ttu-id="f92c7-134">Почетно оптерећење по часовима</span><span class="sxs-lookup"><span data-stu-id="f92c7-134">By Hours Front Load</span></span>
4. <span data-ttu-id="f92c7-135">Кликните на Сачувај.</span><span class="sxs-lookup"><span data-stu-id="f92c7-135">Click Save.</span></span> <span data-ttu-id="f92c7-136">Видећете ресурс на мрежи тима, а његове часове означене као Фиксне.</span><span class="sxs-lookup"><span data-stu-id="f92c7-136">You’ll see the resource on the team grid and their hours indicated as Hard.</span></span>
5. <span data-ttu-id="f92c7-137">Одржите резервације ресурса кликом на Одржавање резервација.</span><span class="sxs-lookup"><span data-stu-id="f92c7-137">Maintain the resource’s bookings by clicking Maintain Bookings.</span></span>
6. <span data-ttu-id="f92c7-138">Када се отвори табела распореда, развијте ресурс да бисте приказали његове резервације.</span><span class="sxs-lookup"><span data-stu-id="f92c7-138">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="f92c7-139">Видећете резервацију означену као „Фиксна“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-139">You will see the booking indicated as Hard.</span></span>
7. <span data-ttu-id="f92c7-140">Кликните десним тастером миша на резервацију, у оквиру опције „Промена статуса“, изаберите „Условно резервиши“ и затим „Условно“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-140">Right-click the booking, under Change Status, select Soft Book and then Soft.</span></span> <span data-ttu-id="f92c7-141">Статус резервације је сада „Условна“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-141">The booking status is now Soft.</span></span>
8. <span data-ttu-id="f92c7-142">Након затварања табеле распореда, видећете да су сати за ресурс промењени из „Фиксни“ на „Условни“ на мрежи члана тима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-142">After closing the schedule board, you’ll see that the hours for the resource have changed from Hard to Soft on the team member grid.</span></span>
<span data-ttu-id="f92c7-143">Имајте у виду да ако фиксно резервишете ресурс за тима, а затим му доделите задатке у САП-у, када користите одржавање резервација да бисте променили статус из „Фиксна“ у „Условна“, уклонићете доделе из задатака за тај ресурс, јер само фиксно резервисани ресурси могу бити додељени задацима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-143">Note that if you hard book a resource onto the team and then assign them tasks in the WBS, when you use maintain bookings to change the status of Hard to Soft, it will remove the assignments from the tasks for that resource, as only hard booked resources can be assigned to tasks.</span></span>

## <a name="soft-book-by-creating-a-generic-resource"></a><span data-ttu-id="f92c7-144">Условно резервисање креирањем генеричког ресурса</span><span class="sxs-lookup"><span data-stu-id="f92c7-144">Soft-book by creating a generic resource</span></span>

<span data-ttu-id="f92c7-145">Условно резервисање можете да креирате генерисањем генеричког члана тима, испуњавањем са табелом распореда или Захтевом за ресурс и променом типа током резервације.</span><span class="sxs-lookup"><span data-stu-id="f92c7-145">You can create a soft-booking by generating a generic resource team member, fulfilling with schedule board or Resource Request and changing the type during the booking.</span></span>
<span data-ttu-id="f92c7-146">То можете да урадите помоћу следеће процедуре:</span><span class="sxs-lookup"><span data-stu-id="f92c7-146">To do this, use the following procedure:</span></span>

1. <span data-ttu-id="f92c7-147">У САП-у пројекта доделите улоге задацима за које желите да генеришете генеричке чланове тима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-147">On the project WBS, assign roles to the tasks you wish to generate generic team members for.</span></span>
2. <span data-ttu-id="f92c7-148">Кликните на Генерисање пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-148">Click Generate Project Team.</span></span>
3. <span data-ttu-id="f92c7-149">На мрежи члана пројектног тима изаберите генерички ресурс и кликните на дугме „Резервиши“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-149">On the project team member grid, select the generic resource and click Book.</span></span>
4. <span data-ttu-id="f92c7-150">На табели распореда, изаберите ресурс који желите да резервишете.</span><span class="sxs-lookup"><span data-stu-id="f92c7-150">On the schedule board, select the resource that you wish to book.</span></span>
5. <span data-ttu-id="f92c7-151">На табли „Креирање резервације ресурса“ табеле распореда, промените Статус резервације на „Условна“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-151">On the schedule board’s Create Resource Booking panel, change the Booking Status to Soft.</span></span>
6. <span data-ttu-id="f92c7-152">Кликните на дугме „Резервиши“ и „Резервиши и изађи“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-152">Click Book or Book and Exit.</span></span>

<span data-ttu-id="f92c7-153">Након затварања табеле распореда, видећете да је изабрани ресурс додат у тим са условно резервисаним, као и са додељеним часовима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-153">After closing the schedule board, you’ll see the selected resource added to the team with Soft booked hours as well as assigned hours.</span></span> <span data-ttu-id="f92c7-154">Видећете и да генерички ресурс остаје у тиму као индикатор да су задаци додељени члану тима који је условно резервисан.</span><span class="sxs-lookup"><span data-stu-id="f92c7-154">You’ll also see that the generic resource remains on the team as an indicator that the tasks are assigned to a soft-booked team member.</span></span>

<span data-ttu-id="f92c7-155">Када будете спремни да промените ресурс условно резервисаног члана тима у фиксно резервисаног члана тима како бисте могли да му додељујете задатке, поступите на следећи начин:</span><span class="sxs-lookup"><span data-stu-id="f92c7-155">When you’re ready to change a soft-booked team member resource to a hard-booked team member so that you can assign them to tasks, do the following:</span></span>

1. <span data-ttu-id="f92c7-156">Изаберите тај ресурс и кликните на дугме „Одржавање резервација“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-156">Select that resource and click Maintain Bookings.</span></span>
2. <span data-ttu-id="f92c7-157">Када се отвори табела распореда, развијте ресурс да бисте приказали његове резервације.</span><span class="sxs-lookup"><span data-stu-id="f92c7-157">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="f92c7-158">Видећете да је резервација означена као „Условна“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-158">You’ll see the booking marked as Soft.</span></span>
3. <span data-ttu-id="f92c7-159">Кликните десним тастером миша на резервацију, у оквиру опције „Промена статуса“, изаберите „Фиксно резервиши“ и затим „Фиксно“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-159">Right-click the booking, under Change Status, select Hard Book and then Hard.</span></span> <span data-ttu-id="f92c7-160">Статус резервације је сада „Фиксно“.</span><span class="sxs-lookup"><span data-stu-id="f92c7-160">The booking status is now Hard.</span></span>
4. <span data-ttu-id="f92c7-161">Након затварања табеле распореда, видећете да су сати за ресурс промењени из „Фиксни“ на „Условни“ на мрежи члана тима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-161">After closing the schedule board, you’ll see that the hours for the resource have changed from Soft to Hard on the team member grid.</span></span> <span data-ttu-id="f92c7-162">Сада можете да доделите ресурс задацима (уколико постоји усклађеност између фиксно резервисаних часова и часова ангажовања задатка за доделу).</span><span class="sxs-lookup"><span data-stu-id="f92c7-162">You may now assign the resource to tasks (provided there is alignment between the hard-booked hours and the effort hours of the task for assignment).</span></span> <span data-ttu-id="f92c7-163">Имајте у виду да ако сте пратили кораке испуњења генеричког ресурса у ставци бр. 3 изнад, када промените статус условно резервисаног ресурса у фиксно резервисани, генерички члан тима се уклања из тима.</span><span class="sxs-lookup"><span data-stu-id="f92c7-163">Note that if you followed the generic resource fulfilment steps in item #3 above, when you change the status of the soft-booked bookable resource to hard, the generic team member is removed from the team.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]