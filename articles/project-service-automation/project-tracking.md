---
title: Напредак пројекта и трошкови коришћења
description: Ова тема пружа информације о томе како да пратите напредак пројекта и трошкове коришћења.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755434"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="59ec7-103">Напредак пројекта и трошкови коришћења</span><span class="sxs-lookup"><span data-stu-id="59ec7-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="59ec7-104">Потреба да се прати напредак у односу на распоред разликује се од делатности до делатности.</span><span class="sxs-lookup"><span data-stu-id="59ec7-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="59ec7-105">Неке делатности обављају праћење на најдетаљнијем нивоу, док друге то раде на вишем нивоу.</span><span class="sxs-lookup"><span data-stu-id="59ec7-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="59ec7-106">Ова тема показује како обавити заказивање да бисте испунили потребе своје организације.</span><span class="sxs-lookup"><span data-stu-id="59ec7-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="59ec7-107">Приказ за праћење ангажовања</span><span class="sxs-lookup"><span data-stu-id="59ec7-107">Effort tracking view</span></span>

<span data-ttu-id="59ec7-108">Приказ **Праћење активности** прати напредак задатака у распореду.</span><span class="sxs-lookup"><span data-stu-id="59ec7-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="59ec7-109">Пореди стварно утрошене сате ангажовања на задатку са планираним сатима ангажовања за тај задатак.</span><span class="sxs-lookup"><span data-stu-id="59ec7-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="59ec7-110">PSA користи следеће формуле за израчунавање метрика за праћење:</span><span class="sxs-lookup"><span data-stu-id="59ec7-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="59ec7-111">Проценат напретка = Стварно време ангажовања до данас ÷ Планирано ангажовање за задатак</span><span class="sxs-lookup"><span data-stu-id="59ec7-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="59ec7-112">Процена до завршетка (ETC) = Планирано ангажовање - Стварно време ангажовања до данас</span><span class="sxs-lookup"><span data-stu-id="59ec7-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="59ec7-113">Процена по завршетку (EAC) = Преостало ангаживање + Стварно време ангажовања до данас</span><span class="sxs-lookup"><span data-stu-id="59ec7-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="59ec7-114">Одступање од пројектованог ангажовања = Планирано ангажовање - EAC</span><span class="sxs-lookup"><span data-stu-id="59ec7-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="59ec7-115">PSA приказује пројекцију одступања од ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="59ec7-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="59ec7-116">Ако је EAC већи од планираног ангажовања, предвиђа се да ће задатак одузети више времена него што је првобитно планирано.</span><span class="sxs-lookup"><span data-stu-id="59ec7-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="59ec7-117">Стога, заостаје за планом.</span><span class="sxs-lookup"><span data-stu-id="59ec7-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="59ec7-118">Ако је EAC мањи од планираног ангажовања, предвиђа се да ће задатак одузети мање времена него што је првобитно планирано.</span><span class="sxs-lookup"><span data-stu-id="59ec7-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="59ec7-119">Стога ће бити довршен пре него што је планирано.</span><span class="sxs-lookup"><span data-stu-id="59ec7-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="59ec7-120">Поновно пројектовање ангажовања</span><span class="sxs-lookup"><span data-stu-id="59ec7-120">Re-projecting effort</span></span>

<span data-ttu-id="59ec7-121">Уобичајено је да менаџер пројекта ревидира оригиналне процене задатка.</span><span class="sxs-lookup"><span data-stu-id="59ec7-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="59ec7-122">Поновне пројекције пројеката представљају начин на који менаџер пројекта перципира процене, с обзиром на тренутни статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="59ec7-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="59ec7-123">Међутим, не препоручујемо да менаџери пројекта мењају основне вредности зато што основне вредности пројекта представљају успостављен извор истине за распоред пројекта и процену трошкова, а сви заинтересовани за пројекат су је прихватили.</span><span class="sxs-lookup"><span data-stu-id="59ec7-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="59ec7-124">Постоје два начина на које менаџер пројекта може поново да пројектује ангажовање на задацима:</span><span class="sxs-lookup"><span data-stu-id="59ec7-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="59ec7-125">Измените подразумевани ETC новом проценом стварног преосталог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="59ec7-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="59ec7-126">Измените подразумевани проценат напретка новом проценом стварног напретка задатка.</span><span class="sxs-lookup"><span data-stu-id="59ec7-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="59ec7-127">Сваки од ових приступа доводи до тога да се поново израчунају ETC, EAC и проценат напретка задатка, као и одступање од пројектованог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="59ec7-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="59ec7-128">EAC, ETC и проценат напретка у резимираним задацима такође се поново израчунавају и стварају нову пројекцију одступања од ангажовања.</span><span class="sxs-lookup"><span data-stu-id="59ec7-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="59ec7-129">Поновна пројекција ангажовања за резимиране задатке</span><span class="sxs-lookup"><span data-stu-id="59ec7-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="59ec7-130">Ангажовање на резимираним задацима или задацима контејнера може се поновно пројектовати.</span><span class="sxs-lookup"><span data-stu-id="59ec7-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="59ec7-131">Без обзира да ли корисник поново пројектује помоћу преосталог ангажовања или процента напретка резимираних задатака, започиње следећи низ израчунавања:</span><span class="sxs-lookup"><span data-stu-id="59ec7-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="59ec7-132">EAC, ETC и проценат напретка задатка се израчунавају.</span><span class="sxs-lookup"><span data-stu-id="59ec7-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="59ec7-133">Нови EAC се дистрибуира до надређених задатака у истој пропорцији као и изворни EAC за задатак.</span><span class="sxs-lookup"><span data-stu-id="59ec7-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="59ec7-134">Израчунава се нови EAC за сваки од појединачних задатака све до задатака чвора листа.</span><span class="sxs-lookup"><span data-stu-id="59ec7-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="59ec7-135">Надређени задаци на које ово утиче, све до чворова листа, имају поновно израчунат ETC и проценат напретка на основу EAC вредности.</span><span class="sxs-lookup"><span data-stu-id="59ec7-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="59ec7-136">То резултира новом пројекцијом одступања од ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="59ec7-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="59ec7-137">Поново се израчунавају EAC-ови резимираних задатака све до основног чвора.</span><span class="sxs-lookup"><span data-stu-id="59ec7-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="59ec7-138">Приказ праћења трошкова</span><span class="sxs-lookup"><span data-stu-id="59ec7-138">Cost tracking view</span></span> 

