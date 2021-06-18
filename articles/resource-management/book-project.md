---
title: Резервисање за пројекат
description: Ова тема пружа информације о резервисању ресурса у пројекат.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 15de5735ba6d25994a68192ebdf80aefec772d6e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998834"
---
# <a name="book-to-a-project"></a><span data-ttu-id="466cf-103">Резервисање за пројекат</span><span class="sxs-lookup"><span data-stu-id="466cf-103">Book to a project</span></span>

<span data-ttu-id="466cf-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="466cf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="466cf-105">Постоје случајеви у којима ће менаџер пројекта или менаџер ресурса морати да додели ресурс пројекту, ада од генеричког члана тима није дефинисан посебан захтев.</span><span class="sxs-lookup"><span data-stu-id="466cf-105">There are times where a Project manager or Resource manager will need to allocate a resource to project without a specific requirement being defined from a generic team member.</span></span> <span data-ttu-id="466cf-106">То се може постићи на један од три начина.</span><span class="sxs-lookup"><span data-stu-id="466cf-106">This can be achieved in one of three ways.</span></span>

- <span data-ttu-id="466cf-107">Резервација из мреже члана тима</span><span class="sxs-lookup"><span data-stu-id="466cf-107">Book from the team member grid</span></span>
- <span data-ttu-id="466cf-108">Резервисање са табеле распореда</span><span class="sxs-lookup"><span data-stu-id="466cf-108">Book from the schedule board</span></span>
- <span data-ttu-id="466cf-109">Резервација из обрасца **Пројекат**</span><span class="sxs-lookup"><span data-stu-id="466cf-109">Book from the **Project** form</span></span>

## <a name="book-from-the-team-member-grid"></a><span data-ttu-id="466cf-110">Резервација из мреже члана тима</span><span class="sxs-lookup"><span data-stu-id="466cf-110">Book from the team member grid</span></span>

<span data-ttu-id="466cf-111">Ако ваша организација ради у хибридном режиму доделе ресурса, менаџер пројекта може резервисати ресурс директно у пројекат тако што ће извршити следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="466cf-111">If your organization is operating in hybrid Resource allocation mode, the Project manager can book a resource directly to the project by completing the following steps.</span></span>

1. <span data-ttu-id="466cf-112">Из пројекта идите на мрежу чланова тима и изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="466cf-112">From the project, go to the team member grid and select **New**.</span></span>
2. <span data-ttu-id="466cf-113">Дефинишите назив позиције и улогу ресурса.</span><span class="sxs-lookup"><span data-stu-id="466cf-113">Define the position name and the role of the resource.</span></span>
3. <span data-ttu-id="466cf-114">Изаберите ресурс који може да се резервише из доступног проналажења.</span><span class="sxs-lookup"><span data-stu-id="466cf-114">Select the bookable resource from the available lookup.</span></span>
4. <span data-ttu-id="466cf-115">Када одаберете ресурс, дефинишите следеће информације о пољу да бисте резервирали ресурс:</span><span class="sxs-lookup"><span data-stu-id="466cf-115">After you select the resource, define the following field information to book the resource:</span></span>

    - <span data-ttu-id="466cf-116">Датум почетка</span><span class="sxs-lookup"><span data-stu-id="466cf-116">Start date</span></span>
    - <span data-ttu-id="466cf-117">Датум завршетка</span><span class="sxs-lookup"><span data-stu-id="466cf-117">Finish date</span></span>
    - <span data-ttu-id="466cf-118">Начин доделе</span><span class="sxs-lookup"><span data-stu-id="466cf-118">Allocation method</span></span>
    - <span data-ttu-id="466cf-119">Сати, ако је применљиво</span><span class="sxs-lookup"><span data-stu-id="466cf-119">Hours, if applicable</span></span>
    - <span data-ttu-id="466cf-120">Давалац одобрења за пројекат</span><span class="sxs-lookup"><span data-stu-id="466cf-120">Project approver</span></span>

6. <span data-ttu-id="466cf-121">Изаберите **Сачувај и затвори**</span><span class="sxs-lookup"><span data-stu-id="466cf-121">Select **Save and Close**</span></span>

## <a name="book-from-the-schedule-board"></a><span data-ttu-id="466cf-122">Резервисање са табеле распореда</span><span class="sxs-lookup"><span data-stu-id="466cf-122">Book from the schedule board</span></span>

