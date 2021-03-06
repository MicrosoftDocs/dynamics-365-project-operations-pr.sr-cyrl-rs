---
title: Понуде – кључни концепти
description: Ова тема пружа информације о понудама за пројекте и понудама за продају које су доступне у услузи Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: b252f6e02d0809c352d3665731ec5e02e4e9a73f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898460"
---
# <a name="quotes---key-concepts"></a>Понуде – кључни концепти

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_

У услузи Dynamics 365 Project Operations постоје два типа понуда – за пројекат и за продају. Ова два типа понуда се разликују на следеће начине:

- **Мреже за ставке**: у понуди за продају постоји само једна мрежа за ставке. У понуди за пројекат постоје две мреже за ставке. Једна мрежа је за пројектне линије, а друга за производне линије.
- **Активација и ревизије** : понуде за продају подржавају активацију и ревизије. Ови процеси нису подржани у понуди за пројекат.
- **Приложене понуде**: понуди за продају можете приложити више поруџбина. У понуду за пројекат можете да приложите само један уговор о пројекту.
- **Освајање понуде**: када освојите понуду за продају, сродна прилика може остати отворена. Када вам одобре понуду за пројекат, биће затворена повезана могућност за пословање.
- **Поља и концепти**: понуда за продају не садржи нека поља и концепте који су обухваћени у понуди за пројекат. У поља спадају **Уговорна јединица**, **Менаџер за пословне контакте** и **Име контакта за фактурисање**.  
- **Тип**: Понуде за продају и понуде за пројекте идентификује и поље засновано на скупу опција под називом **Тип**. За понуду за продају, ово поље има вредност **Засновано на ставци**. За понуду за пројекат, има вредност **Засновано на раду**.

Ова тема се фокусира на детаље понуда пројеката.

Понуда за пројекат у апликацији Project Operations може да има више ставки предмета или ставки понуде. У ствари, понуда за пројекат има две мреже за ставке предмета. Једна мрежа је намењена ставкама заснованим на пројекту и омогућава детаљне процене. Друга мрежа је намењена ставкама заснованим на производу и користи једноставну јединичну цену и приступ заснован на количини.

- **Засновано на пројекту**: износ (понуђена вредност) утврђује се након процене количине посла. Можете проценити рад на високом нивоу, директно као детаље реда испод сваке ставке понуде, или на основу основаних процена, користећи пројекат и пројектни план. Ставке понуде засноване на пројекту се налазе само у понудама заснованим на пројекту које се креирају помоћу апликације Project Operations. Овај тип ставке понуде је прилагођени образац ручно додатих ставки понуде које су доступне у систему Microsoft Dynamics 365 Sales.

- **Засновано на производу**: понуђена вредност се одређује на основу количине продатих јединица и продајне цене. Производ у ставци заснованој на производу може доћи из каталога производа у Продаји или може бити производ који дефинишете. Овај тип ставке понуде је такође доступан у понудама заснованим на пројекту које се креирају помоћу апликације Project Operations.

Износ у понуди је збирна вредност свих ставки заснованих на производу и ставки заснованих на пројекту.

> [!NOTE]
> Понуде и ставке понуда нису потребне у апликацији Project Operations. Процес пројекта можете започети уговором о пројекту (продат пројекат). Међутим, увек је потребна могућност за пословање, без обзира на то да ли сте започели понудом или уговором о пројекту.

## <a name="project-based-quote-lines"></a>Ставке понуде засноване на пројекту

Ставка понуде заснована на пројекту у апликацији Project Operations има следеће начине наплате:

- Време и материјал
- Фиксна цена

### <a name="time-and-material"></a>Време и материјал

Начин наплате времена и материјала је заснован на утрошку. Када изаберете овај начин наплате, клијенту се фактурише током остваривања трошкова пројекта. Учесталост креирања фактуре је периодична и заснована на датуму. Током процеса продаје, понуђена вредност компоненте времена и материјала клијенту даје само процену коначних трошкова. Продавац се не обавезује да ће довршити пројекат са тачном понуђеном вредношћу. Компоненте времена и материјала повећавају ризик клијента. Клијенти ће можда желети да испреговарају додатне одреднице у вези са износом који не сме да се премаши да би умањили ризик. Project Operations не подржава подешавање одредница у вези са износом који не сме да се премаши.

### <a name="fixed-price"></a>Фиксна цена

Начин наплате Фиксна цена омогућава продавцу да се обавеже да ће пројекат испоручити клијенту по фиксној цену. Клијенту се наплаћује понуђена вредност ставке понуде са фиксном ценом, без обзира на трошкове које продавац остварује приликом испоруке те ставке понуде. Вредност ставке понуде са фиксном ценом се наплаћује на један од следећих начина: 

- Као обједињена сума износа на почетку или крају пројекта или када се дође до контролне тачке у пројекту. 
- На једнаке рате фиксне вредности у ставци понуде. Њихова учесталост је заснована на одређеном датуму. Ове рате су познате као периодичне контролне тачке.
- У ратама са монетарном вредношћу која је усклађена са напретком посла или специфичним контролним тачкама које испуњавате за пројекат. У овом случају, вредност сваке рате може да се разликује, али износ свих рата мора да буде фиксна вредност у ставци понуде.

Project Operations подржава све три врсте распореда фактурисања за ставке понуде са фиксном ценом.

## <a name="transaction-classification"></a>Класификација трансакције

Организације које пружају професионалне услуге обично дају понуде клијентима и фактуришу клијентима по класификацији трошкова. Трошкови су представљени следећим класификацијама трансакција:

