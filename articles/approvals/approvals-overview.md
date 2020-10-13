---
title: Преглед одобрења
description: Ова тема пружа информације о раду са одобрењима у услузи Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 37994422e9146765076fdbb77f5c763b4f1d0802
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961184"
---
# <a name="approvals-overview"></a><span data-ttu-id="876ba-103">Преглед одобрења</span><span class="sxs-lookup"><span data-stu-id="876ba-103">Approvals overview</span></span>

<span data-ttu-id="876ba-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="876ba-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="876ba-105">Прослеђивања времена и трошкова се крећу кроз ток посла одобравања.</span><span class="sxs-lookup"><span data-stu-id="876ba-105">Time and Expense submissions move through an approval workflow.</span></span> <span data-ttu-id="876ba-106">Након одобравања ставки, трансакције се евидентирају у стварности или се у распореду резервише време.</span><span class="sxs-lookup"><span data-stu-id="876ba-106">After the entries are approved, transactions are recorded in actuals or time is booked in the schedule.</span></span>

## <a name="approvals-workflow"></a><span data-ttu-id="876ba-107">Ток посла одобрења</span><span class="sxs-lookup"><span data-stu-id="876ba-107">Approvals workflow</span></span>
<span data-ttu-id="876ba-108">Када креирате и пошаљете ставку времена или трошкова, креира се ставка за одобрење.</span><span class="sxs-lookup"><span data-stu-id="876ba-108">When you create and submit a time or expense entry, an approval entry is created.</span></span> <span data-ttu-id="876ba-109">Давалац одобрења пројекта или ваш менаџер прегледају и одобравају вашу ставку.</span><span class="sxs-lookup"><span data-stu-id="876ba-109">The Project approver or your manager reviews and approves your entry.</span></span> <span data-ttu-id="876ba-110">Ако се ставка односи на пројекат, када се одобри, креираће се стварни подаци.</span><span class="sxs-lookup"><span data-stu-id="876ba-110">If the entry is related to a project, when it's approved, the actuals will be created.</span></span> <span data-ttu-id="876ba-111">То омогућава праћење трошкова и обрачуна.</span><span class="sxs-lookup"><span data-stu-id="876ba-111">This allows the cost and billing to be tracked.</span></span> 

## <a name="approve-an-entry"></a><span data-ttu-id="876ba-112">Одобравање ставке</span><span class="sxs-lookup"><span data-stu-id="876ba-112">Approve an entry</span></span>
<span data-ttu-id="876ba-113">Образац **Одобрења** вам омогућава да се пребацујете између различитих приказа како бисте могли да видите различите врсте одобрења.</span><span class="sxs-lookup"><span data-stu-id="876ba-113">The **Approvals** form allows you to switch between different views so that you can view the different types of approvals.</span></span>
  
1. <span data-ttu-id="876ba-114">Идите на образац **Одобрења** и изаберите **Трошкови**,**Време** или **Опозиви**.</span><span class="sxs-lookup"><span data-stu-id="876ba-114">Go to the **Approvals** form and select **Expenses**, **Time**, or **Recalls**.</span></span>
2. <span data-ttu-id="876ba-115">Прегледајте свако одобрење и изаберите она која желите да одобрите.</span><span class="sxs-lookup"><span data-stu-id="876ba-115">Review each approval, and select the ones you want to approve.</span></span>
3. <span data-ttu-id="876ba-116">Изаберите **Одобри** да бисте одобрили изабране ставке.</span><span class="sxs-lookup"><span data-stu-id="876ba-116">Select **Approve** to approve the selected entries.</span></span>
<span data-ttu-id="876ba-117">Систем ће обрадити ове ставке и креирати стварне податке или резервацију.</span><span class="sxs-lookup"><span data-stu-id="876ba-117">The system will process these entries and create actuals or a booking.</span></span>

## <a name="reject-an-entry"></a><span data-ttu-id="876ba-118">Одбијање ставке</span><span class="sxs-lookup"><span data-stu-id="876ba-118">Reject an entry</span></span>
<span data-ttu-id="876ba-119">Као давалац одобрења за пројекат, можда ћете морати да вратите ставку кориснику ради исправке.</span><span class="sxs-lookup"><span data-stu-id="876ba-119">As the Project approver, you may have to send an entry back to a user for correction.</span></span>
  
