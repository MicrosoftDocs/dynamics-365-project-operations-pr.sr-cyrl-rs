---
title: Преглед преосталог фактурирања за пројекте и уговоре о пројектима
description: Ова тема пружа информације о томе како прегледати преостало време, трошкове и производе и како их означити као спремне за фактурирање.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: ''
ms.author: rumant
ms.date: 03/11/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: eb6d942d61bf8b5d20afb75c88716132a596bcbd
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084181"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="2ccf3-103">Преглед преосталог фактурирања за пројекте и уговоре о пројектима</span><span class="sxs-lookup"><span data-stu-id="2ccf3-103">Review the invoicing backlog on projects and project contracts</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="2ccf3-104">Када трансакција буде била спремна за креирање и обраду фактуре, трансакција треба бити обележена као **Спремно за фактурирање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="2ccf3-105">Ова тема описује врсте трансакција које се могу креирати.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="2ccf3-106">Преглед преостале наплате времена и материјала</span><span class="sxs-lookup"><span data-stu-id="2ccf3-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="2ccf3-107">Када се ставка времена и трошкова проследи и одобри за пројект, PSA креира стварну вредност пројекта.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="2ccf3-108">Ако се комбинација пројекта и класе трансакције мапирају у предмет уговора за пројекат заснован на времену и материјалу, када се ставка одобри, креирају се две стварне вредности:</span><span class="sxs-lookup"><span data-stu-id="2ccf3-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="2ccf3-109">Стварна вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="2ccf3-109">Cost actual</span></span> 
- <span data-ttu-id="2ccf3-110">Стварна вредност ненаплаћене продаје</span><span class="sxs-lookup"><span data-stu-id="2ccf3-110">Unbilled sales actual</span></span>

<span data-ttu-id="2ccf3-111">Стварне вредности ненаплаћене продаје представљају преосталу наплату и њихов статус наплате мора бити подешен на **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="2ccf3-112">Када се креира фактура за пројекат, стварне вредности ненаплаћене продаје означене као **Спремно за фактурисање** копирају се као детаљи ставке фактуре.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="2ccf3-113">Да бисте прегледали преостале наплате за време и материјале, идите на **Продаја** \> **Наплата** \> **Преостала наплата времена и материјала**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="2ccf3-114">Одаберите све стварне вредности ненаплаћене продаје које су спремне за фактурисање, а затим изаберите **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="2ccf3-115">Статус наплате ових стварних вредности је промењен у **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![Преостала наплата времена и материјала](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="2ccf3-117">Преглед преостале наплате за производ</span><span class="sxs-lookup"><span data-stu-id="2ccf3-117">Review the product billing backlog</span></span>

<span data-ttu-id="2ccf3-118">У апликацији PSA, када пројектни уговор има предмете уговора засноване на производима, ти предмети се узимају у обзир за фактурисање сваки пут када се креира фактура за пројектни уговор.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="2ccf3-119">Сваки производ који има предмете уговора обележене као **Спремно за фактурисање** копира се у фактуру пројекта као ставке фактуре за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="2ccf3-120">Да бисте прегледали преосталу наплату за производ, идите на **Продаја** \> **Наплата** \> **Преостала наплата за производ**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="2ccf3-121">Одаберите све предмете уговора засноване на производима који су спремни за фактурисање, а затим изаберите **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="2ccf3-122">Статус наплате ових ставки је промењен у **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![Преостала наплата за производ](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="2ccf3-124">Прегед контролних тачака наплате у уговорима са фиксном ценом</span><span class="sxs-lookup"><span data-stu-id="2ccf3-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="2ccf3-125">Сваки предмет уговора за пројекат који користи начин наплате фиксне цене мора дефинисати контролне тачке у уговору.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="2ccf3-126">Ове контролне тачке у уговору могу се фактурисати само ако су означене као **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="2ccf3-127">Да бисте прегледали контролне тачке наплате, идите на **Продаја** \> **Наплата** \> **Контролне тачке са фиксном ценом**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="2ccf3-128">Одаберите контролне тачке које су спремне за фактурисање, а затим изаберите **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="2ccf3-129">Статус наплате ових контролних тачака је промењен у **Спремно за фактурисање**.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![Контролне тачке са фиксном ценом](media/FPBacklog.png)
