---
title: Фазе пројекта
description: Ова тема пружа информације о фазама пројекта које су доступне у услузи Microsoft Dynamics Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: b11c67ebd21fdf423eeae2db8154f26787c2e64f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897964"
---
# <a name="project-stages"></a><span data-ttu-id="a52c5-103">Фазе пројекта</span><span class="sxs-lookup"><span data-stu-id="a52c5-103">Project stages</span></span>

<span data-ttu-id="a52c5-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="a52c5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a52c5-105">Фазе пројекта се дизајнирају тако да одражавају статус пројекта током његовом напретка.</span><span class="sxs-lookup"><span data-stu-id="a52c5-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="a52c5-106">Прилагођавања се могу користити за аутоматско ажурирање фаза са токовима пословних процеса, Power Automate или проширења додатних компоненти.</span><span class="sxs-lookup"><span data-stu-id="a52c5-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="a52c5-107">Следеће фазе су дефинисане у подразумеваном току пословног процеса:</span><span class="sxs-lookup"><span data-stu-id="a52c5-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="a52c5-108">Нови</span><span class="sxs-lookup"><span data-stu-id="a52c5-108">New</span></span>
- <span data-ttu-id="a52c5-109">Понуда</span><span class="sxs-lookup"><span data-stu-id="a52c5-109">Quote</span></span>
- <span data-ttu-id="a52c5-110">План</span><span class="sxs-lookup"><span data-stu-id="a52c5-110">Plan</span></span>
- <span data-ttu-id="a52c5-111">Испорука</span><span class="sxs-lookup"><span data-stu-id="a52c5-111">Deliver</span></span>
- <span data-ttu-id="a52c5-112">Доврши</span><span class="sxs-lookup"><span data-stu-id="a52c5-112">Complete</span></span>
- <span data-ttu-id="a52c5-113">Затворите</span><span class="sxs-lookup"><span data-stu-id="a52c5-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="a52c5-114">Нови</span><span class="sxs-lookup"><span data-stu-id="a52c5-114">New</span></span>

<span data-ttu-id="a52c5-115">Када креирате пројекат, фаза пројекта се подешава на **Ново**.</span><span class="sxs-lookup"><span data-stu-id="a52c5-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="a52c5-116">Ако је пројекат креиран из предлошка, можда ће имати распоред, процену и податке о тиму.</span><span class="sxs-lookup"><span data-stu-id="a52c5-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="a52c5-117">У супротном, то је скица пројекта, а преостале компоненте морају бити унете.</span><span class="sxs-lookup"><span data-stu-id="a52c5-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="a52c5-118">Понуда</span><span class="sxs-lookup"><span data-stu-id="a52c5-118">Quote</span></span>

<span data-ttu-id="a52c5-119">Када повежете пројекат са понудом или га креирате из понуде, фаза пројекта се подешава на **Понуда**, а процењени датум почетка и завршетка се ажурирају.</span><span class="sxs-lookup"><span data-stu-id="a52c5-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="a52c5-120">Док је пројекат је у фази **понуде**, картица **Продаја** на страници **Ентитет пројекта** приказује детаље понуде.</span><span class="sxs-lookup"><span data-stu-id="a52c5-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="a52c5-121">План</span><span class="sxs-lookup"><span data-stu-id="a52c5-121">Plan</span></span>

<span data-ttu-id="a52c5-122">Када вам буде одобрена понуда повезана са пројектом и када се пројекат пребаци у фазу **уговора**, фаза пројекта се ажурира на **План**.</span><span class="sxs-lookup"><span data-stu-id="a52c5-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="a52c5-123">Док је пројекат је у фази **плана**, на страници **Ентитет пројекта** се приказују детаљи уговора.</span><span class="sxs-lookup"><span data-stu-id="a52c5-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="a52c5-124">Испорука</span><span class="sxs-lookup"><span data-stu-id="a52c5-124">Deliver</span></span>

<span data-ttu-id="a52c5-125">Када је пројектни план завршен, а ви сте спремни за почетак пројекта, менаџер пројекта треба да ажурира фазу пројекта на **Испорука** да би показао да је пројекат започет.</span><span class="sxs-lookup"><span data-stu-id="a52c5-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="a52c5-126">Довршено</span><span class="sxs-lookup"><span data-stu-id="a52c5-126">Complete</span></span> 

<span data-ttu-id="a52c5-127">Када је посао за пројекат завршен, менаџер пројекта може да ажурира фазу на **Довршено**.</span><span class="sxs-lookup"><span data-stu-id="a52c5-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="a52c5-128">Ажурирањем фазе пројекта на **Довршено**, менаџер пројекта показује да је посао завршен 100%, али да је пројекат и даље отворен тако да се могу евидентирати било какве ставке времена или трошкова на чекању.</span><span class="sxs-lookup"><span data-stu-id="a52c5-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="a52c5-129">Затворите</span><span class="sxs-lookup"><span data-stu-id="a52c5-129">Close</span></span>

<span data-ttu-id="a52c5-130">Када се све трансакције евидентирају за пројекат, менаџер пројекта може да ажурира фазу на **Затворено**.</span><span class="sxs-lookup"><span data-stu-id="a52c5-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="a52c5-131">У том тренутку не могу се евидентирати никакве трансакције и пројект се подешава на „само за читање“.</span><span class="sxs-lookup"><span data-stu-id="a52c5-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>