<span data-ttu-id="466cf-123">Када менаџер ресурса треба да резервише ресурс директно за пројекат, може да користи таблу распореда и захтеве пројекта.</span><span class="sxs-lookup"><span data-stu-id="466cf-123">When a Resource manager needs to book a resource directly to a project, they can use the schedule board and the project requirement.</span></span> <span data-ttu-id="466cf-124">Захтев пројекта је захтев за ресурсом који је увек доступан за резервисање.</span><span class="sxs-lookup"><span data-stu-id="466cf-124">The project requirement is a resource requirement that is always available to be booked against.</span></span> <span data-ttu-id="466cf-125">Да бисте резервисали директно у образац пројекта из табеле распореда, обавите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="466cf-125">To book directly to a project form the schedule board, complete the following steps.</span></span>

1. <span data-ttu-id="466cf-126">Идите на табелу распореда и на левој страници филтрирајте ресурсе које узимате у обзир за захтев.</span><span class="sxs-lookup"><span data-stu-id="466cf-126">Navigate to the schedule board and on the left page, filter for the resources you are considering for the requirement.</span></span>
2. <span data-ttu-id="466cf-127">У доњем окну изаберите картицу **Пројекат** да бисте видели листу пројектних захтева.</span><span class="sxs-lookup"><span data-stu-id="466cf-127">In the bottom pane, select the **Project** tab to view a list of project requirements.</span></span>
3. <span data-ttu-id="466cf-128">Превуците захтев на ресурс и дефинишите следеће информације:</span><span class="sxs-lookup"><span data-stu-id="466cf-128">Drag the requirement onto a resource and define the following information:</span></span>

    - <span data-ttu-id="466cf-129">Датум почетка</span><span class="sxs-lookup"><span data-stu-id="466cf-129">Start date</span></span>
    - <span data-ttu-id="466cf-130">Датум завршетка</span><span class="sxs-lookup"><span data-stu-id="466cf-130">Finish date</span></span>
    - <span data-ttu-id="466cf-131">Статус резервације</span><span class="sxs-lookup"><span data-stu-id="466cf-131">Booking status</span></span>
    - <span data-ttu-id="466cf-132">Метод резервације</span><span class="sxs-lookup"><span data-stu-id="466cf-132">Booking method</span></span>
    - <span data-ttu-id="466cf-133">Трајање</span><span class="sxs-lookup"><span data-stu-id="466cf-133">Duration</span></span>

## <a name="book-from-the-project-form"></a><span data-ttu-id="466cf-134">Резервација из обрасца Пројекат</span><span class="sxs-lookup"><span data-stu-id="466cf-134">Book from the Project form</span></span>

<span data-ttu-id="466cf-135">Као менаџер пројекта, можда ћете морати да резервишете ресурс за пројекат, али знате само критеријуме, а не и назив ресурса.</span><span class="sxs-lookup"><span data-stu-id="466cf-135">As a Project manager, you might need to book a resource to a project, but only know the criteria rather than the name of the resource.</span></span> <span data-ttu-id="466cf-136">Довршите следеће кораке да бисте помоћу помоћника за планирање пронашли ресурс на основу било којих доступних атрибута ресурса.</span><span class="sxs-lookup"><span data-stu-id="466cf-136">Complete the following steps to use the schedule assistant to find a resource based on any available attributes of the resource.</span></span> 

1. <span data-ttu-id="466cf-137">Дођите до пројекта и изаберите **Резервиши** да бисте отворили помоћника за планирање.</span><span class="sxs-lookup"><span data-stu-id="466cf-137">Navigate to the project and select **Book** to open the Schedule Assistant.</span></span>
2. <span data-ttu-id="466cf-138">Помоћу филтера на левој страни помоћника за планирање, сузите критеријуме и изаберите **Претрага.**</span><span class="sxs-lookup"><span data-stu-id="466cf-138">Using the filters on the left side of the Schedule Assistant, narrow the criteria and select **Search.**</span></span>
3. <span data-ttu-id="466cf-139">На основу ресурса враћених у резултатима, можете резервирати ресурс.</span><span class="sxs-lookup"><span data-stu-id="466cf-139">Based on resources returned in the results, you can book a resource.</span></span>

> [!NOTE]
> <span data-ttu-id="466cf-140">Ова метода не креира никакве резервације за ресурс.</span><span class="sxs-lookup"><span data-stu-id="466cf-140">This method doesn't create any bookings for the resource.</span></span> <span data-ttu-id="466cf-141">Уместо тога, додаје ресурс тиму.</span><span class="sxs-lookup"><span data-stu-id="466cf-141">Instead, it adds the resource to the team.</span></span> <span data-ttu-id="466cf-142">Када се члан тима дода у пројекат, менаџер пројекта може користити одржавање резервација или продужити резервације да би потребне резервације додао ресурсу.</span><span class="sxs-lookup"><span data-stu-id="466cf-142">After the team member has been added to the project, the project manager can use maintain bookings or extend bookings to add the required bookings to the resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]