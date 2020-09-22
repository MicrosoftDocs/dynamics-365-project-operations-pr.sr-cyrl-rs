---
title: Управљање пројектима и резервацијама у Office 365 календару
description: Како да управљате пројектима и резервацијама у Office 365 календару
author: ruhercul
manager: kfend
ms.service: dynamics-365-projectservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 92428956-1058-4490-934f-907fbbdc8f25
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 5c075e0b63db35c1e189a62a6b5b00f5bcb7ea97
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755292"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a><span data-ttu-id="c5b3a-103">Управљање пројектима и резервацијама у календару (Project Service)</span><span class="sxs-lookup"><span data-stu-id="c5b3a-103">Manage projects and bookings in your calendar (Project Service)</span></span>

> [!Note]
> <span data-ttu-id="c5b3a-104">ЗАСТАРЕЛО: Ова функција је застарела и није више доступна.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-104">DEPRECATED: This feature has been deprecated and is no longer available.</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

<span data-ttu-id="c5b3a-105">Прикажите личне заказане обавезе, резервације пројеката и посла, као и доделе радних налога у апликацији field service коришћењем [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календара.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-105">View personal appointments, project-work bookings, and field service work order assignments using the [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span>  
  
 <span data-ttu-id="c5b3a-106">Када је све на једном месту, лако је управљати вашим даном.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-106">With everything in one place, it’s easy to manage your day.</span></span> <span data-ttu-id="c5b3a-107">Ваши састанци, заказане обавезе, резервације и задаци су сви доступни у вашем [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календару.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-107">Your meetings, appointments, bookings, and tasks are all available in your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span>  
  
 <span data-ttu-id="c5b3a-108">Ако користите [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], можете унети и ваше личне заказане обавезе у приказу уноса времена за Project Service.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-108">If you’re using [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you can also enter your personal appointments in the Project Service time entry view.</span></span> <span data-ttu-id="c5b3a-109">На тај начин менаџери пројекта и ресурса знају вашу доступност за пројекте.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-109">This lets project and resource managers know your availability for projects.</span></span> <span data-ttu-id="c5b3a-110">То вам штеди и време, јер не морате да уносите информације о вашим личним заказаним обавезама двапут.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-110">It also saves you time, because you don’t have to enter info about your personal appointments twice.</span></span> <span data-ttu-id="c5b3a-111">Можете једноставно да увезете личне заказане обавезе из календара у приказ уноса времена у апликацији Project Service.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-111">You can simply import your personal appointments from your calendar to Project Service time entry view.</span></span>  
  
 <span data-ttu-id="c5b3a-112">Ваш календара ће синхронизовати пројекат и резервације радних налога од данас до предстојеће четири недеље.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-112">Your calendar will sync project and work order bookings from today to upcoming four weeks.</span></span> <span data-ttu-id="c5b3a-113">Ово подешавање не може да се промени.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-113">This setting can’t be changed.</span></span>  
  
 <span data-ttu-id="c5b3a-114">Синхронизација је подржана само у једном смеру, из PSA на ваш [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календар.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-114">Syncing is only supported one way, from PSA to your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span> <span data-ttu-id="c5b3a-115">Можете да синхронизујете обрнутим редоследом.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-115">You can sync in the reverse order.</span></span> 
  
 <span data-ttu-id="c5b3a-116">Да бисте сазнали како да користите [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календар, погледајте [Календар у програму Outlook на вебу за предузећа](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936)</span><span class="sxs-lookup"><span data-stu-id="c5b3a-116">To learn how to use your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar, see [Calendar in Outlook on the web for business](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936).</span></span>  
  
## <a name="setup"></a><span data-ttu-id="c5b3a-117">Инсталација</span><span class="sxs-lookup"><span data-stu-id="c5b3a-117">Setup</span></span>  
 <span data-ttu-id="c5b3a-118">Пре него што можете да видите и управљате резервацијама у вашем [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календару, морате да подесите неколико ствари.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-118">Before you can see and manage your bookings on your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar, you need to set a few things up.</span></span>  
  
- <span data-ttu-id="c5b3a-119">Биће вам потребни акредитиви [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] глобалног администратора или администратора система.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-119">You will need to have [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] Global Administrator or System Administrator credentials.</span></span>  
  
- <span data-ttu-id="c5b3a-120">Ваш администратор ће морати да конфигурише профилу сервера е-поште и сваки корисник ће морати да конфигурише своје поштанско сандуче.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-120">Your Admin will need to configure the email server profile and each user will need to configure their mailbox.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="c5b3a-121">[Подешавање обраде е-поште путем синхронизације на страни сервера](../admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks.md)</span><span class="sxs-lookup"><span data-stu-id="c5b3a-121">[Set up email processing through server-side synchronization](../admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks.md)</span></span>  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a><span data-ttu-id="c5b3a-122">Укључите синхронизацију за организацију (задатак администратора)</span><span class="sxs-lookup"><span data-stu-id="c5b3a-122">Turn on synchronization for your organization (admin task)</span></span>  
  
1.  <span data-ttu-id="c5b3a-123">У главном менију кликните на **Подешавања** > **Администрација**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-123">From the main menu, click **Settings** > **Administration**.</span></span>  
  
2.  <span data-ttu-id="c5b3a-124">Кликните на **Системска подешавања**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-124">Click **System Settings**.</span></span>  
  
3.  <span data-ttu-id="c5b3a-125">Кликните на картицу **Синхронизација**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-125">Click the **Synchronization** tab.</span></span>  
  
4.  <span data-ttu-id="c5b3a-126">У оквиру опције **Изаберите да ли желите да омогућите синхронизацију резервације ресурса са** означите **Синхронизуј резервацију ресурса са програмом Outlook**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-126">Under **Select whether to enable syncing of resource booking with**, check the **Synchronize resource booking with Outlook**.</span></span>  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a><span data-ttu-id="c5b3a-127">Укључите синхронизацију за ваш кориснички профил (задатак корисника)</span><span class="sxs-lookup"><span data-stu-id="c5b3a-127">Turn on synchronization for your user profile (user task)</span></span>  
  
1.  <span data-ttu-id="c5b3a-128">Кликните на дугме **Подешавања** у горњем десном углу екрана.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-128">Click the **Settings** button in the upper-right corner of the screen.</span></span>  
  
2.  <span data-ttu-id="c5b3a-129">Кликните на дугме **Опције**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-129">Click **Options**.</span></span>  
  
3.  <span data-ttu-id="c5b3a-130">Кликните на картицу **Синхронизација**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-130">Click the **Synchronization** tab.</span></span>  
  
4.  <span data-ttu-id="c5b3a-131">У оквиру **Синхронизација резервације ресурса са програмом Outlook**, означите **Синхронизација резервације ресурса са програмом Outlook**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-131">Under **Resource booking sync with Outlook**, check the **Synchronization resource booking with Outlook**.</span></span>  
  
## <a name="import-your-personal-appointments-user-task"></a><span data-ttu-id="c5b3a-132">Увезите ваше личне заказане обавезе (задатак корисника)</span><span class="sxs-lookup"><span data-stu-id="c5b3a-132">Import your personal appointments (user task)</span></span>  
 <span data-ttu-id="c5b3a-133">Можете да увезете личне заказане обавезе из календара у приказ уноса времена у апликацији Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-133">You can import your personal appointments from your calendar to Project Service Automation time entry view.</span></span>  
  
1. <span data-ttu-id="c5b3a-134">Отворите [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календар и кликните на **Увоз података**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-134">Open [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar and click **Import Data**.</span></span>  
  
2. <span data-ttu-id="c5b3a-135">На екрану Филтери изаберите **Заказане обавезе из услуге Exchange**, а затим кликните на **Примени**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-135">On the Filters screen, select **Appointments from Exchange** and then click **Apply**.</span></span>  
  
3. <span data-ttu-id="c5b3a-136">Систем ће извући заказане обавезе у приказу уноса времена као предложеним уносима за тренутну недељу.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-136">The system will pull appointments into time entry view as suggested entries from the current week.</span></span> <span data-ttu-id="c5b3a-137">Да бисте додали ставке за другу недељу, кликните на дугме **Претходно** или **Следеће**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-137">To add entries for another week, click **Previous** or **Next**.</span></span>  
  
4. <span data-ttu-id="c5b3a-138">Изаберите заказану обавезу коју желите да додате у приказ уноса времена у апликацији Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-138">Select the appointment that you want to add to Project Service Automation time entry view.</span></span>  
  
5. <span data-ttu-id="c5b3a-139">У искачућем пољу **Унос времена** изаберите одговарајуће опције за конвертовање заказане обавезе у приказ уноса времена у апликацији Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-139">On the **Time Entry** popup box, select the appropriate options to convert the appointment to a Project Service Automation time entry view.</span></span>  
  
6. <span data-ttu-id="c5b3a-140">Кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="c5b3a-140">Click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="c5b3a-141">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="c5b3a-141">See Also</span></span>  
 [<span data-ttu-id="c5b3a-142">Водич за време, трошак и сарадњу</span><span class="sxs-lookup"><span data-stu-id="c5b3a-142">Time, Expense, and Collaboration Guide</span></span>](../project-service/time-expense-collaboration-guide.md)
