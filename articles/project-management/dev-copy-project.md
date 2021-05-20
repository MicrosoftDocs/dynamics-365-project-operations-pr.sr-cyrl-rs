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
# <a name="develop-project-templates-with-copy-project"></a>Развијте предлошке пројеката помоћу опције за копирање пројеката

_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations подржава могућност копирања пројекта и враћања било којих задатака генеричким ресурсима који представљају улогу. Клијенти могу да користе ову функционалност за израду основних предложака пројеката.

Када одаберете **Копирај пројекат**, статус циљног пројекта се ажурира. Користите **Разлог статуса** да би се утврдило када је акција копирања завршена. Избор **Копирај пројекат** такође ажурира датум почетка пројекта на тренутни датум почетка ако није откривен циљни датум у циљном ентитету пројекта.

## <a name="copy-project-custom-action"></a>Прилагођена радња копирања пројекта 

### <a name="name"></a>Именуј 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>Улазни параметри
Постоје три улазна параметра:

| Параметар          | Тип   | Вредности                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** или **{"clearTeamsAndAssignments":true}** |
| SourceProject      | Референтни ентитет | Изворни пројекат |
| Циљ             | Референтни ентитет | Циљни пројекат |


- **{"clearTeamsAndAssignments":true}**: Подразумевано понашање за Project за веб и уклониће све задатке и чланове тима.
- **{"removeNamedResources":true}** Подразумевано понашање за Project Operations и вратиће задатке на генеричке ресурсе.

За више подразумеваних вредности радњи погледајте [Користите веб API радње](/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>Наведите поља за копирање 
Када је акција позвана, **Копирај пројекат** погледаће приказ пројекта **Копирајте колоне пројекта** да би се утврдило која поља треба копирати када се пројекат копира.


### <a name="example"></a>Пример
Следећи пример показује како да позовете прилагођену радњу **CopyProject** помоћу скупа параметара **removeNamedResources**.
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