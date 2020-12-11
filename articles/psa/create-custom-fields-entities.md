---
title: Креирање прилагођених поља и ентитета
description: Ова тема објашњава како се креирају скупови опција и ентитети у решењу платформе Power Apps.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 442ff9cf2206bec307cea7ff30b9266502d8f77b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084041"
---
# <a name="create-custom-fields-and-entities"></a>Креирање прилагођених поља и ентитета 

Обавите следеће кораке када желите да креирате прилагођени скуп опција или ентитет на Power Apps платформи.  
Процедуре у овој теми би требало да буду завршене коришћењем веб интерфејса апликације Project Service Automation (PSA).

> [!IMPORTANT]
> Препоручује се да се све промене димензије прилагођене цене уносе у одвојеном решењу. Ова важна најбоља пракса пружа флексибилност у будућности за ажурирање или уклањање промена по потреби, помоћи ће при поновној употреби посла и олакшава прилагођавање ових промена другој инстанци. Након што унесете све потребне промене, извезите ово решење као **Комплетно решење** и увезите га у друге инстанце да бисте поново користили подешавање цена.

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>Креирање прилагођених поља и скупова опција у решењу за димензије одређивања цена

Димензија одређивања цена може бити скуп опција или ентитет. И једно и друго морате да креирате у решењу за одређивање цена. Кораци у овој процедури објашњавају како да креирате димензије засноване на ентитетима и димензије засноване на скупу опција.

### <a name="entity-based-dimensions"></a>Димензије засноване на ентитетима

1. У PSA кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**.
2. У левом окну за навигацију истраживача решења изаберите **Ентитети**.
3. Кликните на **Нови** да бисте креирали нови ентитет под називом **Стандардна позиција**. Унесите преостале потребне информације, а затим кликните на **Сачувај**.

> ![Дефиниција стандардног ентитета назива](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a>Димензије засноване на скупу опција 
Можете креирати две димензије засноване на скуповима опција. Помоћу поља **Радна локација ресурса** пратите цену радне локације **Код куће** и **На локацији** и користите **Радно време ресурса** са вредностима **Стандардно** и **Прековремено** да бисте применили провизију када се посао заврши.


1. У PSA кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**. 
2. У левом окну за навигацију истраживача решења изаберите **Скупови опција**. 
3. Кликните на **Ново** да бисте креирали нови скуп опција, унесите преостале захтеване информације, а затим кликните на **Сачувај**.

> ![Димензија одређивања цена заснована на скупу опција под називом Радна локација ресурса ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![Димензија одређивања цена заснована на скупу опција под називом Радно време ресурса ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a>Креирање података за димензије засноване на ентитетима

Можете ручно креирати податке за димензије засноване на ентитетима или коришћењем Microsoft Excel позива за увоз или услуге. Користите кораке из ове процедуре да бисте креирали две стандардне позиције, **Инжењер система** и **Виши инжењер система** из димензије засноване на ентитетима **Стандардна позиција**. Ако је обим података које желите да креирате мали, као у следећем примеру, можете да користите стандардни образац.

1. У апликацији PSA, кликните на **Напредна претрага**. Изаберите ентитет **Стандардна позиција** а, а затим кликните на **Резултати**. Биће приказани сви редови у ентитету **Стандардна позиција**.
2. Кликните на дугме **Ново**. У поље **Назив** унесите „Инжењер система“, а затим кликните на **Сачувај**.
3. Затворите образац. 
4. Поновите кораке 1-3 да бисте креирали још једну стандардну позицији „Виши инжењер система“.

> ![Пробни подаци за ентитет Стандардна позиција ](media/ST-data.png)

