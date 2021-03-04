---
title: Групе јединица и јединице
description: Ова тема пружа информације о групама јединица и јединицама.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 6620c99563394d1f3881d6bfdb72d01c1c4e8d6f
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145601"
---
# <a name="unit-groups-and-units"></a><span data-ttu-id="a7d56-103">Групе јединица и јединице</span><span class="sxs-lookup"><span data-stu-id="a7d56-103">Unit groups and units</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a7d56-104">Групе јединица и јединице су основни ентитети у систему Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a7d56-104">Unit groups and units are basic entities in Microsoft Dynamics 365.</span></span> <span data-ttu-id="a7d56-105">Јединица је јединица мере, а више јединица може бити груписано у групе јединица.</span><span class="sxs-lookup"><span data-stu-id="a7d56-105">A unit is a single unit of measure, and multiple units can be grouped into unit groups.</span></span> <span data-ttu-id="a7d56-106">Група јединица се понекад зове распоред јединице у Dynamics 365 корисничком систему.</span><span class="sxs-lookup"><span data-stu-id="a7d56-106">A unit group is sometimes referred to as a unit schedule in the Dynamics 365 user interface (UI).</span></span> 

<span data-ttu-id="a7d56-107">Ево неколико примера јединица и група јединица:</span><span class="sxs-lookup"><span data-stu-id="a7d56-107">Here are some examples of units and unit groups:</span></span>
 
- <span data-ttu-id="a7d56-108">**Група јединица**: Раздаљина</span><span class="sxs-lookup"><span data-stu-id="a7d56-108">**Unit group**: Distance</span></span> 
    - <span data-ttu-id="a7d56-109">**Јединице**: Миља, километар итд.</span><span class="sxs-lookup"><span data-stu-id="a7d56-109">**Units**: Mile, Kilometer, and so on.</span></span>
- <span data-ttu-id="a7d56-110">**Група јединица**: Време</span><span class="sxs-lookup"><span data-stu-id="a7d56-110">**Unit group**: Time</span></span>
    - <span data-ttu-id="a7d56-111">**Јединице**: Час, дан, седмица и тако даље.</span><span class="sxs-lookup"><span data-stu-id="a7d56-111">**Units**: Hour, day, week, and so on.</span></span> 

<span data-ttu-id="a7d56-112">Када подесите више јединица у групи јединица, морате подесити и фактор конверзије између њих тако што ћете означити прву јединицу коју сте подесили као подразумевану или примарну јединицу за групу јединица.</span><span class="sxs-lookup"><span data-stu-id="a7d56-112">When you set up multiple units in a unit group, you must also set up a conversion factor between them by designating the first unit that you set up as the default or primary unit for the unit group.</span></span> 

<span data-ttu-id="a7d56-113">На пример, у групи јединица **Време**, ако подесите **Час** као прву јединицу, систем одређује **Час** као подразумевану јединицу.</span><span class="sxs-lookup"><span data-stu-id="a7d56-113">For example, in a **Time** unit group, if you set up **Hour** as the first unit, the system designates **Hour** as the default unit.</span></span> <span data-ttu-id="a7d56-114">Ако је **Дан** следећа јединица коју подесите, морате подесити фактор конверзије за јединицу **Дан** на **Час.**</span><span class="sxs-lookup"><span data-stu-id="a7d56-114">If the next unit that you set up is **Day**, you must set up a conversion factor for **Day** to **Hour**.</span></span> <span data-ttu-id="a7d56-115">Ако затим додате трећу јединицу **Седмица**, морате да подесите фактор конверзије за јединицу **Седмица** у односу на **Дан** или **Час**.</span><span class="sxs-lookup"><span data-stu-id="a7d56-115">If you then add **Week** as a third unit, you must set up a conversion factor for **Week** in terms of **Day** or **Hour**.</span></span> 

