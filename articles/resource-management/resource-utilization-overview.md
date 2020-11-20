---
title: Преглед укупне искоришћености ресурса
description: Ова тема пружа информације о приказу укупне искоришћености ресурса у услузи Project Operations.
author: ruhercul
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8b85464dbb68523b122116225a604f67e7236f3e
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401394"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="cbe42-103">Преглед укупне искоришћености ресурса</span><span class="sxs-lookup"><span data-stu-id="cbe42-103">Resource utilization overview</span></span>

<span data-ttu-id="cbe42-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="cbe42-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cbe42-105">Ресурси могу имати циљану наплативу укупну искоришћеност.</span><span class="sxs-lookup"><span data-stu-id="cbe42-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="cbe42-106">Укупна искоришћеност се дефинише као атрибут подразумеване улоге ресурса или је подешена у запису појединачног ресурса који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="cbe42-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="cbe42-107">Израчунавање укупне искоришћености темељи се на стварним сатима које су ресурси пријавили коришћењем одобрених ставки времена.</span><span class="sxs-lookup"><span data-stu-id="cbe42-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="cbe42-108">Следеће формуле се користе за израчунавање укупне искоришћености:</span><span class="sxs-lookup"><span data-stu-id="cbe42-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="cbe42-109">Наплатива укупна искоришћеност = наплативи стварни сати ÷ капацитет ресурса</span><span class="sxs-lookup"><span data-stu-id="cbe42-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="cbe42-110">Ненаплатива укупна искоришћеност = Стварно време са ID-ом врсте наплате = Ненаплативо, допунско или недоступно ÷ Капацитет ресурса</span><span class="sxs-lookup"><span data-stu-id="cbe42-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="cbe42-111">Интерно = Стварно време без продајног уговора ÷ Капацитет ресурса</span><span class="sxs-lookup"><span data-stu-id="cbe42-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="cbe42-112">Капацитет ресурса = Радно време ресурса – Ван канцеларије – Нерадни дани</span><span class="sxs-lookup"><span data-stu-id="cbe42-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="cbe42-113">Можете пронаћи приказ **Укупна искоришћеност ресурса** у окну **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="cbe42-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="cbe42-114">Свака ћелија у мрежи представља проценат наплативе укупне искоришћености ресурса у неком периоду, као што је дан, недеља или месец.</span><span class="sxs-lookup"><span data-stu-id="cbe42-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="cbe42-115">Следеће формуле се користе за бојење ћелија:</span><span class="sxs-lookup"><span data-stu-id="cbe42-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="cbe42-116">**Зелена**: Наплатива укупна искоришћеност >= Циљна укупна искоришћеност ресурса</span><span class="sxs-lookup"><span data-stu-id="cbe42-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="cbe42-117">**Жута**: Циљна укупна искоришћеност – 20 <= Наплатива укупна искоришћеност < Циљна укупна искоришћеност</span><span class="sxs-lookup"><span data-stu-id="cbe42-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="cbe42-118">**Црвена**: Наплатива укупна искоришћеност < Циљна укупна искоришћеност – 20</span><span class="sxs-lookup"><span data-stu-id="cbe42-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="cbe42-119">Због тога што је приказ **Укупна искоришћеност ресурса** заснована на табли распореда, за филтрирање резултата можете користити могућности филтрирања табле распореда.</span><span class="sxs-lookup"><span data-stu-id="cbe42-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="cbe42-120">Мрежа захтева да подесите циљну укупну искоришћеност за улогу или појединачни ресурс.</span><span class="sxs-lookup"><span data-stu-id="cbe42-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="cbe42-121">Да бисте то подесили, идите на ставку **Ресурси** > **Улоге ресурса**.</span><span class="sxs-lookup"><span data-stu-id="cbe42-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="cbe42-122">Уз то, сваком ресурсу који се може резервисати мора се доделити подразумевана улога.</span><span class="sxs-lookup"><span data-stu-id="cbe42-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="cbe42-123">Идите на **Ресурси** > **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="cbe42-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="cbe42-124">На картици **Project Service** потврдите да је дефинисана улога ресурса и да је поље **Да ли је подразумевано** за ту улогу подешено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="cbe42-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="cbe42-125">Можете додати додатне улоге за које важи **Да ли је подразумевано** = **Не**.</span><span class="sxs-lookup"><span data-stu-id="cbe42-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="cbe42-126">Улога где се **Да ли је подразумевано** = **Да** користи за процену укупне искоришћености ресурса у односу на циљну искоришћеност за ту улогу.</span><span class="sxs-lookup"><span data-stu-id="cbe42-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="cbe42-127">На картици **Project Service** можете подесити и појединачну циљну укупну искоришћеност за ресурс.</span><span class="sxs-lookup"><span data-stu-id="cbe42-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="cbe42-128">Калкулација укупне искоришћености затим користи ту циљну укупну искоришћеност за процену циља ресурса уместо циља подразумеване улоге ресурса.</span><span class="sxs-lookup"><span data-stu-id="cbe42-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="cbe42-129">Укупна искоришћеност се приказује за ресурс само ако је тај ресурс одобрио наплативо време током периода који је приказан на мрежи.</span><span class="sxs-lookup"><span data-stu-id="cbe42-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>
