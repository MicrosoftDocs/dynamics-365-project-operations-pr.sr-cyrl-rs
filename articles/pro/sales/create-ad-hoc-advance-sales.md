---
title: Креирање ад-хок авансне уплате за уговор – једноставно
description: Ова тема пружа информације о креирању аванса за уговор по потреби.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a6bf02c2e2ab2f3c696b1eab1b92a20272187bf5
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181380"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract---lite"></a>Креирање ад-хок авансне уплате за уговор – једноставно

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Microsoft Dynamics 365 Project Operations подржава сценарије фактурисања који укључују претплату и авансе. Процес коришћења **Аванса** у услузи **Project Operations** је сличан **авансним** уговорима. 

Довршите следеће кораке да бисте клијенту фактурисали аванс.

1. Идите на страницу **Уговор за пројекат**, а затим изаберите картицу **Аконтације и аванси**.
2. У подформи која садржи списак свих претходно забележених аванса и авансних плаћања, изаберите **+ Аванс на уговор за нови пројекат**. 

    Отвориће се образац **Брзо креирање** за евидентирање претплате или аванса.
    
3. У табели у наставку наведена су поља за бележење аванса и разматрања која треба имати на уму приликом креирања нових:

    | Поље | Опис | Последични утицај |
    | --- | --- | --- |
    | **Клијент уговора за пројекат** | Ово поље означава којем клијенту на уговору ће се фактурисати за ову аконтацију. | Ако имате више клијената на уговору и желите да фактуришете сваком од њих за одређену аконтацију или авансни износ, ручно креирајте аванс за сваког клијента понаособ. |
    | **Опис** | Опис сврхе или времена аванса који ће вам помоћи да га идентификујете. | Овај опис се приказује у ставки фактуре за овај аванс. |
    | **Износ** | Износ претплате или аванса. | Овај износ се приказује у ставки фактуре за овај аванс. |
    | **Датум фактуре** | Датум на који се клијенту фактурише овај аванс. | Ово је датум за поступак аутоматског креирања фактуре за креирање ставке фактуре за овај аванс. |
    | **Статус фактуре** | Ово је подешавање опције које показује да ли је овај аванс додат радној верзији фактуре за овог клијента. Могуће вредности су следеће:</br>- **Није спремно за фактурисање**</br>- **Спремно за фактурисање** | Када се аванс или претплата означи као **Спремно за фактурисање**, додаје се као време ставке на радној верзији фактуре. Само потпуно фактурисани аванс се може користити за усаглашавање са пројектним трошковима за следећи период фактурисања. |

4. Изаберите **Сачувај и затвори** у дијалогу за брзо креирање за бележење аванса или претплате.