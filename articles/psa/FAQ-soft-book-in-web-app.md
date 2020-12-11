---
title: Како да „услово резервишете“ ресурсе у апликацији у верзији 2.x?
description: У овом чланку описано је како да условно резервишете чланове пројектног тима уз помоћ програма Project Service.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a35799b422fa338c2666e1b2aa11bc2a54f5cce3
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122271"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a>Како да „условно резервишем“ ресурсе у веб апликацији (апликација Project Service у верзији v2.x)?

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Условно можете да распоредите или „условно резервишете“ ресурс у пројектни тим како бисте приказали да намеравате да доделите ресурс пројекту. Условне резервације не троше доступни капацитет ресурса. Условно резервисани чланови тима не могу бити додељени пројектним задацима. Само ресурси који имају статус Фиксно резервисани и тип примене Примењено могу бити додељени задацима (под претпоставком да имају довољно фиксно резервисаних радних часова да покрију ангажовање за доделу).

Условно резервисани чланови тима се приказују у координатној мрежи Члан тима са условно резервисаним часовима приказаним у колони Условно резервисање. Приказују се и на табели распореда. Поново, они не означавају никакво коришћење капацитета, јер условно резервисање не користи капацитет ресурса.

Постоје три начина да условно резервишете члана тима за пројекат помоћу програма Project Service у верзији 2.x. Можете условно да резервишете са табелом распореда, да користите функцију Одржавање резервација или да креирате генерички ресурс. Ови начини су описани у наставку.

## <a name="soft-book-with-the-schedule-board"></a>Условно резервисање са табелом распореда

Да бисте условно резервисали помоћу табеле распореда, пратите ову процедуру: 
1. Отвори табелу распореда.
2. Изаберите картицу Пројекат на дну табле Захтеви за резервацију у оквиру табле распореда.
3. Пронађите пројекат за који желите да условно резервишете ресурс. Ако имате више пројеката, кликните на заглавље колоне Пројекат, а затим пронађите свој пројекат помоћу филтера.
4. Кликните на пројекат, а затим га превуците на координатну мрежу времена ресурса.
5. То отвара таблу Креирање резервације ресурса са десне стране. Подесите датуме почетка и завршетка, изаберите Статус резервације као Условно и подесите часове. 
6. Кликните на Резервиши.
7. Натраг на пројекту, ресурс ће се сада приказивати као члан тима са условно резервисаним часовима у колони Условно резервисање.

Имајте на уму да не можете да их доделите задацима у структурној анализи посла (САП) јер ресурси морају да буду фиксно резервисани за тим да би били додељени.

## <a name="soft-book-using-the-maintain-bookings-feature"></a>Условно резервисање коришћењем функције Одржавање резервација

Да бисте условно резервисали помоћу Одржавања резервација, пратите ову процедуру:
1. Са мреже члана тима, кликните на Нови.
2. Изаберите ресурс који је могуће резервисати, улогу, од/до.
3. Изаберите начин доделе који није Ниједно:
- Пуни капацитет
- Капацитет у процентима
- Равномерно распоређивање по сатима
- Почетно оптерећење по часовима
4. Кликните на Сачувај. Видећете ресурс на мрежи тима, а његове часове означене као Фиксне.
5. Одржите резервације ресурса кликом на Одржавање резервација.
6. Када се отвори табела распореда, развијте ресурс да бисте приказали његове резервације. Видећете резервацију означену као „Фиксна“.
7. Кликните десним тастером миша на резервацију, у оквиру опције „Промена статуса“, изаберите „Условно резервиши“ и затим „Условно“. Статус резервације је сада „Условна“.
8. Након затварања табеле распореда, видећете да су сати за ресурс промењени из „Фиксни“ на „Условни“ на мрежи члана тима.
Имајте у виду да ако фиксно резервишете ресурс за тима, а затим му доделите задатке у САП-у, када користите одржавање резервација да бисте променили статус из „Фиксна“ у „Условна“, уклонићете доделе из задатака за тај ресурс, јер само фиксно резервисани ресурси могу бити додељени задацима.

## <a name="soft-book-by-creating-a-generic-resource"></a>Условно резервисање креирањем генеричког ресурса

Условно резервисање можете да креирате генерисањем генеричког члана тима, испуњавањем са табелом распореда или Захтевом за ресурс и променом типа током резервације.
То можете да урадите помоћу следеће процедуре:

1. У САП-у пројекта доделите улоге задацима за које желите да генеришете генеричке чланове тима.
2. Кликните на Генерисање пројектног тима.
3. На мрежи члана пројектног тима изаберите генерички ресурс и кликните на дугме „Резервиши“.
4. На табели распореда, изаберите ресурс који желите да резервишете.
5. На табли „Креирање резервације ресурса“ табеле распореда, промените Статус резервације на „Условна“.
6. Кликните на дугме „Резервиши“ и „Резервиши и изађи“.

Након затварања табеле распореда, видећете да је изабрани ресурс додат у тим са условно резервисаним, као и са додељеним часовима. Видећете и да генерички ресурс остаје у тиму као индикатор да су задаци додељени члану тима који је условно резервисан.

Када будете спремни да промените ресурс условно резервисаног члана тима у фиксно резервисаног члана тима како бисте могли да му додељујете задатке, поступите на следећи начин:

1. Изаберите тај ресурс и кликните на дугме „Одржавање резервација“.
2. Када се отвори табела распореда, развијте ресурс да бисте приказали његове резервације. Видећете да је резервација означена као „Условна“.
3. Кликните десним тастером миша на резервацију, у оквиру опције „Промена статуса“, изаберите „Фиксно резервиши“ и затим „Фиксно“. Статус резервације је сада „Фиксно“.
4. Након затварања табеле распореда, видећете да су сати за ресурс промењени из „Фиксни“ на „Условни“ на мрежи члана тима. Сада можете да доделите ресурс задацима (уколико постоји усклађеност између фиксно резервисаних часова и часова ангажовања задатка за доделу). Имајте у виду да ако сте пратили кораке испуњења генеричког ресурса у ставци бр. 3 изнад, када промените статус условно резервисаног ресурса у фиксно резервисани, генерички члан тима се уклања из тима.