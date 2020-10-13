---
title: Додавање чланова тима из мреже чланова тима
description: Ова тема пружа информације о томе како можете да управљате ресурсима чланова тима.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 0f975d295b4c0ccef9827767beabd32ffd761faa
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897739"
---
# <a name="add-team-members-from-the-team-member-grid"></a>Додавање чланова тима из мреже чланова тима

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_

Dynamics 365 Project Operations укључује контролну таблу менаџера ресурса која пружа визуелни преглед потражње и укупне искоришћености ресурса у целој организацији. Можете користити графиконе на овој контролној табли да бисте визуализовали следеће информације:

- **Потражња за ресурсима**: Графикон **Активни захтеви за ресурсима** приказује ресурсе који су прослеђени. Ресурси се обједињују по улози или пројекту.
- **Непрослеђена потражња за ресурсима**: Графикон **Недодељена потражња за ресурсима** приказује све захтеве за ресурсима који нису прослеђени. Овај графикон помаже менаџерима ресурса да погледају потражњу која није чврста и која може бити прослеђена путем захтева за ресурсе.
- **Наплатива укупна искоришћеност током прошле седмице**: Графикон **Укупна искоришћеност према улози** приказује проценат стварне укупне искоришћености према улогама у организацији у односу на циљану наплативу укупну искоришћеност по улози.

    > [!NOTE]
    > Да би графикон **Укупна искоришћеност према улози** био доступан, креирајте посао који покреће ток посла **UpdateRoleUtilization**. Овај периодичан посао се покреће сваких седам дана како би се израчунала наплатива укупна искоришћеност за претходних седам дана. Резултати се обједињују по улогама.

## <a name="manage-project-team-members"></a>Управљање члановима пројектног тима

Менаџери пројеката могу користити контролну таблу за менаџере ресурса који ће управљати ресурсима на пројектима. На пример, могу да додају члана тима директно у пројекат и резервишу члана тима да испуне потребе за ресурсима које је евидентирао генерички ресурс.

### <a name="add-a-team-member-directly-to-a-project"></a>Додавање члана тима директно у пројекат

Да бисте директно додали члана тима у пројекат, у обрасцу **Пројекти**, на картици **Тим** изаберите **Нови**. Појавиће се дијалог **Брзо креирање члана пројектног тима**. У овом дијалогу можете извршити ове задатке:

- **Резервисање именованог ресурса**: У пољу **Ресурс који може да се резервише** изаберите име ресурса. Затим изаберите улогу, подесите период и изаберите начин додељивања. Именовани ресурс који сте одабрали додаје се пројекту употребом одабраног начина доделе и календара ресурса.
- **Додавање генеричког ресурса**: Оставите поље **Ресурс који може да се резервише** празно, а затим изаберите улогу, подесите период и изаберите жељени начин додељивања. Генерички ресурс се додаје тиму као чувар места. Резервисано место садржи образац потражње који се користи за резервисање именованих ресурса у тиму. Захтев се поставља према календару пројекта.
- **Додавање именованог ресурса у тим без трошења капацитета ресурса**: У пољу **Ресурс који може да се резервише** изаберите ресурс. Изаберите период, а затим изаберите **Ниједан** као начин додељивања. Ресурс се додаје у тим, али капацитет ресурса се не троши резервацијом.

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a>Резервисање члана тима ради испуњавања потребе за генеричким ресурсом

У услузи Project Operations можете резервисати генерички ресурс за пројектни тим. Такође можете одредити улогу, потребан капацитет и начин на који се тај капацитет дистрибуира. За потребу за ресурсом можете да наведете атрибуте који су повезани са генеричким ресурсом. Ови атрибути укључују тражене вештине, жељену организациону јединицу и жељене ресурсе.

Обавите следеће кораке да бисте навели потребне вештине генеричког ресурса за програмера.

