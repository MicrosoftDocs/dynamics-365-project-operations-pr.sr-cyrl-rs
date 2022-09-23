---
title: Коришћење API-ја за распоред пројеката за извођење операција са ентитетима распоређивања
description: Овај чланак обезбеђује информације и узорке за коришћење АПИ-ја са планом пројекта.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541143"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Коришћење API-ја за распоред пројеката за извођење операција са ентитетима распоређивања

_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_


**Ентитети планирања**

API-ји за распоред пројеката пружају могућност извршавања операција креирања, ажурирања и брисања помоћу **ентитета за заказивање**. Тим ентитетима се управља путем механизма за распоређивање у апликацији Project за веб. Креирање, ажурирање и брисање операција помоћу **ентитета планирања** били су ограничени у ранијим издањима услуге Dynamics 365 Project Operations.

Следећа табела даје потпуну листу ентитета за распоред пројеката.

| **Име ентитета**         | **Логичко име ентитета**     |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Пројектни задатак            | msdyn_projecttask           |
| Зависност пројектног задатка | msdyn_projecttaskdependency |
| Додела ресурса     | msdyn_resourceassignment    |
| Контејнер пројекта          | msdyn_projectbucket         |
| Члан пројектног тима     | msdyn_projectteam           |
| Листе за проверу пројекта      | msdyn_projectchecklist      |
| Ознака пројекта           | msdyn_projectlabel          |
| Пројектни задатак на ознаку   | msdyn_projecttasktolabel    |
| Спринт пројекта          | msdyn_projectsprint         |

**OperationSet**

Ентитет OperationSet је образац јединице рада који се може користити када се у трансакцији мора обрадити неколико захтева који утичу на распоред.

**API-ји за распоред пројеката**

Следи листа актуелних API-ја за распоред пројеката.

| **Апи**                                 | Опис                                                                                                                       |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | Овај АПИ се користи за креирање пројекта. Пројекат и подразумевана кофа пројекта се креирају одмах.                         |
| **msdyn_CreateTeamMemberV1**            | Овај АПИ се користи за креирање члана пројектног тима. Евиденција члана тима креира се одмах.                                  |
| **msdyn_CreateOperationSetV1**          | Овај АПИ се користи за планирање неколико захтева који се морају извршити у оквиру трансакције.                                        |
| **msdyn_PssCreateV1**                   | Овај АПИ се користи за креирање ентитета. Ентитет може бити било који ентитет распоређивања пројекта који подржава операцију креирања. |
| **msdyn_PssUpdateV1**                   | Овај АПИ се користи за ажурирање ентитета. Ентитет може бити било који од ентитета за планирање пројекта који подржавају операцију ажурирања  |
| **msdyn_PssDeleteV1**                   | Овај АПИ се користи за брисање ентитета. Ентитет може бити било који ентитет распоређивања пројекта који подржава операцију брисања. |
| **msdyn_ExecuteOperationSetV1**         | Овај АПИ се користи за извршавање свих операција у оквиру датог скупа операција.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | Овај АПИ се користи за ажурирање планиране радне контуре додељивање ресурса.                                                        |



**Коришћење API-ја за распоред пројеката са ентитетом OperationSet**

Пошто се записи са **CreateProjectV1** и **CreateTeamMemberV1** креирају одмах, ови API-ји се не могу користити у **OperationSet ентитету** директно. Међутим, API можете користити за креирање потребних записа, креирајте **OperationSet ентитет**, а затим користите ове унапред креиране записе у **OperationSet ентитету**.

**Подржане операције**

