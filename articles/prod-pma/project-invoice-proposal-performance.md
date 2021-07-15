---
title: Перформансе предлога пројектних фактура
description: Ова тема пружа информације о побољшањима перформанси предлога пројектних фактура.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 5a14acf51d277b16896d64c4b12ee00bfb326910
ms.sourcegitcommit: 3a4b181be08ef0428104d72b54a3e61ac2782f14
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/17/2021
ms.locfileid: "6269808"
---
# <a name="project-invoice-proposal-performance"></a><span data-ttu-id="c14e4-103">Перформансе предлога пројектних фактура</span><span class="sxs-lookup"><span data-stu-id="c14e4-103">Project invoice proposal performance</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="c14e4-104">Када креирате нови предлог фактуре, можда ћете наићи на проблеме са перформансама како се буде повећавао број пројеката и потпројеката.</span><span class="sxs-lookup"><span data-stu-id="c14e4-104">When you create a new invoice proposal you might encounter performance issues as the number of projects and subprojects increase.</span></span> <span data-ttu-id="c14e4-105">Да би се побољшале перформансе, доступна је функција која смањује време потребно за креирање новог предлога фактуре за књижене трансакције пројеката.</span><span class="sxs-lookup"><span data-stu-id="c14e4-105">To improve performance, a feature is available that reduces the time needed to create a new invoice proposal for posted project transactions.</span></span>

## <a name="enable-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="c14e4-106">Омогућите побољшање перформанси предлога пројектних фактура</span><span class="sxs-lookup"><span data-stu-id="c14e4-106">Enable project invoice proposal performance enhancement</span></span>
<span data-ttu-id="c14e4-107">Да бисте омогућили функцију побољшања перформанси предлога пројектних фактура, извршите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="c14e4-107">To enable the project invoice proposal performance enhancement feature, complete the following steps.</span></span>

1.  <span data-ttu-id="c14e4-108">Идите на **Управљање функцијама** > **Све**.</span><span class="sxs-lookup"><span data-stu-id="c14e4-108">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="c14e4-109">На листи функција, пронађите **Побољшање перформанси предлога пројектних фактура**.</span><span class="sxs-lookup"><span data-stu-id="c14e4-109">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="c14e4-110">Изаберите дугме **Омогући одмах**.</span><span class="sxs-lookup"><span data-stu-id="c14e4-110">Select **Enable now**.</span></span>
3.  <span data-ttu-id="c14e4-111">Освежите прегледач, а затим направите нови предлог фактуре.</span><span class="sxs-lookup"><span data-stu-id="c14e4-111">Refresh your browser, and then create a new invoice proposal.</span></span>

## <a name="turn-off-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="c14e4-112">Искључите побољшање перформанси предлога пројектних фактура</span><span class="sxs-lookup"><span data-stu-id="c14e4-112">Turn off project invoice proposal performance enhancement</span></span>
<span data-ttu-id="c14e4-113">Извршите следеће кораке да бисте искључили функцију побољшања перформанси предлога пројектних фактура.</span><span class="sxs-lookup"><span data-stu-id="c14e4-113">Complete the following steps to turn off the project invoice proposal performance enhancement.</span></span>

1.  <span data-ttu-id="c14e4-114">Идите на **Управљање функцијама** > **Све**.</span><span class="sxs-lookup"><span data-stu-id="c14e4-114">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="c14e4-115">На листи функција, пронађите **Побољшање перформанси предлога пројектних фактура**.</span><span class="sxs-lookup"><span data-stu-id="c14e4-115">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="c14e4-116">Изаберите дугме **Онемогући**.</span><span class="sxs-lookup"><span data-stu-id="c14e4-116">Select **Disable**.</span></span>
3.  <span data-ttu-id="c14e4-117">Освежите прегледач.</span><span class="sxs-lookup"><span data-stu-id="c14e4-117">Refresh your browser.</span></span>

> [!NOTE]
> <span data-ttu-id="c14e4-118">Перформансе предлога фактуре се не могу применити када су омогућена правила обрачуна.</span><span class="sxs-lookup"><span data-stu-id="c14e4-118">Invoice proposal performance can't be applied when billing rules are enabled.</span></span>
> 
> <span data-ttu-id="c14e4-119">Током групног поступка за креирање предлога фактура, број подзадатака поделиће задатке на максималан број на основу броја уговора са трансакцијама подложним фактурисању, без обзира на то шта сте унели.</span><span class="sxs-lookup"><span data-stu-id="c14e4-119">During the batch process to create invoice proposals, the number of subtasks will split the tasks to a maximum number based on the number of contracts with invoiceable transactions, regardless of what you have entered.</span></span> <span data-ttu-id="c14e4-120">На пример, ако унесете **3** за број подзадатака за креирање предлога фактуре у пакету, а постоје само два уговора са трансакцијама које могу да се фактуришу, креирају се само два подзадатка.</span><span class="sxs-lookup"><span data-stu-id="c14e4-120">For example, if you enter **3** for the number of subtasks for invoice proposal creation in batch, and there are only two contracts with invoiceable transactions, only two subtasks are created.</span></span>
