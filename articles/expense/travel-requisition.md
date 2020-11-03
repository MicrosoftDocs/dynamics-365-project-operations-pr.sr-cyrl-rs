---
title: Захтеви за путовање
description: Ова тема пружа информације о захтевима за путовање.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 0261405abb9305d7f6abcde9cb90d9b184868580
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083841"
---
# <a name="travel-requisitions"></a><span data-ttu-id="5d1f7-103">Захтеви за путовање</span><span class="sxs-lookup"><span data-stu-id="5d1f7-103">Travel requisitions</span></span>

<span data-ttu-id="5d1f7-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="5d1f7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="5d1f7-105">Захтев за путовање наводи трошкове који ће настати у сврху путовања.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-105">A travel requisition lists the expenses that will be incurred for the purpose of travel.</span></span> <span data-ttu-id="5d1f7-106">Захтев за путовање се подноси на увид и може се користити за одобравање трошкова.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-106">A travel requisition is submitted for review and can be used to authorize expenses.</span></span>

<span data-ttu-id="5d1f7-107">Можда ћете морати да предате захтев за путовање пре него што настане било какав трошак који се наплаћује организацији.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-107">You may be required to submit a travel requisition before you incur any expense that is charged to the organization.</span></span> <span data-ttu-id="5d1f7-108">Овај услов се примењује, без обзира на то да ли наплаћујете трошкове на кредитној картици предузећа, трошите готовину коју сте добили као аконтацију или ћете плаћати трошкове из свог џепа које ће вам организација надокнадити.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-108">This requirement applies, regardless of whether you charge expenses to a corporate credit card, spend cash that you received from a cash advance, or incur out-of-pocket expenses that will be reimbursed by the organization.</span></span>

<span data-ttu-id="5d1f7-109">Захтеви за путовање и смернице могу се користити за лакше управљање трошковима организације.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-109">Travel requisitions and policies can be used to help manage organization expenditures.</span></span> <span data-ttu-id="5d1f7-110">На пример, ако ваша организација ради на пројекту са фиксном ценом који захтева путовање, путни трошкови чланова пројектног тима морају се уклапати у буџет пројекта.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-110">For example, if your organization is working on a fixed-price project that requires travel, the travel expenses of the project's team members must fit within the project budget.</span></span> <span data-ttu-id="5d1f7-111">Захтевањем да се путни трошкови одобре пре него што настану, организација може да помогне да пројекат остане у оквиру буџета.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-111">By requiring that travel expenses be approved before they are incurred, the organization can help make sure that the project remains within budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="5d1f7-112">Конфигурисање</span><span class="sxs-lookup"><span data-stu-id="5d1f7-112">Configuration</span></span> 

<span data-ttu-id="5d1f7-113">Захтеви за путовање могу се конфигурисати као „обавезни“ омогућавањем параметра „Претходно одобрење путовања је обавезно“ у параметрима управљања трошковима.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-113">Travel Requisitions can be configured as "mandatory" by enabling the "Pre-authorization of travel is mandatory" parameter in Expense Management Parameters.</span></span> 

## <a name="create-and-submit-a-travel-requisition"></a><span data-ttu-id="5d1f7-114">Креирање и прослеђивање захтева за путовање</span><span class="sxs-lookup"><span data-stu-id="5d1f7-114">Create and submit a travel requisition</span></span>

1. <span data-ttu-id="5d1f7-115">Идите на **Моји трошкови: Захтев за путовање** и изаберите **Нови захтев за путовање**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-115">Go to **My expenses: Travel Requisition** , and select **New travel Requisition**.</span></span>
2. <span data-ttu-id="5d1f7-116">Унесите сврху и одредиште за захтев.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-116">Enter a purpose and destination for the requisition.</span></span>
3. <span data-ttu-id="5d1f7-117">У поље **Опис путовања** унесите све додатне информације.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-117">In the  **Travel description** field, enter any additional information.</span></span> 
4. <span data-ttu-id="5d1f7-118">За сваки од очекиваних трошкова, попут лета, оброка или изнајмљивања аутомобила, направите ставку трошка.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-118">For each of the expected expenses, such as Flight, meals, or car rental, create an expense line item.</span></span> <span data-ttu-id="5d1f7-119">Укључите процењени датум, процењени износ и валуту за сваки трошак.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-119">Include the estimated date, estimated amount, and the currency for each expense.</span></span> 
5. <span data-ttu-id="5d1f7-120">Када завршите са додавањем очекиваних трошкова, изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-120">When you have finished adding the expected expenses, select **Save**.</span></span>
6. <span data-ttu-id="5d1f7-121">Када будете спремни да предате захтев за путовање, изаберите **Ток посла** > **Проследи**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-121">When you are ready to submit the travel requisition, select **Workflow** > **Submit**.</span></span>

<span data-ttu-id="5d1f7-122">Одобрене захтеве за путовање можете прегледати у одељку **Моји трошкови: Захтев за путовање**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-122">You can view your approved travel requisitions under **My Expenses: Travel Requisition**.</span></span> 

## <a name="view-available-travel-requisitions"></a><span data-ttu-id="5d1f7-123">Приказ доступних захтева за путовање</span><span class="sxs-lookup"><span data-stu-id="5d1f7-123">View available travel requisitions</span></span>

<span data-ttu-id="5d1f7-124">Све своје захтеве за путовање можете прегледати у одељку **Моји трошкови: Захтеви за путовање**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-124">You can view all of your travel requisitions under **My Expenses: Travel Requisitions**.</span></span>

## <a name="approve-travel-requisitions"></a><span data-ttu-id="5d1f7-125">Одобравање захтева за путовање</span><span class="sxs-lookup"><span data-stu-id="5d1f7-125">Approve travel requisitions</span></span>

<span data-ttu-id="5d1f7-126">Изаберите захтев за путовање који желите да одобрите, а затим изаберите **Ток посла** > **Одобри**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-126">Select the travel requisition that you want to approve, and then select **Workflow** > **Approve**.</span></span>  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a><span data-ttu-id="5d1f7-127">Пошаљите извештај о трошковима користећи одобрени захтев за путовање</span><span class="sxs-lookup"><span data-stu-id="5d1f7-127">Submit an expense report using your approved travel requisition</span></span>

1. <span data-ttu-id="5d1f7-128">Направите нови извештај о трошковима и у заглављу извештаја о трошковима и са листе одобрених путних захтева изаберите **Мапирај на захтев за путовање**.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-128">Create a new expense report and in the expense report header, and from the list of approved travel requisitions, select **Map to Travel requisition**.</span></span>
2. <span data-ttu-id="5d1f7-129">Поље **Износ захтева за путовање** се аутоматски ажурира у заглављу извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-129">The **Travel requisition amount** field is automatically updated in the expense report header.</span></span>
3. <span data-ttu-id="5d1f7-130">Додајте сваки трошак настао током путовања.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-130">Add each expense incurred for the trip.</span></span> <span data-ttu-id="5d1f7-131">Ако је поље **Унапред овлашћено** омогућено, усклађени износ и одобрени износ за одређену категорију трошкова ће се ажурирати.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-131">If the **Pre-authorized** field is enabled, the reconciled amount and authorized amount for the specific expense category will be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="5d1f7-132">Када мапирате извештај о трошковима у одобрени захтев за путовање, износ трансакције не може бити већи од одобреног износа.</span><span class="sxs-lookup"><span data-stu-id="5d1f7-132">When you map an expense report to an approved travel requisition, the transaction amount can't be greater than the authorized amount.</span></span> 
