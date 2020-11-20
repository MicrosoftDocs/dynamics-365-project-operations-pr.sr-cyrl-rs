---
title: Опозивање одобрених ставки времена или трошкова
description: Ова тема пружа информације о томе како се опозивају претходно одобрено време или трансакција трошкова.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom: ''
ms.author: rumant
ms.date: 03/08/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 102da39d5940874a8e1f4220437ecdf386a7187b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120561"
---
# <a name="recall-approved-time-or-expense-entries"></a><span data-ttu-id="024ee-103">Опозивање одобрених ставки времена или трошкова</span><span class="sxs-lookup"><span data-stu-id="024ee-103">Recall approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="024ee-104">Члан пројектног тима или друга особа која прослеђује ставку времена или трошкова може је опозвати након што је одобрена.</span><span class="sxs-lookup"><span data-stu-id="024ee-104">A project team member or an other person who submits a time or expense entry can recall that time or expense entry after it has been approved.</span></span> <span data-ttu-id="024ee-105">Процес опозивања одобрене ставке времена или трошкова има два корака:</span><span class="sxs-lookup"><span data-stu-id="024ee-105">The process for recalling an approved time or expense entry has two steps:</span></span>

1. <span data-ttu-id="024ee-106">Подносилац захтева опозивање.</span><span class="sxs-lookup"><span data-stu-id="024ee-106">A submitter requests a recall.</span></span>
2. <span data-ttu-id="024ee-107">Давалац одобрења одобрава опозив.</span><span class="sxs-lookup"><span data-stu-id="024ee-107">An approver approves the recall.</span></span>

## <a name="request-a-recall"></a><span data-ttu-id="024ee-108">Затражите опозивање</span><span class="sxs-lookup"><span data-stu-id="024ee-108">Request a recall</span></span>

<span data-ttu-id="024ee-109">Следите ове кораке да бисте затражили опозивање одобрене ставке времена или трошкова.</span><span class="sxs-lookup"><span data-stu-id="024ee-109">Follow these steps to request a recall of an approved time or expense entry.</span></span>

1. <span data-ttu-id="024ee-110">За ставке времена, идите на **Пројекти** \> **Мој посао** \> **Ставка времена**.</span><span class="sxs-lookup"><span data-stu-id="024ee-110">For time entries, go to **Projects** \> **My Work** \> **Time Entry**.</span></span>

    <span data-ttu-id="024ee-111">–или–</span><span class="sxs-lookup"><span data-stu-id="024ee-111">–or–</span></span>

    <span data-ttu-id="024ee-112">За ставке трошкова, идите на **Пројекти** \> **Мој посао** \> **Трошкови**.</span><span class="sxs-lookup"><span data-stu-id="024ee-112">For expense entries, go to **Projects** \> **My Work** \> **Expenses**.</span></span>

2. <span data-ttu-id="024ee-113">За ставке времена одаберите све ставке за одређену комбинацију пројекта и задатка.</span><span class="sxs-lookup"><span data-stu-id="024ee-113">For time entries, select all the time entries for a specific combination of a project and a task.</span></span> <span data-ttu-id="024ee-114">Алтернативно, у мрежи одаберите појединачне ћелије за време за одређени датум и пројекат.</span><span class="sxs-lookup"><span data-stu-id="024ee-114">Alternatively, in the grid, select the individual cells for time on a specific date for a specific project.</span></span>

    <span data-ttu-id="024ee-115">–или–</span><span class="sxs-lookup"><span data-stu-id="024ee-115">–or–</span></span>

    <span data-ttu-id="024ee-116">За ставке трошкова одаберите ред за ставку трошка да бисте је опозвали.</span><span class="sxs-lookup"><span data-stu-id="024ee-116">For expense entries, select the row for the expense entry to recall.</span></span>

3. <span data-ttu-id="024ee-117">Изаберите **Опозови**.</span><span class="sxs-lookup"><span data-stu-id="024ee-117">Select **Recall**.</span></span> <span data-ttu-id="024ee-118">Појављује се дијалог за потврду.</span><span class="sxs-lookup"><span data-stu-id="024ee-118">A confirmation dialog box appears.</span></span> <span data-ttu-id="024ee-119">Ако су одабране ставке времена и трошкова већ одобрене, од вас ће се тражити да унесете разлог опозива.</span><span class="sxs-lookup"><span data-stu-id="024ee-119">If the selected time and expense entries were already approved, you're prompted to enter a reason for the recall.</span></span>
4. <span data-ttu-id="024ee-120">Унесите разлог опозива, а затим изаберите **У реду** да потврдите операцију.</span><span class="sxs-lookup"><span data-stu-id="024ee-120">Enter a reason for the recall, and then select **OK** to confirm the operation.</span></span> <span data-ttu-id="024ee-121">Систем шаље особи која је одобрила ставке захтев за одобрење опозива.</span><span class="sxs-lookup"><span data-stu-id="024ee-121">The system sends the person who approved the entries a request to approve the recall.</span></span>

