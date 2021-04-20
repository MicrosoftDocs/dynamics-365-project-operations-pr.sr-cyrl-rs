---
title: Преглед ставки понуде засноване на пројекту
description: Ова тема пружа информације о коришћењу ставки понуде заснованим на пројекту за рад на пројекту.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cfe98fc89130c93dd0a36af8583881fdcb4550c0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858716"
---
# <a name="project-based-quote-lines-overview"></a>Преглед ставки понуде засноване на пројекту 

_**Односи се на:** Једноставна примена – од погодбе до профактуре, Project Operations за сценарије засноване на ресурсима / без залиха_

Ставке понуде засноване на пројекту осмишљене су да помогну у процени рада на пројекту при ангажовању. Структура ставке понуде на основу пројекта проширена је за процене пројеката следећим концептима:

- Начин наплате
- Мапирање пројеката и задатака
- Укључене класе трансакција
- Ограничење које не сме да се прекорачи
- Подешавање наплативости
- Процена помоћу детаља ставки понуде
- Клијенти ставки понуде

Следећа табела пружа информације о пољима на картици **Општи подаци** ставке понуде засноване на пројекту. Ова поља помажу у постављању основе за детаљну, основну процену рада на пројекту.

| **Поље** | **Опис** | **Последични утицај** |
| --- | --- | --- |
| Име | Назив понуде који вам помаже да препознате дискретну компоненту понуде која се процењује. | Копира се у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари. |
| Начин наплате | У понуди креираној из могућности за пословање, ова вредност се копира из одговарајућег поља у ставци могућности за пословање. Ово поље укључује два главна модела уговарања које Dynamics 365 Project Operations подржава:</br>- Фиксна цена</br>- Време и материјал.| Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Project | Користите ово опционално поље за идентификовање пројекта који ће се користити за извођење радова при овом ангажовању. Када се пројекат мапира у ставку понуде, то помаже у постављању наплативих задатака, као и у доношењу процене засноване на пројекту у ставци понуде као детаље ставке понуде. Када пројекат није мапиран у ставку понуде засновану на пројекту, процену треба креирати ручно креирањем сваког детаља ставке понуде. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.|
| Обухваћени задаци | Означава да ли се ова ставка понуде користи за све или неке пројектне задатке за изабрани пројекат. Ово поље подложно уређивању има следеће могуће вредности:</br>- Сви пројектни задаци</br>- Само изабрани пројектни задаци</br>Празна вредност у овом пољу је еквивалентна опцији **Сви пројектни задаци**. | Када се на страници пројекта изабере **Само изабрани пројектни задаци**, картица **Подешавање наплате за задатак** вам омогућава да изаберете одређене задатке да бисте их повезали са овом ставком понуде. Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Садржи време | Вредност **Да**/**Не** показује да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде. Вредност **Не** означава да временске трансакције или трошкови рада неће бити укључени у процену ове ставке понуде. Вредност **Да** означава да ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Садржи трошак | Вредност **Да**/**Не** показује да ли ће цена трошкова на изабраном пројекту бити укључена у процену ове ставке понуде. Вредност **Не** означава да цена трошка неће бити укључена у процену ове ставке понуде. Вредност **Да** означава да ће цена трошка бити укључена у процену ове ставке понуде. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Садржи материјал | Вредност **Да**/**Не** показује да ли ће цена материјала на изабраном пројекту бити укључена у процену ове ставке понуде. Вредност **Не** показује да цена материјала неће бити укључена у процену ове ставке понуде. Вредност **Да** показује да цена материјала неће бити укључена у процену ове ставке понуде. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Садржи надокнаду | Вредност **Да**/**Не** показује да ли ће накнаде на изабраном пројекту бити укључене у процену ове ставке понуде. Вредност **Не** означава да накнаде неће бити укључене у процену ове ставке понуде. Вредност **Да** означава да ће накнаде бити укључене у процену ове ставке понуде. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Понуђени износ | Ово је износ који ће бити наведен клијенту за све радове предвиђене на овој ставци понуде засноване на пројекту. У понуди креираној из могућности за пословање, ова вредност се копира из поља **Буџет клијента** у ставци могућности за пословање. Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа на детаљима ставке понуде. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Процењени порез | То поље може да уређује корисник да би додао процењени износ пореза у ставку понуде. Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа пореза на детаљима ставке понуде. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Понуђени опорезовани износ | Ово поље је опорезовани износ ставке понуде и само је за читање. Износ у овом пољу се израчунава као *Понуђени износ + порез*. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Ограничење које не сме да се прекорачи | Ово поље је могуће уређивати и доступно је само у ставкама понуде заснованим на пројекту чији начин обрачуна је **Време и материјал**. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |
| Буџет клијента | Ово поље може да се уређује и копира се из одговарајућег поља ставке могућности за пословање ако је понуда креирана из могућности за пословање. | Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>Правила за валидацију за поља на картици Општи подаци ставки понуде заснованих на пројекту

