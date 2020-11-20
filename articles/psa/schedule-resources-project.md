---
title: Планирајте ресурсе за пројекат
description: Како да планирате ресурсе за пројекат у апликацији Project Service
author: JohnPBurrows
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 1479bf920be897a6ee3498aada7a6c36692a01fc
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4132170"
---
# <a name="schedule-resources-for-a-project-project-service"></a><span data-ttu-id="cfcbe-103">Планирање ресурса за пројекат (Project Service)</span><span class="sxs-lookup"><span data-stu-id="cfcbe-103">Schedule resources for a project (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="cfcbe-104">Можете да проверите доступност ресурса да бисте добили укупан приказ тога колико су резервисани ресурси или можете филтрирати приказ према вештинама, тиму, локацији и осталим опцијама.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-104">You can check resource availability to get an overall view of how booked your resources are, or you can filter the view by skills, team, location, and other options.</span></span>  
  
<span data-ttu-id="cfcbe-105">Табла распореда приказује листу ресурса и њихову доступност.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-105">The schedule board shows list of resources and their availability.</span></span> <span data-ttu-id="cfcbe-106">Изаберите режим приказа за приказивање доступности према **Сатима**, **Данима**, **Недељи** или **Месецу**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-106">Select a view mode to show availability by **Hours**, **Day**, **Week**, or **Month**.</span></span>  
  
<span data-ttu-id="cfcbe-107">Пре него што можете да користите табелу распореда, важно је да је подесите.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-107">Before you use the schedule board, it’s important to set it up.</span></span> <span data-ttu-id="cfcbe-108">Више информација потражите у одељку [Конфигуришите таблу распореда (Field Service или Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span><span class="sxs-lookup"><span data-stu-id="cfcbe-108">For more information, see [Configure the schedule board (Field Service or Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span></span>
  
