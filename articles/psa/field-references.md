---
title: Додавање прилагођених поља у подешавање цена и ентитете трансакције
description: Ова тема пружа информације о додавању прилагођених поља у подешавање цена и ентитете трансакције.
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
ms.openlocfilehash: 32d0dbc3a69d713dcae8d27e52f2a0c6fc296127
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084078"
---
# <a name="add-custom-fields-to-price-setup-and-transactional-entities"></a>Додавање прилагођених поља у подешавање цена и ентитете трансакције 
Ова тема претпоставља да сте довршили процедуре у теми [Креирање прилагођених поља и ентитета](create-custom-fields-entities.md). Ако нисте довршили те процедуре, вратите се и довршите их, а затим се вратите на ову тему. 

У овој теми, процедуре ће вам показати како можете да додате захтеване референце прилагођеног поља у ентитете и елементе корисничког интерфејса као што су обрасци и прикази.

## <a name="add-custom-pricing-dimension-fields"></a>Додавање прилагођеног поља димензија за одређивање цена 
Након креирања прилагођених поља и ентитета, следећи корак јесте да подешавање цена и трансакциони ентитети постану свесни свих прилагођених ентитета или скупова опција креирањем референтних поља. У зависности од тога да ли листа димензија за одређивање цена укључује димензије скупа опција, димензије ентитета или обоје, следите само кораке у прилагођеним димензијама за одређивање цена **Прилагођене димензије за одређивање цена засноване на скупу опција** или **Прилагођене димензије за одређивање цена засноване на ентитету**.

### <a name="option-set-based-custom-pricing-dimensions"></a>Прилагођене димензије за одређивање цена засноване на скупу опција
Када је прилагођена димензија за одређивање цена заснована на скупу опција, додајте је као поље у кључне Project Service ентитете. У следећој процедури, **Радна локација ресурса** и **Радно време ресурса** користе се као димензије за одређивање цена засноване на скупу опција. Оне прво морају да се додају као поља у ентитете за одређивање цена **Цена улоге** и **Провизија на цену улоге**.

1. У услузи Project Service Automation (PSA) кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**. 
2. У левом окну за навигацију истраживача решења изаберите **Ентитети > Цена улоге**.
3. Развијте ентитет **Цена улоге** и изаберите опцију **Поља**.
4. Кликните на **Ново** да бисте креирали ново поље под називом **Радна локација ресурса** и изаберите **Скуп опција** као тип поља. 
5. Изаберите **Користи постојећи скуп опција** , па скуп опција **Радна локација ресурса** , а затим кликните на **Сачувај**.
6. Поновите кораке 1-5 да бисте додали ово поље у ентитет **Провизија на цену улоге**. 
7. Поновите кораке 1-5 за скуп опција **Радно време ресурса**.

> [!IMPORTANT]
> Када додате поље у више од једног ентитета, користите исто име поља у свим ентитетима. 

> ![Додавање радне локације ресурса у цену улоге](media/RWL-Field.png)

У фазама продаје и процене пројекта, процена радних напора који су неопходни да би се довршио **локални** посао и посао **на локацији** ако се користе **Стандардно радно време** и **Прековремено радно време** , користе се за процену вредност понуде/пројекта. Поља **Радна локација ресурса** и **Радно време ресурса** ће бити додата у ентитете процене **Детаљ ставке понуде** , **Детаљи предмета уговора** , **Пројектни задатак** , **Члан пројектног тима** и **Ставка процене**.

1. У PSA кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**. 
2. У левом окну за навигацију истраживача решења изаберите **Ентитети > Детаљ ставке понуде**.
3. Развијте ентитет **Детаљ ставке понуде** и изаберите **Поља**.
4. Кликните на **Ново** да бисте креирали ново поље под називом **Радна локација ресурса** и изаберите тип поља **Скуп опција**. 
5. Изаберите **Користи постојећи скуп опција** и **Радна локација ресурса** , а затим кликните на **Сачувај**.
6. Поновите кораке 1–5 да бисте додали ово поље у ентитете **Детаљ предмета уговора за пројекат** , **Пројектни задатак** , **Члан пројектног тима** и **Ставка процене**.
7. Поновите кораке 1-6 за скуп опција **Радно време ресурса**. 

> ![Додавање радне локације ресурса у ставку процене](media/RWL-Default-Value.png)


За испоруку и фактурисање, цена довршеног посла треба да буде прецизно одређена да бисте изабрали да ли је обављен **локално** или **на локацији** , као и да ли је довршен уз опцију **Стандардно радно време** или **Прековремено** у делу Стварне вредности пројекта. Поља **Радна локација ресурса** и **Радно време ресурса** треба да додате у ентитете **Ставка времена** , **Стварна вредност** , **Детаљ ставке фактуре** и **Ставка у главној књизи**.

