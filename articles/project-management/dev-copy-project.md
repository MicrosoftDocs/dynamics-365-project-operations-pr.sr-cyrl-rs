---
title: Развијте предлошке пројеката помоћу опције за копирање пројеката
description: Ова тема пружа информације о томе како креирати предлошке пројеката помоћу прилагођене радње Копирање пројекта.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 72aa2db7c717eeab85ada448c673bf702087baeb
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/14/2022
ms.locfileid: "8590918"
---
# <a name="develop-project-templates-with-copy-project"></a>Развијте предлошке пројеката помоћу опције за копирање пројеката

_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_

Dynamics 365 Project Operations подржава могућност копирања пројекта и враћања било којих задатака генеричким ресурсима који представљају улогу. Клијенти могу да користе ову функционалност за израду основних предложака пројеката.

Када одаберете **Копирај пројекат**, статус циљног пројекта се ажурира. Користите **Разлог статуса** да би се утврдило када је акција копирања завршена. Избор **Копирај пројекат** такође ажурира датум почетка пројекта на тренутни датум почетка ако није откривен циљни датум у циљном ентитету пројекта.

## <a name="copy-project-custom-action"></a>Прилагођена радња копирања пројекта

### <a name="name"></a>Именуј 

мсдyн \_ CopyProjectV3

### <a name="input-parameters"></a>Улазни параметри

Постоје три улазна параметра:

- **РеплацеНамедРесоурцес** или **ЦлеарТеамсАндАссигнментс** – Поставите само једну од опција. Не постављај оба.

    - **\{"РеплацеНамедРесоурцес ":труе \}** – Подразумевано понашање за пројектне операције. Сви именовани ресурси се замењују генеричким ресурсима.
    - **\{"ЦлеарТеамсАндАссигнментс ":труе \}** – Подразумевано понашање за Пројекат за Wеб. Сви задаци и чланови тима су уклоњени.

- **СоурцеПројецт** – Референца ентитета изворног пројекта из којег треба копирати. Овај параметар не може бити без вредности.
- **Циљ** – Референца ентитета циљног пројекта у који треба копирати. Овај параметар не може бити без вредности.

Следећа табела обезбеђује резиме три параметра.

| Параметар                | Тип             | Value                 |
|--------------------------|------------------|-----------------------|
| ЗамениНамедРесоурцес    | Логичка вредност          | **Тачно или** нетачно **·** |
| ЦлеарТеамсАндАссигнментс | Логичка вредност          | **Тачно или** нетачно **·** |
| SourceProject            | Референтни ентитет | Изворни пројекат    |
| Циљ                   | Референтни ентитет | Циљни пројекат    |

Више подразумеваних вредности радњи потражите у чланку [Коришћење Радњи са Wеб АПИ-ја](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>Провере ваљаности

Следеће провере ваљаности су завршене.

1. Нулл проверава и преузима изворне и циљне пројекте како би потврдио постојање оба пројекта у организацији.
2. Систем проверава да ли је циљни пројекат важећи за копирање верификацијом следећих услова:

    - Не постоји претходна активност на пројекту (укључујући избор картице " **Задаци** ") и пројекат је новокреиран.
    - Не постоји претходна копија, није захтеван увоз на овом пројекту, а пројекат нема статус "Неуспешно **·** ".

3. Операција се не позива помоћу ХТТП-а.

## <a name="specify-fields-to-copy"></a>Наведите поља за копирање

Када је акција позвана, **Копирај пројекат** погледаће приказ пројекта **Копирајте колоне пројекта** да би се утврдило која поља треба копирати када се пројекат копира.

### <a name="example"></a>Пример

Следећи пример приказује како се назива copyProjectV3 **прилагођена** радња са скупом **параметара РемовеНамедРесоурцес**.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

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
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