> [!NOTE]
> <span data-ttu-id="024ee-122">Иако се одобрене ставке времена и трошкова могу опозвати, ако је одобрено време или трошак већ фактурисан клијенту, захтев за опозив не може да се креира.</span><span class="sxs-lookup"><span data-stu-id="024ee-122">Although approved time and expense entries can be recalled, if an approved time or expense has already been invoiced to the customer, a recall request can't be created.</span></span> <span data-ttu-id="024ee-123">Корисник који покуша да креира захтев за опозив добиће поруку у којој стоји да се време или трошак не могу опозвати јер су већ фактурисани.</span><span class="sxs-lookup"><span data-stu-id="024ee-123">A user who tries to create a recall request will receive a message that states that the time or expense can't be recalled because it was already invoiced.</span></span>

## <a name="approve-or-reject-a-recall-request"></a><span data-ttu-id="024ee-124">Одобравање или одбацивање захтева за опозив</span><span class="sxs-lookup"><span data-stu-id="024ee-124">Approve or reject a recall request</span></span>

<span data-ttu-id="024ee-125">Следите ове кораке да бисте одобрили или одбацили захтев за опозив.</span><span class="sxs-lookup"><span data-stu-id="024ee-125">Follow these steps to approve or reject a recall request.</span></span>

1. <span data-ttu-id="024ee-126">Идите на **Пројекти** \> **Мој посао** \> **Одобрења**.</span><span class="sxs-lookup"><span data-stu-id="024ee-126">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="024ee-127">На страници листе **Одобрења** промените приказ на **Опозови захтеве за одобрења**.</span><span class="sxs-lookup"><span data-stu-id="024ee-127">On the **Approvals** list page, change the view to **Recall requests for approval**.</span></span> <span data-ttu-id="024ee-128">Приказује се листа прослеђених захтева за опозив.</span><span class="sxs-lookup"><span data-stu-id="024ee-128">A list of submitted recall requests is shown.</span></span>
3. <span data-ttu-id="024ee-129">Изаберите једну или више ставки, а затим either **Одобри** или **Одбаци**.</span><span class="sxs-lookup"><span data-stu-id="024ee-129">Select one or more entries, and then select either **Approve** or **Reject**.</span></span>
4. <span data-ttu-id="024ee-130">Ако сте изабрали **Одобри**, добијате поруку упозорења која објашњава ефекат одобрења.</span><span class="sxs-lookup"><span data-stu-id="024ee-130">If you selected **Approve**, you receive a warning message that explains the impact of the approval.</span></span> <span data-ttu-id="024ee-131">Изаберите **У реду** да бисте потврдили операцију.</span><span class="sxs-lookup"><span data-stu-id="024ee-131">Select **OK** to confirm the operation.</span></span> <span data-ttu-id="024ee-132">Захтев за опозив је одобрен.</span><span class="sxs-lookup"><span data-stu-id="024ee-132">The recall request is approved.</span></span>

    <span data-ttu-id="024ee-133">–или–</span><span class="sxs-lookup"><span data-stu-id="024ee-133">–or–</span></span>

    <span data-ttu-id="024ee-134">Ако сте изабрали **Одбаци**, захтев за опозив је одбијен.</span><span class="sxs-lookup"><span data-stu-id="024ee-134">If you selected **Reject**, the recall request is rejected.</span></span>

> [!NOTE]
> <span data-ttu-id="024ee-135">Као и у случају захтевања опозива, када се опозив одобри, систем проверава да ли има било каквих активности фактурисања у ставкама времена или трошкова.</span><span class="sxs-lookup"><span data-stu-id="024ee-135">As when a recall is requested, when a recall is approved, the system checks for any invoicing activity on the time or expense entries.</span></span> <span data-ttu-id="024ee-136">Ако је ставка већ фактурисана или је у радној верзији фактуре, давалац одобрења ће добити поруку о грешци у којој стоји да се опозив времена или трошка не може одобрити јер је већ фактурисан.</span><span class="sxs-lookup"><span data-stu-id="024ee-136">If an entry was already invoiced, or if it's on a draft invoice, the approver will receive an error message that states that the time or expense can't be approved for recall, because it was already invoiced.</span></span>

## <a name="impact-of-a-recall-request"></a><span data-ttu-id="024ee-137">Ефекат захтева за опозив</span><span class="sxs-lookup"><span data-stu-id="024ee-137">Impact of a recall request</span></span>

<span data-ttu-id="024ee-138">Када се одобрење опозове, постоји и оперативни и финансијски утицај.</span><span class="sxs-lookup"><span data-stu-id="024ee-138">When an approval is recalled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="024ee-139">Оперативни утицај</span><span class="sxs-lookup"><span data-stu-id="024ee-139">Operational impact</span></span>

