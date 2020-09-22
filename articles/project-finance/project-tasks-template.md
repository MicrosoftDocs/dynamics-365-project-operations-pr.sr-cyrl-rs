---
title: Синхронизовање пројектних задатака директно из услуге Project Service Automation са услугом Finance and Operations
description: Ова тема описује предложак и основни задатак који се користе за синхронизацију пројектних задатака директно из услуге Microsoft Dynamics 365 Project Service Automation у Dynamics 365 Finance.
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
ms.assetid: d7f32327-33c4-43ab-b799-786210e93277
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 66a255346727c7ee4fbbf2920d2ef437ded03308
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755440"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="3bf07-103">Синхронизовање пројектних задатака директно из услуге Project Service Automation са услугом Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="3bf07-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="3bf07-104">Ова тема описује предложак и основни задатак који се користе за синхронизацију пројектних задатака директно из услуге Dynamics 365 Project Service Automation у Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="3bf07-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="3bf07-105">Интеграција пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и закључавање функционалности доступни су у верзији 8.0.</span><span class="sxs-lookup"><span data-stu-id="3bf07-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="3bf07-106">Ако користите Enterprise Edition 7.3.0, када инсталирате KB 4132657 и KB 4132660, моћи ћете да користите предлошке за интегрисање пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и стварних података, као и да конфигуришите закључавање функционалности.</span><span class="sxs-lookup"><span data-stu-id="3bf07-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="3bf07-107">Ако морате да ресетујете рачуноводствене дистрибуције, препоручили смо да инсталирате и KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="3bf07-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="3bf07-108">Интеграција стварних података доступна је у верзији 8.0.1 или новијој.</span><span class="sxs-lookup"><span data-stu-id="3bf07-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="3bf07-109">Ток података из услуге Project Service Automation у Finance</span><span class="sxs-lookup"><span data-stu-id="3bf07-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="3bf07-110">Решење за интеграцију из услуге Project Service Automation у Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="3bf07-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="3bf07-111">Предложак за интеграцију који је доступан са функцијом Интеграција података омогућава ток података о пројектним задацима из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="3bf07-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="3bf07-112">Следећа илустрација приказује како се подаци синхронизују између услуга Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="3bf07-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="3bf07-113">[![Ток података за интеграцију услуге Project Service Automation са услугом Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="3bf07-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="3bf07-114">Предложак и задатак</span><span class="sxs-lookup"><span data-stu-id="3bf07-114">Template and task</span></span>

<span data-ttu-id="3bf07-115">Да бисте приступили предлошку, у Microsoft Power Apps центру администрације изаберите **Пројекти**, а затим у горњем десном углу изаберите **Нови пројекат** за одабир јавних образаца.</span><span class="sxs-lookup"><span data-stu-id="3bf07-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="3bf07-116">Следећи предложак и основни задатак који се користе за синхронизацију пројектних задатака из услуге Project Service Automation у Finance:</span><span class="sxs-lookup"><span data-stu-id="3bf07-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="3bf07-117">**Назив предлошка у Интеграцији података:** Пројектни задаци (из PSA у Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="3bf07-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="3bf07-118">**Назив задатка у пројекту:** Пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="3bf07-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="3bf07-119">Да би могло да дође до синхронизације пројектних задатака, морате синхронизовати уговоре о пројекту и пројекте.</span><span class="sxs-lookup"><span data-stu-id="3bf07-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="3bf07-120">Скуп ентитета</span><span class="sxs-lookup"><span data-stu-id="3bf07-120">Entity set</span></span>

| <span data-ttu-id="3bf07-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="3bf07-121">Project Service Automation</span></span> | <span data-ttu-id="3bf07-122">Finance</span><span class="sxs-lookup"><span data-stu-id="3bf07-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="3bf07-123">Пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="3bf07-123">Project Tasks</span></span>              | <span data-ttu-id="3bf07-124">Ентитет интеграције за пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="3bf07-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="3bf07-125">Ток ентитета</span><span class="sxs-lookup"><span data-stu-id="3bf07-125">Entity flow</span></span>

<span data-ttu-id="3bf07-126">Пројектним задацима се управља у услузи Project Service Automation и они се синхронизују са услугом Finance као активности пројекта.</span><span class="sxs-lookup"><span data-stu-id="3bf07-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="3bf07-127">Предуслови и подешавање мапирања</span><span class="sxs-lookup"><span data-stu-id="3bf07-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="3bf07-128">Да би могло да дође до синхронизације пројектних задатака, морате синхронизовати уговоре о пројекту и пројекте.</span><span class="sxs-lookup"><span data-stu-id="3bf07-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="3bf07-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="3bf07-129">Power Query</span></span>

<span data-ttu-id="3bf07-130">Морате користити Microsoft Power Query за Excel за филтрирање података ако је испуњен овај услов:</span><span class="sxs-lookup"><span data-stu-id="3bf07-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="3bf07-131">У пројектном задатку имате записе специфичне за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="3bf07-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="3bf07-132">Ако морате да користите Power Query, следите ове смернице:</span><span class="sxs-lookup"><span data-stu-id="3bf07-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="3bf07-133">Предложак пројектних задатака (из PSA у Fin and Ops) има подразумевани филтер који из пројектног задатка искључује записе специфичне за ресурсе постављањем филтера на **IsLineTask** на **Нетачно**.</span><span class="sxs-lookup"><span data-stu-id="3bf07-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="3bf07-134">Ако креирате сопствени образац, морате додати овај филтер.</span><span class="sxs-lookup"><span data-stu-id="3bf07-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="3bf07-135">Мапирање предложака у услузи Data Integration</span><span class="sxs-lookup"><span data-stu-id="3bf07-135">Template mapping in Data integration</span></span>

<span data-ttu-id="3bf07-136">Следећа илустрација приказује пример мапирања задатака предлошка у интеграцији података.</span><span class="sxs-lookup"><span data-stu-id="3bf07-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="3bf07-137">Мапирање приказује информације о терену које ће се синхронизовати из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="3bf07-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="3bf07-138">[![Мапирање предложака](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="3bf07-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>
