---
title: Напредак пројекта и трошкови коришћења
description: Ова тема пружа информације о праћењу напретка пројекта и трошкова коришћења.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 08/21/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 4fe6adf1a16c1eafc5e37dbd8878dda44cbca230
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009049"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="b3fc8-103">Напредак пројекта и трошкови коришћења</span><span class="sxs-lookup"><span data-stu-id="b3fc8-103">Project progress and cost consumption</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b3fc8-104">Потреба да се прати напредак у односу на распоред разликује се од делатности до делатности.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="b3fc8-105">Неке делатности обављају праћење на најдетаљнијем нивоу, док друге то раде на вишем нивоу.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="b3fc8-106">Ова тема показује како обавити заказивање да бисте испунили потребе своје организације.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="b3fc8-107">Приказ за праћење ангажовања</span><span class="sxs-lookup"><span data-stu-id="b3fc8-107">Effort tracking view</span></span>

<span data-ttu-id="b3fc8-108">Приказ **Праћење активности** прати напредак задатака у распореду.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="b3fc8-109">Приказ пореди стварно утрошене часове ангажовања на задатку према планираним часовима ангажовања за задатак.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-109">It compares the actual effort hours spent on a task to the task's planned effort hours.</span></span> <span data-ttu-id="b3fc8-110">Project Service Automation користи следеће формуле за израчунавање метрика за праћење:</span><span class="sxs-lookup"><span data-stu-id="b3fc8-110">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="b3fc8-111">У почетку на креирању задатка: Планирани трошкови ће бити постављени на процењене трошкове по завршетку.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-111">Initially on the task creation: Planned cost will be set to the Estimated cost at complete.</span></span> <span data-ttu-id="b3fc8-112">Када се стварне вредности евидентирају у задатку, следи израчунавање на основу приказа праћења за ангажовање</span><span class="sxs-lookup"><span data-stu-id="b3fc8-112">Once Actuals are recorded on the task, the following will be calculation on the Tracking view for Effort</span></span>

- <span data-ttu-id="b3fc8-113">Проценат напретка = Стварно време ангажовања до данас ÷ Процена при завршетку (EAC)</span><span class="sxs-lookup"><span data-stu-id="b3fc8-113">Progress percentage = Actual effort spent to date ÷ Estimate at complete (EAC)</span></span> 
- <span data-ttu-id="b3fc8-114">Процена до завршетка (ETC) = Процена при завршетку (EAC) – Стварно време ангажовања до данас</span><span class="sxs-lookup"><span data-stu-id="b3fc8-114">Estimate to complete (ETC) = Estimate at complete (EAC)  – Actual effort spent to date</span></span> 
- <span data-ttu-id="b3fc8-115">EAC = Преостало ангажовање + Стварно време ангажовања до данас</span><span class="sxs-lookup"><span data-stu-id="b3fc8-115">EAC = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="b3fc8-116">Одступање од пројектованог ангажовања = Планирано ангажовање - EAC</span><span class="sxs-lookup"><span data-stu-id="b3fc8-116">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="b3fc8-117">Project Service Automation приказује пројекцију одступања од ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-117">Project Service Automation shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="b3fc8-118">Ако је EAC већи од планираног ангажовања, предвиђа се да ће задатак одузети више времена него што је првобитно планирано.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-118">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="b3fc8-119">Стога, заостаје за планом.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-119">Therefore, it's behind schedule.</span></span> <span data-ttu-id="b3fc8-120">Ако је EAC мањи од планираног ангажовања, предвиђа се да ће задатак одузети мање времена него што је првобитно планирано.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-120">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="b3fc8-121">Стога ће бити довршен пре него што је планирано.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-121">Therefore, it's ahead of schedule.</span></span>

## <a name="reprojecting-effort"></a><span data-ttu-id="b3fc8-122">Поновно пројектовање ангажовања</span><span class="sxs-lookup"><span data-stu-id="b3fc8-122">Reprojecting effort</span></span>

