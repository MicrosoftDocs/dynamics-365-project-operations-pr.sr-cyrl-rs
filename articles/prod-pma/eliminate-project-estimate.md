---
title: Елиминисање процене за пројекат
description: Ова тема пружа информације о елиминисању процене пројекта након што је завршена.
author: Yowelle
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: a4ad06bef7ed66a626c6d2ad7ef01ba5b99d1c0f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006934"
---
# <a name="eliminate-a-project-estimate"></a><span data-ttu-id="2cf81-103">Елиминисање процене за пројекат</span><span class="sxs-lookup"><span data-stu-id="2cf81-103">Eliminate a project estimate</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2cf81-104">Процене пројекта пружају финансијски приказ за посао који је процењен и заказан за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2cf81-104">Project estimates provide the financial view for work that is estimated and scheduled for a project.</span></span> <span data-ttu-id="2cf81-105">Да бисте радили са проценама за пројекат, морате приложити пројекат пројекту за процену.</span><span class="sxs-lookup"><span data-stu-id="2cf81-105">To work with estimates for a project, you must attach the project to an estimate project.</span></span> <span data-ttu-id="2cf81-106">Пројект процене увек се заснива на постојећем пројекту, међутим више пројеката може се односити на један пројекат процене.</span><span class="sxs-lookup"><span data-stu-id="2cf81-106">An estimate project is always based on an existing project, however multiple projects can refer to a single estimate project.</span></span> <span data-ttu-id="2cf81-107">За процену пројеката могу се приложити само пројекти са фиксном ценом и инвестициони пројекти, који морају припадати истој пројектној групи као и пројекат процене.</span><span class="sxs-lookup"><span data-stu-id="2cf81-107">Only fixed-price and investment projects can be attached to estimate projects, and those projects must belong to the same project group as the estimate project.</span></span>

<span data-ttu-id="2cf81-108">Да би се елиминисао пројект процене, он мора бити потпун.</span><span class="sxs-lookup"><span data-stu-id="2cf81-108">To eliminate an estimate project, it must be complete.</span></span> <span data-ttu-id="2cf81-109">Следећи кораци објашњавају како елиминисати процену.</span><span class="sxs-lookup"><span data-stu-id="2cf81-109">The following steps explain how to eliminate an estimate.</span></span>

1. <span data-ttu-id="2cf81-110">Идите на **Управљање пројектима и рачуноводство** > **Сви пројекти** и отворите пројекат.</span><span class="sxs-lookup"><span data-stu-id="2cf81-110">Go to **Project management and accounting** > **All Projects** and open the project.</span></span> 
2. <span data-ttu-id="2cf81-111">На картици **Управљање** изаберите **Процене** и на страници **Процена** изаберите страницу **Елиминисање**.</span><span class="sxs-lookup"><span data-stu-id="2cf81-111">On the **Manage** tab, select **Estimates**, and on the **Estimate** page select **Eliminate**.</span></span>
3. <span data-ttu-id="2cf81-112">На страници **Елиминишите процену** на картици **Општи подаци** поставите следеће опције:</span><span class="sxs-lookup"><span data-stu-id="2cf81-112">On the **Eliminate estimate** page on the **General** tab, set the following options:</span></span>

   - <span data-ttu-id="2cf81-113">**Шифра периода**: Изаберите шифру периода да бисте изабрали одговарајуће процене пројеката.</span><span class="sxs-lookup"><span data-stu-id="2cf81-113">**Period code**: Select the period code to choose the appropriate estimate projects.</span></span> 
   - <span data-ttu-id="2cf81-114">**Датум процене**: Изаберите одговарајући датум процене за елиминисање.</span><span class="sxs-lookup"><span data-stu-id="2cf81-114">**Estimate date**: Select the appropriate estimate date for elimination.</span></span>
   - <span data-ttu-id="2cf81-115">**Елиминишите WIP упозорења**: Омогућите ову опцију да бисте пружили обавештење када ће процена која је повезана са радом у току (WIP) бити уклоњена.</span><span class="sxs-lookup"><span data-stu-id="2cf81-115">**Eliminate with WIP warnings**: Enable this option to provide notification when an estimate that is associated with a work in progress (WIP) will be eliminated.</span></span> <span data-ttu-id="2cf81-116">Када ова опција није омогућена, уклањање се не може наставити ако постоје непроцењене трансакције.</span><span class="sxs-lookup"><span data-stu-id="2cf81-116">When this option is not enabled, elimination can’t continue if any non-estimated transactions exist.</span></span> 
   > [!NOTE]
   > <span data-ttu-id="2cf81-117">Ова опција је доступна само када се елиминација примењује на процењени пројекат.</span><span class="sxs-lookup"><span data-stu-id="2cf81-117">This option is available only when elimination is applied to an estimate project.</span></span> <span data-ttu-id="2cf81-118">Није доступна ако користите периодична објављивања.</span><span class="sxs-lookup"><span data-stu-id="2cf81-118">It is not available if you are using periodic postings.</span></span> <span data-ttu-id="2cf81-119">Ово подешавање ради са подешавањима на картици **Процена**, на страници **Параметри пројекта**, у групи поља **Дозволите елиминацију када постоје непроцењене трансакције**.</span><span class="sxs-lookup"><span data-stu-id="2cf81-119">This setting works with the settings on the **Estimate** tab on the **Project parameters** page, in the **Allow elimination when non-estimated transactions exist** field group.</span></span>
   - <span data-ttu-id="2cf81-120">**Поставите фазу на Завршено**: Омогућите ову опцију да бисте поставили фазу процене пројекта на **Завршено** након што покренете елиминацију.</span><span class="sxs-lookup"><span data-stu-id="2cf81-120">**Set stage to Finished**: Enable this option to set the estimate project’s stage to **Finished** after you run the elimination.</span></span>
   - <span data-ttu-id="2cf81-121">**Одштампајте листу процена**: Изаберите информације које ће бити укључене када се одштампа листа процена.</span><span class="sxs-lookup"><span data-stu-id="2cf81-121">**Print estimate list**: Select the information to be included when the estimate list is printed.</span></span>
   - <span data-ttu-id="2cf81-122">**Прикажи Infolog**: Омогућите ову опцију за приказ Infolog-а.</span><span class="sxs-lookup"><span data-stu-id="2cf81-122">**Show Infolog**: Enable this option to display the Infolog.</span></span>
   - <span data-ttu-id="2cf81-123">**Датум књижења**: Изаберите датум књижења процене у књизи.</span><span class="sxs-lookup"><span data-stu-id="2cf81-123">**Posting date**: Choose the ledger posting date of the estimate.</span></span>

4.  <span data-ttu-id="2cf81-124">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="2cf81-124">Select **OK**.</span></span>
5. <span data-ttu-id="2cf81-125">Након завршетка поступка елиминације, пројекат са елиминисаном проценом приказује се са негативном вредношћу.</span><span class="sxs-lookup"><span data-stu-id="2cf81-125">After the elimination process is complete, the eliminated estimate project is displayed with a negative value.</span></span> 

<span data-ttu-id="2cf81-126">Ако нисте намеравали да елиминишете процену, можете да изаберете елиминисану процену и изаберете **Опозови елиминацију**.</span><span class="sxs-lookup"><span data-stu-id="2cf81-126">If you did not intend to eliminate an estimate, you can select the eliminated estimate and select **Reverse elimination**.</span></span>   


[!INCLUDE[footer-include](../includes/footer-banner.md)]