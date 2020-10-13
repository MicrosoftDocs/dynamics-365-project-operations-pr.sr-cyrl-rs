---
title: Ставке понуде засноване на пројекту (Pro)
description: Ова тема пружа информације о коришћењу ставки понуде заснованим на пројекту за рад на пројекту. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908563"
---
# <a name="project-based-quote-lines-pro"></a>Ставке понуде засноване на пројекту (Pro)

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Ставке понуде засноване на пројекту осмишљене су да помогну у процени рада на пројекту при ангажовању. Структура ставке понуде на основу пројекта проширена је за процене пројеката следећим концептима:

- Начин наплате
- Мапирање пројеката и задатака
- Укључене класе трансакција
- Ограничење које не сме да се прекорачи
- Подешавање наплативости
- Процена помоћу детаља ставки понуде
- Клијенти ставки понуде

Следећа табела пружа информације о пољима на картици **Општи подаци** ставке понуде засноване на пројекту. Ова поља помажу у постављању основе за детаљну, основну процену рада на пројекту.

| **Поље** | **Релевантност, сврха и смернице** | **Последични утицај** |
| --- | --- | --- |
| Име | Назив ставке понуде која би требало да вам помогне да идентификујете дискретну компоненту понуде која се процењује. | Копира се у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Начин наплате | У понуди креираној из могућности за пословање, ова вредност се копира из одговарајућег поља у ставци могућности за пословање. Ово поље обухвата два главна модела уговарања које подржава Dynamics 365 Project Operations:</br>- Фиксна цена</br>- Време и материјал.| Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Project | Користите ово опционално поље за идентификовање пројекта који ће се користити за извођење радова при овом ангажовању. Када се пројекат мапира у ставку понуде, то помаже у постављању наплативих задатака, као и у доношењу процене засноване на пројекту у ставци понуде као детаље ставке понуде. Када пројекат није мапиран у ставку понуде засновану на пројекту, процену треба креирати ручно креирањем сваког детаља ставке понуде. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.|
| Обухваћени задаци | Означава да ли се ова ставка понуде користи за све или неке пројектне задатке за изабрани пројекат. Ово поље подложно уређивању има следеће могуће вредности:</br>- Сви пројектни задаци</br>- Само изабрани пројектни задаци</br>Празна вредност у овом пољу је еквивалентна опцији **Сви пројектни задаци**. | Када је на страници пројекта изабрана опција **Само изабрани пројектни задаци**, картица **Постављање задатка за обрачун** омогућава вам да изаберете одређене задатке да бисте их повезали са овом ставком понуде. Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Садржи време | Заставица **Да**/**Не** означава да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде. Вредност **Не** означава да временске трансакције или трошкови рада на изабраном пројекту неће бити укључени у процену ове ставке понуде. Вредност **Да** означава да ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Садржи трошак | Заставица **Да**/**Не** означава да ли ће цене трошкова на изабраном пројекту бити укључене у процену ове ставке понуде. Вредност **Не** означава да цена трошка неће бити укључена у процену ове ставке понуде. Вредност **Да** означава да ће цена трошка бити укључена у процену ове ставке понуде. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Садржи надокнаду | Заставица **Да**/**Не** означава да ли ће накнаде на изабраном пројекту бити укључене у процену ове ставке понуде. Вредност **Не** означава да накнаде неће бити укључене у процену ове ставке понуде. Вредност **Да** означава да ће накнаде бити укључене у процену ове ставке понуде. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Понуђени износ | Ово је износ који ће бити наведен клијенту за све радове предвиђене у овој ставци понуде засноване на пројекту. У понуди креираној из могућности за пословање, ова вредност се копира из поља **Буџет клијента** у ставци могућности за пословање. Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа на детаљима ставке понуде. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Процењени порез | То поље може да уређује корисник да би додао процењени износ пореза у ставку понуде. Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа пореза на детаљима ставке понуде. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Понуђени опорезовани износ | Ово поље је опорезовани износ ставке понуде и само је за читање. Износ у овом пољу се израчунава као *Понуђени износ + порез*. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Ограничење које не сме да се прекорачи | Ово поље је могуће уређивати и доступно је само у ставкама понуде заснованим на пројекту чији начин обрачуна је **Време и материјал**. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Буџет клијента | Ово поље може да се уређује и копира се из одговарајућег поља ставке могућности за пословање ако је понуда креирана из могућности за пословање. | Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>Правила за валидацију за поља на картици Општи подаци ставки понуде заснованих на пројекту

**1. правило**: Ако је поље **Укључени задаци** празно или ако је подешено на **Сви пројектни задаци**, пројекат је укључен у ставку понуде.

**2. правило**: Ако је поље **Укључени задаци** празно или ако је постављено на **Сви пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени само у једну ставку понуде засноване на пројекту.

**3. правило**: Ако је поље **Укључени задаци** постављено на **Само изабрани пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени у више ставки понуде засноване на пројекту.

**4. правило**: Ако могућност за пословање има више понуда, могу постојати ставке понуде из различитих понуда које се односе на исти пројекат и укључују исту класу трансакције.

**5. правило**: Ако понуде не припадају истој могућности за пословање, не могу да укључују исти пројекат и класу трансакције.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p>
                    <strong>Могућност за пословање</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Понуда</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Ставка понуде</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="90" valign="top">
                <p>
                    <strong>Обухваћени задаци</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Садржи време</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Садржи трошак</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Уврсти</strong>
                </p>
                <p>
                    <strong>Накнада</strong>
                </p>
            </td>
            <td width="54" valign="top">
                <p>
                    <strong>Важи / Не важи</strong>
                </p>
            </td>
            <td width="308" valign="top">
                <p>
                    <strong>Разлог</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Празно </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Не важи </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Кршење правила бр. 2. Време, трошкови и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Празно </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Празно </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Не </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Не важи </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Кршење правила бр. 2. Време и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Празно </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Празно </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Не </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Важећи </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
Време и накнаде за пројекат P1 су укључени у QL1.
Трошкови за пројекат P1 укључени су у QL2.
Нема преклапања у ономе што је укључено у сваку ставку понуде и што је важеће.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Празно </p>
            </td>
            <td width="48" valign="top">
                <p>
Не </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Не </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Само изабрани задаци </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Не важи </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Кршење горенаведеног правила бр. 2 </p>
                <p>
Q1 укључује време, трошкове и накнаде за подскуп задатака на пројекту P1.
                </p>
                <p>
QL2 укључује време, трошкове и накнаде за цео пројекат P1 и преклапа се са оним што је укључено у Q1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Празно </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Само изабрани задаци </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Важећи </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
По горенаведеном правилу бр. 3, </p>
                <p>
Q1 укључује време, трошкове и накнаде за подскуп задатака на пројекту P1.
                </p>
                <p>
QL2 укључује време, трошкове и накнаде за подскуп задатака на пројекту P1.
                </p>
                <p>
Једина додатна провера ваљаности односи се на подскуп задатака на QL1 који се разликују од подскупа задатака на QL2. Ово осигурава да нема преклапања. То систем ради када су задаци повезани.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Само изабрани задаци </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" valign="top">
                <p>
Важећи </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
На основу правила бр. 5, Q1 и Q2 су две понуде у истој могућности за пословање, тако да обе могу проценити исте компоненте пројекта.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q2 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
К1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" valign="top">
                <p>
Важећи </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
На основу правила бр. 4, Q1 и Q2 су две понуде у различитим могућностима за пословање, тако да оне не могу проценити компоненте истог пројекта.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O2 </p>
            </td>
            <td width="41" valign="top">
                <p>
К1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="48" valign="top">
                <p>
Да </p>
            </td>
            <td width="42" valign="top">
                <p>
Да </p>
            </td>
            <td width="54" valign="top">
                <p>
Не важи </p>
            </td>
        </tr>
    </tbody>
</table>

