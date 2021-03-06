---
title: Понашање корисничког интерфејса за ставку времена
description: Ова тема пружа информације о понашању корисничког интерфејса за ставку времена.
author: stsporen
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 86f805cd33f81e70bf9ae3c1fb20a1c310473604
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961745"
---
# <a name="time-entry-ui-behavior"></a>Понашање корисничког интерфејса за ставку времена

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_


Мрежа **Седмична ставка времена** је прилагођена контрола која садржи два главна одељка, **Димензије** и **Трајање**.

## <a name="dimensions"></a>Димензије
Одељак **Димензије** приказује димензије за које се време може унети. Следеће димензије су подржане као унапред дефинисане:

  - Project
  - Пројектни задатак
  - Улога
  - Тип
  - Статус ставке

Одељак **Димензије** не дозвољава унутрашње уређивање. Овај одељак је подржан приказом који омогућава да се прилагођена поља додају у мрежу седмичних ставки времена.

## <a name="duration"></a>Трајање
Одељак Трајање приказује дане у недељи као заглавља колона. Овај одељак омогућава унутрашње уређивање. Када се креира ред за ставку времена са одговарајућим димензијама, корисници могу брзо унети количину времена коју су утрошили за те димензије.

## <a name="create-a-new-time-entry"></a>Креирање нове ставке времена

1. У мрежи ставке времена, изаберите **Ново**. 
2. У дијалогу **Брзо креирање ставке времена** изаберите датум ставке времена.
3. Унесите податке за димензије **Пројекат**, **Пројектни задатак**, **Улога** и **Трајање**. Ове информације треба додавати за минуте, сате или дане куцањем **h**, **m** или **d**, заједно са бројем. 
4. Унесите опис за ставку и све коментаре који се могу делити екстерно у вези са ставком времена. 

Када сачувате ставку, унете вредности се приказују у одељку **Димензије**. Информације унете у поље **Трајање** се појављују за датум за који је креирана ставка времена.

Поља за проналажење подржавају системски прикази. На пример, након што корисник унесе пројекат, поље **Пројектни задатак** се подразумевано подешава на приказ **Копирање**. Да бисте креирали ставке времена за задатке који нису додељени кориснику, изаберите **Промени приказ** у дијалогу за претраживање, а затим изаберите **Сви задаци активног пројекта**.

## <a name="edit-a-time-entry"></a>Уређивање ставке времена 
Детаљи из неких поља на страници за ставку времена, као што су **Опис** и **Спољни коментари**, нису приказани у мрежи седмичних ставки времена. Уместо тога, у ћелијама **Трајање** приказује се мали троугласти индикатор који има ове додатне детаље. 

1. Да бисте уредили ставку времена, изаберите ћелију коју желите да ажурирате у ставци времена.
2. Изаберите **Уреди детаље** да бисте ажурирали податке у окну **Главни образац за унос времена**. 

## <a name="copy-a-time-entry-row"></a>Копирање реда ставке времена
Када се креира први ред, можете изабрати **Копирај ред** да бисте ископирали цео ред у нови ред. Када се ред копира на овај начин, димензије и трајање се такође копирају. Такође можете да изаберете **Измени ред** да бисте ажурирали вредности димензија и трајања у одељку **Трајање**.

## <a name="open-a-time-entry-behavior"></a>Отварање понашања ставке времена
Да би се подржао оптималан и брз унос у најистакнутија поља, мрежа седмичних ставки времена показује подскуп изабраних димензија и трајања времена. Да бисте видели све детаље једне ставке времена, у делу **Измена ставке** одаберите **Отвори**.

## <a name="submit-a-time-entry"></a>Прослеђивање ставке времена
Можете проследити једну ставку времена или групу ставки времена избором блока ћелија или целог реда ставке времена, а затим избором опције **Проследи**. Прослеђене ставке времена појављују се као ставке које чекају одобрење на страници даваоца одобрења **Одобрење**. Након успешног прослеђивања ставки времена, оне се не могу уређивати.

## <a name="recall-a-time-entry"></a>Опозивање ставке времена
Можете опозвати ставке времена које сте проследили. Можете да опозовете једну ставку времена, блок ставки времена или читав ред ставки времена. Опозване ставке времена можете уређивати.

## <a name="time-entry-status"></a>Статус ставке времена

- **Радна верзија**: Новим ставкама времена аутоматски се додељује статус **Радна верзија**. Само ставке времена које имају статус **Радна верзија** можете да избришете.
- **Прослеђено**: Када се проследи ставка времена, статус се ажурира на **Прослеђено**. 
- **Одобрено**: Када се прослеђена ставка времена одобри, статус се ажурира на **Одобрено**. 
- **Враћено**: Ако је ставка времена одбијена, статус се ажурира на **Враћено** и ставка постаје доступна за исправку и поновно прослеђивање. 

## <a name="view-rejection-comments"></a>Преглед коментара о одбацивању
Када давалац одобрења одбаци ставку времена, може да дода коментаре о како би помогао ресурсу да схвати разлог одбацивања. Да бисте видели коментаре о одбацивању ставке времена, изаберите **Отвори ставку**. Коментари о одбацивању биће приказани на временској оси. Корисник може одговорити на коментаре о одбијању пре него што поново пошаље ставку.

## <a name="copy-week"></a>Копирај седмицу
Након креирања неколико ставки времена, корисници могу истовремено креирати више ставки времена.

1. У обрасцу **Ставке времена** изаберите **Копирај недељу** да бисте групно креирали додатне ставке времена. 
2. У дијалогу **Копирање**, у одељку **Од периода** користите поља **Датум почетка** и **Датум завршетка** да дефинишете опсег датума из којег треба копирати ставке времена. 
3. У одељку **У период**, у пољу **Датум почетка**, одредите датум за који ћете креирати ставке времена. 
4. Изаберите **Копирај**. За одређени датум у одељку **До периода**, креира се копија ставки времена за одговарајући дан у недељи у одељку **Од периода**. На пример, ставка времена за понедељак из прошле недеље се копира у понедељак оне седмице која је наведена као **До периода**.

## <a name="import"></a>Увоз
Исти основни поступак користи се за увоз из резервација, додела и размена. Можете одредити опсег датума резервација за увоз, а затим експлицитно изабрати резервације које би требало да буду креиране као радне верзије ставки времена. 
