---
title: Уговори о пројекту
description: Ова тема даје примере уговора о пројекту које можете креирати за различите врсте пројеката и изворе финансирања, као и како можете управљати уговорима и фактурисати клијентима пројеката.
author: Yowelle
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a794ec38ac07c1418f9e95b741941a83492bb3d5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999779"
---
# <a name="project-contracts"></a><span data-ttu-id="2635e-103">Уговори о пројекту</span><span class="sxs-lookup"><span data-stu-id="2635e-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2635e-104">Овај чланак даје примере уговора о пројекту које можете креирати за различите врсте пројеката и изворе финансирања, као и како можете управљати уговорима и фактурисати клијентима пројеката.</span><span class="sxs-lookup"><span data-stu-id="2635e-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="2635e-105">Тип пројекта који креирате за уговор о пројекту одређује методу који се користи за фактурисање клијената пројекта.</span><span class="sxs-lookup"><span data-stu-id="2635e-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="2635e-106">Можете да промените уговор о пројекту и с њим повезани пројекат, али не можете да промените тип пројекта.</span><span class="sxs-lookup"><span data-stu-id="2635e-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="2635e-107">Коришћењем уговора о пројекту можете истовремено фактурисати један или више пројеката.</span><span class="sxs-lookup"><span data-stu-id="2635e-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="2635e-108">Уговор о пројекту такође гарантује доследне процедуре фактурисања за сваки подпројекат у структури пројекта.</span><span class="sxs-lookup"><span data-stu-id="2635e-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="2635e-109">Сваки пројекат који ће бити фактурисан мора бити повезан са уговором о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="2635e-110">Поставке за уговор о пројекту односе се на све пројекте и потпројекте који су повезани са тим уговором о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="2635e-111">У уговору о пројекту може се навести један или више извора финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="2635e-112">Према томе, можете поделити обрачун између више донатора, поставити ограничења финансирања тако да се изворима финансирања не наплаћује више од одређеног износа и конфигурисати правила финансирања за наплату трошкова.</span><span class="sxs-lookup"><span data-stu-id="2635e-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="2635e-113">Финансирање уговора о пројекту</span><span class="sxs-lookup"><span data-stu-id="2635e-113">Funding for project contracts</span></span>
<span data-ttu-id="2635e-114">Неки уговори о пројекту наводе да више страна дели одговорност за финансирање трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="2635e-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="2635e-115">У наставку су наведени неки примери:</span><span class="sxs-lookup"><span data-stu-id="2635e-115">Here are some examples:</span></span>