**1. правило**: Ако је поље **Укључени задаци** празно или ако је подешено на **Сви пројектни задаци**, пројекат је укључен у ставку понуде.

**2. правило**: Ако је поље **Укључени задаци** празно или ако је постављено на **Сви пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени само у једну ставку понуде засноване на пројекту.

**3. правило**: Ако је поље **Укључени задаци** постављено на **Само изабрани пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени у више ставки понуде засноване на пројекту.

**4. правило**: Ако могућност за пословање има више понуда, могу постојати ставке понуде из различитих понуда које се односе на исти пројекат и укључују исту класу трансакције.

**5. правило**: Ако понуде не припадају истој могућности за пословање, не могу да укључују исти пројекат и класу трансакције.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p>
                    <strong>Могућност за пословање</strong>
                </p>
            </td>
            <td width="39" valign="top">
                <p>
                    <strong>Понуда</strong>
                </p>
            </td>
            <td width="40" valign="top">
                <p>
                    <strong>Ставка понуде</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="77" valign="top">
                <p>
                    <strong>Обухваћени задаци</strong>
                </p>
            </td>
            <td width="45" valign="top">
                <p>
                    <strong>Садржи време</strong>
                </p>
            </td>
            <td width="46" valign="top">
                <p>
                    <strong>Садржи трошак</strong>
                </p>
            </td>
            <td width="43" valign="top">
                <p>
                    <strong>Садржи материјал</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Уврсти</strong>
                </p>
                <p>
                    <strong>Накнада</strong>
                </p>
            </td>
            <td width="49" valign="top">
                <p>
                    <strong>Важи / Не важи</strong>
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    <strong>Разлог</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Празно </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Не важи </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
Кршење правила бр. 2. Време, трошкови и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2 </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Празно </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Празно </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
No </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Не важи </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
Кршење правила бр. 2. Време, материјал и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2 </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Празно </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Празно </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
No </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Важеће </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
Време, материјал и накнаде за пројекат P1 укључени су у QL1 <br>
Трошкови за пројекат P1 укључени су у QL2 <br>
Нема преклапања у ономе што је укључено у сваку ставку понуде и стога је важеће.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Празно </p>
            </td>
            <td width="45" valign="top">
                <p>
No </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
No </p>
            </td>
            <td width="41" valign="top">
                <p>
No </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Само изабрани задаци </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Не важи </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
Кршење правила бр. 2 </p>
                <p>
Q1 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1 </p>
                <p>
QL2 укључује време, трошкове и накнаде за цео пројекат P1 и стога се преклапа са оним што је укључено у Q1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Празно </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Само изабрани задаци </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Важеће </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
По правилу бр. 3, </p>
                <p>
Q1 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1.
                </p>
                <p>
QL2 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1.
                </p>
                <p>
Једина додатна провера ваљаности око подскупа задатака на QL1 која се разликује од подскупа задатака на QL2 како би се осигурало да тамо нема преклапања. То систем ради када су задаци повезани.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Само изабрани задаци </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Важеће </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
По правилу бр. 5, Q1 и Q2 су две понуде у истој могућности за пословање, тако да се могу обе проценити за исте компоненте пројекта.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К2 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Не важи </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
По правилу бр. 4, Q1 и Q2 су две понуде у различитим могућностима за пословање, тако да се не могу проценити за исте компоненте истог пројекта.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O2 </p>
            </td>
            <td width="39" valign="top">
                <p>
К1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
П1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Сви пројектни задаци или празни </p>
            </td>
            <td width="45" valign="top">
                <p>
Да </p>
            </td>
            <td width="46" valign="top">
                <p>
Да </p>
            </td>
            <td width="43" valign="top">
                <p>
Да </p>
            </td>
            <td width="41" valign="top">
                <p>
Да </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
