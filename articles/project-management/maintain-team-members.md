---
title: Одржавање чланова тима
description: Ова тема пружа информације о резервисању именованих ресурса за тимове пројекта и њиховом додељивању задацима.
author: ruhercul
ms.date: 10/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 00312c5a701768e0042e7e0236477c192690ded3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998654"
---
# <a name="maintain-team-members"></a><span data-ttu-id="ad0c7-103">Одржавање чланова тима</span><span class="sxs-lookup"><span data-stu-id="ad0c7-103">Maintain team members</span></span>

<span data-ttu-id="ad0c7-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="ad0c7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ad0c7-105">Можете да додате именовани ресурс у пројектни тим тако што ћете га директно резервисати за тим.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-105">You can add a named resource to your project team by booking them directly to the team.</span></span>

1. <span data-ttu-id="ad0c7-106">У апликацији Dynamics 365 Project Operations идите на ставку **Пројекти** и отворите пројекат за који резервишете ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-106">In Dynamics 365 Project Operations, go to **Projects**, and select the open the project that you're booking for.</span></span>
2. <span data-ttu-id="ad0c7-107">На страници **Пројекат**, на картици **Тим** изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-107">On the **Project** page, on the **Team** tab, select **New**.</span></span> 
3. <span data-ttu-id="ad0c7-108">У дијалогу **Брзо креирање члана пројектног тима** изаберите ресурс који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-108">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="ad0c7-109">Поље **Улога** ће се попунити подразумеваном улогом ресурса ако је она додељена.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-109">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="ad0c7-110">Можете да промените улогу.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-110">You can change the role.</span></span> 
4. <span data-ttu-id="ad0c7-111">Изаберите датум почетка и завршетка када вам је ресурс потребан и изаберите начин доделе капацитета ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-111">Select the from and to dates that the resource will be needed, and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="ad0c7-112">У пољу **Давалац одобрења за пројекат** изаберите опцију **Да** ако желите да члан тима буде давалац одобрења за пројекат.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-112">In the **Project Approver** field, select **Yes** if you want the team member to be a project approver.</span></span> <span data-ttu-id="ad0c7-113">Члан тима може да одобри прослеђене ставке времена и трошкова за овај пројекат.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-113">The team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="ad0c7-114">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-114">Select **Save**.</span></span>

<span data-ttu-id="ad0c7-115">Сада можете доделити резервисани ресурс задацима у пројекту.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-115">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="ad0c7-116">На страници **Пројекат** кликните на картицу **Распоред** да бисте доделили задатке новом ресурсу.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-116">On the **Project** page, on the **Schedule** tab, assign tasks to the new resource.</span></span> <span data-ttu-id="ad0c7-117">Бирач ресурса који је покренут из поља **Ресурси** у мрежи задатака ће приказати чланове тима које можете изабрати.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-117">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>


<span data-ttu-id="ad0c7-118">У услузи Project Operations, резервисања ресурса и доделе задатака нису уско повезани.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-118">In Project Operations, resource bookings and task assignments aren't tightly coupled.</span></span> <span data-ttu-id="ad0c7-119">Када користите бирач ресурса у распореду, можете да доделите задатке члановима тима за више сати него што покрива њихово време резервисања за пројекат.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-119">When you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>

<span data-ttu-id="ad0c7-120">Разлике између резервација и додела чланова тима приказане су на картицама **Тим** и **Усаглашавање ресурса**.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-120">The differences between team member bookings and assignments are shown on the **Team** and **Resource Reconciliation** tabs.</span></span> <span data-ttu-id="ad0c7-121">Разлике између резервација и доделе ресурса можете ускладити и на детаљнијем нивоу.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-121">You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

<span data-ttu-id="ad0c7-122">Користите бирач ресурса на картици **Распоред** да бисте потражили и изабрали ресурсе који могу да се резервишу, а који још нису део пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-122">Use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="ad0c7-123">Ови ресурси се приказују у бирачу ресурса као **Остали ресурси**.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-123">These resources are shown in the resource picker as **Other Resources**.</span></span>

<span data-ttu-id="ad0c7-124">Када то направите избор, ресурс ће бити додат у пројектни тим и додељен задатку, али се не генеришу резервације.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-124">When you make a selection, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

<span data-ttu-id="ad0c7-125">Можете користити могућност продужења резервације на картици **Усаглашеност** или **табелу распореда** да бисте резервисали капацитет ресурса за пројекат.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-125">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

<span data-ttu-id="ad0c7-126">Када се члан тима резервише за пројекат, можете да користите **Одржавање резервација** или **табелу распореда** директно да бисте управљали резервацијама.</span><span class="sxs-lookup"><span data-stu-id="ad0c7-126">After a team member is booked on your project, you can use **Maintain bookings** or the **Schedule Board** directly to manage their bookings.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]