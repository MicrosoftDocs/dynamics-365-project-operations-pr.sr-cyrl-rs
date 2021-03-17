---
title: Перформансе планирања ресурса за пројекат
description: Ова тема пружа информације о томе како побољшати перформансе планирања ресурса за велики број пројеката.
author: Yowelle
manager: AnnBe
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 34c31570778f9b64c23387112cf56fa1139cd0fd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289027"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="db31a-103">Перформансе планирања ресурса за пројекат</span><span class="sxs-lookup"><span data-stu-id="db31a-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="db31a-104">Проблеми са учинком који се односе на планирање ресурса могу се појавити када број пројеката достигне више хиљада.</span><span class="sxs-lookup"><span data-stu-id="db31a-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="db31a-105">Да би се побољшале перформансе планирања ресурса, доступна је функција која омогућава корисницима да смање време потребно за покретање обрасца доступности ресурса.</span><span class="sxs-lookup"><span data-stu-id="db31a-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="db31a-106">Конкретно, ово уклања поступак збирне синхронизације капацитета ресурса и користи табелу **ResProjectResource** за убрзање претраживања ресурса.</span><span class="sxs-lookup"><span data-stu-id="db31a-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="db31a-107">Имајте на уму да се табела **ResRollup** више неће користити.</span><span class="sxs-lookup"><span data-stu-id="db31a-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="db31a-108">Ако постоји зависност или поступка збирне синхронизације капацитета ресурса или табеле **ResProjectResource**, немојте користити ову функцију.</span><span class="sxs-lookup"><span data-stu-id="db31a-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="db31a-109">Омогућите побољшање перформанси планирања ресурса</span><span class="sxs-lookup"><span data-stu-id="db31a-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="db31a-110">Да бисте омогућили побољшање перформанси планирања ресурса, извршите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="db31a-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="db31a-111">Идите на **Управљање функцијама** > **Све**, а на листи функција пронађите **Омогући функцију побољшања перформанси планирања ресурса пројекта**.</span><span class="sxs-lookup"><span data-stu-id="db31a-111">Go to **Feature management** > **All**, and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="db31a-112">Изаберите дугме **Омогући одмах**.</span><span class="sxs-lookup"><span data-stu-id="db31a-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="db31a-113">Ако не можете да пронађете функцију на листи, изаберите **Провери да ли има ажурирања** да бисте освежили листу.</span><span class="sxs-lookup"><span data-stu-id="db31a-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="db31a-114">Освежите прегледач, а затим идите на **Управљање пројектима и рачуноводство** > **Периодично** > **Ресурси пројекта** > **Синхронизујте капацитет календара ресурса у свим компанијама**.</span><span class="sxs-lookup"><span data-stu-id="db31a-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="db31a-115">Подесите **Уклоните постојеће евиденције о капацитету** на **Да** да бисте уклонили претходне податке.</span><span class="sxs-lookup"><span data-stu-id="db31a-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="db31a-116">Ако желите да генеришете инкременталне податке, подесите га на **Не**.</span><span class="sxs-lookup"><span data-stu-id="db31a-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="db31a-117">У пољу **Шифра периода**, изаберите период у којем треба генерисати податке.</span><span class="sxs-lookup"><span data-stu-id="db31a-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="db31a-118">Ако изаберете шифру периода, датуми почетка и завршетка не морају бити дефинисани.</span><span class="sxs-lookup"><span data-stu-id="db31a-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="db31a-119">Ако оставите поље **Шифра периода** празно, одаберите одређене датуме почетка и завршетка да бисте генерисали податке.</span><span class="sxs-lookup"><span data-stu-id="db31a-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="db31a-120">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="db31a-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="db31a-121">Ово ће дистрибуирати опште податке у табели **ResCalendarCapacity** у свим компанијама у вашем окружењу, тако да групни посао треба покренути само у једном правном лицу.</span><span class="sxs-lookup"><span data-stu-id="db31a-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="db31a-122">Подаци у овом групном послу потребни су за израчунавање капацитета ресурса кроз придружени календар.</span><span class="sxs-lookup"><span data-stu-id="db31a-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="db31a-123">Идите на **Управљање пројектима и рачуноводство** > **Периодично** > **Ресурси пројекта** > **Попуните пројектне ресурсе у свим компанијама**, а затим изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="db31a-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="db31a-124">Ово је скрипта за надоградњу података за опште податке у табелама **ResProjectResource**, **ResCalendarDateTimeRange** и **ResEffectiveDateTimeRange**.</span><span class="sxs-lookup"><span data-stu-id="db31a-124">This is the data upgrade script for general data in the **ResProjectResource**, **ResCalendarDateTimeRange**, and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="db31a-125">Вредности за поље **PSAPRojSchedRole.RootActivity** такође се ажурирају.</span><span class="sxs-lookup"><span data-stu-id="db31a-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="db31a-126">Ако се ово не покрене, примићете упозорење када покушате да извршите операције планирања ресурса.</span><span class="sxs-lookup"><span data-stu-id="db31a-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="db31a-127">Искључите побољшање перформанси планирања ресурса</span><span class="sxs-lookup"><span data-stu-id="db31a-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="db31a-128">Идите на **Управљање функцијама** > **Све**, па потражите **Омогући функцију побољшања перформанси планирања ресурса пројекта**.</span><span class="sxs-lookup"><span data-stu-id="db31a-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="db31a-129">Изаберите функцију, а затим одаберите дугме **Онемогући**.</span><span class="sxs-lookup"><span data-stu-id="db31a-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="db31a-130">Освежите прегледач.</span><span class="sxs-lookup"><span data-stu-id="db31a-130">Refresh your browser.</span></span>
4. <span data-ttu-id="db31a-131">Идите на **Управљање пројектима и рачуноводство** > **Периодично** > **Синхронизација капацитета** > **Синхронизуј збирне вредности капацитета ресурса**.</span><span class="sxs-lookup"><span data-stu-id="db31a-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="db31a-132">На страници **Збирна синхронизација капацитета** подесите **Уклони постојеће евиденције о капацитету** на **Да** како бисте уклонили претходне податке.</span><span class="sxs-lookup"><span data-stu-id="db31a-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="db31a-133">Ако желите да генеришете инкременталне податке, подесите га на **Не**.</span><span class="sxs-lookup"><span data-stu-id="db31a-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="db31a-134">У пољу **Шифра периода**, изаберите период у којем треба генерисати податке.</span><span class="sxs-lookup"><span data-stu-id="db31a-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="db31a-135">Ако изаберете шифру периода, датуми почетка и завршетка не морају бити дефинисани.</span><span class="sxs-lookup"><span data-stu-id="db31a-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="db31a-136">Ако оставите поље **Шифра периода** празно, одаберите одређене датуме почетка и завршетка да бисте генерисали податке.</span><span class="sxs-lookup"><span data-stu-id="db31a-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="db31a-137">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="db31a-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="db31a-138">Ово ће дистрибуирати опште податке у табели **ResRollup** у свим компанијама у вашем окружењу, тако да групни посао треба покренути само у једном правном лицу.</span><span class="sxs-lookup"><span data-stu-id="db31a-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="db31a-139">Овај групни посао потребан је свим приказима **Доступност ресурса**.</span><span class="sxs-lookup"><span data-stu-id="db31a-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="db31a-140">Ако се овај групни посао не покрене, **ResRollup** подаци ће се генерисати у ходу, што може потрајати.</span><span class="sxs-lookup"><span data-stu-id="db31a-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]