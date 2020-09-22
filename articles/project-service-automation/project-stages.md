---
title: Фазе пројекта
description: Ова тема пружа информације о стварним фазама пројекта.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 983c25a0-ed21-4151-a109-b385a88285fa
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 70aa057e127df7ba925e84f5d056a06a4cc8833e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755350"
---
# <a name="project-stages"></a><span data-ttu-id="54d22-103">Фазе пројекта</span><span class="sxs-lookup"><span data-stu-id="54d22-103">Project stages</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="54d22-104">Фазе пројекта ажурирају се тако да одражавају статус пројекта током његовом напретка.</span><span class="sxs-lookup"><span data-stu-id="54d22-104">Project stages are updated to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="54d22-105">Подразумевани ток пословног процеса аутоматски ажурира неке фазе пројекта, док друге ручно ажурира менаџер пројекта.</span><span class="sxs-lookup"><span data-stu-id="54d22-105">The default business process flow automatically updates some stages of the project while others are manually updated by the project manager.</span></span> 

<span data-ttu-id="54d22-106">Следеће фазе су дефинисане у подразумеваном току пословног процеса:</span><span class="sxs-lookup"><span data-stu-id="54d22-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="54d22-107">Ново</span><span class="sxs-lookup"><span data-stu-id="54d22-107">New</span></span>
- <span data-ttu-id="54d22-108">Понуда</span><span class="sxs-lookup"><span data-stu-id="54d22-108">Quote</span></span>
- <span data-ttu-id="54d22-109">План</span><span class="sxs-lookup"><span data-stu-id="54d22-109">Plan</span></span>
- <span data-ttu-id="54d22-110">Испорука</span><span class="sxs-lookup"><span data-stu-id="54d22-110">Deliver</span></span>
- <span data-ttu-id="54d22-111">Довршено</span><span class="sxs-lookup"><span data-stu-id="54d22-111">Complete</span></span>
- <span data-ttu-id="54d22-112">Затворите</span><span class="sxs-lookup"><span data-stu-id="54d22-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="54d22-113">Ново</span><span class="sxs-lookup"><span data-stu-id="54d22-113">New</span></span>

<span data-ttu-id="54d22-114">Када креирате пројекат, фаза пројекта се подешава на **Ново**.</span><span class="sxs-lookup"><span data-stu-id="54d22-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="54d22-115">Ако је пројекат креиран из предлошка, можда ће имати распоред, процену и податке о тиму.</span><span class="sxs-lookup"><span data-stu-id="54d22-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="54d22-116">У супротном, то је само скица пројекта, а преостале компоненте морају бити унете.</span><span class="sxs-lookup"><span data-stu-id="54d22-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="54d22-117">Понуда</span><span class="sxs-lookup"><span data-stu-id="54d22-117">Quote</span></span>

<span data-ttu-id="54d22-118">Када повежете пројекат са понудом или га креирате из понуде, фаза пројекта се подешава на **Понуда**, а процењени датум почетка и завршетка се ажурирају.</span><span class="sxs-lookup"><span data-stu-id="54d22-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="54d22-119">Док је пројекат је у фази **понуде**, картица **Продаја** на страници **Ентитет пројекта** приказује детаље понуде.</span><span class="sxs-lookup"><span data-stu-id="54d22-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="54d22-120">План</span><span class="sxs-lookup"><span data-stu-id="54d22-120">Plan</span></span>

<span data-ttu-id="54d22-121">Када вам буде одобрена понуда повезана са пројектом и када се пројекат пребаци у фазу **уговора**, фаза пројекта се ажурира на **План**.</span><span class="sxs-lookup"><span data-stu-id="54d22-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="54d22-122">Док је пројекат је у фази **плана**, на страници **Ентитет пројекта** се приказују детаљи уговора.</span><span class="sxs-lookup"><span data-stu-id="54d22-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="54d22-123">Испорука</span><span class="sxs-lookup"><span data-stu-id="54d22-123">Deliver</span></span>

<span data-ttu-id="54d22-124">Када је пројектни план завршен, а ви сте спремни за почетак пројекта, менаџер пројекта треба да ажурира фазу пројекта на **Испорука** да би показао да је пројекат започет.</span><span class="sxs-lookup"><span data-stu-id="54d22-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="54d22-125">Довршено</span><span class="sxs-lookup"><span data-stu-id="54d22-125">Complete</span></span> 

<span data-ttu-id="54d22-126">Када је посао за пројекат завршен, менаџер пројекта може да ажурира фазу на **Довршено**.</span><span class="sxs-lookup"><span data-stu-id="54d22-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="54d22-127">Ажурирањем фазе пројекта на **Довршено**, менаџер пројекта показује да је посао завршен 100%, али да је пројекат и даље отворен тако да се могу евидентирати било какве ставке времена или трошкова на чекању.</span><span class="sxs-lookup"><span data-stu-id="54d22-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="54d22-128">Затворите</span><span class="sxs-lookup"><span data-stu-id="54d22-128">Close</span></span>

<span data-ttu-id="54d22-129">Када се све трансакције евидентирају за пројекат, менаџер пројекта може да ажурира фазу на **Затворено**.</span><span class="sxs-lookup"><span data-stu-id="54d22-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="54d22-130">У том тренутку не могу се евидентирати никакве трансакције и пројект се подешава на „само за читање“.</span><span class="sxs-lookup"><span data-stu-id="54d22-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>