1. У обрасцу **Пројекти**, на картици **Тим**, изаберите **Нови** да бисте резервисали генерички ресурс.
2. У приказу **Сви чланови тима**, у колони **Потреба за ресурсом** изаберите везу да додате потребне вештине за генерички ресурс.
3. У обрасцу **Захтев за ресурсом**, у мрежи **Вештине** изаберите три тачке (**...**), а затим изаберите **Додај нову карактеристику захтева** да бисте додали потребне вештине за програмера.
4. У обрасцу дијалога **Брзо креирање: Карактеристике захтева**, у пољу **Карактеристике** изаберите жељену вештину.
5. У пољу **Вредност оцене** изаберите ниво стручности за ову вештину. 
6. У пољу **Захтев за ресурсом** подесите захтев да бисте обезбедили изворне ресурсе из организационих јединица или чак именованих ресурса. Када завршите, изаберите **Сачувај**.
7. У обрасцу **Захтев за ресурсом** изаберите **Резервиши** да бисте испунили захтев за ресурсом. Такође можете одабрати генерички ресурс у мрежи **Сви чланови тима**, а затим изабрати **Резервиши**.

    > [!NOTE]
    > У овом примеру, постоји 40 захтеваних сати, али нема стварно резервираних сати, јер генерички ресурси немају резервације. Поред тога, нема додељених сати, јер је генерички ресурс додат директно у тим уместо да је додат коришћењем доделе задатка.

    У обрасцу **Помоћник за планирање** можете филтрирати доступне ресурсе према потребама које су наведене у потреби за ресурсом. Ресурси су сортирани према параметрима сортирања који су наведени на табели распореда.

   Неки од најчешће коришћених филтера су:

    - **Карактеристике уз оцену**: Филтрирајте по вештинама, цертификацијама и другим квалитетима ресурса, поред оцена стручности.
    - **Улоге**: Филтрирајте према подразумеваним улогама које су додељене ресурсима који могу да се резервишу.
    - **Организационе јединице**: Филтрирајте ресурсе који могу да се резервишу према организационим јединицама којима су додељени.

8. Ако нисте задовољни резултатима иницијалне претраге захтева, можете променити критеријуме филтрирања. Проширите окно **Приказ филтера** са леве стране, а затим изаберите **Претражи** да бисте пронашли додатне ресурсе. Да бисте променили начин сортирања резултата, изаберите **Сортирај**.
9. Одаберите ресурсе у складу са потражњом која је наведена у захтеву, као што је назначено у врху мреже. Можете избрисати избор ћелија у мрежи и оставити отворен капацитет ресурса. Само један ресурс може бити изабран као резервисан у одређеном тренутку.
10. Изаберите **Резервиши** да резервишете изабрани ресурс и оставите табелу распореда отворену, тако да можете да изаберете додатне ресурсе. Или одаберите **Резервиши и изађи** да резервишете изабрани ресурс и затворите табелу распореда.
11. Вратите се на приказ **Сви чланови тима**. У мрежи можете да приметите да је генерички ресурс замењен именованим ресурсом и да је 40 сати наведено као резервирано за тај ресурс.

    > [!NOTE]
    > Нису приказани додељени сати јер су резервисани директно у тиму. Нису резервисани коришћењем додела задатка.

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a>Додељивање генеричких ресурса задацима и генерисање потреба за ресурсима

У услузи Project Operations можете да креирате задатке и да им онда доделите генеричке ресурсе. Потражња за ресурсима потом може бити представљена чуварима места док процењујете свој распоред и финансијске показатеље. Затим можете да генеришете потребе за генеричким ресурсима и испуните их.

1. У обрасцу **Пројекти**, на картици **Распоред** изаберите **Додај** да креирате задатак.
2. У пољу **Ресурси** изаберите симбол **бирача ресурса**. Појављује се бирач ресурса и показује постојеће чланове тима за пројекат.
3. Унесите име новог генеричког ресурса, а затим изаберите **Креирај**.
4. У дијалогу **Брзо креирање члана пројектног тима** који се појављује, у пољу **Улога** одаберите улогу генеричког ресурса. 
5. У пољу **Јединица за обезбеђивање ресурса** изаберите организациону јединицу за генерички ресурс. Затим изаберите **Сачувај**. Генерички члан тима је сада додељен задатку.

   На картици **Тим** видећете новог генеричког члана тима. Имајте на уму да има само додељене сате. Ови часови су збир свих задатака који су додељени генеричком члану тима. Генерички члан тима нема захтеване сате нити потребу за ресурсом.