<span data-ttu-id="b3fc8-123">Уобичајено је да менаџер пројекта ревидира оригиналне процене задатка.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-123">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="b3fc8-124">Поновне пројекције пројеката представљају начин на који менаџер пројекта перципира процене, с обзиром на тренутни статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-124">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="b3fc8-125">Међутим, не препоручујемо да менаџери пројекта мењају основне вредности зато што основне вредности пројекта представљају успостављен извор истине за распоред пројекта и процену трошкова, а сви заинтересовани за пројекат су је прихватили.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-125">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="b3fc8-126">Постоје два начина на које менаџер пројекта може поново да пројектује ангажовање на задацима:</span><span class="sxs-lookup"><span data-stu-id="b3fc8-126">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="b3fc8-127">Измените подразумевани ETC новом проценом стварног преосталог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-127">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="b3fc8-128">Измените подразумевани проценат напретка новом проценом стварног напретка задатка.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-128">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="b3fc8-129">Сваки од ових приступа доводи до тога да се поново израчунају ETC, EAC и проценат напретка задатка, као и одступање од пројектованог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-129">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="b3fc8-130">EAC, ETC и проценат напретка у резимираним задацима такође се поново израчунавају и стварају нову пројекцију одступања од ангажовања.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-130">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="reprojection-of-effort-on-summary-tasks"></a><span data-ttu-id="b3fc8-131">Поновна пројекција ангажовања за резимиране задатке</span><span class="sxs-lookup"><span data-stu-id="b3fc8-131">Reprojection of effort on summary tasks</span></span>

<span data-ttu-id="b3fc8-132">Ангажовање на резимираним задацима или задацима контејнера може се поновно пројектовати.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-132">Effort on summary tasks or container tasks can be reprojected.</span></span> <span data-ttu-id="b3fc8-133">Без обзира да ли корисник поново пројектује помоћу преосталог ангажовања или процента напретка резимираних задатака, започиње следећи низ израчунавања:</span><span class="sxs-lookup"><span data-stu-id="b3fc8-133">Regardless of whether the user reprojects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="b3fc8-134">EAC, ETC и проценат напретка задатка се израчунавају.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-134">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="b3fc8-135">Нови EAC се дистрибуира до надређених задатака у истој пропорцији као и изворни EAC за задатак.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-135">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="b3fc8-136">Израчунава се нови EAC за сваки од појединачних задатака све до задатака чвора листа.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-136">The new EAC on each of the individual tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="b3fc8-137">Надређени задаци на које ово утиче, све до чворова листа, имају поновно израчунат ETC и проценат напретка на основу EAC вредности.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-137">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="b3fc8-138">То резултира новом пројекцијом одступања од ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-138">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="b3fc8-139">Поново се израчунавају EAC-ови резимираних задатака све до основног чвора.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-139">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="b3fc8-140">Приказ праћења трошкова</span><span class="sxs-lookup"><span data-stu-id="b3fc8-140">Cost tracking view</span></span> 

<span data-ttu-id="b3fc8-141">Приказ **Праћење трошкова** упоређује стварне трошкове потрошене на задатак и планиране трошкове.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-141">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost.</span></span> 

> [!NOTE]
> <span data-ttu-id="b3fc8-142">Овај приказ приказује само трошкове рада и не укључује трошкове из процена трошкова.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-142">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="b3fc8-143">Project Service Automation користи следеће формуле за израчунавање метрика за праћење:</span><span class="sxs-lookup"><span data-stu-id="b3fc8-143">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="b3fc8-144">Када се креира задатак, планирани трошак једнак је процењеним трошковима при завршетку.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-144">When a task is created, the planned cost is equal to the estimated cost at complete.</span></span> <span data-ttu-id="b3fc8-145">Када се стварне вредности евидентирају у задатку, следеће ће бити израчунато на основу приказа **Праћење** за трошкове:</span><span class="sxs-lookup"><span data-stu-id="b3fc8-145">After actuals are recorded on the task, the following is calculated on the **Tracking** view for cost:</span></span>

 - <span data-ttu-id="b3fc8-146">Проценат остварених трошкова = Стварни трошкови до данас ÷ Процењени трошкови по завршетку за задатак</span><span class="sxs-lookup"><span data-stu-id="b3fc8-146">Percentage of cost consumed = Actual cost spent to date ÷ Estimated cost at complete for the task</span></span>
 - <span data-ttu-id="b3fc8-147">Трошкови до завршетка (CTC) = Процењени трошкови по завршетку – Стварни трошкови остварени до данас</span><span class="sxs-lookup"><span data-stu-id="b3fc8-147">Cost to complete (CTC) = Estimated cost at complete – Actual cost spent to date</span></span>
 - <span data-ttu-id="b3fc8-148">Процењени трошкови по завршетку = CTC + Стварни трошкови остварени до данас</span><span class="sxs-lookup"><span data-stu-id="b3fc8-148">Estimated cost at complete = CTC + Actual cost spent to date</span></span>
 - <span data-ttu-id="b3fc8-149">Предвиђено одступање од трошкова = Планирани трошкови – Процењени трошкови по завршетку</span><span class="sxs-lookup"><span data-stu-id="b3fc8-149">Projected cost variance = Planned cost – Estimated cost at complete</span></span>

