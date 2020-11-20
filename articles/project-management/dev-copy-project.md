---
title: Развијте предлошке пројеката помоћу опције за копирање пројеката
description: Ова тема пружа информације о томе како креирати предлошке пројеката помоћу прилагођене радње Копирање пројекта.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0100c29873be6346614e958ef6ea0c77da2c9590
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131631"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="9abee-103">Развијте предлошке пројеката помоћу опције за копирање пројеката</span><span class="sxs-lookup"><span data-stu-id="9abee-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="9abee-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="9abee-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9abee-105">Dynamics 365 Project Operations подржава могућност копирања пројекта и враћања свих задатака у генеричке ресурсе који представљају улогу.</span><span class="sxs-lookup"><span data-stu-id="9abee-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="9abee-106">Клијенти могу да користе ову функционалност за израду основних предложака пројеката.</span><span class="sxs-lookup"><span data-stu-id="9abee-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="9abee-107">Када одаберете **Копирај пројекат**, статус циљног пројекта се ажурира.</span><span class="sxs-lookup"><span data-stu-id="9abee-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="9abee-108">Користите **Разлог статуса** да би се утврдило када је акција копирања завршена.</span><span class="sxs-lookup"><span data-stu-id="9abee-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="9abee-109">Избор **Копирај пројекат** такође ажурира датум почетка пројекта на тренутни датум почетка ако није откривен циљни датум у циљном ентитету пројекта.</span><span class="sxs-lookup"><span data-stu-id="9abee-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="9abee-110">Прилагођена радња копирања пројекта</span><span class="sxs-lookup"><span data-stu-id="9abee-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="9abee-111">Именуј</span><span class="sxs-lookup"><span data-stu-id="9abee-111">Name</span></span> 

<span data-ttu-id="9abee-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="9abee-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="9abee-113">Улазни параметри</span><span class="sxs-lookup"><span data-stu-id="9abee-113">Input parameters</span></span>
<span data-ttu-id="9abee-114">Постоје три улазна параметра:</span><span class="sxs-lookup"><span data-stu-id="9abee-114">There are three input parameters:</span></span>

| <span data-ttu-id="9abee-115">Параметар</span><span class="sxs-lookup"><span data-stu-id="9abee-115">Parameter</span></span>          | <span data-ttu-id="9abee-116">Тип</span><span class="sxs-lookup"><span data-stu-id="9abee-116">Type</span></span>   | <span data-ttu-id="9abee-117">Вредности</span><span class="sxs-lookup"><span data-stu-id="9abee-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="9abee-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="9abee-118">ProjectCopyOption</span></span>  | <span data-ttu-id="9abee-119">String</span><span class="sxs-lookup"><span data-stu-id="9abee-119">String</span></span> | <span data-ttu-id="9abee-120">**{"removeNamedResources":true}** или **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="9abee-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="9abee-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="9abee-121">SourceProject</span></span>      | <span data-ttu-id="9abee-122">Референтни ентитет</span><span class="sxs-lookup"><span data-stu-id="9abee-122">Entity Reference</span></span> | <span data-ttu-id="9abee-123">Изворни пројекат</span><span class="sxs-lookup"><span data-stu-id="9abee-123">Source Project</span></span> |
| <span data-ttu-id="9abee-124">Циљ</span><span class="sxs-lookup"><span data-stu-id="9abee-124">Target</span></span>             | <span data-ttu-id="9abee-125">Референтни ентитет</span><span class="sxs-lookup"><span data-stu-id="9abee-125">Entity Reference</span></span> | <span data-ttu-id="9abee-126">Циљни пројекат</span><span class="sxs-lookup"><span data-stu-id="9abee-126">Target Project</span></span> |


- <span data-ttu-id="9abee-127">**{"clearTeamsAndAssignments":true}**: Подразумевано понашање за Project за веб и уклониће све задатке и чланове тима.</span><span class="sxs-lookup"><span data-stu-id="9abee-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="9abee-128">**{"removeNamedResources":true}** Подразумевано понашање за Project Operations и вратиће задатке на генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="9abee-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="9abee-129">За више подразумеваних вредности радњи погледајте [Користите веб API радње](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="9abee-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="9abee-130">Наведите поља за копирање</span><span class="sxs-lookup"><span data-stu-id="9abee-130">Specify fields to copy</span></span> 
<span data-ttu-id="9abee-131">Када је акција позвана, **Копирај пројекат** погледаће приказ пројекта **Копирајте колоне пројекта** да би се утврдило која поља треба копирати када се пројекат копира.</span><span class="sxs-lookup"><span data-stu-id="9abee-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
