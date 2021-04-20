---
title: Коришћење API-ја за распоред за обављање операција са ентитетима планирања
description: Ова тема пружа информације и примере за коришћење API-ја за распоред.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868147"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Коришћење API-ја за распоред за обављање операција са ентитетима планирања

_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_

> [!IMPORTANT] 
> Неке или све функционалности забележене у овој теми доступне су као део издања верзије за преглед. Садржај и функционалност су подложни променама. 

## <a name="scheduling-entities"></a>Ентитети планирања

API-ји за распоред пружају могућност извршавања операција креирања, ажурирања и брисања помоћу **ентитета планирања**. Тим ентитетима се управља путем механизма за распоређивање у апликацији Project за веб. Креирање, ажурирање и брисање операција помоћу **ентитета планирања** били су ограничени у ранијим издањима услуге Dynamics 365 Project Operations.

Следећа табела даје потпуну листу **ентитета планирања**.

| Назив ентитета  | Логичко име ентитета |
| --- | --- |
| Project | msdyn_project |
| Пројектни задатак  | msdyn_projecttask  |
| Зависност пројектног задатка  | msdyn_projecttaskdependency  |
| Додела ресурса | msdyn_resourceassignment |
| Контејнер пројекта  | msdyn_projectbucket |
| Члан пројектног тима | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

Ентитет OperationSet је образац јединице рада који се може користити када се у трансакцији мора обрадити неколико захтева који утичу на распоред.

## <a name="schedule-apis"></a>API-ји за распоред

Следи листа актуелних API-ја за распоред.

- **msdyn_CreateProjectV1**: Овај API се може користити за креирање пројекта. Пројекат и подразумевани контејнер пројекта креирају се одмах.
- **msdyn_CreateTeamMemberV1**: Овај API се може користити за креирање члана пројектног тима. Евиденција члана тима креира се одмах.
- **msdyn_CreateOperationSetV1**: Овај API се може користити за заказивање неколико захтева који се морају извршити у оквиру трансакције.
- **msdyn_PSSCreateV1**: Овај API се може користити за креирање ентитета. Ентитет може бити било који ентитет планирања који подржава операцију креирања.
- **msdyn_PSSUpdateV1**: Овај API се може користити за ажурирање ентитета. Ентитет може бити било који ентитет планирања који подржава операцију ажурирања.
- **msdyn_PSSDeleteV1**: Овај API се може користити за брисање ентитета. Ентитет може бити било који ентитет планирања који подржава операцију брисања.
- **msdyn_ExecuteOperationSetV1**: Овај API се користи за извршавање свих операција унутар датог скупа операција.

## <a name="using-schedule-apis-with-operationset"></a>Коришћење API-ја распореда са OperationSet ентитетом

Пошто се записи са **CreateProjectV1** и **CreateTeamMemberV1** креирају одмах, ови API-ји се не могу користити у **OperationSet ентитету** директно. Међутим, API можете користити за креирање потребних записа, креирајте **OperationSet ентитет**, а затим користите ове унапред креиране записе у **OperationSet ентитету**.

## <a name="supported-operations"></a>Подржане операције

| Ентитет планирања | Направи | Ажурирање | Delete | Важна разматрања |
| --- | --- | --- | --- | --- |
Пројектни задатак | Да | Да | Да | Ниједно |
| Зависност пројектног задатка | Да | Да | | Записи зависности пројектних задатака се не ажурирају. Уместо тога, стари запис може да се избрише и може да се креира нови запис. |
| Додела ресурса | Да | Да | | Нису подржане операције са следећим пољима: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**. Записи о додели ресурса се не ажурирају. Уместо тога, стари запис може да се избрише и може да се креира нови запис. |
| Контејнер пројекта | Није применљиво | Није применљиво | Није применљиво | Подразумевани контејнер се креира се помоћу API-ја **CreateProjectV1**. |
| Члан пројектног тима | Да | Да | Да | За операцију креирања користите API **CreateTeamMemberV1**. |
| Project | Да | Да | Није применљиво | Нису подржане операције са следећим пољима: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**. |

Ови API-ји се могу позивати са објектима ентитета који укључују прилагођена поља.

Својство ID је опционално. Ако је обезбеђено, систем покушава да га користи и избацује изузетак ако не може да га користи. Ако није обезбеђено, систем ће га генерисати.

## <a name="limitations-and-known-issues"></a>Ограничења и познати проблеми
Следи листа ограничења и познатих проблема:

- API-је за распоред могу да користе само **корисници са лиценцом за Microsoft Project.** Не могу их користити:
    - Корисници апликације
    - Корисници система
    - Корисници интеграције
    - Остали корисници који немају потребну лиценцу
- Сваки **OperationSet ентитет** може да има највише 100 операција.
- Сваки корисник може да има највише 10 отворених **OperationSet ентитета**.
- Project Operations тренутно подржава максимално 500 укупних задатака на пројекту.
- Статус грешке и евиденције грешака **OperationSet ентитета** тренутно нису доступне.
- API-ји за распоред су у верзији за јавни преглед. Microsoft не подржава употребу ових API-ја у производном окружењу.

## <a name="sample-scenario"></a>Пример сценарија

У овом сценарију, креираћете пројекат, члана тима, четири задатка и два задатка ресурса. Затим ћете ажурирати један задатак, ажурирати пројекат, избрисати један задатак, избрисати једну доделу ресурса и креирати зависност задатка.

```C#
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>Додатни примери

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };
    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
    return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";
    return project;
}

private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
        task["new_amount"] = 591.34m;
        task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }
    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;
    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);
    return taskDependency;
}

#endregion

#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
