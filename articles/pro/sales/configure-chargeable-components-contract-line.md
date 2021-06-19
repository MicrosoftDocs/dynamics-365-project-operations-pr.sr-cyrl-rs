---
title: Конфигурисање наплативих компоненти за предмет уговора заснован на пројекту
description: Ова тема пружа информације о томе како додати наплативе компоненте у предмете уговора у услузи Project Operations.
author: rumant
ms.date: 10/08/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b29c912828aa4af2d2d9cb47869012087cb834b4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003739"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="dece1-103">Конфигурисање наплативих компоненти за предмет уговора заснован на пројекту</span><span class="sxs-lookup"><span data-stu-id="dece1-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="dece1-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре, Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="dece1-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="dece1-105">Предмет уговора заснован на пројекту има *укључене* компоненте и *наплативе* компоненте.</span><span class="sxs-lookup"><span data-stu-id="dece1-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="dece1-106">Укључене компоненте су компоненте које подлежу:</span><span class="sxs-lookup"><span data-stu-id="dece1-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="dece1-107">Начину наплате и поделама клијената</span><span class="sxs-lookup"><span data-stu-id="dece1-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="dece1-108">Ограничења која не смеју да се прекораче</span><span class="sxs-lookup"><span data-stu-id="dece1-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="dece1-109">Поставке учесталости фактуре дефинисане у предмету уговора заснованог на пројекту</span><span class="sxs-lookup"><span data-stu-id="dece1-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="dece1-110">Подскуп укључених компоненти може се означити као наплатив помоћу поља **Тип обрачуна**.</span><span class="sxs-lookup"><span data-stu-id="dece1-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="dece1-111">Поље **Тип обрачуна** је скуп опција који омогућава следеће вредности у контексту предмета уговора:</span><span class="sxs-lookup"><span data-stu-id="dece1-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="dece1-112">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-112">Chargeable</span></span>
  - <span data-ttu-id="dece1-113">Ненаплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-113">Non-chargeable</span></span>

<span data-ttu-id="dece1-114">Компоненте које се наплаћују могу се дефинисати на задацима, улогама и категоријама трансакција.</span><span class="sxs-lookup"><span data-stu-id="dece1-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="dece1-115">Наплативост је дефинисана на задацима за предмет уговора о пројекту и односи се на све класе трансакција укључене у линију.</span><span class="sxs-lookup"><span data-stu-id="dece1-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="dece1-116">Ако је поље **Укључи задатке** на предмету уговора празно или постављено на **Читав пројекат**, картица **Задаци који се наплаћују** неће бити доступна.</span><span class="sxs-lookup"><span data-stu-id="dece1-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="dece1-117">Наплативост дефинисана у улогама за предмет уговора о пројекту односи се само на класу трансакција **Време**.</span><span class="sxs-lookup"><span data-stu-id="dece1-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="dece1-118">Ако је поље **Укључи време** на предмету уговора постављено на **Не**, картица **Улоге које се наплаћују** неће бити доступна.</span><span class="sxs-lookup"><span data-stu-id="dece1-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="dece1-119">Наплативост дефинисана у категоријама трансакција за предмет уговора о пројекту односи се само на класу трансакција **Трошак**.</span><span class="sxs-lookup"><span data-stu-id="dece1-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="dece1-120">Ако је поље **Укључи трошкове** постављено на **Не**, картица **Категорије које се наплаћују** неће бити доступна.</span><span class="sxs-lookup"><span data-stu-id="dece1-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="dece1-121">Ажурирајте пројектни задатак као наплативи или ненаплативи</span><span class="sxs-lookup"><span data-stu-id="dece1-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="dece1-122">Пројектни задатак може бити наплатив или ненаплатив на одређеном предмету уговора, што омогућава следеће подешавање:</span><span class="sxs-lookup"><span data-stu-id="dece1-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="dece1-123">Ако предмет уговора заснован на пројекту укључује **Време** и одређени задатак, **Т1** је повезан са њим као наплатив.</span><span class="sxs-lookup"><span data-stu-id="dece1-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="dece1-124">Ако постоји други предмет уговора који укључује **Трошак**, задатак Т1 на предмету уговора линији можете повезати као ненаплатив.</span><span class="sxs-lookup"><span data-stu-id="dece1-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="dece1-125">Резултат је да је све време евидентирано у задатку наплативо, а сви трошкови ненаплативи.</span><span class="sxs-lookup"><span data-stu-id="dece1-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="dece1-126">Тип наплате задатка може се конфигурисати на картици **Задаци који се наплаћују** предмета уговора ажурирањем поља **Тип наплате** на подформи задатака предмета уговора.</span><span class="sxs-lookup"><span data-stu-id="dece1-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="dece1-127">Поред тога, можете да ажурирате поље **Тип наплате** на подформи задатка Постављање обрачуна пројекта које приказује предмете уговора повезане са задатком.</span><span class="sxs-lookup"><span data-stu-id="dece1-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="dece1-128">Ажурирајте улогу као наплативу или ненаплативу</span><span class="sxs-lookup"><span data-stu-id="dece1-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="dece1-129">Улога може бити наплатива или ненаплатива на одређеном предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="dece1-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="dece1-130">Тип обрачуна улоге може се конфигурисати на картици **Улоге које се наплаћују** предмета уговора.</span><span class="sxs-lookup"><span data-stu-id="dece1-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="dece1-131">Да бисте то урадили, ажурирајте поље **Тип наплате** на подформи **Наплативе улоге**.</span><span class="sxs-lookup"><span data-stu-id="dece1-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="dece1-132">Ажурирајте категорију трансакција као наплативу или ненаплативу</span><span class="sxs-lookup"><span data-stu-id="dece1-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="dece1-133">Категорија трансакција може бити наплатива или ненаплатива на одређеном предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="dece1-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="dece1-134">Тип обрачуна трансакције може се конфигурисати на картици **Категорије које се наплаћују** предмета уговора заснованом на пројекту.</span><span class="sxs-lookup"><span data-stu-id="dece1-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="dece1-135">Да бисте то урадили, ажурирајте поље **Тип наплате** на подформи **Наплативе категорије**.</span><span class="sxs-lookup"><span data-stu-id="dece1-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="dece1-136">Решите наплативост</span><span class="sxs-lookup"><span data-stu-id="dece1-136">Resolve chargeability</span></span>

