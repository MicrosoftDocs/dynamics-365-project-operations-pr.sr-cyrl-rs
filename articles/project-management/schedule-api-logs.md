---
title: Евиденције распореда пројеката
description: Овај чланак пружа информације и узорке који ће вам помоћи да користите евиденције за планирање пројекта да бисте пратили кварове који су повезани са услугом планирања пројекта и API-јем за планирање пројекта.
author: ruhercul
ms.date: 11/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: c57419642e90e4def01f2cd2474c9e82dc162b86
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923713"
---
# <a name="project-scheduling-logs"></a>Евиденције распореда пројеката

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, једноставну примену – погодбу о предрачунима_, _Project for the Web_

Microsoft Dynamics 365 Project Operations користи [Project for the Web](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) као примарни механизам планирања. Уместо коришћења стандардних Microsoft Dataverse интерфејса за програмирање веб апликација (API-ja), Project Operations користе нове API-је за планирање пројекта за креирање, ажурирање и брисање пројектних задатака, додела ресурса, зависности задатака, контејнере пројеката и чланова пројектних тимова. Међутим, када се операције креирања, ажурирања или брисања програмски извршавају на ентитетима структурне анализе посла (САП), може доћи до грешака. Да би се пратиле ове грешке и историју операција, примењене су две нове административне евиденције: **Скуп операција** и **Услуге планирања пројекта (PSS)**. Да бисте приступили овим евиденцијама, идите на **Поставке** \> **Интеграција распореда**.

Следећа илустрација приказује модел података за евиденције планирања пројекта.