<span data-ttu-id="59ec7-139">Приказ **Праћење трошкова** упоређује стварне трошкове потрошен на задатак и планиране трошкове задатка.</span><span class="sxs-lookup"><span data-stu-id="59ec7-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="59ec7-140">Овај приказ приказује само трошкове рада и не укључује трошкове из процена трошкова.</span><span class="sxs-lookup"><span data-stu-id="59ec7-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="59ec7-141">PSA користи следеће формуле за израчунавање метрика за праћење:</span><span class="sxs-lookup"><span data-stu-id="59ec7-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="59ec7-142">Проценат остварених трошкова = Стварни трошкови до данас ÷ Планирани трошкови задатка</span><span class="sxs-lookup"><span data-stu-id="59ec7-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="59ec7-143">Трошкови до завршетка (CTC) = Планирани трошкови – Стварни трошкови остварени до данас</span><span class="sxs-lookup"><span data-stu-id="59ec7-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="59ec7-144">EAC = CTC + Стварни трошкови остварени до данас</span><span class="sxs-lookup"><span data-stu-id="59ec7-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="59ec7-145">Одступање од пројектованих трошкова = Планирани трошкови - EAC</span><span class="sxs-lookup"><span data-stu-id="59ec7-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="59ec7-146">Пројекција одступања од трошкова је приказана на задатку.</span><span class="sxs-lookup"><span data-stu-id="59ec7-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="59ec7-147">Ако је EAC већи од планираних трошкова, предвиђа се да ће задатак коштати више него што је првобитно планирано.</span><span class="sxs-lookup"><span data-stu-id="59ec7-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="59ec7-148">Због тога има тренд прекорачења буџета.</span><span class="sxs-lookup"><span data-stu-id="59ec7-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="59ec7-149">Ако је EAC мањи од планираних трошкова, предвиђа се да ће задатак коштати мање него што је првобитно планирано.</span><span class="sxs-lookup"><span data-stu-id="59ec7-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="59ec7-150">Због тога има тренд неискоришћеног буџета.</span><span class="sxs-lookup"><span data-stu-id="59ec7-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="59ec7-151">Поновна пројекција трошкова од стране менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="59ec7-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="59ec7-152">Када се ангажовање поново пројектује, CTC, EAC, проценат остварених трошкова и одступања од пројектованих трошкова се поново израчунавају у приказу **Праћење трошкова**.</span><span class="sxs-lookup"><span data-stu-id="59ec7-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="59ec7-153">Резиме статуса пројекта</span><span class="sxs-lookup"><span data-stu-id="59ec7-153">Project status summary</span></span>

<span data-ttu-id="59ec7-154">Подаци за праћење у приказима **Праћење активности** и **Праћење трошкова** приказују напредак и трошкове коришћења на нивоу основног чвора пројекта, резимираних задатака и задатака чворова листа.</span><span class="sxs-lookup"><span data-stu-id="59ec7-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="59ec7-155">Одељак **Статус** на страници **Ентитет пројекта** приказује резиме статуса на нивоу пројекта.</span><span class="sxs-lookup"><span data-stu-id="59ec7-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="59ec7-156">Поља резимеа статуса</span><span class="sxs-lookup"><span data-stu-id="59ec7-156">Status summary fields</span></span>

<span data-ttu-id="59ec7-157">Поље **Општи статус пројекта** је поље које се може уређивати и које показује општи статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="59ec7-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="59ec7-158">Користи кодирање у боји, као што су зелена, жута и црвена, да укаже на повећани ризик.</span><span class="sxs-lookup"><span data-stu-id="59ec7-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="59ec7-159">Поље **Коментари** омогућава менаџеру пројекта да унесе конкретне коментаре о статусу.</span><span class="sxs-lookup"><span data-stu-id="59ec7-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="59ec7-160">Поље **Статус ажуриран дана** није могуће уређивати и вредност је временска ознака која показује када је статус задњи пут ажуриран.</span><span class="sxs-lookup"><span data-stu-id="59ec7-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="59ec7-161">Поља **Перформансе распореда** и **Перформансе трошкова** су подешена од датума праћења.</span><span class="sxs-lookup"><span data-stu-id="59ec7-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="59ec7-162">Када су одступања од распореда и трошкова за основни чвор у приказу **Праћење ангажовања** позитивна, можете подесити ова поља на **Пре плана**.</span><span class="sxs-lookup"><span data-stu-id="59ec7-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="59ec7-163">Када су одступања од распореда и трошкова за основни чвор негативна, можете их подесити на **Заостаје за планом**.</span><span class="sxs-lookup"><span data-stu-id="59ec7-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
