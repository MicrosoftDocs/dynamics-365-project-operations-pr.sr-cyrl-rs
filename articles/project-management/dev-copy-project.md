---
title: Развијте предлошке пројеката помоћу опције за копирање пројеката
description: Ова тема пружа информације о томе како креирати предлошке пројеката помоћу прилагођене радње Копирање пројекта.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cc17df0c73b276048f7c4b04bd9dc6644e828dc0
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949832"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="83403-103">Развијте предлошке пројеката помоћу опције за копирање пројеката</span><span class="sxs-lookup"><span data-stu-id="83403-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="83403-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="83403-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="83403-105">Dynamics 365 Project Operations подржава могућност копирања пројекта и враћања било којих задатака генеричким ресурсима који представљају улогу.</span><span class="sxs-lookup"><span data-stu-id="83403-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="83403-106">Клијенти могу да користе ову функционалност за израду основних предложака пројеката.</span><span class="sxs-lookup"><span data-stu-id="83403-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="83403-107">Када одаберете **Копирај пројекат**, статус циљног пројекта се ажурира.</span><span class="sxs-lookup"><span data-stu-id="83403-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="83403-108">Користите **Разлог статуса** да би се утврдило када је акција копирања завршена.</span><span class="sxs-lookup"><span data-stu-id="83403-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="83403-109">Избор **Копирај пројекат** такође ажурира датум почетка пројекта на тренутни датум почетка ако није откривен циљни датум у циљном ентитету пројекта.</span><span class="sxs-lookup"><span data-stu-id="83403-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="83403-110">Прилагођена радња копирања пројекта</span><span class="sxs-lookup"><span data-stu-id="83403-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="83403-111">Именуј</span><span class="sxs-lookup"><span data-stu-id="83403-111">Name</span></span> 

<span data-ttu-id="83403-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="83403-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="83403-113">Улазни параметри</span><span class="sxs-lookup"><span data-stu-id="83403-113">Input parameters</span></span>
<span data-ttu-id="83403-114">Постоје три улазна параметра:</span><span class="sxs-lookup"><span data-stu-id="83403-114">There are three input parameters:</span></span>

| <span data-ttu-id="83403-115">Параметар</span><span class="sxs-lookup"><span data-stu-id="83403-115">Parameter</span></span>          | <span data-ttu-id="83403-116">Тип</span><span class="sxs-lookup"><span data-stu-id="83403-116">Type</span></span>   | <span data-ttu-id="83403-117">Вредности</span><span class="sxs-lookup"><span data-stu-id="83403-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="83403-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="83403-118">ProjectCopyOption</span></span>  | <span data-ttu-id="83403-119">String</span><span class="sxs-lookup"><span data-stu-id="83403-119">String</span></span> | <span data-ttu-id="83403-120">**{"removeNamedResources":true}** или **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="83403-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="83403-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="83403-121">SourceProject</span></span>      | <span data-ttu-id="83403-122">Референтни ентитет</span><span class="sxs-lookup"><span data-stu-id="83403-122">Entity Reference</span></span> | <span data-ttu-id="83403-123">Изворни пројекат</span><span class="sxs-lookup"><span data-stu-id="83403-123">Source Project</span></span> |
| <span data-ttu-id="83403-124">Циљ</span><span class="sxs-lookup"><span data-stu-id="83403-124">Target</span></span>             | <span data-ttu-id="83403-125">Референтни ентитет</span><span class="sxs-lookup"><span data-stu-id="83403-125">Entity Reference</span></span> | <span data-ttu-id="83403-126">Циљни пројекат</span><span class="sxs-lookup"><span data-stu-id="83403-126">Target Project</span></span> |


- <span data-ttu-id="83403-127">**{"clearTeamsAndAssignments":true}**: Подразумевано понашање за Project за веб и уклониће све задатке и чланове тима.</span><span class="sxs-lookup"><span data-stu-id="83403-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="83403-128">**{"removeNamedResources":true}** Подразумевано понашање за Project Operations и вратиће задатке на генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="83403-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="83403-129">За више подразумеваних вредности радњи погледајте [Користите веб API радње](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="83403-129">For more defaults on actions, see [Use Web API actions](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="83403-130">Наведите поља за копирање</span><span class="sxs-lookup"><span data-stu-id="83403-130">Specify fields to copy</span></span> 
<span data-ttu-id="83403-131">Када је акција позвана, **Копирај пројекат** погледаће приказ пројекта **Копирајте колоне пројекта** да би се утврдило која поља треба копирати када се пројекат копира.</span><span class="sxs-lookup"><span data-stu-id="83403-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="83403-132">Пример</span><span class="sxs-lookup"><span data-stu-id="83403-132">Example</span></span>
<span data-ttu-id="83403-133">Следећи пример показује како да позовете прилагођену радњу **CopyProject** помоћу скупа параметара **removeNamedResources**.</span><span class="sxs-lookup"><span data-stu-id="83403-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]