1. У PSA кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**.
2. У левом окну за навигацију истраживача решења изаберите **Ентитети > Ставка времена**.
3. Развијте ентитет **Детаљ ставке понуде** , а затим изаберите **Поља**.
4. Кликните на **Ново** да бисте креирали ново поље под називом **Радна локација ресурса** и изаберите **Скуп опција** као тип поља. 
5. Изаберите **Користи постојећи скуп опција** , па скуп опција **Радна локација ресурса** , а затим кликните на **Сачувај**.
6. Поновите кораке 1-5 да бисте додали ово поље у ентитете **Стварна вредност** , **Детаљ ставке фактуре** и **Ставка у главној књизи**.
7. Поновите кораке 1-6 за скуп опција **Радно време ресурса**. 

> ![Додавање радне локације ресурса у ставку времена](media/RWL-time-entry.png)

Овим се довршава промена шеме потребна за прилагођене димензије засноване на скупу опција.

## <a name="entity-based-custom-pricing-dimensions"></a>Прилагођене димензије за одређивање цена засноване на ентитету

Када је прилагођена димензија за одређивање цена ентитет, треба да додате 1:N односе између ентитета димензије и кључних Project Service ентитета. Користећи пример стандардне позиције горе, било би разумно очекивати да сваком запосленом буде додељена стандардна позиција. Стога ће вам требати 1: N однос између стандардне позиције и ресурса који може да се резервише, или N:1 однос ако је креиран из ресурса који се може резервисати у стандардну позицију.

1. У PSA кликните на **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије цене**. 
2. У левом окну за навигацију истраживача решења изаберите **Ентитети > Стандардна позиција**.
3. Проширите ентитет **Стандардна позиција** и изаберите **1:N однос**.
4. Кликните на **Нови** да бисте креирали нови 1:N однос **Између стандардне позиције и ресурса који може да се резервише**. Унесите потребне информације, а затим кликните на **Сачувај**.

> ![Додавање стандардне позиције као референтног поља у ресурс који може да се резервише](media/ST-BR.png)

Стандардна позиција ће такође морати да се дода у Project Service ентитете за одређивање цена **Цена улоге** и **Провизија на цену улоге**. Ово се такође завршава помоћу 1:N односа између ентитета **Стандардна позиција** и **Цене улоге** и ентитета **Стандардна позиција** и **Провизија на цену улоге**.

1. У левом окну за навигацију истраживача решења изаберите **Ентитети > Стандардна позиција**.
2. Проширите ентитет **Стандардна позиција** и изаберите **1:N однос**.
3. Кликните на **Нови** да бисте креирали нови 1:N однос **Између стандардне позиције и цене улоге**. Унесите потребне информације, а затим кликните на **Сачувај**.
4. Поновите кораке 1-4 да бисте креирали 1:N односе између ентитета **Стандардна позиција** и **Провизија на цену улоге**.

У фазама продаје и процене пројекта, да би се одредила цена понуде/пројекта, за сваку стандардну позицију су неопходне процене радних активности. То значи да су потребни 1:N односи између стандардне позиције и сваког од ових ентитета процене у услузи Project Service: 

- **Детаљ ставке понуде**
- **Детаљ предмета уговора за пројекат**
- **Пројектни задатак**
- **Члан пројектног тима**
- **Ставка процене**

5. Поновите кораке 1–5 да бисте креирали релације 1:N између ставке **Стандардна позиција** и ентитета **Детаљ ставке понуде** , **Детаљ предмета уговора за пројекат** , **Пројектни задатак** , **Члан пројектног тима** и **Ставка процене**.

> ![Додавање стандардне позиције као референтног поља у ставку процене](media/ST-Estimate-Line.png)

У фазама испоруке и фактурисања, цена обављеног посла сваке стандардне позиције мора бити прецизно одређена у делу Стварне вредности пројекта. То значи да треба да постоје 1:N односи између ставке **Стандардна позиција** и следећих ентитета: **Ставка времена** , **Стварна вредност** , **Детаљ ставке фактуре** и **Ставка у главној књизи**.

6. Поновите кораке 1-6 да бисте креирали 1:N односе између ставке **Стандардна позиција** и следећих ентитета: **Ставка времена** , **Стварна вредност** , **Детаљ ставке фактуре** и **Ставка у главној књизи**.

> ![Додавање стандардне позиције као референтног поља у ставку времена](media/ST-Mapping.png)