-   <span data-ttu-id="2635e-116">Велики клијент који има више одељења захтева да се финансирање пројекта подели по одсецима.</span><span class="sxs-lookup"><span data-stu-id="2635e-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="2635e-117">Ваша компанија дели трошкове великог пројекта са спољном организацијом.</span><span class="sxs-lookup"><span data-stu-id="2635e-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="2635e-118">Пројекат пута суфинансирају две општине.</span><span class="sxs-lookup"><span data-stu-id="2635e-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="2635e-119">Пројект моста финансира се из државних грантова и приватне корпорације.</span><span class="sxs-lookup"><span data-stu-id="2635e-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="2635e-120">У услузи Dynamics 365 Finance, можете да поделите наплату за једну трансакцију или цео пројекат између више клијената, грантова или организација.</span><span class="sxs-lookup"><span data-stu-id="2635e-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="2635e-121">У пројектима који имају више донатора, све стране које доприносе финансирању напредног пројекта финансирања називају се изворима финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="2635e-122">Након што се клијент, организација или грант дефинише као извор финансирања, може се доделити једном или више правила финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="2635e-123">Правила финансирања садрже критеријуме који одређују начин на који се трошкови додељују различитим изворима финансирања за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2635e-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="2635e-124">Будући да се залихе ставки, попут оних које се појављују у захтевима за куповину и поруџбеницама, не могу поделити, износ трошкова не може се поделити између више извора финансирања у тренутку дистрибуције.</span><span class="sxs-lookup"><span data-stu-id="2635e-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="2635e-125">Стога, вредност извора финансирања остаје 0 (нула) док се проблем са инвентаром не прокњижи.</span><span class="sxs-lookup"><span data-stu-id="2635e-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="2635e-126">Када се проблем са инвентаром прокњижи, износ трошкова се распоређује према правилима расподеле рачуна за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2635e-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="2635e-127">Ево неких корака које можете предузети да бисте олакшали поделу наплате између више извора финансирања:</span><span class="sxs-lookup"><span data-stu-id="2635e-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="2635e-128">Наведите да све трансакције које се уносе за пројекат користе исту валуту продаје као и уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="2635e-129">Поставите ограничења финансирања, тако да извор финансирања не фактурише више од одређеног износа за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2635e-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="2635e-130">Конфигуришите правила финансирања и ограничења финансирања за сваког радника, ставку, категорију, групу категорија и врсту трансакције (или за све врсте трансакција).</span><span class="sxs-lookup"><span data-stu-id="2635e-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="2635e-131">Изаберите необавезне датуме почетка и завршетка да бисте дефинисали период када важи свако правило финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="2635e-132">Наведите проценат за који је одговоран сваки извор финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="2635e-133">Наведите који је извор финансирања одговоран за заокруживање разлика узрокованих прорачунима доделе средстава.</span><span class="sxs-lookup"><span data-stu-id="2635e-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="2635e-134">Поставите правила која одређују како ће се трошкови пројекта фактурисати спољним клијентима, а наплаћивати интерним организацијама.</span><span class="sxs-lookup"><span data-stu-id="2635e-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="2635e-135">Евидентирајте трансакције на рачуну за финансирање на чекању док не буде могуће добити додатна средства или док не одлучите да сносите трошкове интерно.</span><span class="sxs-lookup"><span data-stu-id="2635e-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="2635e-136">Да би се утврдило коју пореску групу треба повезати са трансакцијом, у пројекту се тражи додељивање пореске групе.</span><span class="sxs-lookup"><span data-stu-id="2635e-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="2635e-137">Ако на нивоу пројекта није извршено додељивање пореске групе, претражује се уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="2635e-138">Пример: Више извора финансирања (једноставно)</span><span class="sxs-lookup"><span data-stu-id="2635e-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="2635e-139">Следећа табела даје сценарије за управљање расподелом средстава између више извора финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="2635e-140">Ови сценарији засновани су на следећим претпоставкама:</span><span class="sxs-lookup"><span data-stu-id="2635e-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="2635e-141">Поставке приоритета узимају се у обзир у расподели средстава пре него што се примене други критеријуми правила финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="2635e-142">Није наведен ниједан датумски период који би дефинисао период од када важи правило финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2635e-143"><strong>Сценарио</strong></span><span class="sxs-lookup"><span data-stu-id="2635e-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="2635e-144"><strong>Извор финансирања</strong></span><span class="sxs-lookup"><span data-stu-id="2635e-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="2635e-145"><strong>Проценат доделе</strong></span><span class="sxs-lookup"><span data-stu-id="2635e-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="2635e-146"><strong>Приоритет доделе</strong></span><span class="sxs-lookup"><span data-stu-id="2635e-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2635e-147">Желите да доделите трошкове једном извору финансирања док се његова средства не исцрпе, доделите трошкове другом извору финансирања док се његова средства не исцрпе и коначно доделите преостале трошкове трећем извору финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="2635e-148">Извор　финансирања　1</span><span class="sxs-lookup"><span data-stu-id="2635e-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="2635e-149">Извор　финансирања　2</span><span class="sxs-lookup"><span data-stu-id="2635e-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="2635e-150">Извор　финансирања　3</span><span class="sxs-lookup"><span data-stu-id="2635e-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-151">100%</span><span class="sxs-lookup"><span data-stu-id="2635e-151">100%</span></span></li>
<li><span data-ttu-id="2635e-152">100%</span><span class="sxs-lookup"><span data-stu-id="2635e-152">100%</span></span></li>
<li><span data-ttu-id="2635e-153">100%</span><span class="sxs-lookup"><span data-stu-id="2635e-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-154">1</span><span class="sxs-lookup"><span data-stu-id="2635e-154">1</span></span></li>
<li><span data-ttu-id="2635e-155">2</span><span class="sxs-lookup"><span data-stu-id="2635e-155">2</span></span></li>
<li><span data-ttu-id="2635e-156">3</span><span class="sxs-lookup"><span data-stu-id="2635e-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2635e-157">Желите да доделите 75 процената трошкова једном извору финансирања, а 25 процената другом извору финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="2635e-158">Када се исцрпи било који од тих извора финансирања, преостале трошкове желите да платите из трећег извора финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="2635e-159">Извор　финансирања　1</span><span class="sxs-lookup"><span data-stu-id="2635e-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="2635e-160">Извор　финансирања　2</span><span class="sxs-lookup"><span data-stu-id="2635e-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="2635e-161">Извор　финансирања　3</span><span class="sxs-lookup"><span data-stu-id="2635e-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-162">75%</span><span class="sxs-lookup"><span data-stu-id="2635e-162">75%</span></span></li>
<li><span data-ttu-id="2635e-163">25%</span><span class="sxs-lookup"><span data-stu-id="2635e-163">25%</span></span></li>
<li><span data-ttu-id="2635e-164">100%</span><span class="sxs-lookup"><span data-stu-id="2635e-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-165">1</span><span class="sxs-lookup"><span data-stu-id="2635e-165">1</span></span></li>
<li><span data-ttu-id="2635e-166">1</span><span class="sxs-lookup"><span data-stu-id="2635e-166">1</span></span></li>
<li><span data-ttu-id="2635e-167">2</span><span class="sxs-lookup"><span data-stu-id="2635e-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2635e-168">Желите да доделите 75 процената трошкова једном извору финансирања, а 25 процената другом извору финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="2635e-169">Када се исцрпи било који од тих извора финансирања, преостале трошкове желите да поделите између трећег и четвртог извора финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="2635e-170">Извор　финансирања　1</span><span class="sxs-lookup"><span data-stu-id="2635e-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="2635e-171">Извор　финансирања　2</span><span class="sxs-lookup"><span data-stu-id="2635e-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="2635e-172">Извор　финансирања　3</span><span class="sxs-lookup"><span data-stu-id="2635e-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="2635e-173">Извор　финансирања　4</span><span class="sxs-lookup"><span data-stu-id="2635e-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-174">75%</span><span class="sxs-lookup"><span data-stu-id="2635e-174">75%</span></span></li>
<li><span data-ttu-id="2635e-175">25%</span><span class="sxs-lookup"><span data-stu-id="2635e-175">25%</span></span></li>
<li><span data-ttu-id="2635e-176">50%</span><span class="sxs-lookup"><span data-stu-id="2635e-176">50%</span></span></li>
<li><span data-ttu-id="2635e-177">50%</span><span class="sxs-lookup"><span data-stu-id="2635e-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-178">1</span><span class="sxs-lookup"><span data-stu-id="2635e-178">1</span></span></li>
<li><span data-ttu-id="2635e-179">1</span><span class="sxs-lookup"><span data-stu-id="2635e-179">1</span></span></li>
<li><span data-ttu-id="2635e-180">2</span><span class="sxs-lookup"><span data-stu-id="2635e-180">2</span></span></li>
<li><span data-ttu-id="2635e-181">2</span><span class="sxs-lookup"><span data-stu-id="2635e-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2635e-182">Желите да доделите првих 25 процената трошкова једном извору финансирања, а остатак другом извору финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="2635e-183">Извор　финансирања　1</span><span class="sxs-lookup"><span data-stu-id="2635e-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="2635e-184">Извор　финансирања　2</span><span class="sxs-lookup"><span data-stu-id="2635e-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-185">25%</span><span class="sxs-lookup"><span data-stu-id="2635e-185">25%</span></span></li>
<li><span data-ttu-id="2635e-186">100%</span><span class="sxs-lookup"><span data-stu-id="2635e-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="2635e-187">1</span><span class="sxs-lookup"><span data-stu-id="2635e-187">1</span></span></li>
<li><span data-ttu-id="2635e-188">2</span><span class="sxs-lookup"><span data-stu-id="2635e-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="2635e-189">Пример: Више извора финансирања (сложено)</span><span class="sxs-lookup"><span data-stu-id="2635e-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="2635e-190">Имате три извора финансирања која желите да користите по следећем редоследу:</span><span class="sxs-lookup"><span data-stu-id="2635e-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="2635e-191">Користите извор финансирања 2 и извор 3 једнако док се извор 2 не исцрпи.</span><span class="sxs-lookup"><span data-stu-id="2635e-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="2635e-192">Настављате да користите извор финансирања 3 док се не исцрпи.</span><span class="sxs-lookup"><span data-stu-id="2635e-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="2635e-193">Користите извор финансирања 1 након што се извор 3 исцрпи.</span><span class="sxs-lookup"><span data-stu-id="2635e-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="2635e-194">Да бисте постигли тај циљ, прво морате да урадите следеће:</span><span class="sxs-lookup"><span data-stu-id="2635e-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="2635e-195">Поставите ограничења финансирања за извор финансирања 2 и извор финансирања 3, за њихове одговарајуће износе.</span><span class="sxs-lookup"><span data-stu-id="2635e-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="2635e-196">Креирајте следећа правила финансирања:</span><span class="sxs-lookup"><span data-stu-id="2635e-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="2635e-197">Правило 1 (Приоритет 1): Додели 50 процената трансакција извору финансирања 2 и 50 процента извору финансирања 3.</span><span class="sxs-lookup"><span data-stu-id="2635e-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="2635e-198">Правило 2 (Приоритет 2): Додели 100% трансакција извору финансирања 3.</span><span class="sxs-lookup"><span data-stu-id="2635e-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="2635e-199">Правило 3 (Приоритет 3): Додели 100% трансакција извору финансирања 1.</span><span class="sxs-lookup"><span data-stu-id="2635e-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="2635e-200">Ово подешавање функционише јер се проверава да ли трансакције поштују правила и ограничења како би се утврдило да ли се неко од њих односи на трансакцију.</span><span class="sxs-lookup"><span data-stu-id="2635e-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="2635e-201">Ако се на трансакцију не примењују посебна правила или ограничења, примењује се правило Све трансакције.</span><span class="sxs-lookup"><span data-stu-id="2635e-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="2635e-202">Правило Све трансакције подудара се са свим трансакцијама.</span><span class="sxs-lookup"><span data-stu-id="2635e-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="2635e-203">Ако се пронађе правило које се подудара са трансакцијом, прво се примењује проценат који је додељен у том правилу, али тек након што се подударања провере према било којим ограничењима која су постављена.</span><span class="sxs-lookup"><span data-stu-id="2635e-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="2635e-204">Ако је ограничење испуњено, а средства извора финансирања су исцрпљена, правило финансирања које је повезано са ограничењем финансирања се занемарује, а програм проверава следеће правило које се примењује.</span><span class="sxs-lookup"><span data-stu-id="2635e-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="2635e-205">У неким случајевима, само део трансакције може бити додељен по правилу.</span><span class="sxs-lookup"><span data-stu-id="2635e-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="2635e-206">То се може догодити јер се достигне ограничење када се трансакција додели.</span><span class="sxs-lookup"><span data-stu-id="2635e-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="2635e-207">У овом случају, само се одређени износ додељује према том правилу, попут 50 процената за сваки извор финансирања.</span><span class="sxs-lookup"><span data-stu-id="2635e-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="2635e-208">То је случај у правилу 1, које је описано раније у овом одељку.</span><span class="sxs-lookup"><span data-stu-id="2635e-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="2635e-209">Остатак се додељује према следећем правилу у низу.</span><span class="sxs-lookup"><span data-stu-id="2635e-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="2635e-210">Следећа табела детаљније испитује овај сценарио.</span><span class="sxs-lookup"><span data-stu-id="2635e-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2635e-211"><strong>Фокус</strong></span><span class="sxs-lookup"><span data-stu-id="2635e-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="2635e-212"><strong>Детаљи</strong></span><span class="sxs-lookup"><span data-stu-id="2635e-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2635e-213">Правила финансирања</span><span class="sxs-lookup"><span data-stu-id="2635e-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="2635e-214">Правило 1 (Приоритет 1): Све трансакције.</span><span class="sxs-lookup"><span data-stu-id="2635e-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="2635e-215">Додели извор финансирања 2 са 50% и извор финансирања 3 са 50%.</span><span class="sxs-lookup"><span data-stu-id="2635e-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="2635e-216">Правило 2 (Приоритет 2): Све трансакције.</span><span class="sxs-lookup"><span data-stu-id="2635e-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="2635e-217">Издвој извор финансирања 3 на 100%.</span><span class="sxs-lookup"><span data-stu-id="2635e-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="2635e-218">Правило 3 (Приоритет 2): Све трансакције.</span><span class="sxs-lookup"><span data-stu-id="2635e-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="2635e-219">Издвој извор финансирања 1 на 100%.</span><span class="sxs-lookup"><span data-stu-id="2635e-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2635e-220">Ограничења финансирања</span><span class="sxs-lookup"><span data-stu-id="2635e-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="2635e-221">Ограничење извора финансирања 1 = 10.000,00</span><span class="sxs-lookup"><span data-stu-id="2635e-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="2635e-222">Ограничење извора финансирања 2 = 500,00</span><span class="sxs-lookup"><span data-stu-id="2635e-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="2635e-223">Ограничење извора финансирања 3 = 750,00</span><span class="sxs-lookup"><span data-stu-id="2635e-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2635e-224">Трансакција 1</span><span class="sxs-lookup"><span data-stu-id="2635e-224">Transaction 1</span></span></td>
<td><span data-ttu-id="2635e-225"><strong>Износ трансакције:</strong> 100,00<strong>Финансирање:</strong> Трансакција се плаћа само према правилу 1, јер се трансакција у потпуности плаћа након примене правила 1.</span><span class="sxs-lookup"><span data-stu-id="2635e-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="2635e-226">Трансакција се финансира на једнак начин између извора финансирања 2 и извора финансирања 3.</span><span class="sxs-lookup"><span data-stu-id="2635e-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="2635e-227">Извор финансирања 2: 50,00</span><span class="sxs-lookup"><span data-stu-id="2635e-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="2635e-228">Извор финансирања 3: 50,00</span><span class="sxs-lookup"><span data-stu-id="2635e-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2635e-229">Трансакција 2</span><span class="sxs-lookup"><span data-stu-id="2635e-229">Transaction 2</span></span></td>
<td><span data-ttu-id="2635e-230"><strong>Износ трансакције:</strong> 5.000,00<strong>Финансирање:</strong> Трансакција се плаћа према сва три правила.</span><span class="sxs-lookup"><span data-stu-id="2635e-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="2635e-231"><strong>Правило 1</strong>
</span><span class="sxs-lookup"><span data-stu-id="2635e-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="2635e-232">Извор финансирања 2: 450,00</span><span class="sxs-lookup"><span data-stu-id="2635e-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="2635e-233">Извор финансирања 3: 450,00</span><span class="sxs-lookup"><span data-stu-id="2635e-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="2635e-234">
<strong>Правило 2</strong>
</span><span class="sxs-lookup"><span data-stu-id="2635e-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="2635e-235">Извор финансирања 3: 250,00 (= 750,00 – 50,00 – 450,00)</span><span class="sxs-lookup"><span data-stu-id="2635e-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="2635e-236">
<strong>Правило 3</strong>
</span><span class="sxs-lookup"><span data-stu-id="2635e-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="2635e-237">Извор финансирања 1: 3.850,00 (= 5.000,00 – 450,00 – 450,00 – 250,00)</span><span class="sxs-lookup"><span data-stu-id="2635e-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2635e-238">Укупна средства која се распоређују за сваки извор финансирања</span><span class="sxs-lookup"><span data-stu-id="2635e-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="2635e-239">Извор финансирања 1: 3.850,00</span><span class="sxs-lookup"><span data-stu-id="2635e-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="2635e-240">Извор финансирања 2: 500,00</span><span class="sxs-lookup"><span data-stu-id="2635e-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="2635e-241">Извор финансирања 3: 750,00</span><span class="sxs-lookup"><span data-stu-id="2635e-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="2635e-242">Правила за наплате</span><span class="sxs-lookup"><span data-stu-id="2635e-242">Billing rules</span></span>
<span data-ttu-id="2635e-243">Када преговарате о уговору о пројекту са клијентом, ви дефинишете како и када можете фактурисати клијенту за рад на пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="2635e-244">Након што поставите уговор о пројекту и пројекат, можете поставити правила наплате за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2635e-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="2635e-245">Правила за наплате заснивају се на условима пројекта који су наведени у уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="2635e-246">Правила за наплату која можете креирати зависе од услова уговора о пројекту и врсте пројекта, као што су време и материјал или фиксна цена, које повезујете са правилом за наплату.</span><span class="sxs-lookup"><span data-stu-id="2635e-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="2635e-247">За уговор о пројекту можете креирати више правила за наплату.</span><span class="sxs-lookup"><span data-stu-id="2635e-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="2635e-248">Правило наплате можете доделити и више за пројеката који су повезани са истим уговором о пројекту и имају сличне услове наплате.</span><span class="sxs-lookup"><span data-stu-id="2635e-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="2635e-249">Можете да подесите следеће врсте наплате:</span><span class="sxs-lookup"><span data-stu-id="2635e-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="2635e-250">**Јединица испоруке** – Фактуришите клијенту када завршите јединицу испоруке.</span><span class="sxs-lookup"><span data-stu-id="2635e-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="2635e-251">Јединице испоруке дефинишете у уговору.</span><span class="sxs-lookup"><span data-stu-id="2635e-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="2635e-252">**Напредак** – Фактуришите клијенту када завршите одређени проценат пројекта.</span><span class="sxs-lookup"><span data-stu-id="2635e-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="2635e-253">Можете да подесите правило наплате тако да аутоматски израчунава проценат обављеног посла или можете ручно да израчунате проценат завршеног посла и износ за фактурисање клијенту.</span><span class="sxs-lookup"><span data-stu-id="2635e-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="2635e-254">**Контролна тачка** – Фактуришите клијенту пуни износ контролне тачке пројекта када та контролна тачка буде достигнута.</span><span class="sxs-lookup"><span data-stu-id="2635e-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="2635e-255">**Накнада** – Фактуришите клијенту за ваше услуге плус накнаду за управљање, која је обично проценат трошкова услуга.</span><span class="sxs-lookup"><span data-stu-id="2635e-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="2635e-256">**Време и материјал** – Фактуришите клијенту за вредност времена и материјала који се користе на пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="2635e-257">За све врсте правила наплате, можете одредити проценат задржавања који се одузима од фактура клијента док пројекат не достигне неку договорену фазу.</span><span class="sxs-lookup"><span data-stu-id="2635e-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="2635e-258">Проценат задржавања плаћања се наводи у уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="2635e-259">Износ се израчунава на основу и одузима од укупне вредности линија у фактури клијента.</span><span class="sxs-lookup"><span data-stu-id="2635e-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="2635e-260">За правила обрачуна **Време и материјал** и **Напредак**, можете доделити наплативе категорије.</span><span class="sxs-lookup"><span data-stu-id="2635e-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="2635e-261">Наплативе категорије означавају трансакције које треба да буду укључене у фактуре клијената.</span><span class="sxs-lookup"><span data-stu-id="2635e-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="2635e-262">Када будете спремни да фактуришете клијенту, износ фактуре за пројекат се израчунава на основу правила наплате и генерише се предлог фактуре за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2635e-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="2635e-263">Следећи одељци пружају примере који показују како се постављају правила наплате за пројекат и њима управља.</span><span class="sxs-lookup"><span data-stu-id="2635e-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="2635e-264">Пример: Креирајте правило наплате које се заснива на броју испоручених јединица</span><span class="sxs-lookup"><span data-stu-id="2635e-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="2635e-265">Ваша организација закључује уговор о пружању укупно пет обука запосленима по цени од 10.000 по сесији.</span><span class="sxs-lookup"><span data-stu-id="2635e-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="2635e-266">Клијенту фактуришете након сваке сесије обуке.</span><span class="sxs-lookup"><span data-stu-id="2635e-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="2635e-267">Када поставите правила наплате за уговор, користите следеће вредности:</span><span class="sxs-lookup"><span data-stu-id="2635e-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="2635e-268">Јединица испоруке је једна сесија обуке.</span><span class="sxs-lookup"><span data-stu-id="2635e-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="2635e-269">Јединична цена је 10.000 по сесији обуке.</span><span class="sxs-lookup"><span data-stu-id="2635e-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="2635e-270">Укупан број јединица је пет сесија обуке.</span><span class="sxs-lookup"><span data-stu-id="2635e-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="2635e-271">Када завршите једну сесију обуке, можете да направите фактуру за 10.000 за прву испоручену јединицу и пошаљите фактуру клијенту.</span><span class="sxs-lookup"><span data-stu-id="2635e-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="2635e-272">Пример: Креирајте правило наплате које се заснива на одређеном проценту завршетка пројекта (ручни прорачун)</span><span class="sxs-lookup"><span data-stu-id="2635e-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="2635e-273">Ваша организација, фирма за софтверско саветовање, склапа уговор са клијентом о развоју дела производа који клијент развија.</span><span class="sxs-lookup"><span data-stu-id="2635e-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="2635e-274">Ваша организација пристаје на испоруку софтверског кода у периоду од шест месеци.</span><span class="sxs-lookup"><span data-stu-id="2635e-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="2635e-275">Клијент се слаже да ће вашој организацији платити укупно 100.000 за рад.</span><span class="sxs-lookup"><span data-stu-id="2635e-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="2635e-276">Правило наплате креирате да бисте фактурисали клијенту на основу процента посла који је завршен на пројекту, како је наведено у уговору.</span><span class="sxs-lookup"><span data-stu-id="2635e-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="2635e-277">На крају првог месеца, састајете се са клијентом да бисте утврдили проценат обављеног посла.</span><span class="sxs-lookup"><span data-stu-id="2635e-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="2635e-278">Након што ви и клијент прегледате пројекат, одлучујете да је пројекат завршен 15 посто.</span><span class="sxs-lookup"><span data-stu-id="2635e-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="2635e-279">Креирате фактуру на 15.000 (15 процента од 100.000) и шаљете је клијенту.</span><span class="sxs-lookup"><span data-stu-id="2635e-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="2635e-280">Пример: Креирајте правило наплате које се заснива на одређеном проценту завршетка пројекта (аутоматски прорачун)</span><span class="sxs-lookup"><span data-stu-id="2635e-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="2635e-281">Ваша организација, фирма за развој софтвера, пристаје да развије пакет обрачуна зарада за клијента по цени од 30.000.</span><span class="sxs-lookup"><span data-stu-id="2635e-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="2635e-282">Клијент се слаже да ће вашој организацији платити на основу процента завршеног посла.</span><span class="sxs-lookup"><span data-stu-id="2635e-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="2635e-283">Процењујете да трошкови пројекта износе 20.000.</span><span class="sxs-lookup"><span data-stu-id="2635e-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="2635e-284">Уговор о пројекту наводи категорије посла које користите у поступку наплате.</span><span class="sxs-lookup"><span data-stu-id="2635e-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="2635e-285">Постављате правила наплате која аутоматски израчунавају износе фактура за проценат завршеног посла за сваку категорију.</span><span class="sxs-lookup"><span data-stu-id="2635e-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="2635e-286">Подесили сте буџет за сваку категорију:</span><span class="sxs-lookup"><span data-stu-id="2635e-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="2635e-287">**Развој** – Трошак од 15.000 и приход од 20.000</span><span class="sxs-lookup"><span data-stu-id="2635e-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="2635e-288">**Инсталација** – Трошак од 5.000 и приход од 10.000</span><span class="sxs-lookup"><span data-stu-id="2635e-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="2635e-289">Када први пут креирате фактуру клијента, износ фактуре се аутоматски израчунава на основу следећих информација:</span><span class="sxs-lookup"><span data-stu-id="2635e-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="2635e-290">После месец дана, радник на пројекту подноси временски распоред за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2635e-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="2635e-291">Трошкови радних сати радника су 5.000 за развој и 1.000 за инсталацију.</span><span class="sxs-lookup"><span data-stu-id="2635e-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="2635e-292">Развојни радови су завршени 33 процента (5.000 стварних трошкова / 15.000 трошкова буџета), а инсталациони радови су завршени 20 процената (1.000 стварних трошкова / 5.000 трошкова буџета).</span><span class="sxs-lookup"><span data-stu-id="2635e-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="2635e-293">Износ фактуре од 8.667 се аутоматски израчунава (33 процента од 20.000 + 20 процената од 10.000).</span><span class="sxs-lookup"><span data-stu-id="2635e-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="2635e-294">Креирате фактуру на 8.667 и шаљете је клијенту.</span><span class="sxs-lookup"><span data-stu-id="2635e-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="2635e-295">Пример: Креирајте правило наплате које се заснива на договореним контролним тачкама</span><span class="sxs-lookup"><span data-stu-id="2635e-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="2635e-296">Ваша организација, консултантска фирма за менаџмент, пристаје да спроведе истраживање тржишта за потрошачки производ који клијент планира да прода.</span><span class="sxs-lookup"><span data-stu-id="2635e-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="2635e-297">Клијент се слаже да ће користити ваше услуге у периоду од три месеца, почев од марта, и слаже се да ће вашој организацији платити 50.000.</span><span class="sxs-lookup"><span data-stu-id="2635e-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="2635e-298">Пројекат има три контролне тачке:</span><span class="sxs-lookup"><span data-stu-id="2635e-298">The project has three milestones:</span></span>

