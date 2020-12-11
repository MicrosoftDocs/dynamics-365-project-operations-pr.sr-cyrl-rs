---
title: Чињенице које треба узети у обзир приликом надоградње – Microsoft Dynamics 365 Project Service Automation верзије 2.x или 1.x на верзију 3.x
description: Ова тема пружа информације о чињеницама које морате узети у обзир приликом надоградње апликације Project Service Automation са верзије 2.x или 1.x на верзију 3.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/13/2018
ms.topic: article
author: JohnPBurrows
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 3c51726f71cfd0d4be98982d6a02268d64a70b91
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121731"
---
# <a name="upgrade-considerations---psa-version-2x-or-1x-to-version-3"></a>Чињенице које треба узети у обзир приликом надоградње - PSA верзије 2.x или 1.x на верзију 3.x
[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="project-service-automation-and-field-service"></a>Project Service Automation и Field Service
И Dynamics 365 Project Service Automation и Dynamics 365 Field Service користе Universal Resourcing Scheduling (URS) решење за планирање ресурса. Ако у вашој инстанци имате и Project Service Automation и Field Service, требало би да планирате надоградњу оба решења на најновију верзију (верзију 3.x за Project Service Automation, верзију 8.x за Field Service). Надоградњом апликације Project Service Automation или Field Service ћете инсталирати најновију верзију решења URS, што значи да је неусаглашено понашање могуће ако се и Project Service Automation и Field Service решење у истој инстанци не надограде на најновију верзију.

## <a name="resource-assignments"></a>Доделе ресурса
У апликацији Project Service Automation верзије 2 и 1, додељивања задатака су складиштена као подређени задаци (такође познати као задаци ставке) у **ентитету задатка** и били су индиректно повезани са ентитетом **Додела ресурса**. Задатак ставке је био видљив у искачућем прозору за доделу у оквиру структурне анализа посла (САП).

![Задаци ставке у САП-у у решењу Project Service Automation у верзији 2 и верзији 1](media/upgrade-line-task-01.png)

У верзији 3 апликације Project Service Automation, основна шема додељивања ресурса који се могу резервисати задацима је промењена. Задатак ставке је застарео и постоји директни 1:1 однос између задатка у **ентитету задатка** и члана тима у ентитету **Додела ресурса**. Задаци који су додељени члану пројектног тима сада се складиште директно у ентитету Додела ресурса.  

Ове промене утичу на надоградњу свих постојећих пројеката који имају доделе ресурса за именоване ресурсе који се могу резервисати и генеричке ресурсе у тиму пројекта. Ова тема обезбеђује чињенице које треба узети у обзир за пројекте приликом надоградње на верзију 3. 

### <a name="tasks-assigned-to-named-resources"></a>Задаци су додељени именованим ресурсима
Ако користите основни ентитет задатка, задаци у верзији 2 и 1 дозвољавају члановима тима да приказују улогу која није њихова подразумевана дефинисана улога. На пример, Дуња Николић, којој је подразумевано додељена улога менаџера програмима, може бити додељен задатку са улогом програмера. У верзији 3, улога именованог члана тима је увек подразумевана, тако да сваки задатак који је додељен Дуњи Николић користи њену подразумевану улогу менаџера програмима.

Ако сте доделили ресурс задатку ван његове подразумеване улоге у верзији 2 и 1, када извршите надоградњу, именованом ресурсу ће бити додељена подразумевана улога за све доделе задатака, без обзира на доделу улоге у верзији 2. Ово ће довести до разлика у израчунатим проценама у верзији 2 или 1 у односу на верзију 3 зато што се процене израчунавају на основу улоге ресурса, а не доделе задатка ставке. На пример, у верзији 2, два задатка је додељено Павлу Кнежевићу. Улога у задатку ставке за 1. задатак је програмер, а за 2. задатак менаџер програмима. Павле Кнежевић има подразумевану улогу менаџера програма.

![Више улога је додељено једном ресурсу](media/upgrade-multiple-roles-02.png)

С обзиром на то да се улоге програмера и менаџера програма разликују, процене трошкова и продаје су следеће:

![Процене трошкова за улоге ресурса](media/upggrade-cost-estimates-03.png)

![Процене продаје за улоге ресурса](media/upgrade-sales-estimates-04.png)

Када извршите надоградњу на верзију 3, задаци ставке се замењују доделама ресурса у задатку члана тима ресурса који се може резервисати. Додела ће користити подразумевану улогу ресурса који се може резервисати. На следећем графикону, Павле Кнежевић који има улогу менаџера програмима, јесте ресурс.

![Доделе ресурса](media/resource-assignment-v2-05.png)

Пошто су процене засноване на подразумеваној улози за ресурс, могу се променити процене продаје и трошкова. Имајте на уму да на следећем графикону више нећете видети улогу **Програмер** јер је сада узета из подразумеване улоге ресурса који може да се резервише.

![Cost estimates for default roles](media/resource-assignment-cost-estimate-06.png)
![Процена трошкова за подразумеване улоге](media/resource-assignment-sales-estimate-07.png)

Након надоградње, можете да уредите улогу члана тима тако да буде нешто друго од додељене подразумеване улоге. Међутим, ако промените улогу члана тима, она ће бити промењена у свим додељеним задацима зато што члановима тима више није дозвољено додељивати више улога у верзији 3.

![Ажурирање улоге ресурса](media/resource-role-assignment-08.png)

Ово важи и за задатке ставке који су били додељени именованим ресурсима када промените организациону јединицу ресурса од подразумеване вредности у другу организациону јединицу. Када се заврши надоградња на верзију 3, додела ће користити подразумевану организациону јединицу ресурса уместо оне која је подешена у задатку ставке.

### <a name="tasks-assigned-to-generic-resources"></a>Задатак је додељен генеричким ресурсима
У верзији 2 и 1, можете да подесите улогу и организациону јединицу за задатак, а затим да користите функцију **Генериши тим** да бисте генерисали генеричке ресурсе на основу атрибута који су подешени за задатак. У верзији 3 можете креирати генеричке чланове са улогом и организационом јединицом, а затим доделити чланове тима задацима.

У верзији 2 и 1, пројекти са генеричким ресурсима могу да имају два статуса или њихову комбинацију на нивоу задатка. На пример, можете да имате следеће сценарије:

- Задаци са подешеним улогама и скупом организационих јединица, али без повезан доделе ресурса су генерисани.
- Задаци са доделама генеричких чланова тима који су додељени креирањем генеричког ресурса помоћу функције **Генериши тим**.

Пре него што започнете надоградњу, препоручујемо да поново генеришете тим за сваки пројекат који има задатке додељене генеричким ресурсима или за које тек треба да се покрене процес генеричког тима.

За задатке који су додељени генеричким члановима тима који су генерисани помоћу функције **Генериши тим**, надоградња ће оставити генерички ресурс у тиму и оставиће доделу том генеричком члану тима. Препоручујемо да након надоградње генеришете потребу за ресурсом за генеричког члана тима, али пре него што резервишете или проследите захтев за ресурс. То ће сачувати све доделе организационе јединице за генеричке чланове тима који се разликују од уговорне организационе јединице пројекта.

На пример, у пројекту Ш, уговорна организациона јединица је Contoso US. У пројектном плану, задаци тестирања у фази имплементације си додељени улози Технички консултант, а додељени организациона јединица је Contoso India.

![Додела организације у фази имплементације](media/org-unit-assignment-09.png)

Након фазе имплементације, задатак тестирања интеграције се додељује улози Технички консултант, али се организација подешава на Contoso US.  

![Додела задатка тестирања интеграције у организацији](media/org-unit-generate-team-10.png)

Када генеришете тим за пројекат, два генеричка члана тима се креирају због различитих организационих јединица за задатак. 1. технички консултант биће додељен задацима компаније Contoso India, а 2. технички консултант ће имати задатке компаније ће Contoso US.  

![Генерички чланови тима су генерисани](media/org-unit-assignments-multiple-resources-11.png)

> [!NOTE]
> У апликацији Project Service Automation у верзијама 2 и 1, члан тима не одржава организациону јединицу, која се одржава у задатку ставке.

![Задаци ставке за верзију 2 и верзију 1 у решењу Project Service Automation](media/line-tasks-12.png)

Организациону јединицу можете видети у приказу предвиђања. 

![Процене организационих јединица](media/org-unit-estimates-view-13.png)
 
Када се надоградња доврши, организациона јединица у задатку ставке која одговара генеричком члану тима додаје се том члану, а задатак ставке ће бити уклоњен. Због овога препоручујемо да пре надоградње генеришете или поново генеришете тим за сваки пројекат који садржи генеричке ресурсе.

За задатке који су додељени улози са организационом јединицом која се разликује од организационе јединице пројекта за уговарање, а тим није генерисан, надоградња ће креирати генеричког члана тима за улогу, али ће користити уговорну јединицу пројекта за организациону јединицу члана тима. Ако се вратимо на пример пројекта Ш, то значи да је уговорна организациона јединица Contoso US и да су задаци тестирања пројектног плана у оквиру фазе имплементације додељени улози Технички консултант, а да је организациона јединица додељена компанији Contoso India. Задатак тестирања интеграције, који је довршен након фазе имплементације, додељен је улози Технички консултант. Организациона јединица Contoso US и тим нису генерисани. Надоградња ће креирати једног генеричког члана тима, техничког консултанта који има додељене сате за сва три задатка, као и организациону јединицу Contoso US, уговорну организациону јединицу пројекта.   
 
Промена подразумеваних вредности различитих организационих јединица за обезбеђивање ресурса за чланове тима који нису генерисани је разлог због којег препоручујемо да пре надоградње генеришете или поново генеришете тим за сваки пројекат који садржи генеричке ресурсе, како се доделе организационих јединица не би изгубиле.
