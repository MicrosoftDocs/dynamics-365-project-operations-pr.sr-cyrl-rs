---
title: Креирање резервације у пројекту из табеле распореда
description: Ова тема пружа информације о томе како да креирате резервацију у пројекту на табели распореда.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: 7032af78168c742ac64cb2a7174cabcbda579ff8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146546"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="fd0a5-103">Креирање резервације у пројекту из табеле распореда</span><span class="sxs-lookup"><span data-stu-id="fd0a5-103">Create a project booking from the Schedule board</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="fd0a5-104">Можете да резервишете ресурс за пројекат директно на картици **Тим** за пројекат или да генеришете потребу за ресурсом из доделе генеричког члана тима, а да затим испуните генерисану потребу чланом пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="fd0a5-105">Можете и да резервишете ресурс за пројекат директно из табеле распореда.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="fd0a5-106">То може да се уради на три начина:</span><span class="sxs-lookup"><span data-stu-id="fd0a5-106">There are three ways to do this:</span></span>

- <span data-ttu-id="fd0a5-107">**Резервисање из генерисане потребе за ресурсом:** Потребу за ресурс можете да генеришете након што креирате генерички ресурс и доделите задатке унутар пројекта.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="fd0a5-108">**Резервисање из примарнe потребе:** Примарне потребе се појављују на табели распореда на картици **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="fd0a5-109">**Резервисање из нове потребе за ресурсом:** Можете да креирате потребу за ресурсом испочетка и повежете је са пројектом.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="fd0a5-110">На табели распореда, потреба за ресурсом се приказује на картици **Отворене потребе**.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="fd0a5-111">Резервисање из генерисаног захтева за ресурсом</span><span class="sxs-lookup"><span data-stu-id="fd0a5-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="fd0a5-112">Можете да креирате генерички ресурс и да му доделите задатак или више задатака у оквиру пројекта.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="fd0a5-113">Затим можете да генеришете потребу за ресурсом за генеричког члана тима.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="fd0a5-114">На табели распореда, овај ресурс ће се приказати на картици **Отворене потребе**. Можда ћете морати да користите филтере колона на мрежи уколико имате много отворених захтева.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="fd0a5-115">![Отварање картице Захтеви на табели распореда](media/FAQ-Project-Booking-Schedule-Board-1.png "Снимак екрана табеле резервација и додела")</span><span class="sxs-lookup"><span data-stu-id="fd0a5-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="fd0a5-116">Изаберите захтев.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-116">Select the requirement.</span></span> <span data-ttu-id="fd0a5-117">Картица **Претрага доступности** ће се појавити при врху изабраног реда.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="fd0a5-118">Када изаберете картицу, покреће се режим Помоћник за заказивање у табели распореда, а затим филтрира доступне ресурсе који испуњавају потребе за ресурсима.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="fd0a5-119">После тога можете да резервишете ресурс.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="fd0a5-120">Можете и да превучете и отпустите изабрани ред са дна табеле распореда у ћелију ресурса на мрежи изнад.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="fd0a5-121">Када га спустите, он отвара таблу **Креирање резервације ресурса** са десне стране.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="fd0a5-122">Избор опције **Резервиши** резервише ресурс у пројектном тиму.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-122">Selecting **Book** books the resource onto the project team.</span></span>

![Табла Креирање резервације ресурса](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="fd0a5-124">Резервисање из примарног захтева</span><span class="sxs-lookup"><span data-stu-id="fd0a5-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="fd0a5-125">Креирање пројекта у програму Project Service аутоматски креира захтев за ресурсом под именом Примарни захтев.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="fd0a5-126">То је празан захтев који се користи за брзо резервисање ресурса помоћу табеле распореда без генерисања захтева или креирања захтева из почетка.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="fd0a5-127">Пошто је захтев празан, мораћете да наведете датуме, као и на начин доделе и сате ако је то применљиво.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="fd0a5-128">Да бисте резервисали ресурс са примарним захтевом, у табели распореда изаберите картицу **Пројекат**. Можда ћете морати да користите филтер колоне за колону **Пројекат** уколико имате више пројеката.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="fd0a5-129">![Филтери колоне на табли распореда](media/FAQ-Project-Booking-Schedule-Board-2.png "Снимак екрана табеле резервација и додела")</span><span class="sxs-lookup"><span data-stu-id="fd0a5-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="fd0a5-130">Изаберите захтев који има само име пројекта као своје име и чије трајање износи нула (0).</span><span class="sxs-lookup"><span data-stu-id="fd0a5-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="fd0a5-131">Изаберите картицу **Претрага доступности** која се појављује у реду.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="fd0a5-132">На тај начин табела распореда улази у режим Помоћник за заказивање и приказује доступне ресурсе које је могуће резервисати за пројекат.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="fd0a5-133">Пошто је **Примарни захтев** празан захтев чије трајање износи нула (0), мораћете да подесите трајање на табли **Креирање резервације ресурса** приликом избора и резервисања ресурса.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="fd0a5-134">Можете и да изаберете **Примарни захтев пројекта** у дну табеле распореда и да га превучете до ресурса да бисте га резервисали.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="fd0a5-135">Пошто је **Примарни захтев** празан захтев чије трајање износи нула (0), мораћете да подесите трајање на табли **Креирање резервације ресурса** приликом избора и резервисања ресурса.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="fd0a5-136">Када резервишете ресурс путем **примарног захтева** у табели распореда, додајете га у пројектни тим без иједне доделе.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="fd0a5-137">Резервисање из новог захтева за ресурсом</span><span class="sxs-lookup"><span data-stu-id="fd0a5-137">Book from a new resource requirement</span></span>
<span data-ttu-id="fd0a5-138">Обавите следеће кораке да бисте обавили резервацију из нове потребе за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="fd0a5-139">Идите на **Потребе за ресурсима**, а затим изаберите **Нови** да бисте креирали нову потребу за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-139">Go to **Resource Requirements**, and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="fd0a5-140">На картици **Пројекат** одаберите пројекат како бисте повезали захтев и пројекат.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="fd0a5-141">У табели распореда, овај нови захтев се приказује као **Отворени захтев** који можете да попуните.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="fd0a5-142">Резервишите ресурс да бисте га додали у пројектни тим.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="fd0a5-143">Сада када је ресурс резервисан, морате да му ручно доделите задатке.</span><span class="sxs-lookup"><span data-stu-id="fd0a5-143">Now that the resource is booked, you must assign tasks manually.</span></span>