| **Ентитет планирања**   | **Направи** | **Ажурирање** | **Delete** | **Важна разматрања**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Пројектни задатак            | Да        | Да        | Да        | Поља **"Прогрес** ", " **Довршавање** напора" **и "ЕффортРемаининг** " могу да се уређују у пројекту за Wеб, али се не могу уређивати у операцијама пројекта.                                                                                                                                                                                             |
| Зависност пројектног задатка | Да        | No         | Да        | Записи зависности пројектних задатака се не ажурирају. Уместо тога, може се избрисати стари запис и креирати нови запис.                                                                                                                                                                                                                                 |
| Додела ресурса     | Да        | Да\*      | Да        | Нису подржане операције са следећим пољима: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**. Записи о додели ресурса се не ажурирају. Уместо тога, стари запис се може избрисати и може се креирати нови запис. Обезбеђен је посебан АПИ за ажурирање контура додељивање ресурса. |
| Контејнер пројекта          | Да        | Да        | Да        | Подразумевана кофа се креира помоћу **АПИ-ја CreateProjectV1**. Подршка за креирање и брисање кофа пројекта је додата у издању Упдате Релеасе 16.                                                                                                                                                                                                   |
| Члан пројектног тима     | Да        | Да        | Да        | За операцију креирања користите API **CreateTeamMemberV1**.                                                                                                                                                                                                                                                                                           |
| Project                 | Да        | Да        |            | Нису подржане операције са следећим пољима: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.                                                                                       |
| Листе за проверу пројекта      | Да        | Да        | Да        |                                                                                                                                                                                                                                                                                                                                                         |
| Ознака пројекта           | No         | Да        | No         | Имена ознака се могу променити. Ова функција је доступна само за Пројекат за Wеб                                                                                                                                                                                                                                                                      |
| Пројектни задатак на ознаку   | Да        | No         | Да        | Ова функција је доступна само за Пројекат за Wеб                                                                                                                                                                                                                                                                                                  |
| Спринт пројекта          | Да        | Да        | Да        | Поље **"Старт** " мора имати датум ранији од поља **Заврши**. Спринтеви за исти пројекат не могу да се преклапају једни са другима. Ова функција је доступна само за Пројекат за Wеб                                                                                                                                                                    |




Својство ID је опционално. Ако је обезбеђено, систем покушава да га користи и избацује изузетак ако не може да га користи. Ако није обезбеђено, систем ће га генерисати.

**Ограничења и познати проблеми**

Следи листа ограничења и познатих проблема:

-   АПИ -је за план пројекта могу да користе само корисници **са лиценцом за Мицрософт Пројецт**. Не могу их користити:
    -   Корисници апликације
    -   Корисници система
    -   Корисници интеграције
    -   Остали корисници који немају потребну лиценцу
-   Сваки **OperationSet ентитет** може да има највише 100 операција.
-   Сваки корисник може да има највише 10 отворених **OperationSet ентитета**.
-   Project Operations тренутно подржава максимално 500 укупних задатака на пројекту.
-   Свака операција ажурирања контуре додељивања ресурса се рачуна као једна операција.
-   Свака листа ажурираних контура може да садржи највише 100 временских исечака.
-   Статус грешке и евиденције грешака **OperationSet ентитета** тренутно нису доступне.
-   Постоји највише 400 спринта по пројекту.
-   [Ограничења и границе за пројекте и задатке](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   Ознаке су тренутно доступне само за Пројекат за Wеб.

**Руковање грешкама**

-   Да бисте прегледали грешке генерисане из скупова операција, идите на **Подешавања** \> **Закажи интеграцију** \> **Скупови операција**.
-   Да бисте прегледали грешке које је генерисала услуга распореда пројеката, идите на **Подешавања** \> **Интеграција распореда** \> **PSS евиденције грешака**.

**Уређивање контура доделе ресурса**

За разлику од свих других АПИ-ја за планирање пројекта који ажурирају ентитет, АПИ за додељивање ресурса је искључиво одговоран за исправке једног поља, msdyn_plannedwork, у једном ентитету, msydn_resourceassignment.

Дати режим распореда је:

-   **фиксне јединице**
-   календар пројекта је 9-5p је 9-5pst, Мон, Туе, Тхурс, Петак (БЕЗ ПОСЛА СРЕДОМ)
-   а календар ресурса је 9-1p ПСТ Мон то Фри

Овај задатак је за недељу дана, иетири сата дневно. То је зато што је календар ресурса од 9-1 ПСТ или четири сата дневно.

| &nbsp;     | Задатак | Датум почетка | Датум завршетка  | Количина | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 радник |  T1  | 6/13/2022  | 6/17/2022 | 20       | 4.         | 4.         | 4.         | 4.         | 4.         |

На пример, ако желите да радник ради само три сата сваког дана ове седмице и дозволи један сат за друге задатке.

#### <a name="updatedcontours-sample-payload"></a>Ажурирани Узорак товара:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

Ово је додела након што се покрене АПИ распореда контура ажурирања.

| &nbsp;     | Задатак | Датум почетка | Датум завршетка  | Количина | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 радник | T1   | 6/13/2022  | 6/17/2022 | 15       | 3.         | 3.         | 3.         | 3.         | 3.         |


**Пример сценарија**

У овом сценарију, креираћете пројекат, члана тима, четири задатка и два задатка ресурса. Затим ћете ажурирати један задатак, ажурирати пројекат, избрисати један задатак, избрисати једну доделу ресурса и креирати зависност задатка.

```csharp
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
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

** Додатни узорци

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
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
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
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
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
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
/// </summary>
/// <param name="operationSetId">operationSet id</param>
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
/// <param name="operationSetId">operationSet id</param>
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
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
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
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
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
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