<span data-ttu-id="a7d56-116">Следећа слика приказује пример подешавања јединице **Дан**, при чему поље **Количина** приказује број часова у дану, и **Седмица**, где поље **Количина** приказује број дана у недељи.</span><span class="sxs-lookup"><span data-stu-id="a7d56-116">The following image shows an example setup for the **Day** unit, where the **Quantity** field shows the number of hours that are in a day, and **Week**, where the **Quantity** field show the number of days that are in a week.</span></span>

> ![Група јединица: страница са информацијама](media/advanced-2.png)

## <a name="using-units-and-unit-groups"></a><span data-ttu-id="a7d56-118">Коришћење јединица и група јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-118">Using units and unit groups</span></span>

<span data-ttu-id="a7d56-119">Dynamics 365 Project Service Automation користи јединице и групе јединица за обраду процена и ставки за трошкове и време.</span><span class="sxs-lookup"><span data-stu-id="a7d56-119">Dynamics 365 Project Service Automation uses units and unit groups to process estimates and entries for both expenses and time.</span></span> 

<span data-ttu-id="a7d56-120">За трошкове, свака категорија трошка има подразумевану групу јединица и јединицу.</span><span class="sxs-lookup"><span data-stu-id="a7d56-120">For expenses, each expense category has a default unit group and unit.</span></span> <span data-ttu-id="a7d56-121">Ове вредности се уносе као подразумеване вредности у ставкама ценовника за категорије трошкова.</span><span class="sxs-lookup"><span data-stu-id="a7d56-121">These values are entered as default values on price list entries for expense categories.</span></span> 

<span data-ttu-id="a7d56-122">На пример, имате категорију трошка која се зове **Километража**.</span><span class="sxs-lookup"><span data-stu-id="a7d56-122">For example, you have an expense category that is named **Mileage**.</span></span> <span data-ttu-id="a7d56-123">Она има групу јединица под називом **Раздаљина** и подразумевану јединицу која се зове **Километар**.</span><span class="sxs-lookup"><span data-stu-id="a7d56-123">It has a unit group that is named **Distance** and a default unit that is named **Mile**.</span></span> <span data-ttu-id="a7d56-124">Ако подесите групу јединица **Растојање** тако да има две јединице (**Миља** и **Километар**), можете подесити две цене за категорију **Километража** за један ценовник: цена по миљи и цени по километру.</span><span class="sxs-lookup"><span data-stu-id="a7d56-124">If you set up the **Distance** unit group so that it has two units (**Mile** and **Kilometer**), you can set two prices for the **Mileage** category on one price list: price per mile and price per kilometer.</span></span>

| <span data-ttu-id="a7d56-125">Категорија трошка</span><span class="sxs-lookup"><span data-stu-id="a7d56-125">Expense category</span></span>  | <span data-ttu-id="a7d56-126">Група јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-126">Unit group</span></span>  | <span data-ttu-id="a7d56-127">Јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-127">Unit</span></span>      | <span data-ttu-id="a7d56-128">Начин одређивања цена</span><span class="sxs-lookup"><span data-stu-id="a7d56-128">Pricing method</span></span>  | <span data-ttu-id="a7d56-129">Цена по јединици</span><span class="sxs-lookup"><span data-stu-id="a7d56-129">Price per unit</span></span>  |
|-------------------|---------------|-----------|-------------------|-------------------|
| <span data-ttu-id="a7d56-130">Километража</span><span class="sxs-lookup"><span data-stu-id="a7d56-130">Mileage</span></span>           | <span data-ttu-id="a7d56-131">Удаљеност</span><span class="sxs-lookup"><span data-stu-id="a7d56-131">Distance</span></span>      | <span data-ttu-id="a7d56-132">Миља</span><span class="sxs-lookup"><span data-stu-id="a7d56-132">Mile</span></span>      | <span data-ttu-id="a7d56-133">Цена по јединици</span><span class="sxs-lookup"><span data-stu-id="a7d56-133">Price per unit</span></span>    | <span data-ttu-id="a7d56-134">10 USD</span><span class="sxs-lookup"><span data-stu-id="a7d56-134">10 USD</span></span>            |
| <span data-ttu-id="a7d56-135">Километража</span><span class="sxs-lookup"><span data-stu-id="a7d56-135">Mileage</span></span>           | <span data-ttu-id="a7d56-136">Удаљеност</span><span class="sxs-lookup"><span data-stu-id="a7d56-136">Distance</span></span>      | <span data-ttu-id="a7d56-137">Километар</span><span class="sxs-lookup"><span data-stu-id="a7d56-137">Kilometer</span></span> | <span data-ttu-id="a7d56-138">Цена по јединици</span><span class="sxs-lookup"><span data-stu-id="a7d56-138">Price per unit</span></span>    |  <span data-ttu-id="a7d56-139">6 USD</span><span class="sxs-lookup"><span data-stu-id="a7d56-139">6 USD</span></span>            |

