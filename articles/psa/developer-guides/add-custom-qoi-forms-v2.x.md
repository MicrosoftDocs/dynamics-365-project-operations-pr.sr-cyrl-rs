---
title: Додавање нових образаца прилагођених ентитета (Project Service Automation 2. x)
description: Ова тема пружа информације о додавању прилагођених образаца ентитета за могућности за пословање, понуде, поруџбине или фактуре у апликацији Dynamics 365 Project Service Automation 2.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 31986efed81892cc5722cb8f5e292cde14d8843d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144611"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>Додавање нових образаца прилагођених ентитета (Project Service Automation 2. x)

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a>Поље Тип 

Dynamics 365 Project Service Automation се ослања на поље **Тип** (**msdyn\_ordertype**) ентитета Могућност за пословање, Понуда, Поруџбине и Фактура да би направила разлика између верзија ових ентитета **заснованих на послу** и оних **заснованих на ставци** и **услузи**. PSA управља верзијама ових ентитета заснованих на послу. Велики део пословне логике на клијентској страни и на страни сервера решења зависи од поља **Тип**. Због тога је важно да се ово поље покрене са тачном вредношћу приликом креирања ентитета. Нетачна вредност може проузроковати неправилна понашања, а нека пословна логика неће исправно радити.

## <a name="automatic-form-switching"></a>Аутоматско пребацивање образаца

Да би се избегла потенцијална оштећења података и неочекивано понашање који су последица неправилног покретања и уређивања записа ентитета продаје, PSA сада укључује логику за аутоматско пребацивање образаца у унапред дефинисане обрасце. Ова логика преусмерава кориснике на прави образац за рад са верзијом заснованом на послу или било који други тип ентитета могућности за пословање, понуде, поруџбине или фактуре. Када корисник отвори верзију ентитета Могућност за пословање, Понуда, Поруџбине или Фактура, која је засновану на послу, образац се пребацује у **Информације о пројекту**.

Логика аутоматског пребацивања обрасца ослања се на мапирање између вредности **formId** и поља **msdyn\_ordertype** ". Сви унапред дефинисани обрасци су додати том мапирању. Међутим, прилагођени обрасци морају се ручно додати да би се назначило којом верзијом ентитета би требало да управљају. Ово је засновано на пољу **msdyn\_ordertype**. Ако се пребацивање обрасца не налази на мапирању, логика ће се пребацити на унапред дефинисани образац, на основу вредности сачуване у пољу **msdyn\_ordertype** ентитета.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>Додавање прилагођених образаца и укључивање логике промене обрасца

Следећи пример приказује како се додаје прилагођени образац, **Моје информације о пројекту**, тако да функционише са могућностима за пословање заснованим на послу. Исти процес се користи за додавање прилагођених образаца како би функционисале са понудама, поруџбинама и фактурама.

Следите ове кораке да бисте креирали прилагођену верзију обрасца **Информације о пројекту**.

1. У ентитету Могућност за пословање отворите образац **Информације о пројекту** и сачувајте копију под именом **Моје информације о пројекту**.
2. Отворите нови образац, а затим у својствима проверите да ли се ту налазе скрипте за покретање обрасца из обрасца **Информације о пројекту**. 

    > [!IMPORTANT]
    > Немојте уклањати скрипте. У супротном, неки подаци могу бити неправилно покренути.

3. Проверите да се поље **Тип** (**msdyn\_ordertype**) налази у обрасцу. 

    > [!IMPORTANT]
    > Немојте уклањати ово поље. У супротном, скрипте за покретања неће успети.

4. Пронађите вредност **formId** новог обрасца. Овај корак можете да обавите на два начина:

    - Извезите образац **Моје информације о пројекту** као део некомплетног решења, а затим потражите вредност **formId** у датотеци customization.xml у извезеном решењу.
    - Отворите образац **Моје информације о пројекту** у уређивачу образаца, а затим потражите универзални јединствени идентификатор (GUID) поред параметра **fromId** у URL адреси, као што је приказано на следећој илустрацији.

    ![Вредност formId новог обрасца у URL адреси](media/how-to-add-custom-forms-in-v2.0.png)

5. Креирајте мапирање **msdyn\_ordertype** за вредност **formId** уређивањем веб-ресурса msdyn\_/Документ продаје/PSSalesDocumentCustomFormIds.js. Уклоните кôд из ресурса и замените га следећим кодом.

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. Сачувајте, а затим објавите прилагођавања.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]