---
title: Како да „услово резервишете“ ресурсе у апликацији у верзији 2.x?
description: У овом чланку описано је како да условно резервишете чланове пројектног тима уз помоћ програма Project Service.
author: JohnPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.prod: Applies to Project Service version 2.x
ms.technology: ''
ms.assetid: 27063de4-cb0c-436f-970e-c87ebcab92db
ms.author: john.burrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: aad119c0907cdd31220a0d73e6e7d99ee63e2e13
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755386"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="71183-103">Како да „условно резервишем“ ресурсе у веб апликацији (апликација Project Service у верзији v2.x)?</span><span class="sxs-lookup"><span data-stu-id="71183-103">How do I "soft book" resources in the web app (Project Service app v2.x)?</span></span>

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="71183-104">Условно можете да распоредите или „условно резервишете“ ресурс у пројектни тим како бисте приказали да намеравате да доделите ресурс пројекту.</span><span class="sxs-lookup"><span data-stu-id="71183-104">You can tentatively schedule or "soft book" a resource onto a project team to show you plan to assign the resource to a project.</span></span> <span data-ttu-id="71183-105">Условне резервације не троше доступни капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="71183-105">Soft bookings don’t consume a resource’s available capacity.</span></span> <span data-ttu-id="71183-106">Условно резервисани чланови тима не могу бити додељени пројектним задацима.</span><span class="sxs-lookup"><span data-stu-id="71183-106">Soft-booked team members can’t be assigned to project tasks.</span></span> <span data-ttu-id="71183-107">Само ресурси који имају статус Фиксно резервисани и тип примене Примењено могу бити додељени задацима (под претпоставком да имају довољно фиксно резервисаних радних часова да покрију ангажовање за доделу).</span><span class="sxs-lookup"><span data-stu-id="71183-107">Only resources with the Status Hard Booked and Commit Type Committed can be assigned to tasks (assuming they have enough hard booking hours to cover the assignment effort).</span></span>

<span data-ttu-id="71183-108">Условно резервисани чланови тима се приказују у координатној мрежи Члан тима са условно резервисаним часовима приказаним у колони Условно резервисање.</span><span class="sxs-lookup"><span data-stu-id="71183-108">Soft-booked project team members show up in the Team Member grid with their soft-booked hours shown in the Soft Book column.</span></span> <span data-ttu-id="71183-109">Приказују се и на табели распореда.</span><span class="sxs-lookup"><span data-stu-id="71183-109">They also show up on the schedule board.</span></span> <span data-ttu-id="71183-110">Поново, они не означавају никакво коришћење капацитета, јер условно резервисање не користи капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="71183-110">Again, they don’t indicate any consumption of capacity as soft-booking doesn’t consume capacity of a resource.</span></span>

<span data-ttu-id="71183-111">Постоје три начина да условно резервишете члана тима за пројекат помоћу програма Project Service у верзији 2.x.</span><span class="sxs-lookup"><span data-stu-id="71183-111">There are three ways to soft-book a team member onto a project with Project Service version 2.x.</span></span> <span data-ttu-id="71183-112">Можете условно да резервишете са табелом распореда, да користите функцију Одржавање резервација или да креирате генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="71183-112">You can soft-book with the schedule board, use the Maintain Bookings feature, or by creating a generic resource.</span></span> <span data-ttu-id="71183-113">Ови начини су описани у наставку.</span><span class="sxs-lookup"><span data-stu-id="71183-113">These methods are described below.</span></span>

## <a name="soft-book-with-the-schedule-board"></a><span data-ttu-id="71183-114">Условно резервисање са табелом распореда</span><span class="sxs-lookup"><span data-stu-id="71183-114">Soft-book with the schedule board</span></span>

