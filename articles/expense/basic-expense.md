---
title: Ставка трошка (лагана верзија)
description: Ова тема пружа информације о томе како радити са ставком трошка у једноставној примени.
author: stsporen
manager: AnnBe
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d87094882751f0751a8d9d539fa4cdcfc6b7b0d7
ms.sourcegitcommit: 16c442258ba24c79076cf5877a0f3c1f51a85f61
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/20/2020
ms.locfileid: "4590964"
---
# <a name="expense-entry-lite"></a><span data-ttu-id="6e583-103">Ставка трошка (лагана верзија)</span><span class="sxs-lookup"><span data-stu-id="6e583-103">Expense entry (lite)</span></span>

<span data-ttu-id="6e583-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="6e583-104">_**Applies to:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6e583-105">Основно (или лагано) управљање трошковима је способност евидентирања једноставних трошкова.</span><span class="sxs-lookup"><span data-stu-id="6e583-105">Basic, or lite, expense management is the capability to record simple expenses.</span></span> <span data-ttu-id="6e583-106">Можете евидентирати трошкове на пројекту, а затим ће их давалац одобрења прегледати и одобрити.</span><span class="sxs-lookup"><span data-stu-id="6e583-106">You can record expenses against a project, and then the project approver will review and approve them.</span></span>

