---
title: Мапирање пројеката и задатака на предмет уговора заснован на пројекту – једноставно
description: Ова тема пружа информације о додавању и уклањању пројеката и задатака у предмет уговора.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 30a74f683a032d5bd6caed347f4d0a948376d267
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177664"
---
# <a name="map-projects-and-tasks-to-a-project-based-contract-line---lite"></a>Мапирање пројеката и задатака на предмет уговора заснован на пројекту – једноставно

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

У предметима уговора заснованим на пројекту, можете мапирати одређене задатке у пројекту на предмет уговора.

Када мапирате одређене задатке на предмет уговора, начин наплате, опције наплативости, ограничења која се не прелазе и клијенти дефинисани на предмету уговора биће применљиви само на те одређене задатке.

Ако имате сценарио у којем је једна фаза пројекта, на пример фаза прототипа, фиксна цена, а све остале фазе су време и материјал, моћи ћете да придружите фазу прототипа и све повезане подређене задатке предмету уговора за ту фазу методом обрачуна са фиксном ценом.

Све остале фазе у структурној анализи посла на пројекту (САП) могу се повезати са предметом уговора заснованом на времену и материјалу.

## <a name="associate-tasks-to-project-based-contract-lines"></a>Повезивање задатака са предметима уговора заснованим на пројекту

Задаци се могу повезати са предметима уговора са картице **Наплативи задаци** на страници **Предмет уговора** или са картице **Обрачун задатака** на страници **Пројекат**.

### <a name="from-the-contract-line-page"></a>Са странице Предмет уговора

Довршите следеће кораке за придруживање пројектних задатака предмету уговора са картице **Наплативи задаци** на страници **Предмет уговора**.

1. На картици **Општи подаци** предмета уговора заснованог на пројекту, проверите да ли је поље **Пројекат** попуњено.
2. У пољу **Укључени задаци** изаберите поље **Само изабрани задаци**.
3. Сачувајте промене. Образац ће се освежити и картица **Наплативи задаци** ће бити видљива.
4. Изаберите картицу **Наплативи задаци** и у подформи изаберите **Додај задатак из предмета уговора**.
5. На страници **Задаци из предмета уговора**, у падајућој листи **Задаци**, изаберите задатак. 
6. Унесите информације у поље **Врста обрачуна**, а затим изаберите **Сачувај и затвори**. Изабрани задатак је повезан са предметом уговора.

> [!NOTE]
> Ово није најоптималније искуство за придруживање пројектних задатака предметима уговора. Сваки пројекат ће морати ручно да се повеже у овом искуству. Пожељни начин је са картице **Обрачун задатака** на страници **Пројекат**.

### <a name="from-the-project-page"></a>Са странице пројекта

Ово је оптимална метода за повезивање задатака са предметима уговора. Можете изабрати више задатака и повезати све њих и њихове подређене задатке са изабраним предметом уговора. Довршите следеће кораке да бисте задатке повезали са предметом уговора са странице **Пројекат**.

1. На картици **Општи подаци** предмета уговора заснованог на пројекту, проверите да ли је поље **Пројекат** попуњено.
2. У пољу **Укључени задаци** изаберите **Само изабрани задаци**.
3. Сачувајте предмет уговора заснован на пројекту. Образац ће се освежити и картица **Наплативи задаци** ће бити видљива. Ово је само у сврху верификације.
4. На картици **Општи подаци** предмета уговора заснованог на пројекту, у пољу **Пројекат** изаберите везу ка пројекту.
5. На страници **Пројекат** изаберите картицу **Подешавање наплате за задатак**.
6. Постоје две мреже. Једна мрежа се односи на предмете уговора који се примењују на цео пројекат. Друга мрежа се односи на подешавање обрачуна за одређени задатак. У другој мрежи изаберите један или више задатака, а затим изаберите **Придружени предмети уговора**.
7. На страници дијалога која се отвори, изаберите предмет уговора из падајућег менија.
8. Користите падајући мени **Тип наплате** да бисте задатке означили као наплативе или ненаплативе.
9. Означите поље за потврду да бисте назначили да ли би повезивање требало да укључује и подређене задатке изабраних задатака. Означавање поља ће такође повезати подређене задатке изабраних задатака са предметом уговора.
10. Изаберите **У реду** да бисте затворили дијалог.

## <a name="unassociate-tasks-from-project-based-contract-lines"></a>Неповезани задаци из предмета уговора заснованих на пројекту

### <a name="from-the-contract-line-page"></a>Са странице Предмет уговора

Довршите следеће кораке за раскинете везу пројектних задатака са предметом уговора на картици **Наплативи задаци** на страници **Предмет уговора**.

1. На картици **Наплативи задаци**, изаберите **Избриши задатак предмета уговора**.
2. Порука упозорења указује да уклањање овог повезивања може довести до поништавања стварних података претходно забележених у задатку. Изаберите **У реду** у дијалогу да бисте уклонили везу између задатка и предмета уговора заснованог на пројекту. 

> [!NOTE]
> Ово не брише задатак из пројекта. Уместо тога, уклања повезивање задатака из предмета уговора заснованог на пројекту.

### <a name="from-the-project-page"></a>Са странице пројекта

Ово је оптималније искуство за раскидање везе задатака са предметима уговора. Можете изабрати више задатака и раскинути везу за све њих и њихове подређене задатке са изабраним предметом уговора. Довршите следеће кораке да бисте раскинули везу задатака са предметом уговора.

1. На картици **Општи подаци** предмета уговора заснованог на пројекту, у пољу **Пројекат** кликните на везу ка пројекту.
2. На страници **Пројекат** изаберите картицу **Подешавање наплате за задатак**.
3. На страници постоје две мреже. Једна мрежа се односи на предмете уговора који се примењују на цео пројекат, а друга се односи на подешавање обрачуна специфичних за задатак. У другој мрежи изаберите један или више задатака, а затим изаберите **Прекини везу са предметима уговора**.
4. На страници дијалога која се отвори, изаберите предмет уговора из падајућег менија.
5. Означите поље за потврду да бисте назначили да ли би повезивање уклонило и подређене задатке изабраних задатака. Означавање поља ће такође раскинути везу подређених задатака изабраних задатака са предметом уговора.
6. Изаберите **У реду**. Порука упозорења указује да уклањање овог повезивања може довести до поништавања стварних података претходно забележених у задатку. Изаберите **У реду** у дијалогу упозорења да бисте уклонили везу између задатка и предмета уговора заснованог на пројекту.