<span data-ttu-id="71183-115">Да бисте условно резервисали помоћу табеле распореда, пратите ову процедуру:</span><span class="sxs-lookup"><span data-stu-id="71183-115">To soft-book with the schedule board, follow this procedure:</span></span> 
1. <span data-ttu-id="71183-116">Отвори табелу распореда.</span><span class="sxs-lookup"><span data-stu-id="71183-116">Open the schedule board.</span></span>
2. <span data-ttu-id="71183-117">Изаберите картицу Пројекат на дну табле Захтеви за резервацију у оквиру табле распореда.</span><span class="sxs-lookup"><span data-stu-id="71183-117">Select the Project tab on the bottom Booking Requirements panel of the schedule board.</span></span>
3. <span data-ttu-id="71183-118">Пронађите пројекат за који желите да условно резервишете ресурс.</span><span class="sxs-lookup"><span data-stu-id="71183-118">Find the project you wish to soft-book a resource on.</span></span> <span data-ttu-id="71183-119">Ако имате више пројеката, кликните на заглавље колоне Пројекат, а затим пронађите свој пројекат помоћу филтера.</span><span class="sxs-lookup"><span data-stu-id="71183-119">If you have many projects, click on the Project column header and then use the filter to find your project.</span></span>
4. <span data-ttu-id="71183-120">Кликните на пројекат, а затим га превуците на координатну мрежу времена ресурса.</span><span class="sxs-lookup"><span data-stu-id="71183-120">Click on the project, then drag and drop it on the resource’s time grid.</span></span>
5. <span data-ttu-id="71183-121">То отвара таблу Креирање резервације ресурса са десне стране.</span><span class="sxs-lookup"><span data-stu-id="71183-121">This opens the Create Resource Booking panel on the right.</span></span> <span data-ttu-id="71183-122">Подесите датуме почетка и завршетка, изаберите Статус резервације као Условно и подесите часове.</span><span class="sxs-lookup"><span data-stu-id="71183-122">Adjust the start and end date, select the Booking Status as Soft and set the hours.</span></span> 
6. <span data-ttu-id="71183-123">Кликните на Резервиши.</span><span class="sxs-lookup"><span data-stu-id="71183-123">Click Book.</span></span>
7. <span data-ttu-id="71183-124">Натраг на пројекту, ресурс ће се сада приказивати као члан тима са условно резервисаним часовима у колони Условно резервисање.</span><span class="sxs-lookup"><span data-stu-id="71183-124">Back on the project, the resource will now show as a team member with the soft booked hours in the Soft Book column.</span></span>

<span data-ttu-id="71183-125">Имајте на уму да не можете да их доделите задацима у структурној анализи посла (САП) јер ресурси морају да буду фиксно резервисани за тим да би били додељени.</span><span class="sxs-lookup"><span data-stu-id="71183-125">Note that you can’t assign them to tasks on the work breakdown structure (WBS) as resources must be hard booked on the team to be assigned.</span></span>

## <a name="soft-book-using-the-maintain-bookings-feature"></a><span data-ttu-id="71183-126">Условно резервисање коришћењем функције Одржавање резервација</span><span class="sxs-lookup"><span data-stu-id="71183-126">Soft-book using the Maintain Bookings feature</span></span>