1. <span data-ttu-id="876ba-120">Идите на образац **Одобрења** и изаберите ставку коју желите да одбаците.</span><span class="sxs-lookup"><span data-stu-id="876ba-120">Go to the **Approvals** form and select the entry to reject.</span></span> 
2. <span data-ttu-id="876ba-121">Изаберите **Одбаци**.</span><span class="sxs-lookup"><span data-stu-id="876ba-121">Select **Reject**.</span></span>
3. <span data-ttu-id="876ba-122">Опционално – Додајте коментар у дијалогу **Коментари одбијања** да обавестите корисника зашто се ставка одбија.</span><span class="sxs-lookup"><span data-stu-id="876ba-122">Optional - Add a comment in the **Rejection Comments** dialog to inform the user why the entry is being rejected.</span></span>
4. <span data-ttu-id="876ba-123">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="876ba-123">Select **OK**.</span></span> <span data-ttu-id="876ba-124">Ставка ће бити враћена кориснику.</span><span class="sxs-lookup"><span data-stu-id="876ba-124">The entry will be returned to the user.</span></span>
  
## <a name="recall-entries"></a><span data-ttu-id="876ba-125">Опозив ставки</span><span class="sxs-lookup"><span data-stu-id="876ba-125">Recall entries</span></span>
<span data-ttu-id="876ba-126">У неком тренутку, можда ћете морати да опозовете прослеђену ставку.</span><span class="sxs-lookup"><span data-stu-id="876ba-126">At some point, you might need to recall a submitted entry.</span></span> <span data-ttu-id="876ba-127">Ако ставка није одобрена, одмах ће се вратити.</span><span class="sxs-lookup"><span data-stu-id="876ba-127">If the entry has not been approved, it will be returned immediately.</span></span> <span data-ttu-id="876ba-128">Одобрена ставка, међутим, може да има материјални утицај.</span><span class="sxs-lookup"><span data-stu-id="876ba-128">An approved entry however, may have a material impact.</span></span> <span data-ttu-id="876ba-129">Давалац одобрења за пројекат је дужан да одобри опозив како би се поништила трансакција у стварним подацима.</span><span class="sxs-lookup"><span data-stu-id="876ba-129">The Project approver is required to approve the recall in order to reverse the transaction in Actuals.</span></span>

## <a name="specify-project-approvers"></a><span data-ttu-id="876ba-130">Навођење давалаца одобрења за пројекат</span><span class="sxs-lookup"><span data-stu-id="876ba-130">Specify Project approvers</span></span>
<span data-ttu-id="876ba-131">Сваки пројекат има одређени број чланова пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="876ba-131">Each project has a number of project team members.</span></span> <span data-ttu-id="876ba-132">Можете одредити који чланови тима су такође и даваоци одобрења за пројекат.</span><span class="sxs-lookup"><span data-stu-id="876ba-132">You can specify which team members are also Project approvers.</span></span>

1. <span data-ttu-id="876ba-133">Идите на образац **Пројекти** и отворите пројекат са листе.</span><span class="sxs-lookup"><span data-stu-id="876ba-133">Go to the **Projects** form and open the project from the list.</span></span>
2. <span data-ttu-id="876ba-134">На картици **Тим** изаберите члана тима који ће бити давалац одобрења за пројекат, а затим изаберите **Уреди**.</span><span class="sxs-lookup"><span data-stu-id="876ba-134">On the **Team** tab, select the team member who will be a Project approver and then select **Edit**.</span></span>
3. <span data-ttu-id="876ba-135">Подесите поље **Давалац одобрења за пројекат** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="876ba-135">Set the **Project Approver** field to **Yes**.</span></span>
4. <span data-ttu-id="876ba-136">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="876ba-136">Select **Save**.</span></span>
5. <span data-ttu-id="876ba-137">Поновите кораке 2-4 да бисте додали додатне даваоце одобрења за пројекат.</span><span class="sxs-lookup"><span data-stu-id="876ba-137">Repeat steps 2-4 to add additional Project approvers.</span></span>

## <a name="configure-the-users-manager"></a><span data-ttu-id="876ba-138">Конфигуришите менаџера корисника</span><span class="sxs-lookup"><span data-stu-id="876ba-138">Configure the user's manager</span></span>

1. <span data-ttu-id="876ba-139">Идите на **Подешавања** > **Безбедност** > **Корисници**.</span><span class="sxs-lookup"><span data-stu-id="876ba-139">Go to **Settings** > **Security** > **Users**.</span></span>
2. <span data-ttu-id="876ba-140">Изаберите корисника којем додељујете менаџера, а затим у области **Информације о организацији** изаберите менаџера са листе.</span><span class="sxs-lookup"><span data-stu-id="876ba-140">Select the user to whom you are assigning a manager and in the **Organization Information** area, select the manager from the list.</span></span> 
3. <span data-ttu-id="876ba-141">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="876ba-141">Select **Save**.</span></span>


