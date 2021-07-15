---
title: Преглед услуге Project Service Automation
description: Ова тема пружа информације о решењу за интеграцију услуге Dynamics 365 Project Service Automation са услугом Dynamics 365 Finance.
author: ruhercul
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: intro-internal
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1c756caec6cd7eda8f891446d3e8309aca3b2482
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369637"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="5a687-103">Преглед услуге Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a687-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="5a687-104">Решење за интеграцију из Project Service Automation у Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Dynamics 365 Finance и Dynamics 365 Project Service Automation преко услуге Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="5a687-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="5a687-105">Предлошци интеграције који су доступни са функцијом Интеграција података омогућавају ток пројеката, уговоре о пројекту, предмете уговора о пројекту, контролне тачке предмета уговора о пројекту, пројектне задатке, категорије трансакција трошкова, процене сати и процене трошкова из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="5a687-106">Ако користите верзију 7.3.0, морате инсталирати KB 4074835.</span><span class="sxs-lookup"><span data-stu-id="5a687-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="5a687-107">Тада ћете моћи да интегришете пројекте са фиксном ценом.</span><span class="sxs-lookup"><span data-stu-id="5a687-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="5a687-108">Ако користите верзију 7.3.0, а трансакције накнада преносите из услуге Project Service Automation, морате инсталирати KB 4345320 да бисте те накнаде укључили у фактуру пројекта.</span><span class="sxs-lookup"><span data-stu-id="5a687-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="5a687-109">Ако користите верзију 8.0, моћи ћете да користите интеграцију пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и закључавање функционалности.</span><span class="sxs-lookup"><span data-stu-id="5a687-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="5a687-110">Ако користите верзију 8.0.1 или новију, моћи ћете да синхронизујете актуелне податке.</span><span class="sxs-lookup"><span data-stu-id="5a687-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="5a687-111">Да бисте могли да интегришете Project Service Automation Finance, морате конфигурисати параметре интеграције услуге Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a687-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="5a687-112">За више информација, погледајте: [Интегрисање параметара услуге Project Service Automation](PSA-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="5a687-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="5a687-113">Ово решење за интеграцију омогућава директну синхронизацију у следећим сценаријима:</span><span class="sxs-lookup"><span data-stu-id="5a687-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="5a687-114">Одржавајте уговоре о пројекту у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="5a687-115">Креирајте пројекте у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="5a687-116">Одржавајте предмете уговора о пројекту у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="5a687-117">Одржавајте контролне тачке предмета уговора о пројекту у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="5a687-118">Одржавајте пројектне задатке у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="5a687-119">Одржавајте категорије трансакција трошкова у услузи Finance и синхронизујте их директно из услуге Finance у Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5a687-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="5a687-120">Креирајте процене часова пројекта у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="5a687-121">Креирајте процене трошкова пројекта у услузи Project Service Automation и синхронизујте их директно из услуге Project Service Automation у Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="5a687-122">Креирајте актуелне податке о времену, трошковима и накнадама у услузи Project Service Automation и креирајте пројектне трансакције у дневнику Project Service Automation интеграције тако да могу бити прокњижени у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="5a687-123">Синхронизација података</span><span class="sxs-lookup"><span data-stu-id="5a687-123">Data synchronization</span></span>

<span data-ttu-id="5a687-124">Следећа илустрација приказује како се подаци синхронизују као део интеграције између услуга Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="5a687-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="5a687-125">Тренутно нису доступни сви предлошци.</span><span class="sxs-lookup"><span data-stu-id="5a687-125">Not all templates are currently available.</span></span> <span data-ttu-id="5a687-126">Предлошци ће бити објављени по завршетку.</span><span class="sxs-lookup"><span data-stu-id="5a687-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="5a687-127">[![Интеграција услуге Project Service Automation са услугом Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="5a687-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="5a687-128">Системски захтеви за Finance</span><span class="sxs-lookup"><span data-stu-id="5a687-128">System requirements for Finance</span></span>

<span data-ttu-id="5a687-129">Да бисте користили решење за интеграцију услуге Project Service Automation у Finance, морате инсталирати Enterprise Edition 7.3 са исправком платформе 12 или новијом.</span><span class="sxs-lookup"><span data-stu-id="5a687-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="5a687-130">Системски захтеви за Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a687-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="5a687-131">Да бисте користили решење за интеграцију услуге Project Service Automation у Finance, морате инсталирати следеће компоненте:</span><span class="sxs-lookup"><span data-stu-id="5a687-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="5a687-132">Dynamics 365 Project Service Automation верзија 9.0.0.0 или новија</span><span class="sxs-lookup"><span data-stu-id="5a687-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="5a687-133">Могуће решење за готовину за Dynamics 365 Sales, верзија 1.14.0.0 (v14) или новија</span><span class="sxs-lookup"><span data-stu-id="5a687-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="5a687-134">Решење Project Service Automation у Finance за Dynamics 365 Project Service Automation верзија 1.0.0.0 или новија</span><span class="sxs-lookup"><span data-stu-id="5a687-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="5a687-135">Инсталирање решења за интеграцију услуге Project Service Automation у Finance у вашој инстанци услуге Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a687-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="5a687-136">Преузмите решење за интеграцију Project Service Automation у Finance из [Microsoft центра за преузимање](https://www.microsoft.com/download/details.aspx?id=57016) и следите упутства која сте добили уз решење.</span><span class="sxs-lookup"><span data-stu-id="5a687-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]