6. Сада можете доделити генеричког члана тима другим задацима помоћу бирача ресурса.

   Када завршите са додељивањем генеричког ресурса задацима, можете да генеришете потребу за генеричким ресурсом.

7. На картици **Тим** изаберите генерички ресурс, а затим изаберите **Генериши захтев**. Када се захтев генерише, члан генеричког тима ће имати захтеване сате и везу ка потреби за ресурсом.

  Када резервишете именовани ресурс, генерички ресурс се уклања из тима и замењује именованим ресурсом. На картици **Распоред** се доделе генеричким ресурсима уклањају и замењују именованим ресурсом.

  > [!NOTE]
  > Ово понашање се дешава само када је именовани ресурс у потпуности резервисан за потребу за генеричким ресурсом. Када именовани ресурс делимично замењује потребу за генеричким ресурсом или више именованих ресурса замењује потребу за генеричким ресурсима, генерички ресурс остаје додељен задатку.

Project Operations не додељује оба ресурса задатку, јер би таквим понашањем настао мање предвидљив распоред. У овом једноставном примеру лако је подједнако поделити сате на два ресурса. Међутим, у сложенијим сценаријима који укључују више задатака и више ресурса, PSA би морао да претпостави како треба да распореди резервације које су примљене за више ресурса у више задатака.

Стога је у тим сценаријима менаџер пројекта одговоран за рашчлањивање више резервација и њихово додељивање према потреби. Да би доделио резервације, менаџер пројекта додељује задатке из генеричких ресурса именованим ресурсима и затим користи приказ **Усаглашеност** да би осигурао да додела функционише са резервацијама.

### <a name="edit-a-resource-requirement"></a>Уређивање потребе за ресурсом

Када креира захтев за ресурсом, менаџер пројекта или менаџер ресурса можда ће можда морати да измени детаље како би прецизирао критеријуме за претрагу када се користи табела распореда. Да бисте уредили потребу за ресурсом, следите ове кораке.

1. У обрасцу **Пројекти**, на картици **Тим**, изаберите везу ка било ком захтеву за генерички ресурс.
2. У обрасцу **Захтев за ресурсима** који се појави, унесите потребне податке о пољу

   У обрасцу **Захтев за ресурсима**, менаџер пројекта или менаџер ресурса такође могу да дефинишу вештине, улоге, жељене опције ресурса и жељену организациону јединицу.

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a>Ажурирање резервација ресурса након њиховог резервисања за пројекат

Након што додате генерички или именовани ресурс у пројектни тим, можете променити резервације ресурса.

1. У обрасцу **Пројекти**, на картици **Тим**, изаберите члана тима, а затим изаберите **Одржавање резервација**.
 
   Појављује се табела распореда и приказује резервације члана пројектног тима. Проширите евиденцију члана тима да бисте видели сате који су резервисани за овај пројекат и друге пројекте који троше капацитет члана тима.

2. Изаберите и превуците резервацију да бисте је проширили или скратили. Појавиће се дијалог **Креирање резервације ресурса** који вам омогућава да подесите резервацију.
3. Кликните десним тастером миша на резервацију. Затим можете да користите мени са пречицама да бисте довршили следеће радње:

    - Промена статуса резервације
    - Уређивање резервације
    - Замена ресурса у пројектном тиму

### <a name="change-the-booking-status"></a>Промена статуса резервације

Можете променити било који подразумевани или прилагођени статус резервације.

Следећи статуси су уврштени у Project Operations:

- **Отказано**: Отказује резервацију ресурса и ослобађа капацитет ресурса.
- **Фиксна резервација**: Троши капацитет ресурса. Резервација обично има овај статус када отворите страницу **Одржавање резервација** на мрежи **Сви чланови тима** у обрасцу **Пројекти**.
- **Условна резервација**: Додаје ресурс у тим, али не троши његов капацитет. Овај статус указује на то да је ресурс резервисан за потенцијални рад, али још увек има капацитет ако је потребан на другим пословима. С обзиром на укупну доступност ресурса, условне резервације имају другачији статус од фиксних резервација.
- **Предложен**: Представља предлог менаџера ресурса или менаџера пројекта за ресурс. Предлози не троше капацитет ресурса и ресурс се не додаје пројектном тиму. Да би резервација ресурса за тим била фиксна, менаџер пројекта мора да прихвати предлог.

### <a name="submit-resource-requests"></a>Прослеђивање захтева за ресурсом

Захтеви за ресурсе се користе да пренесу потражњу (или захтев за ресурсима) коју мора да испуни менаџер ресурса. За генерички ресурс који је већ у тиму можете директно да проследите захтев за ресурс. Захтев за ресурс може се испунити на два начина:

- Менаџер ресурса директно испуњава захтев. У овом случају, генерички ресурс замењује фиксна резервација која има именовани ресурс.
- Менаџер ресурса предлаже ресурс менаџеру пројеката, а менаџер пројекта одобрава или одбацује предложени ресурс.

#### <a name="direct-fulfillment-of-resource-requests"></a>Директно испуњавање захтева за ресурсе

Када се генерише потреба за ресурсом, менаџер пројекта може да проследи захтев за генерички ресурс ако изабере ресурс, а затим опцију **Проследи захтев**. Коментари о ресурсу могу се доставити менаџеру ресурса који испуњава захтев. Након прослеђивања захтева, поље **Статус** за члана тима се мења у **Прослеђен**. Када менаџер ресурса испуни захтев, генеричког члана тима замењује именовани ресурс у мрежи **Сви чланови тима**.

#### <a name="use-a-resource-proposal-for-resource-requests"></a>Коришћење предлога ресурса за захтеве за ресурсе

Уместо да директно резервише ресурс у захтеву за ресурсе, менаџер ресурса може да предложи ресурс менаџеру пројекта. Менаџер ресурса могао би користити ову опцију када није доступно тачно подударање са захтевима. Када менаџер ресурса предложи ресурс, менаџер пројеката види да је поље **Статус** за генеричког члана тима промењено у **Захтева преглед**.

Можете погледати предложени ресурс заједно са визуелизацијом ефекта резервације предлога. 

1. Двапут кликните на члана тима који има статус **Потребан преглед**. 
2. Изаберите картицу **Предложени ресурси**.
3. Изаберите **Прихвати све предлоге** да прихвате све предложене ресурсе или **Одбаците све предлоге** да их одбаците. Ако прихватите предложене ресурсе, они се фиксно резервишу за пројекат као чланови тима и замењују генеричке ресурсе.

> [!NOTE]
> Морате или прихватити или одбацити све предложене ресурсе. Не можете их делимично прихватити ни одбацити.

### <a name="substitute-a-resource-on-the-project-team"></a>Замена ресурса у пројектном тиму

Понекад менаџер пројекта мора заменити резервисаног члана тима за пројекат.

1. У обрасцу **Пројекти**, на картици **Тим**, изаберите ресурс којем је потребна замена, а затим изаберите **Одржавање резервација**.
2. Проширите ресурс за преглед пројеката којима је додељен.
3. Кликните десним тастером миша на пројекат, а затим изаберите **Замена ресурса**.
4. Ако знате ресурс који желите да замените тренутним ресурсом, изаберите или унесите име, а затим изаберите **Поново додели**.

Или. ако треба да потражити ресурс, извршите следеће кораке.

1. Изаберите **Проналажење замене**.

   Помоћник за заказивање приказује листу доступних замена. У помоћнику за заказивање можете додатно филтрирати доступне ресурсе да бисте пронашли одговарајућу замену.