### <a name="set-up-dimension-value-defaulting-using-the-mappings-features-of-the-platform"></a>Подешавање подразумеване вредности димензије помоћу функција мапирања у оквиру платформе
За ставку времена, било би од помоћи да систем као подразумевану вредност подеси стандардну позицију за ставку времена из ресурса који се може резервисати и који евидентира ставку времена. Користите следеће кораке да бисте додали мапирања поља за 1:N однос између ентитета **Ресурс који се може резервисати** и **Ставка времена**.

1. У левом окну за навигацију истраживача решења изаберите **Ентитети > Стандардна позиција**.
2. Проширите ентитет **Стандардна позиција** и изаберите **1:N однос**.
3. Двапут кликните на **Ресурса који се може резервисати за ставку времена**. На страници **Однос** кликните на **Коришћење мапирања поља**. 
4. Кликните на **Ново** да бисте креирали ново мапирање из поља **Стандардна позиција** у ентитету **Ресурс који може да се резервише** у референтно поље **Стандардна позиција** ентитета **Ставка времена**. 

> ![Подешавање мапирања поља ради дозвољавања подешавања подразумеване вредности стандардне позиције из Ресурс који се може резервисати у Ставка времена](media/ST-Mapping2.png)


Овим се довршава промена шеме потребна за прилагођене димензије засноване на ентитетима.

##  <a name="add-custom-fields-to-forms-views-and-business-rules"></a>Додавање прилагођених поља у обрасце, приказе и пословна правила

Када извршите све захтеване промене шеме, следећи корак јесте да поља буду видљива у корисничком интерфејсу тако што ћете додати поља у обрасце и приказе.

1. Отворите образац или приказ. У десном окну за навигацију изаберите поље и превуците га на подлогу обрасца. 
2. Ако уређујете приказ, користите десно окно за навигацију, кликните на **Додај поља** и у дијалогу **Листа поља** изаберите потребна поља и кликните на **У реду**.

Следећа табела пружа свеобухватну листу унапред дефинисаних образаца и приказа који су наведени према ентитету, а који ће морати да се ажурирају помоћу нових поља. Ако имате додатне приказе или обрасце у оквиру прилагођавања за ове ентитете, додајте нова поља и у њих.

| Project Service ентитет        | Обрасци којима је потребно ново поље   |Прикази којима је потребно ново поље      |
| ------------------------------|---------------------------------|----------------------------------|
|  Цена улоге|• Информације |• Активне цене категорија ресурса<br> • Везани приказ цена категорија ресурса|
|  Провизија на цену улоге|• Информације|• Активне провизије на цену улоге<br>• Везани приказ провизија на цену улоге|
|  Детаљ ставке понуде|• Информације о пројекту<br>• Брзо креирање пројекта|• Активни детаљ ставке понуде<br>• Комбиновани детаљи ставке понуде<br>• Везани приказ детаља ставки понуде|
|  Детаљ предмета уговора за пројекат|• Информације о пројекту<br>• Брзо креирање пројекта|• Комбиновани детаљи предмета уговора<br>• Активни детаљи предмета уговора<br>• Везани приказ детаља предмета уговора|
|  Пројектни задатак|• Информације<br>• Нови образац||
|  Члан пројектног тима|• Информације<br>• Нови образац|• Активни чланови пројектног тима<br>• Чланови пројектног тима<br>• Везани приказ чланова пројектног тима|
|  Ставка времена|• Информације<br>• Креирање ставке времена|• Моје ставке времена према датуму<br>• Моје ставке времена за ову седмицу<br>• Ставке времена за одобрење|
|  Ставка у главној књизи|• Информације<br>• Брзо креирање|• Активне ставке у главној књизи<br>• Везани приказ ставки у главној књизи|
|  Детаљ ставке фактуре|• Информације<br>• Брзо креирање|• Активни детаљи ставке фактуре<br>• Наплативе трансакције фактуре<br>• Бесплатне трансакције фактуре<br>• Везани приказ детаља ставки фактуре<br>• Ненаплативе трансакције фактуре|
|  Стварно|• Информације<br>• Активне стварне вредности|• Везани приказ стварних вредности|

И прилагођена поља ћете можда морати да додате у пословна правила, у зависности од тога шта сте дефинисали. Један од унапред дефинисаних примера је за пословно правило **Могућност уређивања ставке времена на основу статуса**. Ово правило дефинише поља која треба да буду закључана када ставка времена има статус који не може да се уређује, нпр. **Одобрено**. Додајте поља у ово пословно правило тако да поља буду закључана за уређивање када се статус ставке времена разликује од **Радна верзија** или **Враћена**.