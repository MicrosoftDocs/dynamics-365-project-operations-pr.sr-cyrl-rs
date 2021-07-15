---
title: Ручно распоређивање Project Operations Dataverse апликације са подршком за двоструко уписивање
description: Ова тема објашњава како да ручно примените Project Operations Dataverse апликацију тако да подржава двоструко уписивање.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/18/2021
ms.locfileid: "6274026"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a>Ручно распоређивање Project Operations Dataverse апликације са подршком за двоструко уписивање

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Ова тема објашњава како да ручно примените апликацију Microsoft Dynamics 365 Project Operations на платформи Microsoft Dataverse тако да подржава двоструко уписивање. Project Operations открива конфигурацију окружења и додаје додатну подршку за двоструко уписивање ако су испуњени предуслови.

Током примене преко услуге Microsoft Dynamics Lifecycle Services (LCS), ако сте следили упутства у овој теми, можете прескочити примену Microsoft Power Platform интеграције (раније познате као Common Data Service окружење).

Процес примене услуге Project Operations на платформи Dataverse тако да подржава двоструко уписивање има четири главна корака:

1. [Креирање новог окружења на платформи Dataverse које подржава двоструко уписивање](#create).
2. [Додавање предуслова за двоструко уписивање у окружење](#prerequisites).
3. [Додавање апликације Project Operations Dataverse](#dataverse).
4. [Повезивање окружења](#link).

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a>Креирање новог окружења на платформи Dataverse које подржава двоструко уписивање

Да бисте довршили ову процедуру, морате се пријавити као администратор.

1. Отворите [Power Platform центар администрације](https://admin.powerplatform.com) и пријавите се као администратор.
2. Креирајте ново окружење и именујте га.
3. Изаберите тип окружења. Ако сте се пријавили за понуду пробне верзије, изаберите **Пробна верзија (заснована на претплати)**.
4. Потврдите регион примене.
5. Омогућите опцију **Креирање базе података за ово окружење**. 
6. Потврдите језик, а затим потврдите да се валута подудара са валутом за ваше Finance and Operations апликације.
7. Омогућите **Dynamics 365 апликације** и потврдите да је поље **Аутоматски примени ове апликације** подешено на **Ниједна**.
8. Додајте безбедносну групу ако је потребна безбедносна група.
9. Изаберите **Сачувај** да бисте креирали окружење.
10. Сачекајте док се примена не заврши и окружење не достигне статус **Спремно**.

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a>Додавање предуслова за двоструко уписивање у окружење

Подршка за двоструко уписивање укључује додатна поља која се додају кључним ентитетима, као што је ентитет **Предузеће**. Ако додајете подршку за двоструко уписивање у постојеће окружење, можда ћете морати да ажурирате податке да бисте га омогућили. За информације о начину покретања података, погледајте чланак [Подаци за покретање предузећа](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data). За више информација о двоструком уписивању, погледајте чланак [Системски захтеви за двоструко уписивање](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).

Довршите овај поступак да бисте додали предуслове за двоструко уписивање у своје окружење.

1. Отворите окружење које сте управо креирали, а затим идите у **Ресурс** \> **Dynamics 365 апликације**.
2. Изаберите **Основно решење са двоструким уписивањем** на листи апликација и инсталирајте га.
3. Сачекајте док се инсталација не заврши. Затим изаберите **Решење оркестрације апликације са двоструким уписивањем** на листи апликација и инсталирајте га.

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a>Додавање Project Operations Dataverse апликације

Ову процедуру можете довршити само ако сте завршили претходне процедуре пре него што сте инсталирали Project Operations. Током инсталације, систем анализира конфигурацију окружења и додаје подршку за двоструко уписивање ако је потребно.

1. Отворите окружење које сте раније креирали, а затим идите у **Ресурс** \> **Dynamics 365 апликације**.
2. Изаберите **Microsoft Dynamics 365 Project Operations** на листи апликација и инсталирајте је.

## <a name="link-your-environments"></a><a name="link"></a>Повезивање окружења

Када се Dataverse окружење примени, можете подесити везу у својим Finance and Operations апликацијама. Следите кораке у чланку [Коришћење чаробњака за двоструко уписивање ради повезивања окружења](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).