<span data-ttu-id="a7d56-140">Када унесете трошак за пројекат, систем одређује цену кроз комбинацију категорије и јединице по трошку.</span><span class="sxs-lookup"><span data-stu-id="a7d56-140">When you enter an expense on a project, the system determines the price through the combination of the category and the unit on the expense.</span></span> 

| <span data-ttu-id="a7d56-141">Опис трошка</span><span class="sxs-lookup"><span data-stu-id="a7d56-141">Expense description</span></span>        | <span data-ttu-id="a7d56-142">Категорија трошка</span><span class="sxs-lookup"><span data-stu-id="a7d56-142">Expense category</span></span>  | <span data-ttu-id="a7d56-143">Јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-143">Unit</span></span>  | <span data-ttu-id="a7d56-144">Количина</span><span class="sxs-lookup"><span data-stu-id="a7d56-144">Quantity</span></span>  | <span data-ttu-id="a7d56-145">Цена по јединици</span><span class="sxs-lookup"><span data-stu-id="a7d56-145">Unit price</span></span>   |
|----------------------------|---------------------|-------|-----------|----------------|
| <span data-ttu-id="a7d56-146">Вожња до локације клијента</span><span class="sxs-lookup"><span data-stu-id="a7d56-146">Drive to client location</span></span> | <span data-ttu-id="a7d56-147">Километража</span><span class="sxs-lookup"><span data-stu-id="a7d56-147">Mileage</span></span>             | <span data-ttu-id="a7d56-148">Миља</span><span class="sxs-lookup"><span data-stu-id="a7d56-148">Mile</span></span>  | <span data-ttu-id="a7d56-149">10</span><span class="sxs-lookup"><span data-stu-id="a7d56-149">10</span></span>        | <span data-ttu-id="a7d56-150">10 USD</span><span class="sxs-lookup"><span data-stu-id="a7d56-150">10 USD</span></span>         |

<span data-ttu-id="a7d56-151">За време, свако заглавље ценовника има поље **Подразумевана јединица за време**.</span><span class="sxs-lookup"><span data-stu-id="a7d56-151">For time, each price list header has a **Default Time Unit** field.</span></span> <span data-ttu-id="a7d56-152">Вредност се подешава када креирате заглавље ценовника.</span><span class="sxs-lookup"><span data-stu-id="a7d56-152">The value is set when you create the price list header.</span></span> <span data-ttu-id="a7d56-153">Ова јединица се затим користи за подешавање свих цена заснованих на улогама у том ценовнику.</span><span class="sxs-lookup"><span data-stu-id="a7d56-153">This unit is then used to set all role-based prices on that price list.</span></span>