<span data-ttu-id="024ee-140">Ако је захтев за опозив одобрен, запис одобрења означава се као **Одбачен**.</span><span class="sxs-lookup"><span data-stu-id="024ee-140">If a recall request is approved, the approval record is marked as **Rejected**.</span></span> <span data-ttu-id="024ee-141">Статус ставке се мења у **Враћена** или **Одбачена**, у зависности да ли је то ставка времена или трошкова.</span><span class="sxs-lookup"><span data-stu-id="024ee-141">The status of the entry is changed to either **Returned** or **Rejected**, depending on whether it's a time entry or an expense entry.</span></span>

<span data-ttu-id="024ee-142">Члан пројектног тима може прегледати ставке, уређивати и затим поново прослеђивати ставке или их у потпуности брисати.</span><span class="sxs-lookup"><span data-stu-id="024ee-142">The project team member can view entries, edit and then resubmit entries, or delete entries entirely.</span></span>

<span data-ttu-id="024ee-143">Ако се захтев за опозив одбаци, статус ставке остаје **Одобрена** и ставку не може да уређује члан пројектног тима нити давалац одобрења за пројекат.</span><span class="sxs-lookup"><span data-stu-id="024ee-143">If a recall request is rejected, the status of the entry remains **Approved**, and the entry can't be edited by the project team member or the approver for the project.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="024ee-144">Финансијски утицај</span><span class="sxs-lookup"><span data-stu-id="024ee-144">Financial impact</span></span>

<span data-ttu-id="024ee-145">Ако се захтев за опозив одобри, одговарајуће стварне вредности трошкова и продаје се ажурирају на следећи начин:</span><span class="sxs-lookup"><span data-stu-id="024ee-145">If a recall request is approved, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="024ee-146">Поље **Статус поравнања** се ажурира на **Поравнато**.</span><span class="sxs-lookup"><span data-stu-id="024ee-146">The **Adjustment Status** field is updated to **Adjusted**.</span></span>
- <span data-ttu-id="024ee-147">Поље **Статус наплате** се ажурира на **Отказано**.</span><span class="sxs-lookup"><span data-stu-id="024ee-147">The **Billing Status** field is updated to **Canceled**.</span></span>

<span data-ttu-id="024ee-148">Затим, ставке сторнирања се креирају у табели Стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="024ee-148">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="024ee-149">Да би систем креирао ставке сторнирања, копира вредности поља из оригиналних стварних вредности.</span><span class="sxs-lookup"><span data-stu-id="024ee-149">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="024ee-150">Једине вредности које се не копирају су вредности количине.</span><span class="sxs-lookup"><span data-stu-id="024ee-150">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="024ee-151">Уместо тога, ове вредности се сторнирају.</span><span class="sxs-lookup"><span data-stu-id="024ee-151">These values are reversed instead.</span></span> <span data-ttu-id="024ee-152">Сторниране стварне вредности се креирају за стварне вредности **Трошкови** и **Ненаплаћена продаја**.</span><span class="sxs-lookup"><span data-stu-id="024ee-152">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="024ee-153">Поље **Статус поравнања** у сторнираним стварним вредностима је подешено на **Не може да се поравна**, а поље **Статус наплате** на **Отказано**.</span><span class="sxs-lookup"><span data-stu-id="024ee-153">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the **Billing status** field is set to **Canceled**.</span></span> <span data-ttu-id="024ee-154">Због ових измена, евидентирана потрошња за пројекат и преостали приход од пројекта више неће узимати у обзир износе које ове стварне вредности представљају.</span><span class="sxs-lookup"><span data-stu-id="024ee-154">Because of these changes, the recorded spending and the revenue backlog on the project will no longer account for the amounts that these actuals represent.</span></span>

<span data-ttu-id="024ee-155">Ако се захтев за опозив одбаци, нема финансијског утицаја на пројекат.</span><span class="sxs-lookup"><span data-stu-id="024ee-155">If a recall request is rejected, there is no financial impact on the project.</span></span>

## <a name="changes-to-time-entry-records"></a><span data-ttu-id="024ee-156">Промене записа ставке времена</span><span class="sxs-lookup"><span data-stu-id="024ee-156">Changes to time entry records</span></span>

<span data-ttu-id="024ee-157">Следећа илустрација приказује промене које се дешавају за одобрене ставке времена када су опозване.</span><span class="sxs-lookup"><span data-stu-id="024ee-157">The following illustration shows the changes that occur for approved time entries when they are recalled.</span></span>

![Промене статуса ставке времена](media/TimeEntryStateTransitions.png)

## <a name="changes-to-expense-entry-records"></a><span data-ttu-id="024ee-159">Промене записа ставке трошкова</span><span class="sxs-lookup"><span data-stu-id="024ee-159">Changes to expense entry records</span></span>

<span data-ttu-id="024ee-160">Следећа илустрација приказује промене које се дешавају за одобрене ставке трошкова када су опозване.</span><span class="sxs-lookup"><span data-stu-id="024ee-160">The following illustration shows the changes that occur for approved expense entries when they are recalled.</span></span>

![Промене статуса ставке трошкова](media/ExpenseEntryStateTransitions.png)
