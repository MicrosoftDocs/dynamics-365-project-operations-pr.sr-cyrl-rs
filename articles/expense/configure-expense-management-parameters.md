---
title: Конфигурисање параметара управљања трошковима
description: Ова тема описује параметре који контролишу опште понашање у управљању трошковима.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 8ecbd0abc16d0a29eea47d6bd1653a204a83de4c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897289"
---
# <a name="configure-expense-management-parameters"></a>Конфигурисање параметара управљања трошковима

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Ова тема описује параметре контроле општег понашања у управљању трошковима.

## <a name="general"></a>Опште

| Поље                                                    | Опис |
|----------------------------------------------------------|-------------|
| Стандардна стопа пређених километара                                 | Унесите стопу накнаде за трошкове пређених километара. Ова стопа се множи са километражом која се уноси за трошак да би се израчунао износ који се надокнађује за путни трошак. |
| Потврдите сврху трошка                                 | Укључите ову опцију да бисте ограничили кориснике на постојећи скуп вредности који је конфигурисан у пољу **Сврха извештаја о трошковима** када креирају извештаје о трошковима. |
| Лични трошкови које плаћа                                | Изаберите ко је одговоран за плаћање било ког износа трансакције на кредитној картици који је категорисан као лични. |
| Прикажите целокупан извештај о трошковима враћања               | Изаберите ову опцију да бисте приказали све трошкове за извештај о трошковима када се прегледају детаљи оригиналног документа за одређени ваучер који је генерисан приликом књижења извештаја о трошковима. |
| Претходна ауторизација путовања је обавезна                 | Изаберите ову опцију да бисте захтевали да се захтев за путовање проследи и одобри пре него што запослени буде могао да поднесе извештај о трошковима. |
| Дозволите уређивање дистрибуција пре књижења            | Изаберите да ли се дистрибуције извештаја о трошковима могу уређивати пре књижења. |
| Процените смернице за управљање трошковима                     | Изаберите када ће се трошкови процењивати да бисте утврдили да ли су прекршене смернице за трошкове. Кршење смерница за трошкове се може проценити када се ставка трошка унесе и сачува или када се трошак поднесе на одобрење. Правила смерница за признанице које су обавезне процениће се када се сачува ставка трошка. |
| Омогућите ставке међукомпанијских трошкова                         | Изаберите да ли се трошкови за друга правна лица могу уносити у извештај о трошковима. |
| Дозволите уређивање курса валута за трошкове кредитне картице | Изаберите ову опцију да бисте кориснику дозволили да уређује курс валуте за увезене трошкове кредитне картице. |
| Поља хијерархије на више нивоа за приказ                  | Изаберите која се поља даваоца одобрења приказују када је тип додељивања тока посла постављен као хијерархија, а избор **Хијерархија** је постављен тако да користи хијерархију одобрења, одобрење трошкова на више нивоа. Када се за ток посла користи хијерархија одобрења на више нивоа, изабрана поља ће бити приказана у извештају о трошковима и могу се уређивати. |
| Унесите број кредитне картице запосленог                        | Изаберите да ли се може унети и сачувати број од 15 или 16 знакова у пољу **ID картице** на страници **Кредитне картице** за запосленог. |
| Потврдите сврху захтева за путовање                      | Укључите ову опцију да бисте ограничили кориснике на постојећи скуп вредности који је конфигурисан у пољу **Сврха извештаја о трошковима** када креирају захтеве за путовање. |

## <a name="financial"></a>Финансије

| Поље                                                                                    | Опис |
|------------------------------------------------------------------------------------------|-------------|
| Назив дневног дневника за књижење у главну књигу                                                                | Изаберите назив дневника за књижење у главну књигу у који се књиже одобрени извештаји о трошковима. |
| Омогући повраћај пореза из трошкова                                                        | Изаберите ову опцију да бисте омогућили повраћај пореза на трошкове за прихватљиве трошкове. Ова опција се не може изабрати ако су омогућена америчка правила о порезу на промет и порезу на употребу. |
| Књижи аконтације одмах                                                           | Изаберите ову опцију да бисте књижили одобрену аконтацију када се поступак плаћања и трансфера заврши. Ако ова опција није изабрана, процес плаћања и преноса генерише непрокњижени општи дневник. |
| Тачан датум обрачуна током књижења                                                   | Изаберите ову опцију да бисте ажурирали датум обрачуна када су трошкови прокњижени, ако је текући период на чекању или је затворен. Датум обрачуна биће постављен на следећи отворени период. |
| Дозволи груписање трансакција на основу рачуна за пребијање дуговања и потраживања наведеног у начину плаћања       | Изаберите ову опцију да бисте сумирали трансакције трошкова за извештај о трошковима, на основу рачуна за пребијање дуговања и потраживања који је наведен у начину плаћања трошкова. |
| Порез је укључен                                                                             | Изаберите ову опцију да бисте подразумевано укључили порез на промет у износ трошкова. |
| Ослободи оптерећења приликом затварања захтева за путовање                                      | Изаберите ову опцију да бисте ослободили оптерећена средства када се одобрени захтев за путовање затвори. |
| Дозволи предају захтева за путовање при прекорачењу буџета за буџетски регистар и буџет пројекта | Изаберите ову опцију да бисте запосленима омогућили да поднесу захтеве за путовање на одобрење, иако премашују или дозвољени буџет који је постављен у буџетском регистру или дозвољени буџет за пројекат. |
| Дозволи предају извештаја о трошковима при прекорачењу буџета за буџетски регистар и буџет пројекта     | Изаберите ову опцију да бисте запосленима омогућили да поднесу извештаје о трошковима на одобрење, иако премашују или дозвољени буџет који је постављен у буџетском регистру или дозвољени буџет за пројекат. |
| Дозволи одобрење извештаја о трошковима само при прекорачењу буџета за буџетски регистар                 | Изаберите ову опцију да дозволите даваоцима одобрења да одобре извештаје о трошковима који премашују дозвољени буџет постављен у регистру буџета. |

