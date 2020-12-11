---
title: Разматрања надоградње структурне анализе посла
description: Ова тема пружа информације о надоградњи структурне анализе посла из апликације Project Service Automation верзије 2.x у верзију 3.x.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0b75fd372732f42a3557aaa5eccec1f24a644941
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121821"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a>Разматрања надоградње структурне анализе посла
Ова тема пружа информације о надоградњи структурне анализе посла из апликације Project Service Automation верзије 2.x у верзију 3.x. Ова тема дефинише исправно стање пројекта у апликацији Project Service Automation (PSA), потребно за успешну надоградњу. Постоје и информације о уобичајеним условима блокирања који ће довести до неуспешне надоградње. Више информација о дефинисању пројектних задатака и њиховим функцијама у оквиру распореда пројекта потражите у чланку [Распореди пројеката](project-creating.md).

## <a name="key-entities"></a>Кључни ентитети
За исправну структурну анализу посла која је већ учитана са ресурсима, потребни су следећи ентитети:

- [Пројекат](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [Пројектни тим](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [Пројектни задатак](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [Доделе ресурса](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [Зависност пројектног задатка](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [Ресурси који могу да се резервишу](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

Да бисте дефинисали структурну анализу посла коју је учитао ресурс, морате да довршите следеће кораке:

1. Креирајте нови пројекат. За више информација о томе како да креирате нови пројекат, погледајте [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).
2. Креирајте један или више задатака. За више информација о томе како да креирате нови задатак, погледајте [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).
3. Дефинишите зависне елементе задатка. За још информација погледајте [Зависност пројектног задатка](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).
4. Доделите чланове пројектног тима пројекту. За више информација, погледајте [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).
5. Доделите чланове пројектног тима задацима. За више информација, погледајте [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).

## <a name="project-team-relationships"></a>Односи унутар пројектног тима

Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:
- Сви чланови пројектног тима морају бити повезани са ресурсом који се може резервисати.
- Сви чланови пројектног тима морају бити повезани са истим пројектом. 

## <a name="project-task-relationships"></a>Односи у оквиру пројектног задатка
Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:

- Сви повезани задаци морају бити повезани са истим пројектом.
- Сваки задатак ставке мора имати надређени задатак.
- Сваки задатак мора имати надређени пројекат.

### <a name="valid-conditions"></a>Важећи услови

- Трајање сваког задатка мора бити дуже од сат времена или једнако том времену (>=) и краће од 1.800.000 минута (1250 дана).*
- Сви задаци морају имати датум почетка који није пре 1.1.2000.*
- Сви задаци морају имати датум почетка који је најдаље 17 година од данашњег дана.*
- Сви задаци морају да имају датум почетка који је пре датума завршетка или исти као тај датум.
- Све врсте трансакција за класификације (Трошкови, Материјал, Порез и Време) морају имати вредности за ставке **Подразумевана јединица** и **Група јединица**.
- Формате датума са словима треба избегавати.

### <a name="potential-mitigation-steps"></a>Потенцијални кораци за ублажавање
- Користите напредну претрагу за идентификацију пројектних задатака који не садрже ID пројекта.
- Користите напредну претрагу да бисте идентификовали пројектне задатке где је заказано трајање дуже од > 1.800.000.
- Пре него што унесете било какве промене података, требало би да истражите сва прилагођавања повезана са ентитетом која су могла довести до тога да се подаци доведу у лош статус. Требало би да се позабавите са овим прилагођавањима пре него што наставите са било каквим исправкама које се односе на податке.
- За идентификоване задатке који су наслеђени, размотрите брисање ових задатака ако вам нису потребни или ако би требало бити повезани са исправних надређеним пројектом.
- За све задатке у којима је трајање дуже од 1250 дана, размотрите додавање више задатака како бисте представљали укупно трајање, ако је доступно.

> [!NOTE]
> Ставке забележене звездицом (\*) имају ограничења због чињенице да управљање односима са клијентима (CRM) подржава само 7320 проширења понављања. Не смете да прекорачите ово ограничење.

## <a name="resource-assignment-relationships"></a>Односи између додела ресурса
Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:

- Све доделе ресурса у структурној анализи посла морају бити повезане са истим пројектом.
- Све доделе ресурса у структурној анализи посла морају бити повезане са члановима пројектног тима у истом пројекту.

### <a name="potential-mitigation-steps"></a>Потенцијални кораци за ублажавање
- Идентификујте све задатке који спадају ван гореописаних услова.  
- Све доделе ресурса које више нису важеће би требало бити обрисане.

## <a name="project-task-dependency-relationships"></a>Односи између зависних елемената пројектног задатка
Да бисте осигурали успешну надоградњу, следећи односи морају се правилно одржавати:

- Сви зависни елементи задатка пројекта морају бити повезани са истим пројектом.
- Задатак не може да има исти зависни елемент на који се упућује више пута.