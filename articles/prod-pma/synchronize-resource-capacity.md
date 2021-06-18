---
title: Синхронизација капацитета ресурса
description: Ова тема пружа информације о томе како синхронизовати капацитет ресурса у календарима и пројектима.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8bde3c434680f0651293cbce13ecdce945c3a743
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997529"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="8a83a-103">Синхронизација капацитета ресурса</span><span class="sxs-lookup"><span data-stu-id="8a83a-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="8a83a-104">Процеси за синхронизацију ресурса гарантују да ће се информације за календар и основни календар сливати у планирање ресурса пројекта.</span><span class="sxs-lookup"><span data-stu-id="8a83a-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="8a83a-105">Ако се календар промени, процеси извршавају потребна ажурирања распореда ресурса пројекта.</span><span class="sxs-lookup"><span data-stu-id="8a83a-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="8a83a-106">Процеси такође помажу у побољшању перформанси, јер су информације о ресурсима календара унапред синхронизоване.</span><span class="sxs-lookup"><span data-stu-id="8a83a-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="8a83a-107">Стога се ажурирања података о распореду ресурса дешавају брже.</span><span class="sxs-lookup"><span data-stu-id="8a83a-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="8a83a-108">Препоручујемо да процесе планирате као пакете уместо као један по један.</span><span class="sxs-lookup"><span data-stu-id="8a83a-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="8a83a-109">У супротном, постоји ризик да ће неко заборавити све датуме када су информације последњи пут синхронизоване.</span><span class="sxs-lookup"><span data-stu-id="8a83a-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="8a83a-110">Ако се не користе сви датуми, могу се појавити празнине током синхронизације датума.</span><span class="sxs-lookup"><span data-stu-id="8a83a-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![Синхронизација календара](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="8a83a-112">Синхронизација збирних вредности капацитета ресурса</span><span class="sxs-lookup"><span data-stu-id="8a83a-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="8a83a-113">Процес синхронизације је дизајниран да синхронизује све информације календара ресурса.</span><span class="sxs-lookup"><span data-stu-id="8a83a-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="8a83a-114">Ове информације укључују основне информације о календару о свим променама у табели капацитета календара ресурса пројекта.</span><span class="sxs-lookup"><span data-stu-id="8a83a-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="8a83a-115">Ако се у пројекат додају нови ресурси, синхронизација гарантује доступност ажурираних информација календара.</span><span class="sxs-lookup"><span data-stu-id="8a83a-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="8a83a-116">Ова синхронизација се може извршити у било ком тренутку.</span><span class="sxs-lookup"><span data-stu-id="8a83a-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="8a83a-117">Препоручујемо да користите пакет.</span><span class="sxs-lookup"><span data-stu-id="8a83a-117">We recommend that you use a batch.</span></span> <span data-ttu-id="8a83a-118">Опције су доступне током синхронизације резервација капацитета.</span><span class="sxs-lookup"><span data-stu-id="8a83a-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="8a83a-119">Изаберите **Управљање пројектима и рачуноводство** &gt; **Периодично** &gt; **Синхронизација капацитета** &gt; **Синхронизуј збирне вредности капацитета ресурса**.</span><span class="sxs-lookup"><span data-stu-id="8a83a-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="8a83a-120">Подесите опције у следећој табели.</span><span class="sxs-lookup"><span data-stu-id="8a83a-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="8a83a-121">Опција</span><span class="sxs-lookup"><span data-stu-id="8a83a-121">Option</span></span>      | <span data-ttu-id="8a83a-122">Опис</span><span class="sxs-lookup"><span data-stu-id="8a83a-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="8a83a-123">Шифра периода</span><span class="sxs-lookup"><span data-stu-id="8a83a-123">Period code</span></span> | <span data-ttu-id="8a83a-124">Опционално изаберите шифру интервала датума главне књиге да бисте поставили датуме почетка и завршетка процеса синхронизације за збирне вредности капацитета ресурса.</span><span class="sxs-lookup"><span data-stu-id="8a83a-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="8a83a-125">Датум почетка</span><span class="sxs-lookup"><span data-stu-id="8a83a-125">Start date</span></span>  | <span data-ttu-id="8a83a-126">Унесите датум почетка процеса синхронизације за збирне вредности капацитета ресурса.</span><span class="sxs-lookup"><span data-stu-id="8a83a-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="8a83a-127">Датум завршетка</span><span class="sxs-lookup"><span data-stu-id="8a83a-127">End date</span></span>    | <span data-ttu-id="8a83a-128">Унесите датум завршетка процеса синхронизације за збирне вредности капацитета ресурса.</span><span class="sxs-lookup"><span data-stu-id="8a83a-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="8a83a-129">[![Процес синхронизације](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="8a83a-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]