---
title: Конфигуришите наплативе компоненте ставке понуде
description: Ова тема пружа информације о подешавању наплативих и ненаплативих компонената на линији понуде заснованој на пројекту.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858311"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="c3a2a-103">Конфигуришите наплативе компоненте ставке понуде</span><span class="sxs-lookup"><span data-stu-id="c3a2a-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="c3a2a-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре, Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="c3a2a-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c3a2a-105">Линија понуде заснована на пројекту има концепт *укључених* компоненти и *наплативих* компоненти.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="c3a2a-106">Укључене компоненте подлежу:</span><span class="sxs-lookup"><span data-stu-id="c3a2a-106">Included components are subject to:</span></span>

  - <span data-ttu-id="c3a2a-107">Начину наплате и поделама клијената</span><span class="sxs-lookup"><span data-stu-id="c3a2a-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="c3a2a-108">Ограничења која не смеју да се прекораче</span><span class="sxs-lookup"><span data-stu-id="c3a2a-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="c3a2a-109">Подешавања учесталости фактуре дефинисане у линији понуде засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="c3a2a-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="c3a2a-110">Подскуп укључених компоненти може се означити као наплатив помоћу поља **Тип обрачуна**.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="c3a2a-111">Поље **Тип обрачуна** је скуп опција који омогућава следеће вредности у контексту линије понуде:</span><span class="sxs-lookup"><span data-stu-id="c3a2a-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="c3a2a-112">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-112">Chargeable</span></span>
  - <span data-ttu-id="c3a2a-113">Ненаплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-113">Non-chargeable</span></span>

