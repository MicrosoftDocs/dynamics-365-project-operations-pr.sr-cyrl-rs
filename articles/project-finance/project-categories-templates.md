---
title: Синхронизујте категорије трошкова пројекта између услуга Finance and Operations и Project Service Automation
description: Ова тема описује предлошке и основне задатке који се користе за синхронизацију категорија задатака пројекта између услуга Microsoft Dynamics 365 Finance и Dynamics 365 Project Service Automation.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 7dd914dc-1913-45eb-8a67-e897b00089fa
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 757fe1dbc804b986fc3334ebae7254a3f0491f59
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755404"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="5a501-103">Синхронизујте категорије трошкова пројекта између услуга Finance and Operations и Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a501-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="5a501-104">Ова тема описује предлошке и основне задатке који се користе за синхронизацију категорија задатака пројекта између услуга Dynamics 365 Finance и Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a501-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="5a501-105">Интеграција пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и закључавање функционалности доступни су у верзији 8.0.</span><span class="sxs-lookup"><span data-stu-id="5a501-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="5a501-106">Интеграција стварних података доступна је у верзији 8.0.1 или новијој.</span><span class="sxs-lookup"><span data-stu-id="5a501-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="5a501-107">Ако користите Enterprise Edition 7.3.0, када инсталирате KB 4132657 и KB 4132660, моћи ћете да користите предлошке за интегрисање пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и стварних података, као и да конфигуришите закључавање функционалности.</span><span class="sxs-lookup"><span data-stu-id="5a501-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="5a501-108">Ако морате да ресетујете рачуноводствене дистрибуције, препоручујемо да инсталирате и KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="5a501-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="5a501-109">Ток података за Project Service Automation и Finance</span><span class="sxs-lookup"><span data-stu-id="5a501-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="5a501-110">Решење за интеграцију услуга Project Service Automation и Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="5a501-111">Предлошци за интеграцију који су доступни са функцијом Интеграција података омогућава ток података о категоријама пројектних задатака између услуга Finance и Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a501-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="5a501-112">Ако се категорије трошкова пројекта савладају у услузи Finance, ток интеграције је први из услуге Finance у Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a501-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="5a501-113">ID-ови интеграције категорија трошкова пројекта се затим ажурирају синхронизацијом из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="5a501-114">Ако се категорије трошкова пројекта савладају у услузи Project Service Automation, ток интеграције је први из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="5a501-115">Категорије пројеката морају већ бити конфигурисане у услузи Finance пре синхронизације из услуге Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a501-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="5a501-116">Затим синхронизујте из услуге Finance назад у Project Service Automation, а затим поново из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="5a501-117">На овај начин гарантујете да ће се категорије повезати и да се неће направити дупликати.</span><span class="sxs-lookup"><span data-stu-id="5a501-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="5a501-118">Категорије трошкова пројекта обично се савладавају у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="5a501-119">Међутим, ако није такав случај или ако су категорије трошкова већ креиране у услузи Project Service Automation, прво морате синхронизовати помоћу предлошка категорија трансакција трошкова (из PSA у Fin and Ops).</span><span class="sxs-lookup"><span data-stu-id="5a501-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="5a501-120">Затим синхронизујте помоћу предлошка категорија трансакција трошкова пројекта (из Fin and Ops у PSA).</span><span class="sxs-lookup"><span data-stu-id="5a501-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="5a501-121">Затим би требало да још једном покренете синхронизацију из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="5a501-122">Ако прво извршите синхронизацију из услуге Project Service Automation, у услузи Finance морају бити испуњени следећи захтеви:</span><span class="sxs-lookup"><span data-stu-id="5a501-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="5a501-123">Дељена категорија која се подудара са категоријом пројекта која је постављена у услузи Project Service Automation мора постојати и мора бити омогућена и за **Пројекат** и за **Трошак**.</span><span class="sxs-lookup"><span data-stu-id="5a501-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="5a501-124">За свако правно лице у услузи Finance са којим се мора интегрисати, морају постојати следеће категорије пројеката:</span><span class="sxs-lookup"><span data-stu-id="5a501-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="5a501-125">**Категорија пројекта** постоји.</span><span class="sxs-lookup"><span data-stu-id="5a501-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="5a501-126">**Користи у трошку** је омогућено.</span><span class="sxs-lookup"><span data-stu-id="5a501-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="5a501-127">**Активно у дневнику** је омогућено.</span><span class="sxs-lookup"><span data-stu-id="5a501-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="5a501-128">**Тип трансакције** је подешен на **Трошак**.</span><span class="sxs-lookup"><span data-stu-id="5a501-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="5a501-129">Следећа илустрација приказује како се подаци синхронизују између услуга Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="5a501-130">[![Ток података за интеграцију услуге Project Service Automation са услугом Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="5a501-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="5a501-131">Синхронизација категорије трошкова пројекта из услуге Finance у Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a501-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="5a501-132">Предложак и задатак</span><span class="sxs-lookup"><span data-stu-id="5a501-132">Template and task</span></span>

<span data-ttu-id="5a501-133">Да бисте приступили предлошку, у Microsoft Power Apps центру администрације изаберите **Пројекти**, а затим у горњем десном углу изаберите **Нови пројекат** за одабир јавних образаца.</span><span class="sxs-lookup"><span data-stu-id="5a501-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="5a501-134">Следећи предложак и основни задатак који се користе за синхронизацију категорија трошкова пројекта из услуге Finance у Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="5a501-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="5a501-135">**Назив предлошка у услузи Data Integration:** Категорије трансакција трошкова пројекта (из Fin and Ops у PSA)</span><span class="sxs-lookup"><span data-stu-id="5a501-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="5a501-136">**Назив задатка у пројекту:** Синхронизујте категорије са PSA</span><span class="sxs-lookup"><span data-stu-id="5a501-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="5a501-137">Скуп ентитета</span><span class="sxs-lookup"><span data-stu-id="5a501-137">Entity set</span></span>

| <span data-ttu-id="5a501-138">Finance</span><span class="sxs-lookup"><span data-stu-id="5a501-138">Finance</span></span>                           | <span data-ttu-id="5a501-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a501-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="5a501-140">Ентитет интеграције за категорије</span><span class="sxs-lookup"><span data-stu-id="5a501-140">Integration entity for categories</span></span> | <span data-ttu-id="5a501-141">Категорије трансакција</span><span class="sxs-lookup"><span data-stu-id="5a501-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="5a501-142">Ток ентитета</span><span class="sxs-lookup"><span data-stu-id="5a501-142">Entity flow</span></span>

<span data-ttu-id="5a501-143">Категоријама пројектних задатака се управља у услузи Finance и они се синхронизују са услугом Project Service Automation као категорија трансакција.</span><span class="sxs-lookup"><span data-stu-id="5a501-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="5a501-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="5a501-144">Power Query</span></span>

<span data-ttu-id="5a501-145">Када се синхронизујете са услугом Project Service Automation, морате да користите Microsoft Power Query за Excel да бисте поставили врсту наплате за категорију трансакција.</span><span class="sxs-lookup"><span data-stu-id="5a501-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="5a501-146">Предложак категорија трансакција трошкова пројекта (из Fin and Ops у PSA) пружају подразумевану колону и мапирање.</span><span class="sxs-lookup"><span data-stu-id="5a501-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="5a501-147">Ако креирате сопствени предложак, морате додати условну колону у Power Query.</span><span class="sxs-lookup"><span data-stu-id="5a501-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="5a501-148">Пратите ове кораке.</span><span class="sxs-lookup"><span data-stu-id="5a501-148">Follow these steps.</span></span>

1. <span data-ttu-id="5a501-149">Кликните на стрелицу да бисте отворили мапирање задатка категорија пројектних трошкова у предлошку категорија трансакција трошкова пројекта (из Fin and Ops у PSA).</span><span class="sxs-lookup"><span data-stu-id="5a501-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="5a501-150">Кликните на везу **Напредни упит и филтрирање** да бисте отворили Power Query.</span><span class="sxs-lookup"><span data-stu-id="5a501-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="5a501-151">Изаберите **Додај условну колону**.</span><span class="sxs-lookup"><span data-stu-id="5a501-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="5a501-152">Унесите име за нову колону, као што је **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="5a501-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="5a501-153">Унесите следећи услов: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span><span class="sxs-lookup"><span data-stu-id="5a501-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="5a501-154">Кликните на **У реду** на колони.</span><span class="sxs-lookup"><span data-stu-id="5a501-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="5a501-155">Обавезно мапирајте ову нову колону на страницу за мапирање.</span><span class="sxs-lookup"><span data-stu-id="5a501-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="5a501-156">Следећа илустрација приказује пример мапирања задатака предлошка у услузи Data Integration.</span><span class="sxs-lookup"><span data-stu-id="5a501-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="5a501-157">Мапирање приказује информације о пољу које ће се синхронизовати из услуге Finance у Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a501-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="5a501-158">[![Мапирање предложака](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="5a501-158">[![Template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="5a501-159">Синхронизација категорије трошкова пројекта из услуге Project Service Automation у Finance</span><span class="sxs-lookup"><span data-stu-id="5a501-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="5a501-160">Предложак и задатак</span><span class="sxs-lookup"><span data-stu-id="5a501-160">Template and task</span></span>

<span data-ttu-id="5a501-161">Следећи предложак и основни задатак који се користе за синхронизацију категорија трошкова пројекта из услуге Project Service Automation у Finance:</span><span class="sxs-lookup"><span data-stu-id="5a501-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="5a501-162">**Назив предлошка у услузи Data Integration:** Категорије трансакција трошкова пројекта (из PSA у Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="5a501-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="5a501-163">**Назив задатка у пројекту:** Синхронизујте категорије са Fin Ops</span><span class="sxs-lookup"><span data-stu-id="5a501-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="5a501-164">Скуп ентитета</span><span class="sxs-lookup"><span data-stu-id="5a501-164">Entity set</span></span>

| <span data-ttu-id="5a501-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a501-165">Project Service Automation</span></span> | <span data-ttu-id="5a501-166">Finance</span><span class="sxs-lookup"><span data-stu-id="5a501-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="5a501-167">Категорије трансакција</span><span class="sxs-lookup"><span data-stu-id="5a501-167">Transaction categories</span></span>     | <span data-ttu-id="5a501-168">Ентитет интеграције за категорије</span><span class="sxs-lookup"><span data-stu-id="5a501-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="5a501-169">Ток ентитета</span><span class="sxs-lookup"><span data-stu-id="5a501-169">Entity flow</span></span>

<span data-ttu-id="5a501-170">Категоријама пројектних задатака се управља у услузи Finance и они се синхронизују са услугом Project Service Automation као категорија трансакција.</span><span class="sxs-lookup"><span data-stu-id="5a501-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="5a501-171">Повратна синхронизација у Finance ажурира категорију пројекта у услузи Finance са ID-ом интеграције из услуге Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a501-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="5a501-172">Мапирање предложака у услузи Data Integration</span><span class="sxs-lookup"><span data-stu-id="5a501-172">Template mapping in Data integration</span></span>

<span data-ttu-id="5a501-173">Следећа илустрација приказује пример мапирања задатака предлошка у услузи Data Integration.</span><span class="sxs-lookup"><span data-stu-id="5a501-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="5a501-174">Мапирање приказује информације о терену које ће се синхронизовати из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a501-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="5a501-175">[![Мапирање предложака](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="5a501-175">[![Template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>