![Модел података за евиденције планирања пројекта.](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>Евиденција скупа операција

Евиденција скупа операција прати извршавање скупа операција који се користи за покретање једне или више операција креирања, ажурирања или брисања операција у групи пројеката, пројектних задатака, додела ресурса, зависности задатака, контејнера пројеката или чланова пројектног тима. Поље **Операција у статусу** приказује општи статус скупа операција. Детаљи корисних података скупа операција се бележе у повезаним записима детаља скупа операција.

### <a name="operation-set"></a>Скуп операција

Следећа табела приказује поља која су повезана са ентитетом **Скуп операција**.

| Назив шеме            | Опис                                                                                                  | DisplayName            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | Датум и време када је скуп операција завршен или није успео.                                                | CompletedOn            |
| msdyn_correlationid   | Вредност за **correlationId** захтева.                                                                  | CorrelationId          |
| msdyn_description     | Опис скупа операција.                                                                        | Опис            |
| msdyn_executedon      | Датум и време извршавања записа.                                                                       | Датум извршавања            |
| msdyn_operationsetId  | Јединствени идентификатор инстанци ентитета.                                                                   | OperationSet           |
| msdyn_Project         | Пројекат који се односи на скуп операција.                                                            | Project                |
| msdyn_projectid       | Вредност за **projectId** захтева.                                                                      | ProjectId (застарело) |
| msdyn_projectName     | Није применљиво.                                                                                              | Није примењиво         |
| msdyn_PSSErrorLog     | Јединствени идентификатор евиденције грешака услуге планирања пројекта која је повезана са скупом операција. | PSS евиденција грешака          |
| msdyn_PSSErrorLogName | Није применљиво.                                                                                              | Није примењиво         |
| msdyn_status          | Статус скупа операција.                                                                             | Статус                 |
| msdyn_statusName      | Није применљиво.                                                                                              | Није примењиво         |
| msdyn_useraadid       | ID Azure Active Directory (Azure AD) објекта корисника коме захтев припада.                     | UserAADID              |

### <a name="operation-set-detail"></a>Детаљ скупа операција

Следећа табела приказује поља која су повезана са ентитетом **Детаљ скупа операција**.

| Назив шеме                 | Опис                                                                                 | DisplayName           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | Серијализована Dataverse поља за захтев.                                            | CdsPayload            |
| msdyn_entityname           | Назив ентитета за захтев.                                                     | EntityName            |
| msdyn_httpverb             | Метод захтева.                                                                         | HTTP глагол (застарело) |
| msdyn_httpverbName         | Није применљиво.                                                                             | Није примењиво        |
| msdyn_operationset         | Јединствени идентификатор скупа операција којем запис припада.                      | OperationSet          |
| msdyn_operationsetdetailId | Јединствени идентификатор инстанци ентитета.                                                  | OperationSet детаљ   |
| msdyn_operationsetName     | Није применљиво.                                                                             | Није примењиво        |
| msdyn_operationtype        | Тип операције детаља скупа операција.                                             | OperationType         |
| msdyn_operationtypeName    | Није применљиво.                                                                             | Није примењиво        |
| msdyn_psspayload           | Серијализована поља услуге планирања пројекта за захтев.                           | PssPayload            |
| msdyn_recordid             | Идентификатор записа захтева.                                                       | ID записа             |
| msdyn_requestnumber        | Аутоматски генерисани број који идентификује редослед примања захтева. | Број захтева        |

## <a name="project-scheduling-service-error-logs"></a>Евиденције грешака услуге планирања пројекта

Евиденције грешака услуге планирања пројекта евидентира грешке до којих долази када услуга планирања пројекта покуша операцију **Сачувај** или **Отвори**. Постоје три подржана сценарија у којима се генеришу ове евиденције:

- Радње које је покренуо корисник критички не успевају (на пример, није могуће креирати доделу због привилегија које недостају).
- Услуга планирања пројекта не може програмски да креира, ажурира, избрише или изврши било коју другу каскадну операцију у ентитету.
- Корисник доживљава грешке када се запис не отвори (на пример, када се пројекат отвори или када се ажурирају информације о члану тима).

### <a name="project-scheduling-service-log"></a>Евиденција услуге планирања пројекта

Следећа табела приказује поља која су обухваћена евиденцијом услуге планирања пројекта.

| Назив шеме          | Опис                                                                    | DisplayName    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | Стек позив изузетка.                                               | Стек позив     |
| msdyn_correlationid | ID корелације грешке.                                               | CorrelationId  |
| msdyn_errorcode     | Поље које се користи за складиштење Dataverse кода грешке или HTTP кода грешке. | Код грешке     |
| msdyn_HelpLink      | Веза до јавне документације за помоћ.                                       | Веза за помоћ      |
| msdyn_log           | Евиденција из услуге планирања пројекта.                                   | Евиденција            |
| msdyn_project       | Пројекат који је повезан са одељком евиденцијом грешака.                             | Project        |
| msdyn_projectName   | Назив пројекта ако ће корисни подаци скупа операција бити задржани. | Није примењиво |
| msdyn_psserrorlogId | Јединствени идентификатор инстанци ентитета.                                     | PSS евиденција грешака  |
| msdyn_SessionId     | ID сесије пројекта.                                                        | ID сесије     |

## <a name="error-log-cleanup"></a>Чишћење евиденције грешака

Подразумевано, и евиденције грешака услуге планирања пројекта и евиденција скупа операција могу да се бришу сваких 90 дана. Сви записи старији од 90 дана биће обрисани. Међутим, променом вредности поља **msdyn_StateOperationSetAge** на страници **Параметри пројекта**, администратори могу да прилагоде опсег чишћења тако да буде између 1 и 120 дана. Доступно је неколико метода за промену ове вредности:

- Прилагодите ентитет **Параметар пројекта** креирањем прилагођене странице и додавањем поља **Старост застарелог скупа операција**.
- Користите кôд клијента који користи [WebApi комплет за развој софтвера (SDK)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord).
- Користите SDK кôд услуге који користи метод Xrm SDK **updateRecord** (референца API-ја клијента) у апликацијама заснованим на моделу. Power Apps обухвата опис и подржане параметре за метод **updateRecord**.

    ```C#
    Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter').then(function (response) {
        parameter = response.entities[0];
        var staleOperationValue = prompt("All records older than (x) days will be deleted, please enter X between 1 to 90 days", 1)
        var newData = {};
        newData.msdyn_projectparameterid = parameter.msdyn_projectparameterid;
        newData.msdyn_staleoperationsetage = parseInt(staleOperationValue);
        Xrm.WebApi.updateRecord("msdyn_projectparameter", parameter.msdyn_projectparameterid, newData).then(
            function success(result) {
                console.log("Project Parameter: Stale Operation Expiry is set to: " + newData.msdyn_staleoperationsetage);
                // perform operations on record update
                Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter')
                .then(function (response2) { console.log("Confirmed Project Parameter: Stale Operation Expiry is set to: " + response2.entities[0].msdyn_staleoperationsetage) });
            },
            function (error) {
                console.log("Failed to Update Project Ednpoint with error: " + error.message);
            // handle error conditions
            }
        );
    });
    ```
