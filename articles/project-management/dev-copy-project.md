---
title: Развијте предлошке пројеката помоћу опције за копирање пројеката
description: Ова тема пружа информације о томе како креирати предлошке пројеката помоћу прилагођене радње Копирање пројекта.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083912"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="b512e-103">Развијте предлошке пројеката помоћу опције за копирање пројеката</span><span class="sxs-lookup"><span data-stu-id="b512e-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="b512e-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="b512e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b512e-105">Dynamics 365 Project Operations подржава могућност копирања пројекта и враћања свих задатака у генеричке ресурсе који представљају улогу.</span><span class="sxs-lookup"><span data-stu-id="b512e-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="b512e-106">Клијенти могу да користе ову функционалност за израду основних предложака пројеката.</span><span class="sxs-lookup"><span data-stu-id="b512e-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="b512e-107">Када одаберете **Копирај пројекат** , статус циљног пројекта се ажурира.</span><span class="sxs-lookup"><span data-stu-id="b512e-107">When you select **Copy Project** , the status of the target project is updated.</span></span> <span data-ttu-id="b512e-108">Користите **Разлог статуса** да би се утврдило када је акција копирања завршена.</span><span class="sxs-lookup"><span data-stu-id="b512e-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="b512e-109">Избор **Копирај пројекат** такође ажурира датум почетка пројекта на тренутни датум почетка ако није откривен циљни датум у циљном ентитету пројекта.</span><span class="sxs-lookup"><span data-stu-id="b512e-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="b512e-110">Прилагођена радња копирања пројекта</span><span class="sxs-lookup"><span data-stu-id="b512e-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="b512e-111">Именуј</span><span class="sxs-lookup"><span data-stu-id="b512e-111">Name</span></span> 

<span data-ttu-id="b512e-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="b512e-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="b512e-113">Улазни параметри</span><span class="sxs-lookup"><span data-stu-id="b512e-113">Input parameters</span></span>
<span data-ttu-id="b512e-114">Постоје три улазна параметра:</span><span class="sxs-lookup"><span data-stu-id="b512e-114">There are three input parameters:</span></span>

| <span data-ttu-id="b512e-115">Параметар</span><span class="sxs-lookup"><span data-stu-id="b512e-115">Parameter</span></span>          | <span data-ttu-id="b512e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="b512e-116">Type</span></span>   | <span data-ttu-id="b512e-117">Вредности</span><span class="sxs-lookup"><span data-stu-id="b512e-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="b512e-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="b512e-118">ProjectCopyOption</span></span>  | <span data-ttu-id="b512e-119">String</span><span class="sxs-lookup"><span data-stu-id="b512e-119">String</span></span> | <span data-ttu-id="b512e-120">**{"removeNamedResources":true}** или **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="b512e-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="b512e-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="b512e-121">SourceProject</span></span>      | <span data-ttu-id="b512e-122">Референтни ентитет</span><span class="sxs-lookup"><span data-stu-id="b512e-122">Entity Reference</span></span> | <span data-ttu-id="b512e-123">Изворни пројекат</span><span class="sxs-lookup"><span data-stu-id="b512e-123">Source Project</span></span> |
| <span data-ttu-id="b512e-124">Циљ</span><span class="sxs-lookup"><span data-stu-id="b512e-124">Target</span></span>             | <span data-ttu-id="b512e-125">Референтни ентитет</span><span class="sxs-lookup"><span data-stu-id="b512e-125">Entity Reference</span></span> | <span data-ttu-id="b512e-126">Циљни пројекат</span><span class="sxs-lookup"><span data-stu-id="b512e-126">Target Project</span></span> |


- <span data-ttu-id="b512e-127">**{"clearTeamsAndAssignments":true}** : Подразумевано понашање за Project за веб и уклониће све задатке и чланове тима.</span><span class="sxs-lookup"><span data-stu-id="b512e-127">**{"clearTeamsAndAssignments":true}** : Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="b512e-128">**{"removeNamedResources":true}** Подразумевано понашање за Project Operations и вратиће задатке на генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="b512e-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="b512e-129">За више подразумеваних вредности радњи погледајте [Користите веб API радње](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="b512e-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="b512e-130">Наведите поља за копирање</span><span class="sxs-lookup"><span data-stu-id="b512e-130">Specify fields to copy</span></span> 
<span data-ttu-id="b512e-131">Када је акција позвана, **Копирај пројекат** погледаће приказ пројекта **Копирајте колоне пројекта** да би се утврдило која поља треба копирати када се пројекат копира.</span><span class="sxs-lookup"><span data-stu-id="b512e-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