<span data-ttu-id="c3a2a-114">Компоненте које се наплаћују могу се дефинисати на задацима, улогама и категоријама трансакција.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="c3a2a-115">Наплативост је дефинисана на задацима за линију понуде и односи се на све класе трансакција укључене у ту линију.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="c3a2a-116">Ако је поље **Укључи задатке** празно или постављено на **Читав пројекат**, картица **Задаци који се наплаћују** неће бити доступна.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="c3a2a-117">Наплативост је дефинисана у улогама за линију понуде и односи се само на класу трансакција **Време**.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="c3a2a-118">Ако је поље **Укључи време** постављено на **Не** на линији понуде пројекта, картица **Улоге које се наплаћују** неће бити доступна.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="c3a2a-119">Наплативост је дефинисана у категоријама трансакција за линију понуде и односи се само на класу трансакција **Трошак**.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="c3a2a-120">Ако је поље **Укључи трошкове** постављено на **Не** на линији понуде пројекта, картица **Категорије које се наплаћују** неће бити доступна.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="c3a2a-121">Ажурирајте пројектни задатак тако да буде наплатив или ненаплатив</span><span class="sxs-lookup"><span data-stu-id="c3a2a-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="c3a2a-122">Пројектни задатак може бити наплатив или ненаплатив у контексту одређене линије понуде засноване на пројекту, што омогућава следеће подешавање.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="c3a2a-123">Ако линија понуде заснована на пројекту укључује **Време** и задатак **Т1**, задатак је повезан са линијом понуде као наплатив.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="c3a2a-124">Ако постоји друга линија понуде која укључује **Трошкове**, задатак **Т1** на линији понуде можете повезати као ненаплатив.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="c3a2a-125">Резултат је да је све време евидентирано у задатку наплативо, а сви трошкови евидентирани у задатку ненаплативи.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="c3a2a-126">Тип наплате задатка може се конфигурисати на картици **Наплативи задаци** ставке понуде засноване на пројекту ажурирањем поља **Тип наплате** на подформи **Задаци ставке понуде**.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="c3a2a-127">Поред тога, можете да ажурирате тип наплате за пројектни задатак у пољу **Тип наплате** на подформи задатка Постављање обрачуна пројекта које приказује ставке понуде повезане са задатком.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="c3a2a-128">Ажурирајте улогу да буде наплатива или ненаплатива</span><span class="sxs-lookup"><span data-stu-id="c3a2a-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="c3a2a-129">Улога може бити наплатива или ненаплатива у контексту одређене линије понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="c3a2a-130">Тип наплате улоге се може конфигурисати на картици **Наплативи задаци** ставке понуде засноване на пројекту ажурирањем поља **Тип наплате** на подформи **Задаци ставке понуде**.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="c3a2a-131">Ажурирајте категорију трансакција да буде наплатива или ненаплатива</span><span class="sxs-lookup"><span data-stu-id="c3a2a-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="c3a2a-132">Категорија трансакција може бити наплатива или ненаплатива на одређеној линији понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="c3a2a-133">Тип наплате трансакције се може конфигурисати на картици **Наплативе категорије** ставке понуде засноване на пројекту ажурирањем поља **Тип наплате** на подформи **Наплативе категорије**.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="c3a2a-134">Решите наплативост</span><span class="sxs-lookup"><span data-stu-id="c3a2a-134">Resolve chargeability</span></span>
<span data-ttu-id="c3a2a-135">Процена или стварна вредност креирана за време сматраће се наплативом само ако важи следеће:</span><span class="sxs-lookup"><span data-stu-id="c3a2a-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="c3a2a-136">**Време** је укључено у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="c3a2a-137">**Улога** је конфигурисана као наплатива у ставки понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="c3a2a-138">**Обухваћени задаци** су подешени на вредност **Изабрани задаци** у ставки понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="c3a2a-139">Ако су ове три ствари тачне, **Задатак** се такође конфигурише као наплатив.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="c3a2a-140">Процена или стварна вредност за трошак сматра се наплативом само ако важи следеће:</span><span class="sxs-lookup"><span data-stu-id="c3a2a-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="c3a2a-141">**Трошак** је укључено у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="c3a2a-142">**Категорија трансакције** је конфигурисана као наплатива у ставки понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="c3a2a-143">**Обухваћени задаци** су подешени на вредност **Изабрани задаци** у ставки понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="c3a2a-144">Ако су ове три ствари тачне, **Задатак** се такође конфигурише као наплатив.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="c3a2a-145">Процена или стварна вредност креирана за материјал сматраће се наплативом само ако важи следеће:</span><span class="sxs-lookup"><span data-stu-id="c3a2a-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="c3a2a-146">**Материјали** су укључени у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="c3a2a-147">**Обухваћени задаци** су подешени на вредност **Изабрани задаци** у ставки понуде.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="c3a2a-148">Ако су ове две ствари тачне, **Задатак** би такође требало да се конфигурише као наплатив.</span><span class="sxs-lookup"><span data-stu-id="c3a2a-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-149">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c3a2a-150">
                    <strong>Садржи трошак</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c3a2a-151">
                    <strong>Садржи материјале</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="c3a2a-152">
                    <strong>Обухваћени задаци</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-153">
                    <strong>Улога</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-154">
                    <strong>Категорија</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-155">
                    <strong>Задатак</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="c3a2a-156">
                    <strong>Утицај наплативости</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-157">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-158">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-159">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-160">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="c3a2a-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-161">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-162">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-163">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-164">Обрачун у стварном времену: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-165">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-166">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-167">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-168">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-169">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-170">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c3a2a-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-171">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-172">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-173">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-174">Обрачун у стварном времену: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-175">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-176">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-177">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-178">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-179">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-180">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c3a2a-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-181">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-182">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-183">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-184">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-185">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-186">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-187">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-188">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-189">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-190">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c3a2a-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-191">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-192">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-193">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-194">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-195">Тип обрачуна на стварном трошку: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-196">Тип обрачуна на стварном материјалу: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-197">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-198">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-199">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-200">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c3a2a-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-201">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-202">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-203">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-204">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-205">Тип обрачуна на стварном трошку: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-206">Тип обрачуна на стварном материјалу: <strong> Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-207">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-208">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-209">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-210">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c3a2a-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-211">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-212">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-213">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-214">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-215">Тип обрачуна на стварном трошку: <strong> Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-216">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-218">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-219">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-220">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="c3a2a-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-221">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-222">
                    <strong>Наплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-223">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-224">Обрачун у стварном времену: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-225">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-226">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-228">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-229">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-230">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="c3a2a-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-231">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-232">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-233">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-234">Обрачун у стварном времену: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-235">Тип обрачуна на стварном трошку: <strong> Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-236">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-237">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c3a2a-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-239">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-240">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="c3a2a-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-241">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-242">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-243">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-244">Обрачун у стварном времену: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-245">Тип обрачуна на стварном трошку: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-246">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-247">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c3a2a-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c3a2a-249">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-250">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="c3a2a-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-251">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-252">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-253">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-254">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-255">Тип обрачуна на стварном трошку: <strong>Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-256">Тип обрачуна на стварном материјалу: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-257">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-258">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c3a2a-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-260">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="c3a2a-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-261">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-262">Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-263">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-264">Обрачун у стварном времену: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-265">Тип обрачуна на стварном трошку: Наплативо</span><span class="sxs-lookup"><span data-stu-id="c3a2a-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c3a2a-266">Тип обрачуна на стварном материјалу: <strong> Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c3a2a-267">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c3a2a-268">Да</span><span class="sxs-lookup"><span data-stu-id="c3a2a-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c3a2a-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c3a2a-270">Читав пројекат</span><span class="sxs-lookup"><span data-stu-id="c3a2a-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c3a2a-271">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c3a2a-272">
                    <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c3a2a-273">Не може да се подеси</span><span class="sxs-lookup"><span data-stu-id="c3a2a-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c3a2a-274">Обрачун у стварном времену: <strong>Ненаплативо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-275">Тип обрачуна на стварном трошку:<strong> Ненаплативо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c3a2a-276">Тип обрачуна на стварном материјалу:<strong> Није доступно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c3a2a-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
