---
title: Перформансе предлога пројектних фактура
description: Ова тема пружа информације о побољшањима перформанси предлога пројектних фактура.
author: Yowelle
manager: AnnBe
ms.date: 03/05/2021
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ''
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 20121-03-05
ms.dyn365.ops.version: 10.0.18
ms.openlocfilehash: 78c924cba8107471a5f8e6d6a38265890d32d72b
ms.sourcegitcommit: 2350c6f3728067a8298adde640e6fdd5984eb077
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "5573577"
---
# <a name="project-invoice-proposal-performance"></a><span data-ttu-id="26a8f-103">Перформансе предлога пројектних фактура</span><span class="sxs-lookup"><span data-stu-id="26a8f-103">Project invoice proposal performance</span></span>

[!include [banner](../includes/banner.md)]

[!include [banner](../includes/preview-banner.md)]

<span data-ttu-id="26a8f-104">Када креирате нови предлог фактуре, можда ћете наићи на проблеме са перформансама како се буде повећавао број пројеката и потпројеката.</span><span class="sxs-lookup"><span data-stu-id="26a8f-104">When you create a new invoice proposal you might encounter performance issues as the number of projects and subprojects increase.</span></span> <span data-ttu-id="26a8f-105">Да би се побољшале перформансе, доступна је функција која смањује време потребно за креирање новог предлога фактуре за књижене трансакције пројеката.</span><span class="sxs-lookup"><span data-stu-id="26a8f-105">To improve performance, a feature is available that reduces the time needed to create a new invoice proposal for posted project transactions.</span></span>

## <a name="enable-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="26a8f-106">Омогућите побољшање перформанси предлога пројектних фактура</span><span class="sxs-lookup"><span data-stu-id="26a8f-106">Enable project invoice proposal performance enhancement</span></span>
<span data-ttu-id="26a8f-107">Да бисте омогућили функцију побољшања перформанси предлога пројектних фактура, извршите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="26a8f-107">To enable the project invoice proposal performance enhancement feature, complete the following steps.</span></span>

1.  <span data-ttu-id="26a8f-108">Идите на **Управљање функцијама** > **Све**.</span><span class="sxs-lookup"><span data-stu-id="26a8f-108">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="26a8f-109">На листи функција, пронађите **Побољшање перформанси предлога пројектних фактура**.</span><span class="sxs-lookup"><span data-stu-id="26a8f-109">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="26a8f-110">Изаберите дугме **Омогући одмах**.</span><span class="sxs-lookup"><span data-stu-id="26a8f-110">Select **Enable now**.</span></span>
3.  <span data-ttu-id="26a8f-111">Освежите прегледач, а затим направите нови предлог фактуре.</span><span class="sxs-lookup"><span data-stu-id="26a8f-111">Refresh your browser, and then create a new invoice proposal.</span></span>

## <a name="turn-off-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="26a8f-112">Искључите побољшање перформанси предлога пројектних фактура</span><span class="sxs-lookup"><span data-stu-id="26a8f-112">Turn off project invoice proposal performance enhancement</span></span>
<span data-ttu-id="26a8f-113">Извршите следеће кораке да бисте искључили функцију побољшања перформанси предлога пројектних фактура.</span><span class="sxs-lookup"><span data-stu-id="26a8f-113">Complete the following steps to turn off the project invoice proposal performance enhancement.</span></span>

1.  <span data-ttu-id="26a8f-114">Идите на **Управљање функцијама** > **Све**.</span><span class="sxs-lookup"><span data-stu-id="26a8f-114">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="26a8f-115">На листи функција, пронађите **Побољшање перформанси предлога пројектних фактура**.</span><span class="sxs-lookup"><span data-stu-id="26a8f-115">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="26a8f-116">Изаберите дугме **Онемогући**.</span><span class="sxs-lookup"><span data-stu-id="26a8f-116">Select **Disable**.</span></span>
3.  <span data-ttu-id="26a8f-117">Освежите прегледач.</span><span class="sxs-lookup"><span data-stu-id="26a8f-117">Refresh your browser.</span></span>

> [!NOTE]
> <span data-ttu-id="26a8f-118">Перформансе предлога фактуре не може се применити када су омогућена правила обрачуна или су покренуте групне обраде.</span><span class="sxs-lookup"><span data-stu-id="26a8f-118">Invoice proposal performance can't be applied when billing rules are enabled or batch processes are running.</span></span>