## <a name="per-diem"></a>Дневница

| Поље                                 | Опис |
|---------------------------------------|-------------|
| Минимални број сати за дневницу            | Унесите подразумевани минимални број сати које запослени мора да ради у једном дану да би имао право на дневницу за путне трошкове. Ова вредност се користи као подразумевана вредност само за поље **Минимални број сати** за ниво дневница. |
| Проценат за оброке                          | Унесите подразумевани проценат дневнице за оброке који се користи првог и последњег дана путних трошкова када је поље **Израчунајте смањење оброка за** постављено на било **Тип оброка дневно** или **Број оброка дневно**. Радни дан првог и последњег дана може бити краћи од уобичајеног радног дана. Стога би се износ дневнице тих дана могао разликовати од стандардног износа. Ако је проценат постављен на **0** (нула), одбици за први и последњи дан биће 0,00. |
| Проценат за хотел                         | Унесите подразумевани проценат дневнице за хотеле који се користи првог и последњег дана путних трошкова. Радни дан првог и последњег дана може бити краћи од уобичајеног радног дана. Стога би се износ дневнице тих дана могао разликовати од стандардног износа. Ако је проценат постављен на **0** (нула), одбици за први и последњи дан биће 0,00. |
| Остали проценти                         | Унесите подразумевани проценат дневнице за разне трошкове који се користи првог и последњег дана путних трошкова. Радни дан првог и последњег дана може бити краћи од уобичајеног радног дана. Стога би се износ дневнице тих дана могао разликовати од стандардног износа. Ако је проценат постављен на **0** (нула), одбици за први и последњи дан биће 0,00. |
| Смањење процента за доручак | Унесите износ за који се умањује дневница за доручак. На пример, ако запослени добије бесплатан доручак, можда треба да смањите износ дневнице за 10 процената. |
| Смањење процента за ручак     | Унесите износ за који се умањује дневница за ручак. На пример, ако запослени добије бесплатан ручак, можда треба да смањите износ дневнице за 15 процената. |
| Смањење процента за вечеру    | Унесите износ за који се умањује дневница за вечеру. На пример, ако запослени добије бесплатну вечеру, можда треба да смањите износ дневнице за 25 процената. |
| Израчунајте смањење оброка за           | Наведите како систем треба да израчуна дневну редукцију оброка тако што ћете изабрати да ли се смањење заснива на врсти оброка по путовању, по дану или на основу броја оброка који је дозвољен дневно. |
| Заокруживање дневница                     | Изаберите врсту заокруживања која се користи за дневнице. Ако изаберете нормално заокруживање, сви трошкови дневница који имају износ од 0,50 заокружују се на 1,00, а сви трошкови дневница који имају износ мањи од 0,50 заокружују се на 0,00. |
| Основни обрачун дневнице на          | Изаберите да ли се износ дневнице заснива на календарском дану или периоду од 24 сата. |

## <a name="fax-cover-pages"></a>Насловне странице факса

| Поље                          | Опис |
|--------------------------------|-------------|
| Упутства                   | Унесите упутства која запослени морају следити када креирају насловну страницу за факс који се користи за слање рачуна који се односе на извештај о трошковима. Да бисте унели текст специфичан за језик који ће се приказивати, на основу корисничког језика, изаберите **Преводи**. |
| ID корисника (информације о бар коду) | Изаберите ову опцију да бисте чували јединствени идентификатор запосленог у бар коду који се користи на насловној страници факса. |
| Бар кôд                       | Изаберите бар кôд који се користи на насловној страници факса. У управљању трошковима подржани су бар кодови 39 и 128. |

## <a name="anti-corruption"></a>Борба против корупције

| Поље                                 | Опис |
|---------------------------------------|-------------|
| Приказ атестирања о борби против корупције   | Изаберите ову опцију да бисте приказали текст о борби против корупције када се креира извештај о трошковима. Тада се могу омогућити одређене категорије трошкова које ће захтевати да се у извештају о трошковима изабере потврда о борби против корупције. На пример, категорија поклона која се односи на трошак државног службеника може захтевати да запослени потврди да трошак испуњава смернице предузећа које се односе на државне службенике. |
| Порука о борби против корупције за подносиоца | Унесите текст који треба показати запосленом који креира извештај о трошковима. Да бисте унели текст специфичан за језик који ће се приказивати, на основу корисничког језика, изаберите **Преводи**. |
| Порука о борби против корупције за даваоца одобрења  | Унесите текст који треба показати даваоцу одобрења када креира извештај о трошковима. Да бисте унели текст специфичан за језик који ће се приказивати, на основу корисничког језика, изаберите **Преводи**. |