<span data-ttu-id="dece1-137">Процена или стварна вредност креирана за време сматра се наплативом само ако важи следеће:</span><span class="sxs-lookup"><span data-stu-id="dece1-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="dece1-138">**Време** је укључено у предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="dece1-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="dece1-139">**Улога** је конфигурисана као наплатива у предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="dece1-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="dece1-140">**Обухваћени задаци** су подешени на вредност **Изабрани задаци** у предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="dece1-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="dece1-141">Ако су ове три ствари тачне, задатак се конфигурише као наплатив.</span><span class="sxs-lookup"><span data-stu-id="dece1-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="dece1-142">Процена или стварна вредност за трошак сматра се наплативом само ако важи следеће:</span><span class="sxs-lookup"><span data-stu-id="dece1-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="dece1-143">**Трошак** је укључен у предмет уговора</span><span class="sxs-lookup"><span data-stu-id="dece1-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="dece1-144">**Категорија трансакције** је конфигурисана као наплатива у предмету уговора</span><span class="sxs-lookup"><span data-stu-id="dece1-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="dece1-145">**Обухваћени задаци** су подешени на вредност **Изабрани задатак** у предмету уговора</span><span class="sxs-lookup"><span data-stu-id="dece1-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="dece1-146">Ако су ове три ствари тачне, **Задатак** се конфигурише као наплатив.</span><span class="sxs-lookup"><span data-stu-id="dece1-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="dece1-147">Процена или стварна вредност за материјал сматра се наплативом само ако важи следеће:</span><span class="sxs-lookup"><span data-stu-id="dece1-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="dece1-148">**Материјали** су укључени у предмет уговора</span><span class="sxs-lookup"><span data-stu-id="dece1-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="dece1-149">**Обухваћени задаци** су подешени на вредност **Изабрани задаци** у предмету уговора</span><span class="sxs-lookup"><span data-stu-id="dece1-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="dece1-150">Ако су ове две ствари тачне, **Задатак** се конфигурише као наплатив.</span><span class="sxs-lookup"><span data-stu-id="dece1-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-151">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="dece1-152">
                    <strong>Садржи трошак</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="dece1-153">
                    <strong>Садржи материјале</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="dece1-154">
                    <strong>Обухваћени задаци</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-155">
                    <strong>Улога</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-156">
                    <strong>Категорија</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-157">
                    <strong>Задатак</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="dece1-158">
                    <strong>Утицај наплативости</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-159">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-160">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-161">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-162">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="dece1-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-163">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-164">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-165">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-166">Обрачун у стварном времену: <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-167">Тип обрачуна на стварном трошку: <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-168">Тип обрачуна на стварном материјалу: <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-169">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-170">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-171">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-172">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="dece1-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-173">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-174">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-175">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-176">Обрачун у стварном времену: <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-177">Тип обрачуна на стварном трошку: <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-178">Тип обрачуна на стварном материјалу: <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-179">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-180">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-181">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-182">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="dece1-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-183">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-184">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-185">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-186">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-187">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="dece1-188">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-189">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-190">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-191">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-192">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="dece1-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-193">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-194">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-195">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-196">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-197">Тип обрачуна на стварном трошку: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-198">Тип обрачуна на стварном материјалу: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-199">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-200">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-201">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-202">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="dece1-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-203">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-204">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-205">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-206">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-207">Тип обрачуна на стварном трошку: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-208">Тип обрачуна на стварном материјалу: <strong> Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-209">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-210">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-211">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-212">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="dece1-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-213">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-214">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-215">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-216">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-217">Тип обрачуна на стварном трошку: <strong> Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-218">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-219">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-220">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-221">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-222">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="dece1-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-223">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-224">
                    <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-225">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-226">Обрачун у стварном времену: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-227">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="dece1-228">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-229">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-230">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-231">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-232">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="dece1-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-233">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-234">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-235">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-236">Обрачун у стварном времену: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-237">Тип обрачуна на стварном трошку: <strong> Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-238">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-239">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="dece1-240">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-241">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-242">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="dece1-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-243">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-244">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-245">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-246">Обрачун у стварном времену: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="dece1-247">Тип обрачуна на стварном трошку: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-248">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-249">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="dece1-250">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="dece1-251">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-252">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="dece1-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-253">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-254">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-255">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-256">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-257">Тип обрачуна на стварном трошку: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-258">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-259">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-260">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="dece1-261">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-262">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="dece1-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-263">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-264">Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-265">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-266">Обрачун у стварном времену: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="dece1-267">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="dece1-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="dece1-268">Тип обрачуна на стварном материјалу: <strong> Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="dece1-269">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="dece1-270">Да</span><span class="sxs-lookup"><span data-stu-id="dece1-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="dece1-271">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="dece1-272">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="dece1-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="dece1-273">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="dece1-274">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="dece1-275">Није могуће подесити</span><span class="sxs-lookup"><span data-stu-id="dece1-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="dece1-276">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-277">Тип обрачуна на стварном трошку:<strong> Ненаплативо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="dece1-278">Тип обрачуна на стварном материјалу:<strong> Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dece1-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