<span data-ttu-id="cfcbe-109">Ако користите старију верзију, за доступност ресурса погледајте [Приказ доступности ресурса](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="cfcbe-109">If you are using an older version, for resource availability, see [View resource availability](../psa/view-resource-availability.md).</span></span>  

> [!IMPORTANT]
>  <span data-ttu-id="cfcbe-110">Да бисте користили функционалност резервације табеле распореда, географско кодирање и услуге за локацију, потребно је да укључите мапе.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-110">To use the schedule board booking functionality, geocoding, and location services, you need to turn on maps.</span></span>  
> 
> 1. <span data-ttu-id="cfcbe-111">У главном менију изаберите **Планирање ресурса** > **Администрација**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-111">On the main menu, select **Resource Scheduling** > **Administration**.</span></span>  
> 2. <span data-ttu-id="cfcbe-112">Кликните на **Параметри планирања**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-112">Click **Scheduling parameters**.</span></span>  
> 3. <span data-ttu-id="cfcbe-113">Отворите запис и померите се надоле до одељка **Resource Scheduling Optimization**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-113">Open record and scroll down to the **Resource Scheduling Optimization** section.</span></span>  
> 4. <span data-ttu-id="cfcbe-114">У пољу **Повезивање са мапама** одаберите **Да**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-114">On the **Connect to Maps** field, choose **Yes**.</span></span>  
> 5. <span data-ttu-id="cfcbe-115">Прихватите услове и сачувајте запис.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-115">Accept terms and save the record.</span></span>  
> 6. <span data-ttu-id="cfcbe-116">У главном менију изаберите **Project Service** > **Табела распореда**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-116">On the main menu, select **Project Service** > **Schedule board**.</span></span> <span data-ttu-id="cfcbe-117">Одавде, постоји неколико начина да ручно закажете захтев за резервацију.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-117">From here, there are several ways to manually schedule a booking requirement.</span></span> <span data-ttu-id="cfcbe-118">Изаберите метод који функционише за вас.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-118">Choose the method that works for you.</span></span>
  
## <a name="find-available-resources"></a><span data-ttu-id="cfcbe-119">Пронађите доступне ресурсе</span><span class="sxs-lookup"><span data-stu-id="cfcbe-119">Find available resources</span></span>

1.  <span data-ttu-id="cfcbe-120">На листи **Захтев за резервацију** кликните десним тастером миша на незаказану резервацију и изаберите једно од следећег:</span><span class="sxs-lookup"><span data-stu-id="cfcbe-120">From the **Booking Requirement** list, right-click an unscheduled booking and choose one of the following:</span></span>  
  
- <span data-ttu-id="cfcbe-121">Одаберите **Пронађи доступност – Тренутни ресурси** да бисте пронашли доступан ресурс са листе на табли распореда.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-121">Choose **Find availability - Current Resources** to find an available resource from the list on the schedule board.</span></span>  
- <span data-ttu-id="cfcbe-122">Одаберите **Пронађи доступност – Сви ресурси**, да бисте пронашли доступан ресурс у ресурсима у систему</span><span class="sxs-lookup"><span data-stu-id="cfcbe-122">Choose **Find availability - All Resources**, to find an available resource from resources in the system</span></span>  
   > [!NOTE]
   >  <span data-ttu-id="cfcbe-123">Када то урадите, филтери ће приказати опције за изабрани захтев за резервацију.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-123">When you do this, the filters will show options for the selected booking requirement.</span></span>  
  
2. <span data-ttu-id="cfcbe-124">Када видите доступни термин, кликните десним тастером миша на временски интервал на табели распореда и одаберите **Резервиши овде**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-124">When you see an available slot, right-click the time slot on the schedule board and choose **Book Here**.</span></span> <span data-ttu-id="cfcbe-125">Или превуците и испустите захтев резервације на доступан временски интервал.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-125">Or, drag and drop the booking requirement to the available time slot.</span></span>  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a><span data-ttu-id="cfcbe-126">Резервишите ресурс помоћу дневног приказа и пронађите ко нема довољно резервација</span><span class="sxs-lookup"><span data-stu-id="cfcbe-126">Book a resource using the daily view and find who’s under-booked</span></span>
  
1.  <span data-ttu-id="cfcbe-127">На табели распореда, изаберите **Режим приказа**, а затим изаберите **Дани**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-127">On the schedule board, select **View Mode** and select **Days**.</span></span>  
  
    <span data-ttu-id="cfcbe-128">Ово приказује приказа координатне мреже колико је сати ресурс резервисан по дану и којим данима је слободан.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-128">This shows a grid view of how many hours a resource is booked per day and which days they are free.</span></span>  
  
2.  <span data-ttu-id="cfcbe-129">Кликните на име ресурса који желите да резервишете, а затим изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-129">Click the name of the resource you want to book, and then select **Book**.</span></span>  
  
3.  <span data-ttu-id="cfcbe-130">У дијалогу **Резервација ресурса (креирање)** изаберите пројекат за који желите да резервишете ресурс за заједно са методом резервације и временима почетка и завршетка.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-130">On the **Resource booking (create)** dialog box, choose the project that you want to book the resource for along with booking method and start and end times.</span></span>  
  
4.  <span data-ttu-id="cfcbe-131">Када завршите, изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-131">When you’re done, select **Book**.</span></span>  
  
## <a name="view-to-the-schedule-board"></a><span data-ttu-id="cfcbe-132">Приказ табеле распореда</span><span class="sxs-lookup"><span data-stu-id="cfcbe-132">View to the schedule board</span></span>
  
1.  <span data-ttu-id="cfcbe-133">Изаберите незаказани захтев за резервацију са листе на дну.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-133">Select an unscheduled booking requirement from the list at the bottom.</span></span>  
  
2.  <span data-ttu-id="cfcbe-134">Превуците захтев за резервацију на доступни ресурс/временски интервал на табли распореда.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-134">Drag the booking requirement to an available resource/time slot on the schedule board.</span></span>  
  
3.  <span data-ttu-id="cfcbe-135">Када завршите, изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="cfcbe-135">When you're done, select **Book**.</span></span>  
  
### <a name="additional-resources"></a><span data-ttu-id="cfcbe-136">Додатни ресурси</span><span class="sxs-lookup"><span data-stu-id="cfcbe-136">Additional resources</span></span>  
 [<span data-ttu-id="cfcbe-137">Водич за менаџера ресурса</span><span class="sxs-lookup"><span data-stu-id="cfcbe-137">Resource manager guide</span></span>](../psa/resource-manager-guide.md)
