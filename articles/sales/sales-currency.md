---
title: Валута
description: Ова тема пружа информације о томе како да додате и уклоните типове валута у пројектним операцијама.
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d53bae2f64e7b427f762161ff08917598217bb5a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898369"
---
# <a name="currency"></a>Валута

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_

Валуте одређују цене за производе у каталогу производа и трошкове трансакција, као што су улазне поруџбине. Ако се ваши клијенти налазе у различитим географским областима, додајте њихове валуте да бисте управљали трансакцијама. Додајте валуте које највише одговарају тренутним и будућим пословним потребама.  

> [!NOTE]
> Ако је ваше окружење Common Data Service окружење, налазите се у Power Platform центру администрације и изабрали сте страницу **Валуте** (**Окружења** > [изаберите окружење] > **Подешавања** > **Посао** > **Валуте**), страница ће бити празна. То је зато што подешавање валуте није подржано у Common Data Service окружењима.

## <a name="add-a-currency"></a>Додавање валуте  
Пре него што започнете овај поступак, проверите да ли ваша безбедносна улога укључује дозволе администратора система. 

1. Изаберите окружење у Power Platform центру администрације. 
2. Изаберите **Подешавања** > **Посао**.
3. Изаберите **Валуте**.  
4. Изаберите **Ново**.  
5. Попуните информације по потреби.  


   |          Поље          |                                                                                                                                                                                                                                                                                                                                                                            Опис                                                                                                                                                                                                                                                                                                                                                                            |
   |-------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   |    **Тип валуте**    | - **Системски** – Изаберите ову опцију ако желите да користите валуте доступне у апликацијама заснованим на моделу у систему Dynamics 365. Да бисте потражили валуту, изаберите **Потражи**. Када изаберете шифру валуте, **Назив валуте** и **Симбол валуте** се аутоматски додају изабраној валути.<br />- **Прилагођено** – Изаберите ову опцију ако желите да додате валуту која није доступна у апликацијама заснованим на моделу у систему Dynamics 365. У овом случају морате ручно да унесете вредности за **Шифру валуте**, **Прецизност валуте**, **Назив валуте**, **Симбол валуте** и **Конверзију валуте**. |
   |    **Шифра валуте**    |                                                                                                                                                                                                                                                                                                                                            Кратак облик валуте. На пример **USD** за САД долар.                                                                                                                                                                                                                                                                                                                                            |
   | **Прецизност валуте**  |                                                                                                                                                                                  Унесите број децимала које желите да користите за валуту.  Можете да додате вредност између 0 и 4. **Напомена:** Ако сте подесили вредност прецизности у дијалогу **Подешавања система**, та вредност ће се приказивати овде.                                                                                                                                                                                  |
   |    **Име валуте**    |                                                                                                                                                                                                                                         Ако сте изабрали шифру валуте са листе доступних валута у апликацијама заснованим на моделу у систему Dynamics 365, назив валуте за изабрану шифру је приказан овде. Ако сте изабрали **Прилагођени** за тип валуте, несите назив валуте.                                                                                                                                                                                                                                          |
   |   **Симбол валуте**   |                                                                                                                                                                                                                                                                      Ако сте изабрали шифру валуте са листе доступних валута у систему , симбол за изабрану валуту је приказан овде. Ако сте изабрали **Прилагођени** за тип валуте, унесите симбол за нову валуту.                                                                                                                                                                                                                                                                       |
   | **Конвертовање валуте** |                                                                                                                                                                                                                                     Унесите вредност изабране валуте у односу једног САД долара. Ово је износ на који се изабрана валута конвертује у основну валуту. **Важно:** Уверите се да сте ажурирали ову вредност колико често је потребно да бисте избегли било која непрецизна израчунавања у трансакцијама.                                                                                                                                                                                                                                      |


6. Када завршите, на командној траци изаберите ставку **Сачувај** или **Сачувај и затвори**.  

   > [!TIP]
   >  Да бисте уредили валуту, валуте, изаберите валуту, а затим унесите или изаберите нове вредности.  

## <a name="delete-a-currency"></a>Брисање валуте  

1. Изаберите окружење у Power Platform центру администрације. 
2. Изаберите **Подешавања** > **Посао**.
3. Изаберите **Валуте**.  
4. Са приказане листе валута, изаберите валуту коју треба избрисати.  
5. Изаберите **Избриши**.  
6. Потврдите брисање.  

> [!IMPORTANT]
>  Не можете да избришете валуте које користе други записи. Можете само да их деактивирате. Деактивирањем записа о валути не уклањају се информације о валути ускладиштене у постојеће записе, као што су могућности за пословање или поруџбине. Међутим, нећете моћи да изаберете деактивирану валуту за нове трансакције.  
