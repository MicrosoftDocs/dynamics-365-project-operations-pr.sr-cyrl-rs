---
title: Шта је ново у септембру 2022. – Project Operations за ресурс/сценарије који нису засновани на залихама
description: Овај чланак пружа информације о квалитетним исправкама које су доступне у издању корпорације Мицрософт у септембру Dynamics 365 Project Operations 2022.
author: ramagadu
ms.date: 09/28/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: ef8b4dd98d64dac1e2420f8e6a104258f126f112
ms.sourcegitcommit: a2d720ac6d7ddb20a0967fe87992a376b2478208
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/04/2022
ms.locfileid: "9621369"
---
# <a name="whats-new-september-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Шта је ново у септембру 2022. – Project Operations за ресурс/сценарије који нису засновани на залихама

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Овај чланак се односи на следеће компоненте и верзије корпорације Мицрософт Dynamics 365 Project Operations:

- Операције пројекта у верзији Dataverse окружења 4.46.0.60
- Управљање пројектима и рачуноводство у Дyнамицс 365 Финанце окружењу верзија 10.0.29

## <a name="features-included-in-this-release"></a>Функције укључене у овом издању

| Област функција | Име функције | Више информација |
| --- | --- | --- |
| Управљање могућностима за пословање | **Ревизија и активирање понуда**<br>Пројектне операције доносе пуну подршку процеса продаје. Понуде пројекта се могу активирати тако да представљају стање у којем је понуда само за читање и када се редигује. Активиране понуде се могу кориговати да би се креирале нове понуде које имају постепени број ревизије. Активиране понуде пројекта или ревизије понуда могу бити затворене као освојене или изгубљене. | [Активирање и кориговање понуде за пројекат](/dynamics365/project-operations/sales/activation-and-revision) |
| Наплата и одређивање цена | **Подразумевана агностички цена временске зоне**<br>Пројектне операције су увеле концепт агностичног датума временске зоне на свим стварним пројектима. Ново поље Датум трансакције **је сада доступно** у редовима налога и стварним вредностима и користиће се за складиштење датума када је трансакција извршена, али без конвертовања тог датума у координирано универзално време. Овај датум ће се користити за низводне процесе као што су подразумевана цена и креирање фактура. | <p>[Утврђивање стопе трошкова за процене и стварне вредности засноване на пројекту](/dynamics365/project-operations/pricing-costing/cost-price-resolution)</p><p>[Утврђивање продајних цена за процене и стварне вредности засноване на пројекту](/dynamics365/project-operations/pricing-costing/sales-price-resolution)</p> |
| Наплата и одређивање цена | **Датум -ефективна цена замењује у пројектном пословању**<br>Замене цена које су ефективне за датум обезбеђују начин да се замене или промене одређене цене у ценовник. | [Премошћава цена која је ефективна](/dynamics365/project-operations/pricing-costing/dateffective_price_overrides) |
| Подизвођача | **Сравњење подизвођачи и сравњење фактуре добављача**<br>Ова функција омогућава купцима да креирају подизвођачи за време набавке, категорије трошкова и материјале који се користе за рад на пројекту. Такође омогућава купцима да забележе, у апликацијама за финансије и операције, фактуре добављача које ће бити доступне менаџерима пројекта Dataverse ради провере. | <p>[Управљање подизвођачима](/dynamics365/project-operations/pro/subcontracting/managing-subcontracts-overview)</p><p>[Креирање фактура продавца](/dynamics365/project-operations/procurement/vendor-invoicing-concept-and-creation)</p> |
| Време и трошак | **Глобална особа која врши одобравање**<br>Ова функција омогућава независном продавцу софтвера (ИСВ) и централизовано одобравање, без обзира на статус члана пројекта или тима у пројекту. | [Безбедност и одобрења](/dynamics365/project-operations/approvals/approvals-security) |
| Управљање трошковима | **Могућност књижења одговорности трошкова у валути добављача**<br>Ова функција омогућава књижење извештаја о трошковима у валути добављача за начин плаћања готовином. | [Могућност књижења одговорности трошкова у валути добављача](/dynamics365/project-operations/expense/posting-expense-reports#enable-the-ability-to-post-expense-liability-in-vendor-currency-for-cash-payment-method-feature) |
| Набавка пројеката | **Плаћање приликом плаћања уплатама добављача**<br>Ова функција омогућава да се функција "Плати када се плати(ПWП)" користи са не-берзанским окружењима пројектних операција. Омогућава да се уплате добављача блокирају/задржавају, на основу услова задржавања, све док се уплата не прими од купца. | [Плаћање приликом плаћања уплатама добављача](/dynamics365/project-operations/procurement/pay-when-paid) |
| Набавка пројеката | **Требовања набавке пројекта**<br>Ова функција омогућава корисницима да креирају излазне поруџбине везане за пројекат у правним лицима у којима је омогућена Дyнамицс 365 Цустомер Енгагемент пројекта. Излазне поруџбине пројекта се могу користити за записивање ненапуштене набавке материјала у односу на пројекат од стране одељења за набавке персона. Излазне поруџбине пројекта неће бити синхронизоване са Dataverse. Међутим, виртуелни ентитет можете користити за површину редова излазне поруџбине пројекта за информације Dataverse о менаџеру пројекта. Трошак фактуре добављача повезан са пројектом је интегрисан са ентитетом Пројецт Ацтуалс у програму Dataverse. Трошак пројекта се записује у подстанар пројекта помоћу налога за интеграцију операција пројекта. | |

## <a name="project-operations-dual-write-maps-updates"></a>Ажурирања мапа двоструког уписивања за Project Operations

Следећа табела приказује мапе са два писања које су измењене или додате у издању пројектних операција у септембру 2022.

| Мапа ентитета | Ажурирана верзија | коментара |
| -------------- | ------------------- | ------------|
| Project Operations стварне вредности интеграције (msdyn_actuals) | 1.0.0.15. | Ова мапа подржава обраду стварних подизвођачима са операцијама пројекта за сценарије засноване на ресурсима. |
| Project Operations ентитет извоза фактуре продавца (msdyn_projectvendorinvoices) | 1.0.0.2 | Ова мапа подржава обраду стварних подизвођачима са операцијама пројекта за сценарије засноване на ресурсима. |
| Project Operations ентитет извоза реда фактуре продавца (msdyn_projectvendorinvoicelines) | 1.0.0.5 | Ова мапа подржава обраду стварних подизвођачима са операцијама пројекта за сценарије засноване на ресурсима. |

Увек покрените најновију верзију мапе у окружењу и омогућите све повезане мапе табела док ажурирате решење за пројектне операције Dataverse и верзију финансијског решења. Неке функције и могућности можда неће исправно функционисати ако најновија верзија мапе није активирана. Активну верзију мапе можете видети у колони **Верзија** на страници **Двоструко уписивање**. Да бисте активирали нову верзију мапе, изаберите **Верзије табеле мапе**, изаберите најновију верзију, а затим сачувајте изабрану верзију. Ако сте прилагодили мапу табеле без оквира, поново примените промене. За још информација погледајте [Управљање животним циклусом апликације](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Ако наиђете на проблем приликом почетка мапе, следите упутства [у проблему са колонама табеле које недостају у одељку мапе](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) водича за решавање проблема са двоструким уписивања.

## <a name="quality-updates"></a>Исправке квалитета

### <a name="project-operations-on-dataverse"></a>Project Operations у услузи Dataverse

| Област функција | Референтни број | Исправка квалитета |
| --- | --- | --- |
| Наплата и одређивање цена | 2754422. | Процене материјала и трошкова се не сливају у финансије када се пројекти копирају у Dataverse програму. |
| Време и трошак | 2787409. | Особа која не важи може да одобри унос времена које није пројектно. |
| Управљање могућностима за пословање | 2788907. | Ажурирана порука о грешци приликом провере ваљаности јединствености за редове поруџбине који укључују заставице. |
| Време и трошак | 2842253. | Без начина руковања изузетком за одобравање времена. |
| Наплата и одређивање цена | 2844181. | Ако не добијете ИД корелације, блокира се креирање фактуре. |
| Наплата и одређивање цена | 2876628. | QЛД, ЦЛД - Процена решења ценовног листа треба да користи застарела поља опсега датума ценовник. |
| Подизвођача | 2893222. | Ако није наведена улога за ред подизвођачи, требало би да буде могуће изабрати тај ред у члану тима за било коју улогу. |

### <a name="project-management-and-accounting-in-finance"></a>Управљање пројектима и рачуноводство у финансијама

За информације о исправкама грешака које су укључене у ову исправку пријавите се Microsoft Dynamics у услуге животног циклуса и погледајте чланак у [бази знања](https://fix.lcs.dynamics.com/Issue/Details?bugId=726559).

## <a name="features-turned-on-by-default-in-upcoming-release"></a>Функције су подразумевано укључене у предстојећем издању

Следећа табела наводи функције које су подразумевано укључене у верзији 10.0.30. Већина функција које су аутоматски укључене може бити искључена у управљању [функцијама](/dynamics365/fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview). Убудуће, неке функције које су аутоматски укључене могу бити уклоњене из управљања функцијама и постати обавезне. Ова промена обезбеђује да клијенти користе тренутну функционалност, тако да побољшања могу да се надограде на тренутној функционалности док се додају. Функције никада неће бити аутоматски омогућене за мање од годину дана, осим ако нису утврђене да су од суштинског значаја.

| Име функције | Омогући датум | Додата функција | Статус функције | Модул |
| --- | --- | --- |--- |--- |
| Омогући асинц операцију када корисник треба да се пребацује између операција синхронизације и асинца | 21. октобар 2022. | 9. април 2021. | Укључено по подразумеваној вредности | Управљање трошковима |
| Процена смерница трошкова за потребне потврде | 21. октобар 2022. | 20. децембар 2021. | Укључено по подразумеваној вредности | Управљање трошковима |
| Приказ листе извештаја о трошковима које су креирали делегирање радника | 21. октобар 2022. | 19. фебруар 2020. | Укључено по подразумеваној вредности | Управљање трошковима |
| Укупна километража обрачуна по фискална година | 21. октобар 2022. | 10. мај 2022. | Укључено по подразумеваној вредности | Управљање трошковима |