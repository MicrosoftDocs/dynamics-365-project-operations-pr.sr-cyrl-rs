---
title: Отказивање претходно одобрених ставки времена и трошкова
description: Ова тема пружа информације о томе како се отказује одобрено време пројекта и трансакција трошкова.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
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
ms.openlocfilehash: 40ac37c1070e1c4da01e96bbc4248977b2b6d284
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290872"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="a197d-103">Отказивање претходно одобрених ставки времена или трошкова</span><span class="sxs-lookup"><span data-stu-id="a197d-103">Cancel previously approved time or expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a197d-104">У најновијој верзији апликације Dynamics 365 Project Service Automation, даваоци одобрења могу да откажу ставке за време или трошкове које су претходно одобрили.</span><span class="sxs-lookup"><span data-stu-id="a197d-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="a197d-105">Отказивање претходно одобрене ставке времена или трошкова</span><span class="sxs-lookup"><span data-stu-id="a197d-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="a197d-106">Следите ове кораке да бисте отказали ставку времена или трошкова коју сте претходно одобрили.</span><span class="sxs-lookup"><span data-stu-id="a197d-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="a197d-107">Идите на **Пројекти** \> **Мој посао** \> **Одобрења**.</span><span class="sxs-lookup"><span data-stu-id="a197d-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="a197d-108">На страници листе **Одобрења** промените приказ на **Моја прошла одобрења**.</span><span class="sxs-lookup"><span data-stu-id="a197d-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="a197d-109">Приказује се листа ставки времена и трошкова које сте претходно одобрили.</span><span class="sxs-lookup"><span data-stu-id="a197d-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="a197d-110">Изаберите једну или више ставки, а затим **Откажи одобрење**.</span><span class="sxs-lookup"><span data-stu-id="a197d-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="a197d-111">Добићете поруку упозорења.</span><span class="sxs-lookup"><span data-stu-id="a197d-111">You receive a warning message.</span></span>
4. <span data-ttu-id="a197d-112">Да бисте отказали одобрење, изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="a197d-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="a197d-113">Разумевање утицаја отказивања одобрења ставке времена или трошкова</span><span class="sxs-lookup"><span data-stu-id="a197d-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="a197d-114">Када се одобрење откаже, постоји и оперативни и финансијски утицај.</span><span class="sxs-lookup"><span data-stu-id="a197d-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="a197d-115">Оперативни утицај</span><span class="sxs-lookup"><span data-stu-id="a197d-115">Operational impact</span></span>

<span data-ttu-id="a197d-116">Што се тиче операција, када се одобрење откаже, статус записа ће бити враћен на **Радна верзија**, а одобравање се више не појављује у приказу **Моја последња одобравања**.</span><span class="sxs-lookup"><span data-stu-id="a197d-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft**, and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="a197d-117">Уместо тога, отказано одобрење се појављује у приказу **Ставке времена за одобрење** или **Ставке трошкова за одобрење**, у зависности од тога да ли се ради о ставци времена или ставци трошкова.</span><span class="sxs-lookup"><span data-stu-id="a197d-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="a197d-118">Поред тога, статус повезане ставке времена или трошкова се мења у **Прослеђено**, тако да повезана ставка одговара одобрењима која имају статус **Радна верзија**.</span><span class="sxs-lookup"><span data-stu-id="a197d-118">Additionally, the status of the related time or expense entry is changed to **Submitted**, so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="a197d-119">Као давалац одобрења, можете да уређујете нека од поља одобравања која имају статус **Радна верзија**.</span><span class="sxs-lookup"><span data-stu-id="a197d-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="a197d-120">Ова поља обухватају ставке **Врста наплате** и **Наплативи сати за ставке времена**.</span><span class="sxs-lookup"><span data-stu-id="a197d-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="a197d-121">Након што унесете промене, можете поново да одобрите запис.</span><span class="sxs-lookup"><span data-stu-id="a197d-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="a197d-122">Друга могућност је да одбаците ставку.</span><span class="sxs-lookup"><span data-stu-id="a197d-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="a197d-123">Ако одбаците одобравање ставке времена, статус ставке ће бити промењен у **Враћена**.</span><span class="sxs-lookup"><span data-stu-id="a197d-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="a197d-124">Ако одбаците одобравање ставке трошкова, статус ставке ће бити промењен у **Одбачена**.</span><span class="sxs-lookup"><span data-stu-id="a197d-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="a197d-125">Са функционалне стране, и враћене и одбачене ставке се понашају исто као ставка која има статус **Радна верзија**.</span><span class="sxs-lookup"><span data-stu-id="a197d-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="a197d-126">Члан пројектног тима може да унесе све потребне промене у ставку, а затим да је поново проследи на одобравање или да у потпуности избрише ставку.</span><span class="sxs-lookup"><span data-stu-id="a197d-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="a197d-127">Финансијски утицај</span><span class="sxs-lookup"><span data-stu-id="a197d-127">Financial impact</span></span>

<span data-ttu-id="a197d-128">Постоји и финансијски утицај на пројекат када се одобрење откаже.</span><span class="sxs-lookup"><span data-stu-id="a197d-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="a197d-129">Прво, одговарајуће стварне вредности трошкова и продаје се ажурирају на следећи начин:</span><span class="sxs-lookup"><span data-stu-id="a197d-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="a197d-130">Статус поравнања се подешава на **Поравнато**.</span><span class="sxs-lookup"><span data-stu-id="a197d-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="a197d-131">Статус наплате се подешава на **Отказано**.</span><span class="sxs-lookup"><span data-stu-id="a197d-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="a197d-132">Затим, ставке сторнирања се креирају у табели Стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="a197d-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="a197d-133">Да би систем креирао ставке сторнирања, копира вредности поља из оригиналних стварних вредности.</span><span class="sxs-lookup"><span data-stu-id="a197d-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="a197d-134">Једине вредности које се не копирају су вредности количине.</span><span class="sxs-lookup"><span data-stu-id="a197d-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="a197d-135">Уместо тога, ове вредности се сторнирају.</span><span class="sxs-lookup"><span data-stu-id="a197d-135">These values are reversed instead.</span></span> <span data-ttu-id="a197d-136">Сторниране стварне вредности се креирају за стварне вредности **Трошкови** и **Ненаплаћена продаја**.</span><span class="sxs-lookup"><span data-stu-id="a197d-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="a197d-137">Поље **Статус поравнања** у сторнираним стварним вредностима је подешено на **Не може да се поравна**, а статус наплате на **Отказано**.</span><span class="sxs-lookup"><span data-stu-id="a197d-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="a197d-138">Након ових измена, износ који се евидентира као потрошен за пројекат и преостали приходи од пројект више неће узимати у обзир износе које ове стварне вредности представљају.</span><span class="sxs-lookup"><span data-stu-id="a197d-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]