---
title: Опције подизвођања за чланове пројектног тима
description: Ова тема објашњава опције подизвођања за чланове пројектног тима корпорације Мицрософт Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 4db283db728b50ccf76eafabfd643313620bbce2
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903770"
---
# <a name="subcontracting-options-for-project-team-members"></a>Опције подизвођања за чланове пројектног тима

[!include [banner](../../includes/dataverse-preview.md)]

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

У Dynamics 365 Project Operations корпорацији Мицрософт можете да процените опције подизвођања које су доступне за једног или више чланова пројектног тима. Доступне опције подизвођања вам омогућавају да:

- Креирајте нови подизвођачи и/или креирајте нове редове на постојећем подизвођачи за изабране чланове пројектног тима. 
- Резервишите у односу на већ постојећи ред подизвођаиа и подизвораиа. 

Можете одабрати једну од доступних опција подизвођања за чланове генеричког пројектног тима или одабрати неки од чланова пројектног тима који имају именовани ресурс који је радник по уговору. 

Нема доступних опција подизвођања за следеће:

- Чланови пројектног тима који су били запослени. 
- Чланови пројектног тима који су већ повезани са редом подизвођачима и подизвођачима. 

## <a name="subcontracting-an-unstaffed-project-team-member"></a>Подизвођачи неодобраваног члана пројектног тима

Да бисте прегледали и одабрали једну од доступних опција подизвођача за генеричког или неодобраваног члана пројектног тима, следите ове кораке:

1. Изаберите један или више записа чланова пројектног тима у којима је ресурс генерички ресурс.
2. Уверите се да ниједан од изабраних записа чланова пројектног тима није већ подизвођачен. 
3. Изаберите **опције подизвођања** у подмрежној мрежи чланова пројектног тима. Отвориће **се дијалог опција** подизвођања. 
4. Ако сте изабрали само један запис члана пројектног тима у кораку 1, биће доступне следеће опције:
    - Креирајте нове редове подизвођачи. 
    - Резервишите у односу на постојећи подизвођаи Ако сте изабрали виље записа илака пројектног тима у кораку 1, онда је једина доступна опција креирање нових редова подизвораиа.
5. Опција резервисања у односу на постојећи ред подизвођачи вам омогућава да изаберете ред подизвођачи и подизвођачи против којих желите да резервишете. Када бирате ред подизвођаче да бисте резервисали капацитет, требало би да се уверите да је изабрани ред подизвођаче за време и да се улога потребна члану пројектног тима подудара са улогом која је купљена у реду подизвођаче.
6. Када изаберете да креирате нове редове подизвођачи за чланове пројектног тима, систем ће вам дозволити да изаберете подизвођаи који желите да креирате у овим редовима. Подизвођачи у којима сте изабрали да креирате нове редове требало би да се нађу у **статусу радне** верзије. Помоћу ове опције за креирање нових редова подизвођачима за изабране чланове пројектног тима, систем ће креирати један ред подизвођања за време за сваког члана пројектног тима. Улога, часови и датуми биће копирани из члана пројектног тима у сваки ред подизвођача који је креиран. 
7. Када је генерички члан тима повезан са редом подизвођач и подизвођач, поље"Врста радника" у реду генеричког члана тима биће ажурирано у"Радник **по** уговору", а **вредност** **"Валидност подизвођаца" на** вредност **"Важеће".**

## <a name="subcontracting-a-staffed-project-team-member"></a>Подизвођачи особља пројектног тима

Као и генерички или неодговарајући чланови тима, такође можете да прикажете опције подизвођача за члана тима пројекта са особљем све док је члан тима са особљем радник по уговору. Да бисте прегледали и одабрали једну од доступних опција подизвођања за особље или именованог члана пројектног тима, следите ове кораке:

1. Изаберите један или више записа чланова пројектног тима у којима је ресурс именовани радник по уговору.
2. Уверите се да ниједан од изабраних записа чланова пројектног тима није већ подизвођачен. 
3. Изаберите **опције подизвођања** у подмрежној мрежи чланова пројектног тима. Отвориће **се дијалог опција** подизвођања. 
4. Ако сте изабрали само један запис члана пројектног тима у кораку 1, биће доступне следеће опције:
      - Креирајте нове редове подизвођачи.
      - Резервишите у односу на постојећи подизвођаи.
  Ако сте изабрали више записа чланова пројектног тима у кораку 1, једина доступна опција је креирање нових редова подизвођачи.
5. Опција резервисања у односу на постојећи ред подизвођачи вам омогућава да изаберете ред подизвођачи и подизвођачи против којих желите да резервишете. Када бирате ред подизвођаче да бисте резервисали капацитет, требало би да обезбедите следеће:
      - Изабрани ред подизвођачи је за време. 
      - Улога потребна члану пројектног тима подудара се са улогом која је купљена у реду подизвођачи. 
      - Добављач са ког је повезан радник по уговору је исти као добављач у подизвођачи.
6. Када изаберете да креирате нове редове подизвођачи за чланове пројектног тима, систем ће вам дозволити да изаберете подизвођаи који желите да креирате у овим редовима. Овом опцијом треба да се уверите да је добављач коме припада радник по уговору исти као добављач у подизвођачи. 
7. Подизвођачи у којима сте изабрали да креирате нове редове требало би да се нађу у **статусу радне** верзије. Помоћу ове опције за креирање нових редова подизвођачима за изабране чланове пројектног тима, систем ће креирати један ред подизвођања за време за сваког члана пројектног тима. Улога, часови и датуми биће копирани из члана пројектног тима у сваки ред подизвођача који је креиран.  
8. Када је именовани члан тима повезан са редом подизвођач и подизвођач, поље"Врста радника" у именованом реду члана тима биће ажурирано у"Радник **по** уговору", а **вредност** **"Валидност подизвођаче" на** вредност **"Важеће".**

## <a name="re-costing-subcontractor-assignments"></a>Поновни трошкови додељивања подизвођача

Када је члан пројектног тима (генерички или именован) повезан са редовима подизвођачем помоћу дијалога"Опције подизвођања", све доделе задацима које члан тима има **биће** поново скупљене на основу набавног ценовног списка приложеног подизвођачем. На **картици Процене** на **страници Детаљи пројекта изаберите дугме** **Ажурирај цене** да бисте видели ажуриране цене и/или трошкове који су резултат одлуке о подизвођачима.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]