---
title: Додавање нових образаца прилагођених ентитета (Project Service Automation 2. x)
description: Ова тема пружа информације о додавању прилагођених образаца ентитета за могућности за пословање, понуде, поруџбине или фактуре у апликацији Dynamics 365 Project Service Automation 2.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 9eb9fc5e-4c7d-466c-9362-fdb0faa30506
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
ms.openlocfilehash: 2bd955ad3eb26d31676ac4ad387baccaee913cd2
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755287"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="d217f-103">Додавање нових образаца прилагођених ентитета (Project Service Automation 2. x)</span><span class="sxs-lookup"><span data-stu-id="d217f-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

## <a name="type-field"></a><span data-ttu-id="d217f-104">Поље Тип</span><span class="sxs-lookup"><span data-stu-id="d217f-104">Type field</span></span> 

<span data-ttu-id="d217f-105">Dynamics 365 Project Service Automation се ослања на поље **Тип** (**msdyn\_ordertype**) ентитета Могућност за пословање, Понуда, Поруџбине и Фактура да би направила разлика између верзија ових ентитета **заснованих на послу** и оних **заснованих на ставци** и **услузи**.</span><span class="sxs-lookup"><span data-stu-id="d217f-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="d217f-106">PSA управља верзијама ових ентитета заснованих на послу.</span><span class="sxs-lookup"><span data-stu-id="d217f-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="d217f-107">Велики део пословне логике на клијентској страни и на страни сервера решења зависи од поља **Тип**.</span><span class="sxs-lookup"><span data-stu-id="d217f-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="d217f-108">Због тога је важно да се ово поље покрене са тачном вредношћу приликом креирања ентитета.</span><span class="sxs-lookup"><span data-stu-id="d217f-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="d217f-109">Нетачна вредност може проузроковати неправилна понашања, а нека пословна логика неће исправно радити.</span><span class="sxs-lookup"><span data-stu-id="d217f-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="d217f-110">Аутоматско пребацивање образаца</span><span class="sxs-lookup"><span data-stu-id="d217f-110">Automatic form switching</span></span>

<span data-ttu-id="d217f-111">Да би се избегла потенцијална оштећења података и неочекивано понашање који су последица неправилног покретања и уређивања записа ентитета продаје, PSA сада укључује логику за аутоматско пребацивање образаца у унапред дефинисане обрасце.</span><span class="sxs-lookup"><span data-stu-id="d217f-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="d217f-112">Ова логика преусмерава кориснике на прави образац за рад са верзијом заснованом на послу или било који други тип ентитета могућности за пословање, понуде, поруџбине или фактуре.</span><span class="sxs-lookup"><span data-stu-id="d217f-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="d217f-113">Када корисник отвори верзију ентитета Могућност за пословање, Понуда, Поруџбине или Фактура, која је засновану на послу, образац се пребацује у **Информације о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="d217f-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="d217f-114">Логика аутоматског пребацивања обрасца ослања се на мапирање између вредности **formId** и поља **msdyn\_ordertype** ".</span><span class="sxs-lookup"><span data-stu-id="d217f-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="d217f-115">Сви унапред дефинисани обрасци су додати том мапирању.</span><span class="sxs-lookup"><span data-stu-id="d217f-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="d217f-116">Међутим, прилагођени обрасци морају се ручно додати да би се назначило којом верзијом ентитета би требало да управљају.</span><span class="sxs-lookup"><span data-stu-id="d217f-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="d217f-117">Ово је засновано на пољу **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="d217f-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="d217f-118">Ако се пребацивање обрасца не налази на мапирању, логика ће се пребацити на унапред дефинисани образац, на основу вредности сачуване у пољу **msdyn\_ordertype** ентитета.</span><span class="sxs-lookup"><span data-stu-id="d217f-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="d217f-119">Додавање прилагођених образаца и укључивање логике промене обрасца</span><span class="sxs-lookup"><span data-stu-id="d217f-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="d217f-120">Следећи пример приказује како се додаје прилагођени образац, **Моје информације о пројекту**, тако да функционише са могућностима за пословање заснованим на послу.</span><span class="sxs-lookup"><span data-stu-id="d217f-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="d217f-121">Исти процес се користи за додавање прилагођених образаца како би функционисале са понудама, поруџбинама и фактурама.</span><span class="sxs-lookup"><span data-stu-id="d217f-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="d217f-122">Следите ове кораке да бисте креирали прилагођену верзију обрасца **Информације о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="d217f-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="d217f-123">У ентитету Могућност за пословање отворите образац **Информације о пројекту** и сачувајте копију под именом **Моје информације о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="d217f-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="d217f-124">Отворите нови образац, а затим у својствима проверите да ли се ту налазе скрипте за покретање обрасца из обрасца **Информације о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="d217f-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="d217f-125">Немојте уклањати скрипте.</span><span class="sxs-lookup"><span data-stu-id="d217f-125">Don't remove the scripts.</span></span> <span data-ttu-id="d217f-126">У супротном, неки подаци могу бити неправилно покренути.</span><span class="sxs-lookup"><span data-stu-id="d217f-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="d217f-127">Проверите да се поље **Тип** (**msdyn\_ordertype**) налази у обрасцу.</span><span class="sxs-lookup"><span data-stu-id="d217f-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="d217f-128">Немојте уклањати ово поље.</span><span class="sxs-lookup"><span data-stu-id="d217f-128">Don't remove this field.</span></span> <span data-ttu-id="d217f-129">У супротном, скрипте за покретања неће успети.</span><span class="sxs-lookup"><span data-stu-id="d217f-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="d217f-130">Пронађите вредност **formId** новог обрасца.</span><span class="sxs-lookup"><span data-stu-id="d217f-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="d217f-131">Овај корак можете да обавите на два начина:</span><span class="sxs-lookup"><span data-stu-id="d217f-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="d217f-132">Извезите образац **Моје информације о пројекту** као део некомплетног решења, а затим потражите вредност **formId** у датотеци customization.xml у извезеном решењу.</span><span class="sxs-lookup"><span data-stu-id="d217f-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="d217f-133">Отворите образац **Моје информације о пројекту** у уређивачу образаца, а затим потражите универзални јединствени идентификатор (GUID) поред параметра **fromId** у URL адреси, као што је приказано на следећој илустрацији.</span><span class="sxs-lookup"><span data-stu-id="d217f-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![Вредност formId новог обрасца у URL адреси](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="d217f-135">Креирајте мапирање **msdyn\_ordertype** за вредност **formId** уређивањем веб-ресурса msdyn\_/Документ продаје/PSSalesDocumentCustomFormIds.js.</span><span class="sxs-lookup"><span data-stu-id="d217f-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="d217f-136">Уклоните кôд из ресурса и замените га следећим кодом.</span><span class="sxs-lookup"><span data-stu-id="d217f-136">Remove the code from the resource, and replace it with the following code.</span></span>

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

6. <span data-ttu-id="d217f-137">Сачувајте, а затим објавите прилагођавања.</span><span class="sxs-lookup"><span data-stu-id="d217f-137">Save and then publish the customizations.</span></span>
