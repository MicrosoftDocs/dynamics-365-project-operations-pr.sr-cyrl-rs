---
title: Резервације ресурса и како су оне повезане са доделом задатака
description: Ова тема пружа информације о томе како управљати именованим ресурсима, резервацијама ресурса и доделама задатака, као и какав је њихов међусобни однос.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c4b976b49bd643bc7a774a86b1ba89bd76d7c916
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125026"
---
# <a name="resource-bookings-and-how-they-relate-to-task-assignments"></a>Резервације ресурса и како су оне повезане са доделом задатака


Именовани ресурси могу бити резервисани за пројектни тим и додељени пројектним задацима на два начина:

- Ресурс може бити директно резервисан за пројекат, а затим додељен пројектним задацима.
- Задаци могу бити додељени генеричком ресурсу, који се затим користе за проналажење и замену генеричког ресурса именованим ресурсом. 

У оба случаја, чим резервисања ресурса резервише капацитет ресурса.

Менаџер пројекта који планира пројекат је власник плана и распореда пројекта. Коришћењем генеричког ресурса за доделу, а затим генерисањем захтева за ресурс из њега, менаџер пројекта може да резервише ресурсе за пројекат помоћу скица наведених у плану пројекта. Он може да резервише ресурсе за пројекат, а затим да им додељује задатке. Међутим, не постоји ниједан начин да усклади скице резервације са скицама задатака. Резервације не утичу на распоред пројекта.

Узмите за пример сложени пројекат са више задатака који се преклапају на којима више ресурса истог типа морају истовремено да раде. Ако је ресурсу задата контура која се разликује од контуре скупа њихових додела, тешко је изменити задатке како би се уклопили у контуру резервација за њихове изоловане задатке и њихове првобитне контуре.

У примеру у наставку, укупно ангажовање потребно за исти ресурс из скупа од четири задатка је 62 сата током двонедељног периода, а постоји одређена контура. Ако је ресурс Бранко резервисан за 62 радна сата током те исте две седмице, али са другом контуром, захтев и резервације су усклађени.

| **Контуре задатка**    | **Укупно часова** | пон 6/4 | уто 6/5 | сре 6/6 | чет 6/7 | пет 6/8 | суб 6/9 | не 6/10 | пон 6/11 | уто 6/12 | сре 6/13 | чет 6/14 | пет 6/15 |
|----------------------|-----------------|--------|--------|--------|--------|--------|--------|---------|---------|---------|---------|---------|---------|
| Задатак 1               | 24              | 8      | 8      | 4      |        |        |        |         |         |         | 4       |         |         |
| Задатак 2               | 16              |        |        | 4      | 4      |        |        |         | 8       |         |         |         |         |
| Задатак 3               | 1.0.              |        |        |        |        | 4      |        |         |         | 4       |         | 2       |         |
| Задатак 4               | 12              |        |        |        |        |        |        |         |         |         | 4       |         | 8       |
|                      |                 |        |        |        |        |        |        |         |         |         |         |         |         |
| **Укупан износ**           | 62              | 8      | 8      | 8      | 4      | 4      |        |         | 8       | 4       | 8       | 2       | 8       |
|                      |                 |        |        |        |        |        |        |         |         |         |         |

### <a name="bobs-availability"></a>Бранкова доступност
| **Резервација   ресурса** | **Укупно часова** | пон 6/4 | уто 6/5 | сре 6/6 | чет 6/7 | пет 6/8 | суб 6/9 | не 6/10 | пон 6/11 | уто 6/12 | сре 6/13 | чет 6/14 | пет 6/15 |
|------------------------|-----------------|--------|--------|--------|--------|--------|--------|---------|---------|---------|---------|---------|---------|
| Бранко                    | 62              | 4      | 4      | 8      | 8      | 8      |        |         | 4       | 4       | 8       | 8       | 6       |

Међутим,не постоји систематски начин да додељујете контуру резервисаних сати задацима из дана у дана. Ако је менаџер пројекта спреман да промени распоред пројекта како би изашао у сусрет доступности ресурса, мораће да уклони доделу и да ревидира све задатке како би одговарају контурама резервације.

У случају када је организација задатак планирања дала и менаџеру пројекта и менаџеру ресурса, менаџера пројекта поставља распоред, што обухвата и контурисање потребног посла. Не би требало да менаџер ресурса може да утиче на распоред без знања менаџера пројекта променом контура ангажовања приликом резервације стварних ресурса. Ако менаџер ресурса испуњава нешто друго, а не шта је менаџер пројекта захтевао, они морају да постигну договор о потребним променама у распореду пројекта.

Будући да резервације и доделе нису чврсто повезане, могуће је резервисати контуре које се разликују од контура задатка или променити доделе како би се добиле околности у којима резервације и доделе нису усклађене.

**Приказ усклађености** менаџеру пројекта дозвољава да види резервације и доделе за сваког члана пројектног тима. Приказ користи боје и сенчење за приказивање где постоји неподударање између резервација и додела за чланове тима. На основу ових информација, менаџер пројекта може да предузима корективне радње. Он може да прошири резервацију ресурса за предмете у којима постоје доделе, а нема резервација, или може да откаже резервације тако где су ресурси резервисани, али имају нема доделе.

> [!NOTE]
> Ако преместите задатак који сте сами скицирали, те скице остају. Контуре се поново генеришу у складу са календаром пројекта како би одразиле промене у радном времену и празницима. То је тако пројектовано јер систем не зна намеру првобитне скице и не може да утврди да ли има смисла задржати ту скицу у новом временском периоду. Пошто резервације и доделе нису повезане, резервације задржавају првобитне скице резервације. У том случају, мораћете да откажете и поново резервишете за контуру нове доделе.