2. Да бисте заменили ресурс, одаберите ресурс који желите, а затим изаберите **Замени**.   

   Резервације и доделе замењују се новим ресурсом.

## <a name="reconcile-team-member-bookings-and-assignments"></a>Усаглашавање резервација и додела чланова тима

За чланове тима, резервације и доделе су лабаво повезани. Другим речима, ресурси могу имати доделе, али не и резервације или могу имати резервације, али не и доделе. У идеалном случају, резервације и доделе треба да се ускладе тако да ресурси имају потребан капацитет да изврше додељене задатке. Међутим, резервације се могу заснивати на доступности, а временски распоред задатака може се мењати током пројекта. Стога, лабава повезаност резервација и додела пружа флексибилност.

Project Operations има картицу **Усаглашавање** која омогућава менаџерима пројеката да усагласе резервације чланова тима и њихове доделе за пројектне тимове.

Картица **Усаглашеност** приказује резервације и доделе све до нивоа доделе појединачног задатка за сваког члана тима. Приказује сате у ћелијама који представљају временске периоде, од месеци, па све до дана.

Картица такође приказује укупни нето износ пројекта, заједно са колоном за укупну вредност.

Картица за сваки ресурс израчунава разлику између резервација члана тима и укупног броја додељених задатака члана тима. У идеалном случају, та разлика би требало да буде 0 (нула). Другим речима, не би требало да постоји разлика између резервација и додела. Разлике су обојене и засенчене како би се скренула пажња на две појаве:

- **Недостатак резервација**: Настаје када ресурс има више додела него резервација. Будући да овај капацитет није резервисан, менаџер пројекта може да коригује ту појаву проширивањем резервација ресурса како би покрио недостатак.
- **Прекомерне резервације**: Настаје када је ресурс резервисан за пројекат, али није додељен задацима. Та појава може бити прихватљива у случајевима када је ресурс резервисан за пројекат пре доделе задатка. Међутим, у другим случајевима се не планира додељивање ресурса задацима. У тим случајевима, менаџер пројекта треба да размотри отказивање резервација ресурса, тако да капацитет може да се користи за други пројекат.

У неким случајевима, када прегледате време на вишем нивоу од нивоа дана, нпр. на месечном нивоу, можда ћете видети нето разлику која је нула за ресурс. Другим речима, резервације = доделе. Међутим, ако прегледате време на нивоу недеље, можда ћете видети да постоје доделе од нула сати и резервације од 40 сати у првој недељи, али доделе од 40 сати и резервације од нула сати у другој недељи. Све у свему, резервације и доделе се усклађују, али се разликују од једне до друге недеље.

Када прегледате време на вишим нивоима, ћелије на картици **Усаглашеност** имају индикатор који ће вас обавестити да постоје разлике на нижим нивоима. Двапут кликните на ћелију можете да је повећате како бисте видели разлику. Затим можете да кликните десним тастером миша да бисте је умањили. Ако изаберете ресурс, а затим изаберете контролу **Следећа разлика** на траци са алаткама мреже, можете прећи на следећу разлику између резервација и додела за тај ресурс. Изаберите **Претходна разлика** да се вратите. Такође можете искључити индикатор разлике и понашање у навигацији у делу **Подешавања**.

Ако имате доделе задатака за ресурс, али нема резервација, на обрасцу **Пројекти** на картици **Усаглашавање** изаберите недостатак резервација, а затим **Продужи резервацију**. Појављује се дијалог **Продужење резервације** и приказује резервацију која је потребна да се реши проблем са недостатком ресурса. Дијалог такође показује постојеће резервације ресурса за све пројекте или друге ентитете који се могу заказивати. Ако изаберете **У реду** да бисте креирали резервацију за ресурс, без обзира на доступност тог ресурса, можете проузроковати прекомерну резервацију.

Менаџер пројекта или менаџер ресурса тада може да користи табелу распореда како би управљао било којом ситуацијом у којој је ресурс прекомерно резервисан у односу на његов капацитет.