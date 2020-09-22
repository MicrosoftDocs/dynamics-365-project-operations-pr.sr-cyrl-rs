---
title: Синхронизовање процена пројекта директно из услуге Project Service Automation са услугом Finance and Operations
description: Ова тема описује предлошке и основне задатке који се користе за синхронизацију процене радних сати и процене трошкова пројекта директно из услуге Microsoft Dynamics 365 Project Service Automation у Dynamics 365 Finance.
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
ms.assetid: d688ce9a-41e3-4ebe-952e-700f8351fbe9
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: a24a967d82c2e005e61234d34da8a583b61ff7b1
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755364"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="4d823-103">Синхронизовање процена пројекта директно из услуге Project Service Automation са услугом Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="4d823-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="4d823-104">Ова тема описује предлошке и основне задатке који се користе за синхронизацију процене радних сати и процене трошкова пројекта директно из услуге Dynamics 365 Project Service Automation у Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="4d823-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="4d823-105">Интеграција пројектних задатака, категорије трансакција трошкова, процене радних сати, процене трошкова и закључавање функционалности доступни су у верзији 8.0.</span><span class="sxs-lookup"><span data-stu-id="4d823-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="4d823-106">Интеграција стварних података доступна је у верзији 8.0.1 или новијој.</span><span class="sxs-lookup"><span data-stu-id="4d823-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="4d823-107">Ток података из услуге Project Service Automation у Finance</span><span class="sxs-lookup"><span data-stu-id="4d823-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="4d823-108">Решење за интеграцију из услуге Project Service Automation у Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="4d823-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="4d823-109">Предлошци за интеграцију који су доступни са функцијом Интеграција података омогућава ток података о проценама радних сати пројекта и проценама трошкова пројекта између из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="4d823-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="4d823-110">Следећа илустрација приказује како се подаци синхронизују између услуга Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="4d823-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="4d823-111">[![Ток података за интеграцију услуге Project Service Automation са услугом Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="4d823-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="4d823-112">Процене радних сати за пројекат</span><span class="sxs-lookup"><span data-stu-id="4d823-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="4d823-113">Предлошци и задаци</span><span class="sxs-lookup"><span data-stu-id="4d823-113">Template and tasks</span></span>