<span data-ttu-id="71183-127">Да бисте условно резервисали помоћу Одржавања резервација, пратите ову процедуру:</span><span class="sxs-lookup"><span data-stu-id="71183-127">To soft-book with Maintain Bookings follow this procedure:</span></span>
1. <span data-ttu-id="71183-128">Са мреже члана тима, кликните на Нови.</span><span class="sxs-lookup"><span data-stu-id="71183-128">From the team member grid, Click New.</span></span>
2. <span data-ttu-id="71183-129">Изаберите ресурс који је могуће резервисати, улогу, од/до.</span><span class="sxs-lookup"><span data-stu-id="71183-129">Select the bookable resource, role, from/to.</span></span>
3. <span data-ttu-id="71183-130">Изаберите начин доделе који није Ниједно:</span><span class="sxs-lookup"><span data-stu-id="71183-130">Select an allocation method other than None:</span></span>
- <span data-ttu-id="71183-131">Пуни капацитет</span><span class="sxs-lookup"><span data-stu-id="71183-131">Full Capacity</span></span>
- <span data-ttu-id="71183-132">Капацитет у процентима</span><span class="sxs-lookup"><span data-stu-id="71183-132">Percentage Capacity</span></span>
- <span data-ttu-id="71183-133">Равномерно распоређивање по сатима</span><span class="sxs-lookup"><span data-stu-id="71183-133">By Hours Distribute Evenly</span></span>
- <span data-ttu-id="71183-134">Почетно оптерећење по часовима</span><span class="sxs-lookup"><span data-stu-id="71183-134">By Hours Front Load</span></span>
4. <span data-ttu-id="71183-135">Кликните на Сачувај.</span><span class="sxs-lookup"><span data-stu-id="71183-135">Click Save.</span></span> <span data-ttu-id="71183-136">Видећете ресурс на мрежи тима, а његове часове означене као Фиксне.</span><span class="sxs-lookup"><span data-stu-id="71183-136">You’ll see the resource on the team grid and their hours indicated as Hard.</span></span>
5. <span data-ttu-id="71183-137">Одржите резервације ресурса кликом на Одржавање резервација.</span><span class="sxs-lookup"><span data-stu-id="71183-137">Maintain the resource’s bookings by clicking Maintain Bookings.</span></span>
6. <span data-ttu-id="71183-138">Када се отвори табела распореда, развијте ресурс да бисте приказали његове резервације.</span><span class="sxs-lookup"><span data-stu-id="71183-138">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="71183-139">Видећете резервацију означену као „Фиксна“.</span><span class="sxs-lookup"><span data-stu-id="71183-139">You will see the booking indicated as Hard.</span></span>
7. <span data-ttu-id="71183-140">Кликните десним тастером миша на резервацију, у оквиру опције „Промена статуса“, изаберите „Условно резервиши“ и затим „Условно“.</span><span class="sxs-lookup"><span data-stu-id="71183-140">Right-click the booking, under Change Status, select Soft Book and then Soft.</span></span> <span data-ttu-id="71183-141">Статус резервације је сада „Условна“.</span><span class="sxs-lookup"><span data-stu-id="71183-141">The booking status is now Soft.</span></span>
8. <span data-ttu-id="71183-142">Након затварања табеле распореда, видећете да су сати за ресурс промењени из „Фиксни“ на „Условни“ на мрежи члана тима.</span><span class="sxs-lookup"><span data-stu-id="71183-142">After closing the schedule board, you’ll see that the hours for the resource have changed from Hard to Soft on the team member grid.</span></span>
<span data-ttu-id="71183-143">Имајте у виду да ако фиксно резервишете ресурс за тима, а затим му доделите задатке у САП-у, када користите одржавање резервација да бисте променили статус из „Фиксна“ у „Условна“, уклонићете доделе из задатака за тај ресурс, јер само фиксно резервисани ресурси могу бити додељени задацима.</span><span class="sxs-lookup"><span data-stu-id="71183-143">Note that if you hard book a resource onto the team and then assign them tasks in the WBS, when you use maintain bookings to change the status of Hard to Soft, it will remove the assignments from the tasks for that resource, as only hard booked resources can be assigned to tasks.</span></span>

## <a name="soft-book-by-creating-a-generic-resource"></a><span data-ttu-id="71183-144">Условно резервисање креирањем генеричког ресурса</span><span class="sxs-lookup"><span data-stu-id="71183-144">Soft-book by creating a generic resource</span></span>

<span data-ttu-id="71183-145">Условно резервисање можете да креирате генерисањем генеричког члана тима, испуњавањем са табелом распореда или Захтевом за ресурс и променом типа током резервације.</span><span class="sxs-lookup"><span data-stu-id="71183-145">You can create a soft-booking by generating a generic resource team member, fulfilling with schedule board or Resource Request and changing the type during the booking.</span></span>
<span data-ttu-id="71183-146">То можете да урадите помоћу следеће процедуре:</span><span class="sxs-lookup"><span data-stu-id="71183-146">To do this, use the following procedure:</span></span>