<span data-ttu-id="a7d56-154">Ставке процене за поље **Време за понуду** могу се изразити у било којој јединици времена.</span><span class="sxs-lookup"><span data-stu-id="a7d56-154">Estimate lines for the **Time on Quote** field can be expressed in any unit of time.</span></span> <span data-ttu-id="a7d56-155">Међутим, ставке процене у пројектима и ставке времена за пројекте могу да користи само јединицу времена **Час**.</span><span class="sxs-lookup"><span data-stu-id="a7d56-155">However, estimate lines on projects and time entries for projects can use only the **Hour** unit of time.</span></span> <span data-ttu-id="a7d56-156">Ако се јединица у реду "Ставка времена" или "Ставка процене" не подудара са јединицом у реду ценовника за ту улогу, систем конвертује цену у јединице које су дефинисане у процени пројекта или у трансакцији стварних вредности пројекта.</span><span class="sxs-lookup"><span data-stu-id="a7d56-156">If the unit on the time entry or estimate line doesn't match the unit on the price list line for that role, the system converts the price to the units that are defined in the project estimate or the project actual transaction.</span></span>

<span data-ttu-id="a7d56-157">Следећи пример приказује како PSA користи групу јединица, јединице и факторе конверзије.</span><span class="sxs-lookup"><span data-stu-id="a7d56-157">The following example shows how PSA uses the unit group, units, and conversion factors.</span></span>
- <span data-ttu-id="a7d56-158">Јединице</span><span class="sxs-lookup"><span data-stu-id="a7d56-158">Units</span></span>

   - <span data-ttu-id="a7d56-159">**Група јединица**: Време</span><span class="sxs-lookup"><span data-stu-id="a7d56-159">**Unit group**: Time</span></span> 
   - <span data-ttu-id="a7d56-160">**Јединице**: час</span><span class="sxs-lookup"><span data-stu-id="a7d56-160">**Units**: Hour</span></span> 
    
    - <span data-ttu-id="a7d56-161">**Дан** - Фактор конверзије: 8 часова</span><span class="sxs-lookup"><span data-stu-id="a7d56-161">**Day** - Conversion factor: 8 hours</span></span>       
    - <span data-ttu-id="a7d56-162">**Седмица** - Фактор конверзије: 40 часова</span><span class="sxs-lookup"><span data-stu-id="a7d56-162">**Week** - Conversion factor: 40 hours</span></span>  
        
- <span data-ttu-id="a7d56-163">Подешавање ценовника за пројекат А:</span><span class="sxs-lookup"><span data-stu-id="a7d56-163">Price list setup on Project A:</span></span>

    - <span data-ttu-id="a7d56-164">**Назив**: Продајне цене у УК за 2016</span><span class="sxs-lookup"><span data-stu-id="a7d56-164">**Name**: UK sales prices 2016</span></span> 
    - <span data-ttu-id="a7d56-165">**Подразумевана јединица времена**: дан</span><span class="sxs-lookup"><span data-stu-id="a7d56-165">**Default time unit**: Day</span></span> 
    - <span data-ttu-id="a7d56-166">**Валута**: GBP</span><span class="sxs-lookup"><span data-stu-id="a7d56-166">**Currency**: GBP</span></span>

| <span data-ttu-id="a7d56-167">Улога</span><span class="sxs-lookup"><span data-stu-id="a7d56-167">Role</span></span>      | <span data-ttu-id="a7d56-168">Група јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-168">Unit group</span></span> | <span data-ttu-id="a7d56-169">Јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-169">Unit</span></span> | <span data-ttu-id="a7d56-170">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-170">Organizational unit</span></span> | <span data-ttu-id="a7d56-171">Цена</span><span class="sxs-lookup"><span data-stu-id="a7d56-171">Price</span></span>   |
|-----------|------------|------|---------------------|---------|
| <span data-ttu-id="a7d56-172">Програмер</span><span class="sxs-lookup"><span data-stu-id="a7d56-172">Developer</span></span> | <span data-ttu-id="a7d56-173">Time</span><span class="sxs-lookup"><span data-stu-id="a7d56-173">Time</span></span>       | <span data-ttu-id="a7d56-174">Day</span><span class="sxs-lookup"><span data-stu-id="a7d56-174">Day</span></span>  | <span data-ttu-id="a7d56-175">Contoso UK</span><span class="sxs-lookup"><span data-stu-id="a7d56-175">Contoso UK</span></span>          | <span data-ttu-id="a7d56-176">800 GBP</span><span class="sxs-lookup"><span data-stu-id="a7d56-176">800 GBP</span></span> |