-   <span data-ttu-id="2635e-299">Контролна тачка 1: Прикупљање података о потрошачима – 31. март</span><span class="sxs-lookup"><span data-stu-id="2635e-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="2635e-300">Контролна тачка 2: Анализа података потрошача – 30. април</span><span class="sxs-lookup"><span data-stu-id="2635e-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="2635e-301">Контролна тачка 3: Представљање предлога одрживости производа – 31. мај</span><span class="sxs-lookup"><span data-stu-id="2635e-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="2635e-302">Клијент се слаже да ће вашој организацији платити 10.000 за прву контролну тачку, 20.000 за другу контролну тачку и 20.000 за трећу контролну тачку.</span><span class="sxs-lookup"><span data-stu-id="2635e-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="2635e-303">Када поставите уговор о пројекту, слажете се да ћете клијенту наплатити на основу контролне тачке која је завршена.</span><span class="sxs-lookup"><span data-stu-id="2635e-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="2635e-304">Постављање правила наплате укључује следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="2635e-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="2635e-305">Дефинишите контролне тачке пројекта.</span><span class="sxs-lookup"><span data-stu-id="2635e-305">Define the project milestones.</span></span>
-   <span data-ttu-id="2635e-306">Дефинишите износ за фактурисање клијенту када се заврши свака контролна тачка.</span><span class="sxs-lookup"><span data-stu-id="2635e-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="2635e-307">Када се прва контролна тачка заврши 31. марта, означите је као испуњену, а затим направите фактуру на износ од 10.000 и пошаљите је клијенту.</span><span class="sxs-lookup"><span data-stu-id="2635e-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="2635e-308">Не можете да креирате фактуру за контролну тачку док је не означите као завршену.</span><span class="sxs-lookup"><span data-stu-id="2635e-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="2635e-309">Пример: Креирајте правило наплате које се заснива на услугама уз накнаду за управљање</span><span class="sxs-lookup"><span data-stu-id="2635e-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="2635e-310">Ваша организација, консултантска фирма за менаџмент, пристаје да спроведе истраживање тржишта како би проценила одрживост производа који клијент, малопродајна компанија, управо развија.</span><span class="sxs-lookup"><span data-stu-id="2635e-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="2635e-311">Услови уговора прецизирају да ћете пружати услуге своја три најбоља саветника за менаџмент, који ће спроводити истраживање на основу времена и материјала.</span><span class="sxs-lookup"><span data-stu-id="2635e-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="2635e-312">Клијент се слаже да плаћа 100 на сат, плус 10 посто накнаде за управљање за консултантске сате који се наплаћују за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2635e-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="2635e-313">Када поставите уговор о пројекту, креирајте правило наплате да бисте додали накнаду од 10% за менаџмент на саветодавне сате који се наплаћују пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="2635e-314">Када креирате фактуру за клијента, њему се наплаћује 10% накнаде за управљање уз трошкове консултантских сати.</span><span class="sxs-lookup"><span data-stu-id="2635e-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="2635e-315">На пример, ако су три консултанта радила укупно 200 сати на пројекту, фактура на износ од 22.000 креира се на основу следећег прорачуна:</span><span class="sxs-lookup"><span data-stu-id="2635e-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="2635e-316">200 сати по 100 на сат = 20.000</span><span class="sxs-lookup"><span data-stu-id="2635e-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="2635e-317">Накнада за менаџмент од 10% = 2.000</span><span class="sxs-lookup"><span data-stu-id="2635e-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="2635e-318">Укупан износ фактуре = 22.000</span><span class="sxs-lookup"><span data-stu-id="2635e-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="2635e-319">Ако су накнаде клијенту опорезиве, а у уговору о пројекту одаберете групу за порез на промет, група пореза на промет аутоматски се уноси у правило наплате накнада.</span><span class="sxs-lookup"><span data-stu-id="2635e-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="2635e-320">Пример: Креирајте правило наплате вредности времена и материјала</span><span class="sxs-lookup"><span data-stu-id="2635e-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="2635e-321">Ваша организација, фирма за софтверско саветовање, пристаје да обезбеди пет техничких консултаната који ће радити на пројекту развоја софтвера за клијента у наредних шест месеци.</span><span class="sxs-lookup"><span data-stu-id="2635e-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="2635e-322">Клијент се слаже да плати 150 за сваки сат консултовања, уз трошкове канцеларијског материјала.</span><span class="sxs-lookup"><span data-stu-id="2635e-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="2635e-323">Ваша организација шаље фактуру клијенту на крају сваког месеца.</span><span class="sxs-lookup"><span data-stu-id="2635e-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="2635e-324">Када постављате уговор о пројекту, сагласни сте да клијенту сваког месеца обрачунавате време и материјале на пројекту.</span><span class="sxs-lookup"><span data-stu-id="2635e-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="2635e-325">Креирате правило наплате које укључује следеће информације:</span><span class="sxs-lookup"><span data-stu-id="2635e-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="2635e-326">Период уговора је шест месеци.</span><span class="sxs-lookup"><span data-stu-id="2635e-326">The contract period is six months.</span></span>
-   <span data-ttu-id="2635e-327">Време консултација израчунава се по цени од 150 на сат.</span><span class="sxs-lookup"><span data-stu-id="2635e-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="2635e-328">Канцеларијски материјал се фактурише по цени коштања, а укупни трошкови пројекта не смеју прећи 10.000.</span><span class="sxs-lookup"><span data-stu-id="2635e-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="2635e-329">Фактуру за клијента креирате на крају сваког календарског месеца током трајања пројекта.</span><span class="sxs-lookup"><span data-stu-id="2635e-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="2635e-330">Током првог месеца, консултанти на пројекту бележе укупно 800 сати.</span><span class="sxs-lookup"><span data-stu-id="2635e-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="2635e-331">Трошкови канцеларијског материјала који се наплаћују за пројекат су 2.000.</span><span class="sxs-lookup"><span data-stu-id="2635e-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="2635e-332">Стога на крају месеца креирате фактуру на износ од 122.000, што је израчунато као 800 сати по 150 на сат, плус 2.000 за канцеларијски материјал.</span><span class="sxs-lookup"><span data-stu-id="2635e-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>





[!INCLUDE[footer-include](../includes/footer-banner.md)]