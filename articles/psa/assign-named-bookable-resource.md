---
title: Резервисање именованих ресурса које је могуће резервисати за пројектни тим и додељивање задатака
description: Ова тема пружа информације о томе како да резервишете именоване ресурсе за пројектне тимове и додељујете их задацима.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/28/2018
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
ms.openlocfilehash: 6169f2bdc107e63d666fb32d34f531fd5d472c2f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291457"
---
# <a name="book-named-bookable-resources-to-a-project-team-and-assign-tasks"></a><span data-ttu-id="e1713-103">Резервисање именованих ресурса које је могуће резервисати за пројектни тим и додељивање задатака</span><span class="sxs-lookup"><span data-stu-id="e1713-103">Book named bookable resources to a project team and assign tasks</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e1713-104">Можете да додате именовани ресурс у пројектни тим тако што ћете га директно резервисати за тим.</span><span class="sxs-lookup"><span data-stu-id="e1713-104">You can  add a named resource to your project team by booking them directly onto the team.</span></span> <span data-ttu-id="e1713-105">Да бисте то урадили, обавите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="e1713-105">To do this, complete the following steps.</span></span>

1. <span data-ttu-id="e1713-106">У апликацији Project Service Automation идите на **Пројекат** и отворите пројекат за који резервишете ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e1713-106">In  Project Service Automation, go to **Projects**, and select the open the project that you are booking for.</span></span>
2. <span data-ttu-id="e1713-107">На страници **Пројекат**, на картици **Тим** кликните на **Ново**.</span><span class="sxs-lookup"><span data-stu-id="e1713-107">On the **Project** page, on the **Team** tab, click **New**.</span></span> 

![Додавање члана тима на картици Тим](media/RM-how-to-1.png)

3. <span data-ttu-id="e1713-109">У дијалогу **Брзо креирање члана пројектног тима** изаберите ресурс који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="e1713-109">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="e1713-110">Поље **Улога** ће се попунити подразумеваном улогом ресурса ако је она додељена.</span><span class="sxs-lookup"><span data-stu-id="e1713-110">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="e1713-111">Можете да промените улогу ако је потребно.</span><span class="sxs-lookup"><span data-stu-id="e1713-111">You can change the role if needed.</span></span> 
4. <span data-ttu-id="e1713-112">Изаберите датум почетка и завршетка, односно период у коме вам ресурс треба и изаберите начин доделе капацитета ресурса.</span><span class="sxs-lookup"><span data-stu-id="e1713-112">Select the from and to dates that the resource will be needed and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="e1713-113">Ако желите да члан тима буде особа која одобрава пројекат, изаберите опцију **Да** у пољу **Особа која одобрава пројекат**.</span><span class="sxs-lookup"><span data-stu-id="e1713-113">If you want the team member to be a project approver, select **Yes** in the **Project Approver** field.</span></span> <span data-ttu-id="e1713-114">Ово ће значити да члан тима може да одобри прослеђене ставке за време и трошкове за овај пројекат.</span><span class="sxs-lookup"><span data-stu-id="e1713-114">This will mean that the team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="e1713-115">Кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="e1713-115">Click **Save**.</span></span>

![Додавање члана тима у образац за брзо креирање](media/RM-how-to-2.png)


<span data-ttu-id="e1713-117">Сада можете доделити резервисани ресурс задацима у пројекту.</span><span class="sxs-lookup"><span data-stu-id="e1713-117">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="e1713-118">На страници **Пројекат** кликните на картицу **Распоред** да бисте доделили задатке новом ресурсу.</span><span class="sxs-lookup"><span data-stu-id="e1713-118">On the **Project** page, click the **Schedule** tab to assign tasks to the new resource.</span></span> <span data-ttu-id="e1713-119">Бирач ресурса који је покренут из поља **Ресурси** у мрежи задатака ће приказати чланове тима које можете изабрати.</span><span class="sxs-lookup"><span data-stu-id="e1713-119">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>

![Додељивање члана тима задатку на картици Распоред](media/RM-how-to-3.png)

<span data-ttu-id="e1713-121">У верзији 3 апликације Project Service Automation (PSA), резервисање ресурса и додељивање задатака нису тесно повезани.</span><span class="sxs-lookup"><span data-stu-id="e1713-121">In version 3 for Project Service Automation (PSA), resource bookings and task assignments are not tightly coupled.</span></span> <span data-ttu-id="e1713-122">То значи да када користите бирач ресурса у распореду, можете да доделите задатке члановима тима за више сати него што покрива њихово време резервисања за пројекат.</span><span class="sxs-lookup"><span data-stu-id="e1713-122">This means that when you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>
<span data-ttu-id="e1713-123">Можете да видите разлике између резервација чланова тима и додељених задатака на картици **Тим** или на картици **Усаглашавањe ресурса**. Такође можете да усагласите разлике између резервација и додела ресурса на детаљнијем нивоу.</span><span class="sxs-lookup"><span data-stu-id="e1713-123">You can see the differences between team member bookings and assignments on the **Team** tab or on the **Resource Reconciliation** tab. You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

![Картица Усаглашавањe ресурса](media/RM-how-to-4.png)

<span data-ttu-id="e1713-125">Такође можете користити бирач ресурса на картици **Распоред** да бисте потражили и изабрали ресурсе који могу да се резервишу, а који још нису део пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="e1713-125">You can also use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="e1713-126">Они се приказују у бирачу ресурса као **Остали ресурси**.</span><span class="sxs-lookup"><span data-stu-id="e1713-126">These are shown in the resource picker as **Other Resources**.</span></span>

![Додељивање ресурса који није члан тима задатку](media/RM-how-to-5.png)

<span data-ttu-id="e1713-128">Када то урадите, ресурс ће бити додат у тим пројекта и додељен задатку, али се не генеришу резервације.</span><span class="sxs-lookup"><span data-stu-id="e1713-128">When you do this, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

![Члан тима са доделама и без резервација](media/RM-how-to-6.png)

<span data-ttu-id="e1713-130">Можете користити могућност продужења резервације на картици **Усаглашеност** или **табелу распореда** да бисте резервисали капацитет ресурса за пројекат.</span><span class="sxs-lookup"><span data-stu-id="e1713-130">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

![Продужење резервације члана тима на картици Усаглашеност ресурса](media/RM-how-to-7.png)

<span data-ttu-id="e1713-132">Након што је члан тима резервисан за пројекат, можете да користите одржавање резервација или табелу распореда директно да бисте управљали резервацијама.</span><span class="sxs-lookup"><span data-stu-id="e1713-132">After a team member is booked on your project, you can use maintain bookings or use the Schedule Board directly to manage their bookings.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]