### <a name="time-entry"></a><span data-ttu-id="a7d56-177">Ставка времена</span><span class="sxs-lookup"><span data-stu-id="a7d56-177">Time entry</span></span>

<span data-ttu-id="a7d56-178">Следећа табела приказује крајњу трансакцију на страни продаје коју је креирао PSA за тросатни пројекат.</span><span class="sxs-lookup"><span data-stu-id="a7d56-178">The following table shows the resulting sales-side transaction created by PSA for a three hour project.</span></span>


| <span data-ttu-id="a7d56-179">Пројекат</span><span class="sxs-lookup"><span data-stu-id="a7d56-179">Project</span></span>   | <span data-ttu-id="a7d56-180">Задатак</span><span class="sxs-lookup"><span data-stu-id="a7d56-180">Task</span></span>    | <span data-ttu-id="a7d56-181">Улога</span><span class="sxs-lookup"><span data-stu-id="a7d56-181">Role</span></span>      | <span data-ttu-id="a7d56-182">Количина</span><span class="sxs-lookup"><span data-stu-id="a7d56-182">Quantity</span></span> | <span data-ttu-id="a7d56-183">Јединица</span><span class="sxs-lookup"><span data-stu-id="a7d56-183">Unit</span></span>  | <span data-ttu-id="a7d56-184">Цена по јединици</span><span class="sxs-lookup"><span data-stu-id="a7d56-184">Unit price</span></span> | <span data-ttu-id="a7d56-185">Ненаплаћен износ продаје</span><span class="sxs-lookup"><span data-stu-id="a7d56-185">Unbilled sales amount</span></span> |
|-----------|---------|-----------|----------|-------|------------|-----------------------|
| <span data-ttu-id="a7d56-186">Пројекат А</span><span class="sxs-lookup"><span data-stu-id="a7d56-186">Project A</span></span> | <span data-ttu-id="a7d56-187">Дизајн</span><span class="sxs-lookup"><span data-stu-id="a7d56-187">Design</span></span>  | <span data-ttu-id="a7d56-188">Програмер</span><span class="sxs-lookup"><span data-stu-id="a7d56-188">Developer</span></span> | <span data-ttu-id="a7d56-189">3.</span><span class="sxs-lookup"><span data-stu-id="a7d56-189">3</span></span>        | <span data-ttu-id="a7d56-190">Hour</span><span class="sxs-lookup"><span data-stu-id="a7d56-190">Hour</span></span>  | <span data-ttu-id="a7d56-191">100 GBP</span><span class="sxs-lookup"><span data-stu-id="a7d56-191">100 GBP</span></span>    | <span data-ttu-id="a7d56-192">300 GBP</span><span class="sxs-lookup"><span data-stu-id="a7d56-192">300 GBP</span></span>               |

## <a name="time-unit-faq"></a><span data-ttu-id="a7d56-193">Најчешћа питања о јединици времена</span><span class="sxs-lookup"><span data-stu-id="a7d56-193">Time unit FAQ</span></span>

### <a name="does-psa-convert-to-different-units-in-the-case-of-expenses"></a><span data-ttu-id="a7d56-194">Да ли PSA обавља конверзију у различите јединице у случају трошка?</span><span class="sxs-lookup"><span data-stu-id="a7d56-194">Does PSA convert to different units in the case of expenses?</span></span>
<span data-ttu-id="a7d56-195">Не.</span><span class="sxs-lookup"><span data-stu-id="a7d56-195">No.</span></span> <span data-ttu-id="a7d56-196">Конверзија јединице функционише само за време.</span><span class="sxs-lookup"><span data-stu-id="a7d56-196">Unit conversion works only for time.</span></span> <span data-ttu-id="a7d56-197">За трошкове, ако систем не може да пронађе цену за комбинацију категорије трошка и јединице, цена је подразумевано подешена на 0,00.</span><span class="sxs-lookup"><span data-stu-id="a7d56-197">For expenses, if the system can't find a price for the combination of the expense category and unit, the price is set to 0.00 by default.</span></span>