- **Време**: ова класификација представља трошкове рада или времена људских ресурса на пројекту.
- **Трошак**: ова класификација представља све остале врсте трошкова на пројекту. Пошто трошкови могу да буду широко класификовани, већина организација креира подкатегорије, попут путних трошкова, трошкова изнајмљивања аутомобила, хотелских трошкова или канцеларијских залиха.
- **Накнада**: ова класификација представља разне додатне трошкове, казне и друге ставке које се наплаћују клијенту. 
- **Порез**: ова класификација представља износе пореза које корисници додају док уносе трошкове.
- **Стварна трансакција**: ова класификација представља стварне вредности из ставки производа на потврђеној фактури за пројекат.
- **Контролна тачка**: ову класификацију користи логика наплате фиксне цене.

Неке од ових класификација трансакција могу да се повежу са сваком ставком понуде. Када вам одобре понуду, мапирање између класификације трансакције и ставке понуде се преноси у предмет уговора.
  
На пример, понуда може да садржи следеће две ставке понуде: 

- Консултантски посао који користи метод наплате времена и материјала у ком се могу примењивати класификације трансакција према времену и надокнади. На пример, све трансакције времена и накнаде за пример пројекта **Dynamics AX имплементација** се фактуришу клијенту на основу утрошеног времена и материјала. 
- Сродни путни трошкови који користе начин наплате Фиксна цена. На пример, сви путни трошкови за пример пројекта **Dynamics AX имплементација** се фактуришу по фиксној монетарној вредности.

> [!NOTE]
> Комбинација класификација пројекта и трансакције **Време**, **Трошкови**и **Накнада** повезана са ставком понуде или предметом уговора мора бити јединствена. Ако је иста комбинација класе пројекта и трансакције повезана са више од једног предмета уговора или ставки понуде, Project Operations неће радити исправно.

## <a name="billing-types"></a>Типови наплате

Поље **Врста наплате** дефинише концепт наплативости. То је скуп опција који има следеће могуће вредности:

- **Наплативо**: трошкови које је акумулирала ова улога/категорија су директни трошкови који доводи до извршење пројекта, а клијент ће платити за овај посао. Плаћање се може администрирати као аранжман заснован на времену и материјалу или аранжман са фиксном ценом. Међутим, запослени који утроши ово време добиће одговарајући кредит за наплативу укупну искоришћеност.
- **Ненаплативо**: трошкови које акумулира ова улога/категорија се сматрају директним трошковима који доводе до извршење пројекта, чак и ако клијент не схвата ову чињеницу и не жели да плати за овај посао. Запослени који утроши ово време неће добити кредит у форми наплативе укупне искоришћености рада.
- **Бесплатно**: трошкови које акумулира ова улога/категорија се сматрају директним трошковима који доводи до извршење пројекта, а клијент схвата ову чињеницу. Запослени који утроши ово време ће добити кредит за наплативу укупну искоришћеност рада. Међутим, ови трошкови се не наплаћују клијенту.
- **Није доступно**: трошкови који се акумулирају на интерним пројектима и не захтевају праћење прихода се прате помоћу ове опције.

## <a name="invoice-schedule"></a>Распоред за фактурисање

Распоред за фактурисање представља низ датума када се фактуришу трошкови за пројекат. Опционално можете да креирате распоред за фактурисање у ставци понуде у апликацији. Свака ставка понуде може имати свој распоред за фактурисање. Да бисте креирали распоред за фактурисање, морате обезбедити следеће вредности атрибута:

- Датум почетка наплате 
- Датум испоруке који представља датум завршетка наплате за пројекат
- Учесталост фактурисања

Користе се ове три вредности атрибута за генерисање условни скуп датума за успостављање фактурисања.

## <a name="invoice-frequency"></a>Учесталост фактурисања

Учесталост фактурисања је ентитет који складишти вредности атрибута које помажу да се изрази учесталост креирања фактуре. Следећи атрибути изражавају или дефинишу ентитет учесталости фактурисања:

- **Период**: месечни, двонедељни и седмични периоди су подржани. 
- **Број покретања у току периода:/** - за седмичне и двонедељне периоде можете дефинисати само једно покретање по периоду. За месечне периоде можете дефинисати између једног и четири покретања по периоду. 
- **Дани покретања**: дани када треба покренути фактурисање. Овај атрибут можете да конфигуришете на два начина:
  - **Радним данима**: на пример, можете да наведете да се фактурисање покреће сваког понедељка или сваког другог понедељка. Клијенти који морају да подесе покретање фактурисања радним даном можда преферирају овакву врсту конфигурације. 
  - **Календарски дани**: на пример, можете навести да се фактурисање покреће седмог и двадесетпрвог дана сваког месеца. Неке организације можда преферирају овакву врсту конфигурације, јер гарантује да се фактурисање покреће по фиксном распореду сваког месеца.
  
### <a name="invoice-schedule-for-a-fixed-price-quote-line"></a>Распоред за фактурисање за ставку понуде са фиксном ценом

За ставку понуде са фиксном ценом можете користити мрежу **Распоред фактурисања** да бисте креирали контролне тачке наплате које су једнаке вредношћу у ставци понуде.

- Да бисте креирали контролне тачке за наплату које су подједнако подељене, изаберите учесталост фактурисања, унесите датум почетка наплате у ставку понуде и изаберите **Захтевани датум завршетка** за понуду у одељку **Резиме** заглавља понуде. Затим изаберите **Генерисање периодичних контролних тачака** да бисте креирали подједнако подељене контролне тачке засноване на изабраној учесталости фактурисања. 
- Да бисте креирали контролну тачку наплате обједињене суме, креирајте контролну тачку, а затим унесите вредност ставке понуде као износ за контролну тачку.
- Да бисте креирали контролне тачке за наплату које су засноване на специфичним задацима у плану пројекта, креирајте контролну тачку и мапирајте је на елемент распореда пројекта у корисничком интерфејсу за наплату.
