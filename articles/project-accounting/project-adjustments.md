---
title: Корекције пројекта
description: Овај чланак пружа информације о корекцијама пројекта.
author: ryansandness
ms.date: 11/09/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ryansandness
ms.openlocfilehash: 52a262adce2bb624bc088e50858e25824f845e5c
ms.sourcegitcommit: bb03ac64e01112c93bb24035a51653a0a88cd5fc
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/18/2022
ms.locfileid: "9788374"
---
# <a name="project-adjustments"></a>Корекције пројекта

_**Односи се на:** Project Operations за сценарије засноване на залихама/производњи_

## <a name="adjustments-overview"></a>Преглед корекција

Корпорацију Мицрософт можете да  Dynamics 365 Project Operations  конфигуришете тако да корисници могу да мењају прокњижене трансакције. Трансакције пројекта можете кориговати појединачно или можете изабрати више трансакција истовремено на листи свих пројектних трансакција. Корекције пројекта се користе, на пример, за масовно ажурирање статуса наплате, поновно израчунавање трошкова након промене конфигурације или ажурирање извора финансирања.

Корисници могу да приступе функционалности прилагођавања пројекта на неколико начина:

- Коришћењем странице "  **Прилагођавање трансакција**  " којој се може приступити из прозора"Управљање  **пројектима" и "Подешавање рачуноводства** \> **"**.
- Коришћењем дугмета "  **Корекција**  " на страници  **"Прокњижене трансакције пројекта**  " којој се може приступити из управљања  **пројектима и рачуноводствених** \> **трансакција**.
- Коришћењем дугмета  **"**  Корекција"  **на страници "Прокњижене**  трансакције пројекта" у контексту пројекта. Овој страници се може приступити из пројектног  **менаџмента и књиговодства** \> **Сви пројекти**.

Да бисте дозволили корекције, морате омогућити један или више статуса трансакција из управљања пројектима и књиговодствених пројеката и рачуноводствених параматера на картици Опште  **·** \> **поставке у одељку Дозволи корекцију**  **статуса трансакције**  .  **·** Примери статуса трансакција укључују прокњижене трансакције, фактурисане трансакције или елиминисане трансакције. Сваки статус трансакције који је постављен на "Не  **"**  имаће трансакције у том статусу које се неће појавити у оквиру процеса корекције као што је могуће изабрати за корекцију.

Опција конфигурације која је названа "Увек  **креирај трансакцију корекције"**  тренутно је доступна у параметрима управљања пројектима и рачуноводства. Ову опцију можете онемогућити да бисте ажурирали оригиналну трансакцију уместо да креирате нове трансакције током корекције у подскупу сценарија. Најављено је да ће овај параметар бити депрециран до 1. марта 2023. године. После 1. марта 2023. године, систем ће се увек понашати као да је опција омогућена.

## <a name="adjustments-process-flow"></a>Посагађивања процеса протока

Следећи кораци приказују типичан ток за корекције обраде.

1. Отворите страницу  **"Прилагођавања**  пројекта".
2. Изаберите  **опцију**  Изаберите да бисте потражили трансакције које задовољавају очекиване критеријуме за корекцију.
3. Са листе трансакција изаберите све трансакције или подскуп трансакција за корекцију.
4. Изаберите  **ставку** Прилагоди и измените атрибуте у реду. Друга могућност је да, ако су вредности ручно наведене током ставке трансакције, можете изабрати да унесете подразумеване системске вредности.
5. Листа трансакција се враћа, а потврдни знак се појављује у колони корекције на  **чекању да би**  се означило где су извршене промене. Све корекције које имају необрађене промене приказане су у доњој половини странице. Тамо можете извршити додатне детаљне промене изван онога што је приказано на претходној страници.
6. Изаберите  **ставку Прокњижи**  да бисте прокњижили трансакције корекције.

У зависности од конфигурације, за корекцију се обично креирају нове трансакције.

- Поље  **Статус фактуре**  оригиналне трансакције је подешено на "Кориговано  **"**.
- Трансакција сторнирања се креира да би се сторнирање оригиналне трансакције, а поље  **Статус**  је подешено на "Кориговано  **"**.
- Креирана је нова трансакција која има промене које су извршене током процеса корекције.