### <a name="why-does-psa-convert-time-units"></a><span data-ttu-id="a7d56-198">Зашто PSA конвертује јединице времена?</span><span class="sxs-lookup"><span data-stu-id="a7d56-198">Why does PSA convert time units?</span></span>
<span data-ttu-id="a7d56-199">У неким земљама или регионима постоји законски услов да се стопе наплате подешавају у данима.</span><span class="sxs-lookup"><span data-stu-id="a7d56-199">In some countries or regions, there is a legal requirement that bill rates be set up in days.</span></span> <span data-ttu-id="a7d56-200">Преговарање око цене и попусти током циклуса понуде се обављају коришћењем дневних цена за сваку улогу коју је могуће наплатити.</span><span class="sxs-lookup"><span data-stu-id="a7d56-200">Price negotiation and discounting during the quote cycle is done by using day rates for each billable role.</span></span> <span data-ttu-id="a7d56-201">Процена распореда и ставке времена се уносе у часовима.</span><span class="sxs-lookup"><span data-stu-id="a7d56-201">Schedule estimation and time entry are done in hours.</span></span> <span data-ttu-id="a7d56-202">Да би подржао ову разлику у јединицама времена, PSA их конвертује.</span><span class="sxs-lookup"><span data-stu-id="a7d56-202">To support this difference in time units, PSA converts time units.</span></span>

### <a name="can-time-units-be-changed-on-project-estimates"></a><span data-ttu-id="a7d56-203">Да ли се јединице времена могу мењати у зависности од процена за пројекат?</span><span class="sxs-lookup"><span data-stu-id="a7d56-203">Can time units be changed on project estimates?</span></span>
<span data-ttu-id="a7d56-204">Не.</span><span class="sxs-lookup"><span data-stu-id="a7d56-204">No.</span></span> <span data-ttu-id="a7d56-205">Процена распореда је тренутно ограничена на часове и не може се променити.</span><span class="sxs-lookup"><span data-stu-id="a7d56-205">Schedule estimation is currently restricted to hours and can’t be changed.</span></span>

### <a name="can-units-and-unit-groups-be-edited-deleted-and-added"></a><span data-ttu-id="a7d56-206">Да ли јединице и групе јединица могу да се уређују, бришу и додају?</span><span class="sxs-lookup"><span data-stu-id="a7d56-206">Can units and unit groups be edited, deleted, and added?</span></span>
<span data-ttu-id="a7d56-207">Да.</span><span class="sxs-lookup"><span data-stu-id="a7d56-207">Yes.</span></span> <span data-ttu-id="a7d56-208">Са изузетком група јединица **Време** и **Час**, све јединице могу да се бришу или уређују и могу да се додају нове јединице.</span><span class="sxs-lookup"><span data-stu-id="a7d56-208">With exception of the **Time** unit group and the **Hour** unit, all units can be deleted or edited, and new units can be added.</span></span> <span data-ttu-id="a7d56-209">У апликацији PSA није могуће избрисати групу јединица **Време** и **Час**.</span><span class="sxs-lookup"><span data-stu-id="a7d56-209">In PSA, the **Time** unit group and the **Hour** unit can't be deleted.</span></span> <span data-ttu-id="a7d56-210">Међутим, оне могу да се ажурирају преведеним текстом за поље **Име**.</span><span class="sxs-lookup"><span data-stu-id="a7d56-210">However, they can be updated with a translated text for the **Name** field.</span></span>