<span data-ttu-id="6e583-107">За више информација о могућностима трошкова у услузи Dynamics 365 Project Operations, погледајте [Преглед трошкова](expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="6e583-107">For more information about expense capabilities in Dynamics 365 Project Operations, see [Expense overview](expense-overview.md).</span></span>

## <a name="capture-a-basic-expense"></a><span data-ttu-id="6e583-108">Обухватање основног трошка</span><span class="sxs-lookup"><span data-stu-id="6e583-108">Capture a basic expense</span></span>

<span data-ttu-id="6e583-109">Можете покрити своје трошкове како бисте их могли доставити даваоцу одобрења.</span><span class="sxs-lookup"><span data-stu-id="6e583-109">You can capture your expenses so that you can submit them to the approver.</span></span>

1. <span data-ttu-id="6e583-110">Идите на **Трошкови** и изаберите **Нови**.</span><span class="sxs-lookup"><span data-stu-id="6e583-110">Go to **Expenses**, and select **New**.</span></span>
2. <span data-ttu-id="6e583-111">На страници **Нови трошак**, унесите потребне информације о трошковима, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="6e583-111">On the **New Expense** page, enter the required expense information, and then select **Save**.</span></span>

## <a name="submit-a-basic-expense"></a><span data-ttu-id="6e583-112">Прослеђивање основног трошка</span><span class="sxs-lookup"><span data-stu-id="6e583-112">Submit a basic expense</span></span>

<span data-ttu-id="6e583-113">Када завршите са евидентирањем свих трошкова и будете ли спремни да их одобрите, морате их пријавити.</span><span class="sxs-lookup"><span data-stu-id="6e583-113">After you've finished capturing all your expenses, and you're ready to have them approved, you must submit them.</span></span>

1. <span data-ttu-id="6e583-114">Идите на **Трошкови** и изаберите трошак.</span><span class="sxs-lookup"><span data-stu-id="6e583-114">Go to **Expenses**, and select an expense.</span></span> <span data-ttu-id="6e583-115">Или изаберите све трошкове помоћу поља за потврду у заглављу.</span><span class="sxs-lookup"><span data-stu-id="6e583-115">Or, select all the expenses by using the check box on the header.</span></span>
2. <span data-ttu-id="6e583-116">Изаберите **Проследи**.</span><span class="sxs-lookup"><span data-stu-id="6e583-116">Select **Submit**.</span></span> <span data-ttu-id="6e583-117">Систем обрађује одабране ставке, а затим креира захтеве за одобрење трошкова.</span><span class="sxs-lookup"><span data-stu-id="6e583-117">The system processes the selected entries and then creates expense approval requests.</span></span>

## <a name="add-an-attachment"></a><span data-ttu-id="6e583-118">Додајте прилог</span><span class="sxs-lookup"><span data-stu-id="6e583-118">Add an attachment</span></span>

<span data-ttu-id="6e583-119">Можда ћете одобраваоцу морати да доставите додатну документацију о свом трошку.</span><span class="sxs-lookup"><span data-stu-id="6e583-119">You may have to provide the approver with additional documentation about your expense.</span></span> <span data-ttu-id="6e583-120">У временску осу уноса трошкова можете приложити признаницу.</span><span class="sxs-lookup"><span data-stu-id="6e583-120">You can attach a receipt in the timeline of the expense entry.</span></span> <span data-ttu-id="6e583-121">Изаберите **Уреди** и у одељку **Временска оса**, а затим изаберите икону спајалице да бисте приложили признаницу.</span><span class="sxs-lookup"><span data-stu-id="6e583-121">Select **Edit** and in the **Timeline** section, and then select the paperclip icon to attach your receipt.</span></span>

## <a name="recall-a-basic-expense"></a><span data-ttu-id="6e583-122">Опозив основног трошка</span><span class="sxs-lookup"><span data-stu-id="6e583-122">Recall a basic expense</span></span>

<span data-ttu-id="6e583-123">Када грешком проследите трошак, можете га опозвати.</span><span class="sxs-lookup"><span data-stu-id="6e583-123">When you submit an expense by mistake, you can recall it.</span></span> <span data-ttu-id="6e583-124">Време потребно за опозив ставке трошка зависи од фазе одобрења.</span><span class="sxs-lookup"><span data-stu-id="6e583-124">The time that is required to recall an expense entry depends on its approval stage.</span></span>  <span data-ttu-id="6e583-125">Ако давалац одобрења још није одобрио ставку, опозив се може извршити одмах.</span><span class="sxs-lookup"><span data-stu-id="6e583-125">If the approver hasn't yet approved the entry, the recall can occur immediately.</span></span> <span data-ttu-id="6e583-126">Међутим, ако је ставка већ одобрена, од даваоца одобрења се тражи да одобри опозив и поништи трансакције.</span><span class="sxs-lookup"><span data-stu-id="6e583-126">However, if the entry has already been approved, the approver is asked to approve the recall and reverse the transactions.</span></span>

1. <span data-ttu-id="6e583-127">Идите на **Трошкови**, а затим на листи трошкова одаберите трошак који ћете опозвати.</span><span class="sxs-lookup"><span data-stu-id="6e583-127">Go to **Expenses**, and then, in the list of expenses, select the expense to recall.</span></span>
2. <span data-ttu-id="6e583-128">Изаберите **Опозови**.</span><span class="sxs-lookup"><span data-stu-id="6e583-128">Select **Recall**.</span></span> <span data-ttu-id="6e583-129">Ако ставка трошка још није одобрена, систем је одмах опозива.</span><span class="sxs-lookup"><span data-stu-id="6e583-129">If the expense entry hasn't yet been approved, the system immediately recalls it.</span></span> <span data-ttu-id="6e583-130">Ако је ставка трошка већ одобрена, креира се захтев за опозив да обавести даваоца одобрења да желите да сторнирате трошак.</span><span class="sxs-lookup"><span data-stu-id="6e583-130">If the expense entry has already been approved, a recall request is created to notify the approver that you want to reverse the expense.</span></span> <span data-ttu-id="6e583-131">Давалац одобрења ће затим потврдити да се сторнирање може извршити и ставка ће бити враћена.</span><span class="sxs-lookup"><span data-stu-id="6e583-131">The approver will then confirm that the reversal can be done, and the entry will be returned.</span></span>

## <a name="delete-a-basic-expense"></a><span data-ttu-id="6e583-132">Брисање основног трошка</span><span class="sxs-lookup"><span data-stu-id="6e583-132">Delete a basic expense</span></span>

<span data-ttu-id="6e583-133">Трошкови који још нису прослеђени могу се избрисати.</span><span class="sxs-lookup"><span data-stu-id="6e583-133">Expenses that haven't yet been submitted can be deleted.</span></span> <span data-ttu-id="6e583-134">Да бисте избрисали трошак који је већ прослеђен, прво га морате опозвати.</span><span class="sxs-lookup"><span data-stu-id="6e583-134">To delete an expense that has already been submitted, you must first recall it.</span></span>

## <a name="see-also"></a><span data-ttu-id="6e583-135">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="6e583-135">See also</span></span>

- [<span data-ttu-id="6e583-136">Преглед одобрења</span><span class="sxs-lookup"><span data-stu-id="6e583-136">Approvals overview</span></span>](../approvals/approvals-overview.md)