### <a name="selecting-multiple-posted-project-transactions-at-a-time-for-adjustments-and-credit-notes"></a>Бирање више прокњижених пројектних трансакција истовремено за корекције и кредитне напомене

Нова функција која је уведена у издању 10.0.30 омогућава избор више трансакција за корекцију у исто време са  **странице Прокњижене трансакције**  пројекта.

Да бисте могли да користите ову функцију, она мора бити омогућена у систему. Администратори могу да користе  **радни простор**  за управљање функцијама да би проверили статус функције и омогућили је ако је то потребно. У радном  **простору за управљање**  функцијама потражите и изаберите  **прокњижене трансакције прокњиженог пројекта за корекције и кредитне напомене, а** затим изаберите омогући  **одмах**.

Ова функција омогућава функционалност следећег кључа:

- Њему се може приступити са странице прокњижене трансакције у оквиру пројекта помоћу постојећег дугмета "  **Корекција**  ".
- Омогућава контролу избора у више редова на страници "Прокњижене  **трансакције пројекта**  ". Филтере можете применити на страницу листе и изабрати записе пре него што почнете са подешавањима.
- Онемогућава дугме "Корекција  **" ако**  ниједна трансакција не може да се коригује или ако изаберете комбинацију кредитних напомена и налога заједно уместо појединачно.
- Због додавања контроле избора у више редова,  **веза "Посвећени трошак**  " на главној траци више неће бити онемогућена ако је изабрано више редова.
- Додаје следећу поруку упозорења: "Изабрали сте више од (изабраних бројева) записа за корекцију. Наставак ове акције може потрајати неко време. Желите ли заиста да наставите са овом акцијом?"

Ова функција такође уклања корак 2 из тока процеса који је описан раније у овом чланку. Због тога ће све трансакције које су изабране пре него што је страница  **"Прилагођавање**  трансакција" отворена бити укључене у листу трансакција за корекцију. Не морате да користите дугме "Изабери"  **·**  да бисте их потражили.

> [!NOTE] 
> Чак и ако је ова функција онемогућена, и даље можете да изаберете више записа за подешавање. Међутим, остаће изабран само један запис  *, а* дијалог  **"Избор трансакција**  " ће се појавити одмах након што изаберете да отворите корекције.

## <a name="adjustment-transaction-statuses-that-can-be-enabled-or-disabled-for-adjustments"></a>Корекција статуса трансакције који се могу омогућити или онемогућити за корекције

Следећи статуси се могу омогућити или онемогућити на картици Опште  **поставке странице**  Управљање  **пројектима и рачуноводствени параметри** :

- Објављено
- Предлог фактуре
- Фактурисано
- Процењено
- Елиминисан
- Почетни салдо (час)

## <a name="adjustment-parameters"></a>Параметри подешавања

Ови параметри су наведени на страници  **"Управљање пројектним и рачуноводственим параметрима**  " на  **картици "Опште**  **поставке" у оквиру групе"Подешавање**  " и измениће понашање начина обраде корекција. 

| Назив параметра | Опис |
|----------------|-------------
| Увек креирај трансакцију корекције | Ако је овај параметар омогућен, процес корекције ће увек креирати нову трансакцију сторекта и нову кориговану трансакцију када постоји финансијски или извештајни утицај. Ако је параметар онемогућен, процес корекције ће ажурирати оригиналну трансакцију уместо креирања сторнирања и нове трансакције за сценарио као што је ажурирање текста трансакције. |
| Поље аутоматског означавања | Ако је овај параметар омогућен, систем ће поново обрачунати цену трошка и продајну цену. |
| Користи датум корекције као нови пројекат | Овај параметар се користи за премештање трансакција у будућу фискални период пре него што је систем подржао ову функцију. Не препоручујемо да га користите јер мења датум пословања трансакције и биће запрећен у будућем издању. |
| Дозволи затворене активности | Обично није могуће креирати трансакције за затворене активности. Ако је овај параметар омогућен, то понашање је замењено. Због тога се могу креирати корекције за затворене активности. |