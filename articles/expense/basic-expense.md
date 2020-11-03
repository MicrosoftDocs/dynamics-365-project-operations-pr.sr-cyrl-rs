---
title: Ставка трошка (лагана верзија)
description: Ова тема пружа информације о томе како радити са ставком трошка у једноставној примени.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 746d5d9ff56222e7d6b9b6e264db75d5814365c7
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083856"
---
# <a name="expense-entry-lite"></a><span data-ttu-id="1fefb-103">Ставка трошка (лагана верзија)</span><span class="sxs-lookup"><span data-stu-id="1fefb-103">Expense entry (lite)</span></span>

<span data-ttu-id="1fefb-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="1fefb-104">_**Applies to:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1fefb-105">Основно (или лагано) управљање трошковима је способност евидентирања једноставних трошкова.</span><span class="sxs-lookup"><span data-stu-id="1fefb-105">Basic, or lite, expense management is the capability to record simple expenses.</span></span> <span data-ttu-id="1fefb-106">Можете евидентирати трошкове на пројекту, а затим ће их давалац одобрења прегледати и одобрити.</span><span class="sxs-lookup"><span data-stu-id="1fefb-106">You can record expenses against a project, and then the project approver will review and approve them.</span></span>

<span data-ttu-id="1fefb-107">За више информација о могућностима трошкова у услузи Dynamics 365 Project Operations, погледајте [Преглед трошкова](expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="1fefb-107">For more information about expense capabilities in Dynamics 365 Project Operations, see [Expense overview](expense-overview.md).</span></span>

## <a name="capture-a-basic-expense"></a><span data-ttu-id="1fefb-108">Обухватање основног трошка</span><span class="sxs-lookup"><span data-stu-id="1fefb-108">Capture a basic expense</span></span>

<span data-ttu-id="1fefb-109">Можете покрити своје трошкове како бисте их могли доставити даваоцу одобрења.</span><span class="sxs-lookup"><span data-stu-id="1fefb-109">You can capture your expenses so that you can submit them to the approver.</span></span>

1. <span data-ttu-id="1fefb-110">Идите на **Трошкови** и изаберите **Нови**.</span><span class="sxs-lookup"><span data-stu-id="1fefb-110">Go to **Expenses** , and select **New**.</span></span>
2. <span data-ttu-id="1fefb-111">На страници **Нови трошак** , унесите потребне информације о трошковима, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="1fefb-111">On the **New Expense** page, enter the required expense information, and then select **Save**.</span></span>

## <a name="submit-a-basic-expense"></a><span data-ttu-id="1fefb-112">Прослеђивање основног трошка</span><span class="sxs-lookup"><span data-stu-id="1fefb-112">Submit a basic expense</span></span>

<span data-ttu-id="1fefb-113">Када завршите са евидентирањем свих трошкова и будете ли спремни да их одобрите, морате их пријавити.</span><span class="sxs-lookup"><span data-stu-id="1fefb-113">After you've finished capturing all your expenses, and you're ready to have them approved, you must submit them.</span></span>

1. <span data-ttu-id="1fefb-114">Идите на **Трошкови** и изаберите трошак.</span><span class="sxs-lookup"><span data-stu-id="1fefb-114">Go to **Expenses** , and select an expense.</span></span> <span data-ttu-id="1fefb-115">Или изаберите све трошкове помоћу поља за потврду у заглављу.</span><span class="sxs-lookup"><span data-stu-id="1fefb-115">Or, select all the expenses by using the check box on the header.</span></span>
2. <span data-ttu-id="1fefb-116">Изаберите **Проследи**.</span><span class="sxs-lookup"><span data-stu-id="1fefb-116">Select **Submit**.</span></span> <span data-ttu-id="1fefb-117">Систем обрађује одабране ставке, а затим креира захтеве за одобрење трошкова.</span><span class="sxs-lookup"><span data-stu-id="1fefb-117">The system processes the selected entries and then creates expense approval requests.</span></span>

## <a name="recall-a-basic-expense"></a><span data-ttu-id="1fefb-118">Опозив основног трошка</span><span class="sxs-lookup"><span data-stu-id="1fefb-118">Recall a basic expense</span></span>

<span data-ttu-id="1fefb-119">Када грешком проследите трошак, можете га опозвати.</span><span class="sxs-lookup"><span data-stu-id="1fefb-119">When you submit an expense by mistake, you can recall it.</span></span> <span data-ttu-id="1fefb-120">Време потребно за опозив ставке трошка зависи од фазе одобрења.</span><span class="sxs-lookup"><span data-stu-id="1fefb-120">The time that is required to recall an expense entry depends on its approval stage.</span></span>  <span data-ttu-id="1fefb-121">Ако давалац одобрења још није одобрио ставку, опозив се може извршити одмах.</span><span class="sxs-lookup"><span data-stu-id="1fefb-121">If the approver hasn't yet approved the entry, the recall can occur immediately.</span></span> <span data-ttu-id="1fefb-122">Међутим, ако је ставка већ одобрена, од даваоца одобрења се тражи да одобри опозив и поништи трансакције.</span><span class="sxs-lookup"><span data-stu-id="1fefb-122">However, if the entry has already been approved, the approver is asked to approve the recall and reverse the transactions.</span></span>

1. <span data-ttu-id="1fefb-123">Идите на **Трошкови** , а затим на листи трошкова одаберите трошак који ћете опозвати.</span><span class="sxs-lookup"><span data-stu-id="1fefb-123">Go to **Expenses** , and then, in the list of expenses, select the expense to recall.</span></span>
2. <span data-ttu-id="1fefb-124">Изаберите **Опозови**.</span><span class="sxs-lookup"><span data-stu-id="1fefb-124">Select **Recall**.</span></span> <span data-ttu-id="1fefb-125">Ако ставка трошка још није одобрена, систем је одмах опозива.</span><span class="sxs-lookup"><span data-stu-id="1fefb-125">If the expense entry hasn't yet been approved, the system immediately recalls it.</span></span> <span data-ttu-id="1fefb-126">Ако је ставка трошка већ одобрена, креира се захтев за опозив да обавести даваоца одобрења да желите да сторнирате трошак.</span><span class="sxs-lookup"><span data-stu-id="1fefb-126">If the expense entry has already been approved, a recall request is created to notify the approver that you want to reverse the expense.</span></span> <span data-ttu-id="1fefb-127">Давалац одобрења ће затим потврдити да се сторнирање може извршити и ставка ће бити враћена.</span><span class="sxs-lookup"><span data-stu-id="1fefb-127">The approver will then confirm that the reversal can be done, and the entry will be returned.</span></span>

## <a name="delete-a-basic-expense"></a><span data-ttu-id="1fefb-128">Брисање основног трошка</span><span class="sxs-lookup"><span data-stu-id="1fefb-128">Delete a basic expense</span></span>

<span data-ttu-id="1fefb-129">Трошкови који још нису прослеђени могу се избрисати.</span><span class="sxs-lookup"><span data-stu-id="1fefb-129">Expenses that haven't yet been submitted can be deleted.</span></span> <span data-ttu-id="1fefb-130">Да бисте избрисали трошак који је већ прослеђен, прво га морате опозвати.</span><span class="sxs-lookup"><span data-stu-id="1fefb-130">To delete an expense that has already been submitted, you must first recall it.</span></span>

## <a name="see-also"></a><span data-ttu-id="1fefb-131">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="1fefb-131">See also</span></span>

- [<span data-ttu-id="1fefb-132">Преглед одобрења</span><span class="sxs-lookup"><span data-stu-id="1fefb-132">Approvals overview</span></span>](../approvals/approvals-overview.md)