<span data-ttu-id="b3fc8-150">Пројекција одступања од трошкова је приказана на задатку.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-150">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="b3fc8-151">Ако су процењени трошкови по завршетку већи од планираних трошкова, предвиђа се да ће задатак коштати више него што је првобитно планирано.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-151">If the estimated cost at complete is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="b3fc8-152">Због тога има тренд прекорачења буџета.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-152">Therefore, it's trending over budget.</span></span> <span data-ttu-id="b3fc8-153">Ако су процењени трошкови по завршетку мањи од планираних трошкова, предвиђа се да ће задатак коштати мање него што је првобитно планирано и да има тренд неискоришћеног буџета.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-153">If the Estimated cost at complete is less than the planned cost, the task is projected to cost less than was originally planned and is trending under budget.</span></span>

## <a name="project-managers-reprojection-of-cost"></a><span data-ttu-id="b3fc8-154">Поновна пројекција трошкова од стране менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="b3fc8-154">Project manager’s reprojection of cost</span></span>

<span data-ttu-id="b3fc8-155">Када се ангажовање поново пројектује, CTC, Процењени трошкови по завршетку, проценат остварених трошкова и одступања од пројектованих трошкова поново се израчунавају у приказу **Праћење трошкова**.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-155">When effort is reprojected, the CTC, Estimated cost at complete, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="b3fc8-156">Резиме статуса пројекта</span><span class="sxs-lookup"><span data-stu-id="b3fc8-156">Project status summary</span></span>

<span data-ttu-id="b3fc8-157">Подаци за праћење у приказима **Праћење активности** и **Праћење трошкова** приказују напредак и трошкове коришћења на нивоу основног чвора пројекта, резимираних задатака и задатака чворова листа.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-157">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="b3fc8-158">Одељак **Статус** на страници **Ентитет пројекта** приказује резиме статуса на нивоу пројекта.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-158">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="b3fc8-159">Поља резимеа статуса</span><span class="sxs-lookup"><span data-stu-id="b3fc8-159">Status summary fields</span></span>

<span data-ttu-id="b3fc8-160">Поље **Општи статус пројекта** је поље које може да се уређује и које показује општи статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-160">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="b3fc8-161">Користи кодирање у боји, као што су зелена, жута и црвена, да укаже на повећани ризик.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-161">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="b3fc8-162">Поље **Коментари** омогућава менаџеру пројекта да унесе конкретне коментаре о статусу.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-162">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="b3fc8-163">Поље **Статус ажуриран дана** није могуће уређивати и вредност је временска ознака која показује када је статус задњи пут ажуриран.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-163">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="b3fc8-164">Поља **Перформансе распореда** и **Перформансе трошкова** су подешена од датума праћења.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-164">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="b3fc8-165">Када су одступања од распореда и трошкова за основни чвор у приказу **Праћење ангажовања** позитивна, можете подесити ова поља на **Пре плана**.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-165">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="b3fc8-166">Када су одступања од распореда и трошкова за основни чвор негативна, можете их подесити на **Заостаје за планом**.</span><span class="sxs-lookup"><span data-stu-id="b3fc8-166">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]