1. <span data-ttu-id="71183-147">У САП-у пројекта доделите улоге задацима за које желите да генеришете генеричке чланове тима.</span><span class="sxs-lookup"><span data-stu-id="71183-147">On the project WBS, assign roles to the tasks you wish to generate generic team members for.</span></span>
2. <span data-ttu-id="71183-148">Кликните на Генерисање пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="71183-148">Click Generate Project Team.</span></span>
3. <span data-ttu-id="71183-149">На мрежи члана пројектног тима изаберите генерички ресурс и кликните на дугме „Резервиши“.</span><span class="sxs-lookup"><span data-stu-id="71183-149">On the project team member grid, select the generic resource and click Book.</span></span>
4. <span data-ttu-id="71183-150">На табели распореда, изаберите ресурс који желите да резервишете.</span><span class="sxs-lookup"><span data-stu-id="71183-150">On the schedule board, select the resource that you wish to book.</span></span>
5. <span data-ttu-id="71183-151">На табли „Креирање резервације ресурса“ табеле распореда, промените Статус резервације на „Условна“.</span><span class="sxs-lookup"><span data-stu-id="71183-151">On the schedule board’s Create Resource Booking panel, change the Booking Status to Soft.</span></span>
6. <span data-ttu-id="71183-152">Кликните на дугме „Резервиши“ и „Резервиши и изађи“.</span><span class="sxs-lookup"><span data-stu-id="71183-152">Click Book or Book and Exit.</span></span>

<span data-ttu-id="71183-153">Након затварања табеле распореда, видећете да је изабрани ресурс додат у тим са условно резервисаним, као и са додељеним часовима.</span><span class="sxs-lookup"><span data-stu-id="71183-153">After closing the schedule board, you’ll see the selected resource added to the team with Soft booked hours as well as assigned hours.</span></span> <span data-ttu-id="71183-154">Видећете и да генерички ресурс остаје у тиму као индикатор да су задаци додељени члану тима који је условно резервисан.</span><span class="sxs-lookup"><span data-stu-id="71183-154">You’ll also see that the generic resource remains on the team as an indicator that the tasks are assigned to a soft-booked team member.</span></span>

<span data-ttu-id="71183-155">Када будете спремни да промените ресурс условно резервисаног члана тима у фиксно резервисаног члана тима како бисте могли да му додељујете задатке, поступите на следећи начин:</span><span class="sxs-lookup"><span data-stu-id="71183-155">When you’re ready to change a soft-booked team member resource to a hard-booked team member so that you can assign them to tasks, do the following:</span></span>

1. <span data-ttu-id="71183-156">Изаберите тај ресурс и кликните на дугме „Одржавање резервација“.</span><span class="sxs-lookup"><span data-stu-id="71183-156">Select that resource and click Maintain Bookings.</span></span>
2. <span data-ttu-id="71183-157">Када се отвори табела распореда, развијте ресурс да бисте приказали његове резервације.</span><span class="sxs-lookup"><span data-stu-id="71183-157">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="71183-158">Видећете да је резервација означена као „Условна“.</span><span class="sxs-lookup"><span data-stu-id="71183-158">You’ll see the booking marked as Soft.</span></span>
3. <span data-ttu-id="71183-159">Кликните десним тастером миша на резервацију, у оквиру опције „Промена статуса“, изаберите „Фиксно резервиши“ и затим „Фиксно“.</span><span class="sxs-lookup"><span data-stu-id="71183-159">Right-click the booking, under Change Status, select Hard Book and then Hard.</span></span> <span data-ttu-id="71183-160">Статус резервације је сада „Фиксно“.</span><span class="sxs-lookup"><span data-stu-id="71183-160">The booking status is now Hard.</span></span>
4. <span data-ttu-id="71183-161">Након затварања табеле распореда, видећете да су сати за ресурс промењени из „Фиксни“ на „Условни“ на мрежи члана тима.</span><span class="sxs-lookup"><span data-stu-id="71183-161">After closing the schedule board, you’ll see that the hours for the resource have changed from Soft to Hard on the team member grid.</span></span> <span data-ttu-id="71183-162">Сада можете да доделите ресурс задацима (уколико постоји усклађеност између фиксно резервисаних часова и часова ангажовања задатка за доделу).</span><span class="sxs-lookup"><span data-stu-id="71183-162">You may now assign the resource to tasks (provided there is alignment between the hard-booked hours and the effort hours of the task for assignment).</span></span> <span data-ttu-id="71183-163">Имајте у виду да ако сте пратили кораке испуњења генеричког ресурса у ставци бр. 3 изнад, када промените статус условно резервисаног ресурса у фиксно резервисани, генерички члан тима се уклања из тима.</span><span class="sxs-lookup"><span data-stu-id="71183-163">Note that if you followed the generic resource fulfilment steps in item #3 above, when you change the status of the soft-booked bookable resource to hard, the generic team member is removed from the team.</span></span>
