---
title: Копирање пројекта
description: Ова тема пружа информације о копирању пројеката у услузи Dynamics 365 Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: e35dc725e7938e9f59f7151dd1b37500fabf77a4
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908561"
---
# <a name="copy-a-project"></a>Копирање пројекта

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_

У услузи Dynamics 365 Project Operations можете брзо да градите нове пројекте помоћу радње **Копирај пројекат** на обрасцу **Пројекти**. Да бисте копирали пројекат, изаберите пројекат, а затим изаберите **Копирај**. Радња ће копирати:

- Својства пројекта
- Структурну анализу посла
- Чланови пројектног тима
- Процене за пројекат
- Процене трошкова пројекта

## <a name="project-properties"></a>Својства пројекта

Када се пројекат копира, копирају се вредности у следећим пољима:

- Име
- Опис
- Клијент
- Предложак календара
- Валута
- Јединица уговарања
- Менаџер пројекта
- Статус
- Укупан статус пројекта
- Коментари
- Процене
- Процењени датум почетка
- Датум завршетка
- Ангажовање (часови)
- Процењени трошкови рада
- Процењени износ трошкова

## <a name="work-breakdown-structure"></a>Структурна анализа посла

Када се пројекат копира, копира се целокупна структурна анализа посла учитаног ресурса. Именовани ресурс замењује генеричке ресурсе. Ако именовани ресурси немају исто радно време као генерички ресурс, распоред ће се поново израчунати и трајање задатка се може променити.

## <a name="project-team-members"></a>Чланови пројектног тима

Када се пројектни тим копира из изворног пројекта, копирају се генерички ресурси. Доделе генеричких ресурса такође се одржавају као у изворном пројекту. Именовани ресурси ће се претворити у генеричке чланове тима.

## <a name="estimates"></a>Процене

Када се пројекат копира, из изворног пројекта се копирају и ставке процене ресурса и трошкова.