<span data-ttu-id="4d823-114">Да бисте приступили доступним предлошцима, у Microsoft Power Apps центру администрације изаберите **Пројекти**, а затим у горњем десном углу изаберите **Нови пројекат** за избор јавних предложака.</span><span class="sxs-lookup"><span data-stu-id="4d823-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="4d823-115">Следећи предложак и основни задаци који се користе за синхронизацију процена радних сати пројекта из услуге Project Service Automation у Finance:</span><span class="sxs-lookup"><span data-stu-id="4d823-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="4d823-116">**Назив предлошка у Интеграцији података:** Процене радних сати пројекта (из PSA у Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="4d823-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="4d823-117">**Назив задатака у пројекту:**</span><span class="sxs-lookup"><span data-stu-id="4d823-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="4d823-118">Односи између трансакција</span><span class="sxs-lookup"><span data-stu-id="4d823-118">Transaction relationships</span></span>
    - <span data-ttu-id="4d823-119">Процене трошкова</span><span class="sxs-lookup"><span data-stu-id="4d823-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="4d823-120">Скуп ентитета</span><span class="sxs-lookup"><span data-stu-id="4d823-120">Entity set</span></span>

| <span data-ttu-id="4d823-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="4d823-121">Project Service Automation</span></span> | <span data-ttu-id="4d823-122">Finance</span><span class="sxs-lookup"><span data-stu-id="4d823-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="4d823-123">Пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="4d823-123">Project tasks</span></span>              | <span data-ttu-id="4d823-124">Ентитет интеграције за процене радних сати пројекта</span><span class="sxs-lookup"><span data-stu-id="4d823-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="4d823-125">Ток ентитета</span><span class="sxs-lookup"><span data-stu-id="4d823-125">Entity flow</span></span>

<span data-ttu-id="4d823-126">Проценама радних сати пројекта се управља у услузи Project Service Automation и они се синхронизују са услугом Finance као предвиђања сати пројекта.</span><span class="sxs-lookup"><span data-stu-id="4d823-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="4d823-127">Предуслови</span><span class="sxs-lookup"><span data-stu-id="4d823-127">Prerequisites</span></span>

<span data-ttu-id="4d823-128">Да би могла да се изврши синхронизација процена радних сати пројекта, морате синхронизовати пројекте, пројектне задатке и категорије трансакција трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="4d823-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="4d823-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="4d823-129">Power Query</span></span>

<span data-ttu-id="4d823-130">У предлошку за процену радног времена пројекта морате да користите Microsoft Power Query за Excel да бисте извршили ове задатке:</span><span class="sxs-lookup"><span data-stu-id="4d823-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="4d823-131">Поставите ID подразумеваног модела предвиђања који ће се користити када интеграција креира нова предвиђања сати.</span><span class="sxs-lookup"><span data-stu-id="4d823-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="4d823-132">У задатку филтрирајте све записе специфичне за ресурсе који неће успети у интеграцији предвиђања радних сати.</span><span class="sxs-lookup"><span data-stu-id="4d823-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="4d823-133">Филтрирајте све празне редове категорија трансакција.</span><span class="sxs-lookup"><span data-stu-id="4d823-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="4d823-134">Неиспуњавање овог задатка може резултирати нетачним предвиђањима радних сати.</span><span class="sxs-lookup"><span data-stu-id="4d823-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="4d823-135">Подесите подразумевани ID модела предвиђања</span><span class="sxs-lookup"><span data-stu-id="4d823-135">Set the default forecast model ID</span></span>

<span data-ttu-id="4d823-136">Да бисте ажурирали подразумевани ID модела предвиђања у предлошку, кликните на стрелицу **Мапа** за отварање мапирања.</span><span class="sxs-lookup"><span data-stu-id="4d823-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="4d823-137">Затим изаберите везу **Напредни упит и филтрирање**.</span><span class="sxs-lookup"><span data-stu-id="4d823-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="4d823-138">Ако користите подразумевани предложак процене радних сати пројекта (из PSA у Fin and Ops), изаберите **Услов уметања** у лист **Примењени кораци**.</span><span class="sxs-lookup"><span data-stu-id="4d823-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="4d823-139">У ставци **Функција**, замените **O\_forecast** називом ID-а модела предвиђања који треба користити уз интеграцију.</span><span class="sxs-lookup"><span data-stu-id="4d823-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="4d823-140">Подразумевани предложак садржи ID модела предвиђања из демо података.</span><span class="sxs-lookup"><span data-stu-id="4d823-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="4d823-141">Ако креирате нови образац, морате додати ову колону.</span><span class="sxs-lookup"><span data-stu-id="4d823-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="4d823-142">У услузи Power Query изаберите **Додај условну колону** и унесите назив за нову колону, као што је **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="4d823-142">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="4d823-143">Унесите услов за колону, где, ако пројектни задатак није празан, онда \<унесите ID модела предвиђања\>; иначе је празно.</span><span class="sxs-lookup"><span data-stu-id="4d823-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="4d823-144">Филтрирање записа специфичних за ресурсе</span><span class="sxs-lookup"><span data-stu-id="4d823-144">Filter out resource-specific records</span></span>

<span data-ttu-id="4d823-145">Предложак процена радних сати пројекта (из PSA у Fin and Ops) има подразумевани филтер који уклања све записе специфичне за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4d823-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="4d823-146">Ако креирате сопствени образац, морате додати овај филтер.</span><span class="sxs-lookup"><span data-stu-id="4d823-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="4d823-147">Изаберите везу **Напредни упит и филтрирање** да филтрирате по колони **msdyn\_islinetask** тако да буду увршћени само **Нетачни** записи.</span><span class="sxs-lookup"><span data-stu-id="4d823-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="4d823-148">Филтрирајте празне редове категорија трансакција</span><span class="sxs-lookup"><span data-stu-id="4d823-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="4d823-149">Морате додати филтер да бисте уклонили све редове који имају празне категорије трансакција.</span><span class="sxs-lookup"><span data-stu-id="4d823-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="4d823-150">Овај задатак је обавезан, без обзира на то да ли користите подразумевани предложак или креирате сопствени предложак.</span><span class="sxs-lookup"><span data-stu-id="4d823-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="4d823-151">Овај филтер уклања све редове резимеа из услуге Project Service Automation који могу проузроковати нетачна предвиђања радних сати у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="4d823-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="4d823-152">Изаберите везу **Напредни упит и филтрирање** да филтрирате празне записе у колони **msdyn\_transactioncategory\_value**.</span><span class="sxs-lookup"><span data-stu-id="4d823-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="4d823-153">Мапирање предложака у услузи Data Integration</span><span class="sxs-lookup"><span data-stu-id="4d823-153">Template mapping in Data integration</span></span>

<span data-ttu-id="4d823-154">Следећа илустрација приказује пример мапирања задатака предлошка у услузи Data Integration.</span><span class="sxs-lookup"><span data-stu-id="4d823-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="4d823-155">Мапирање приказује информације о терену које ће се синхронизовати из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="4d823-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="4d823-156">[![Мапирање предложака](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="4d823-156">[![Template mapping](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="4d823-157">Процене трошкова пројекта</span><span class="sxs-lookup"><span data-stu-id="4d823-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="4d823-158">Предлошци и задаци</span><span class="sxs-lookup"><span data-stu-id="4d823-158">Template and tasks</span></span>

<span data-ttu-id="4d823-159">Следећи предложак и основни задаци који се користе за синхронизацију процена трошкова из услуге Project Service Automation у Finance:</span><span class="sxs-lookup"><span data-stu-id="4d823-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="4d823-160">**Назив предлошка у Интеграцији података:** Процене трошкова пројекта (из PSA у Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="4d823-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="4d823-161">**Назив задатака у пројекту:**</span><span class="sxs-lookup"><span data-stu-id="4d823-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="4d823-162">Односи између трансакција</span><span class="sxs-lookup"><span data-stu-id="4d823-162">Transaction relationships</span></span> 
    - <span data-ttu-id="4d823-163">Процене трошкова</span><span class="sxs-lookup"><span data-stu-id="4d823-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="4d823-164">Скуп ентитета</span><span class="sxs-lookup"><span data-stu-id="4d823-164">Entity set</span></span>

| <span data-ttu-id="4d823-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="4d823-165">Project Service Automation</span></span> | <span data-ttu-id="4d823-166">Finance</span><span class="sxs-lookup"><span data-stu-id="4d823-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="4d823-167">Везе трансакција</span><span class="sxs-lookup"><span data-stu-id="4d823-167">Transaction Connections</span></span>    | <span data-ttu-id="4d823-168">Ентитет интеграције за односе трансакција пројекта</span><span class="sxs-lookup"><span data-stu-id="4d823-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="4d823-169">Ставке процене</span><span class="sxs-lookup"><span data-stu-id="4d823-169">Estimate Lines</span></span>             | <span data-ttu-id="4d823-170">Ентитет интеграције за процене трошкова пројекта</span><span class="sxs-lookup"><span data-stu-id="4d823-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="4d823-171">Ток ентитета</span><span class="sxs-lookup"><span data-stu-id="4d823-171">Entity flow</span></span>

<span data-ttu-id="4d823-172">Проценама трошкова се управља у услузи Project Service Automation и оне се синхронизују са услугом Finance као предвиђања трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="4d823-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="4d823-173">Предуслови</span><span class="sxs-lookup"><span data-stu-id="4d823-173">Prerequisites</span></span>

<span data-ttu-id="4d823-174">Да би могла да се изврши синхронизација процена трошкова пројекта, морате синхронизовати пројекте, пројектне задатке и категорије трансакција трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="4d823-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="4d823-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="4d823-175">Power Query</span></span>

<span data-ttu-id="4d823-176">У предлошку за процену трошкова пројекта морате да користите Power Query да бисте извршили следеће задатке:</span><span class="sxs-lookup"><span data-stu-id="4d823-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="4d823-177">Филтрирајте да бисте укључили само записе линија процене трошкова.</span><span class="sxs-lookup"><span data-stu-id="4d823-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="4d823-178">Поставите ID подразумеваног модела предвиђања који ће се користити када интеграција креира нова предвиђања сати.</span><span class="sxs-lookup"><span data-stu-id="4d823-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="4d823-179">Трансформишите врсте наплате.</span><span class="sxs-lookup"><span data-stu-id="4d823-179">Transform the billing types.</span></span>
- <span data-ttu-id="4d823-180">Трансформишите врсте трансакција.</span><span class="sxs-lookup"><span data-stu-id="4d823-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="4d823-181">Филтрирајте да бисте укључили само линије процене трошкова</span><span class="sxs-lookup"><span data-stu-id="4d823-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="4d823-182">Предложак за процену трошкова пројекта (из PSA у Fin and Ops) има подразумевани филтер који укључује само линије трошкова у интеграцији.</span><span class="sxs-lookup"><span data-stu-id="4d823-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="4d823-183">Ако креирате сопствени образац, морате додати овај филтер.</span><span class="sxs-lookup"><span data-stu-id="4d823-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="4d823-184">Изаберите задатак **Односи између трансакција**, а затим кликните на стрелицу **Мапа** да бисте отворили мапирање.</span><span class="sxs-lookup"><span data-stu-id="4d823-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="4d823-185">Изаберите везу **Напредни упит и филтрирање**.</span><span class="sxs-lookup"><span data-stu-id="4d823-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="4d823-186">Филтрирајте колону **msdyn\_transactiontype1**колона тако да укључује само **msdyn\_estimateline**.</span><span class="sxs-lookup"><span data-stu-id="4d823-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="4d823-187">Подесите подразумевани ID модела предвиђања</span><span class="sxs-lookup"><span data-stu-id="4d823-187">Set the default forecast model ID</span></span>

<span data-ttu-id="4d823-188">Да бисте ажурирали подразумевани ID модела предвиђања у предлошку, изаберите задатак **Процене трошкова**, а затим кликните на стрелицу **Мапирај** да бисте отворили мапирање.</span><span class="sxs-lookup"><span data-stu-id="4d823-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="4d823-189">Изаберите везу **Напредни упит и филтрирање**.</span><span class="sxs-lookup"><span data-stu-id="4d823-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="4d823-190">Ако користите подразумевани предложак процене трошкова пројекта (из PSA у Fin and Ops), у услузи Power Query изаберите **Услов уметања** у одељку **Примењени кораци**.</span><span class="sxs-lookup"><span data-stu-id="4d823-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="4d823-191">У ставци **Функција**, замените **O\_forecast** називом ID-а модела предвиђања који треба користити уз интеграцију.</span><span class="sxs-lookup"><span data-stu-id="4d823-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="4d823-192">Подразумевани предложак садржи ID модела предвиђања из демо података.</span><span class="sxs-lookup"><span data-stu-id="4d823-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="4d823-193">Ако креирате нови образац, морате додати ову колону.</span><span class="sxs-lookup"><span data-stu-id="4d823-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="4d823-194">У услузи Power Query изаберите **Додај условну колону** и унесите назив за нову колону, као што је **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="4d823-194">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="4d823-195">Унесите услов за колону, где, ако ID реда процене није празан, онда \<унесите ID модела предвиђања\>; иначе је празно.</span><span class="sxs-lookup"><span data-stu-id="4d823-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="4d823-196">Трансформисање врста наплате</span><span class="sxs-lookup"><span data-stu-id="4d823-196">Transform the billing types</span></span>

<span data-ttu-id="4d823-197">Предложак процене трошкова пројекта (из PSA у Fin and Ops) укључује условну колону која се користи за трансформисање типова наплате који су примљени из услуге Project Service Automation током интеграције.</span><span class="sxs-lookup"><span data-stu-id="4d823-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="4d823-198">Ако креирате сопствени образац, морате додати ову условну колону.</span><span class="sxs-lookup"><span data-stu-id="4d823-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="4d823-199">Изаберите везу **Напредни упит и филтрирање**, а затим изаберите **Додај условну колону**.</span><span class="sxs-lookup"><span data-stu-id="4d823-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="4d823-200">Унесите име за нову колону, као што је **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="4d823-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="4d823-201">Затим унесите следећи услов:</span><span class="sxs-lookup"><span data-stu-id="4d823-201">Then enter the following condition:</span></span>

<span data-ttu-id="4d823-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span><span class="sxs-lookup"><span data-stu-id="4d823-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="4d823-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span><span class="sxs-lookup"><span data-stu-id="4d823-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="4d823-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span><span class="sxs-lookup"><span data-stu-id="4d823-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="4d823-205">else **NotAvailable**</span><span class="sxs-lookup"><span data-stu-id="4d823-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="4d823-206">Трансформисање врста трансакција</span><span class="sxs-lookup"><span data-stu-id="4d823-206">Transform the transaction types</span></span>

<span data-ttu-id="4d823-207">Предложак процене трошкова пројекта (из PSA у Fin and Ops) укључује условну колону која се користи за трансформисање врста трансакција које су примљене из услуге Project Service Automation током интеграције.</span><span class="sxs-lookup"><span data-stu-id="4d823-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="4d823-208">Ако креирате сопствени образац, морате додати ову условну колону.</span><span class="sxs-lookup"><span data-stu-id="4d823-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="4d823-209">Изаберите везу **Напредни упит и филтрирање**, а затим изаберите **Додај условну колону**.</span><span class="sxs-lookup"><span data-stu-id="4d823-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="4d823-210">Унесите назив за нову колону, као што је **TransactionType**.</span><span class="sxs-lookup"><span data-stu-id="4d823-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="4d823-211">Затим унесите следећи услов:</span><span class="sxs-lookup"><span data-stu-id="4d823-211">Then enter the following condition:</span></span>

<span data-ttu-id="4d823-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span><span class="sxs-lookup"><span data-stu-id="4d823-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="4d823-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span><span class="sxs-lookup"><span data-stu-id="4d823-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="4d823-214">else **null**</span><span class="sxs-lookup"><span data-stu-id="4d823-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="4d823-215">Мапирање предложака у услузи Data Integration</span><span class="sxs-lookup"><span data-stu-id="4d823-215">Template mapping in Data integration</span></span>

<span data-ttu-id="4d823-216">Следеће илустрације приказују примере мапирања задатака предлошка у услузи Data Integration.</span><span class="sxs-lookup"><span data-stu-id="4d823-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="4d823-217">Мапирање приказује информације о терену које ће се синхронизовати из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="4d823-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="4d823-218">[![Мапирање предложака](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="4d823-218">[![Template mapping](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="4d823-219">[![Мапирање предложака](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="4d823-219">[![Template mapping](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>
