---
title: Креирање структурне анализе посла
description: Ова тема објашњава како да креирате структурну анализу посла (САП) која укључује основне контроле у новом интерфејсу за планирање.
author: ruhercul
manager: tfehr
ms.date: 01/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d7fa645e78d2206e333d9f85fcec0f7a9c213c23
ms.sourcegitcommit: 260ce052fed760bb44c514517806049ca13a5459
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 01/08/2021
ms.locfileid: "4841397"
---
# <a name="create-a-work-breakdown-structure-wbs"></a>Креирање структурне анализе посла (САП)

Распоред пројекта наводи који посао треба да се заврши, који ресурси ће обављати посао и временски оквир у ком посао мора да се заврши. Распоред одражава сав посао повезан са завршавањем пројекта на време. У услузи Dynamics 365 Project Operations креирате распоред пројеката на следећи начин:

  - Рашчлањујете посао у задатке којима је лако управљати.
  - Процењујете време потребно за обављање сваког задатка.
  - Подешавате зависне елементе задатака.
  - Подешавате трајања задатака.
  - Процењујете генеричке ресурсе који ће извршити задатке. 

Распоред пројеката креиран је на картици **Распоред** на страници **Пројекат**.

## <a name="tasks"></a>Задаци

Први корак у креирању пројектног распореда је рашчлањивање посла на управљиве делове. Распоред у услузи Project Operations подржава следеће функције:

- Резиме или задаци спремишта
- Задаци чвора листа

### <a name="summary-tasks"></a>Резимирани задаци

Резимирани задаци могу да ускладиште друге резимиране задатке или задатке чвора листа. Они немају сопствене радне активности ни трошкове. Уместо тога, њихове радне активности и трошкови су збирна вредност радних активности и трошкова њихових задатака у контејнеру. Датум почетка резимираног задатака је датум почетка задатака у контејнеру, а датум завршетка је датум завршетка задатака у контејнеру. Назив резимираног задатка може се уређивати, али својства заказивања, укључујући активности, датуме и трајање, не могу се уређивати. Ако обришете резимирани задатак, бришете и све његове задатке у контејнеру.

### <a name="leaf-node-tasks"></a>Задаци чвора листа

Задаци чвора листа представља најдетаљнији посао на пројекту. Они имају процењене активности, ресурсе, планиране датуме почетка и завршетка и трајање.

## <a name="create-a-task-hierarchy"></a>Креирање хијерархије задатка

### <a name="add-a-task"></a>Додавање задатка

Довршите следеће кораке да бисте додали један или више задатака.

1. Идите на **Пројекти**, изаберите и отворите запис пројекта за који желите да креирате распоред. 
2. Изаберите картицу **Задаци**. 
3. Изаберите **Додајте нови задатак**, унесите име задатка, а затим притисните тастер Enter.
2. Унесите име другог задатка и поново притисните Enter док не добијете комплетну листу задатака.

### <a name="manage-hierarchy-of-a-task"></a>Управљање хијерархијом задатка

Када је задатак разведен, постаје дете задатка који се налази непосредно изнад њега. ID распореда задатка се затим поново израчунава тако да се заснива на ID-у распореда његовог новог надређеног елемента и следи шему нумерисања. Надређени задатак је сада резимирани задатак. Стога постаје збирна вредност подређених задатака. Када се задатак унапреди, то више није подређени задатак надређеног задатка. ID распореда се затим поново израчунава тако да одражава ажурирану дубину и положај задатка у хијерархији. Активности, трошкови и датуми претходног надређеног задатка се поново израчунавају како не би укључили овај задатак.

Довршите следеће кораке да бисте увукли или промовисали задатак.

1. На страници **Пројекат**, на картици **Задаци**, у делу **Резимирани задаци** изаберите три вертикалне тачке по називу задатка, а затим изаберите **Направите подзадатак**. 
2. Изаберите задатак за увлачење или промоцију. Да бисте изабрали више задатака, изаберите задатак, притисните и држите тастер Ctrl, а затим изаберите додатне задатке.
2. Изаберите **Увуци** или **Промовиши подзадатак** за премештање задатака испод или изнад резимираних задатака.

### <a name="move-tasks-up-and-down"></a>Премештање задатака нагоре и надоле

Задаци могу да се преместе на било који ниво у структурној анализи посла на један од два начина:

- Изаберите још један задатак и превуците га на жељено место.
- Изаберите један или више задатака, кликните десним тастером миша и изаберите **Исеци**, изаберите одредишну ћелију у распореду, а затим кликните десним тастером миша и изаберите **Налепи**.

## <a name="task-attributes"></a>Атрибути задатка

Име задатка описује посао који мора да се доврши. У услузи Project Operations, атрибути који су повезани са задатком описују распоред задатка и његове потребе за ангажовањем ресурса.

## <a name="schedule-attributes"></a>Заказивање атрибута

Атрибути **Активности**, **Датум почетка**, **Датум завршетка** и **Трајање** дефинишу распоред за задатак.

Следећа табела приказује додатне атрибуте распореда.

| **Коначно име за приказ** | **Коначан опис** |
| --- | --- |
| Ангажовање на завршетку (часови) | Одрађени посао за задатак у часовима. |
| Трајање | Приказује трајање задатка у данима. |
| Укупно ангажовање | Укупан посао на задатку у часовима. |
| Завршетак | Датум и време завршетка. |
| % довршености | Проценат задатка који је завршен. |
| Контејнер пројекта | Табла задатака може бити груписана према контејнеру тако да сваки контејнер има сопствену колону. |
| Преостало ангажовање (часови) | Преостали посао за задатак у часовима. |
| Покрени | Датум и време почетка. |
| Име | Име задатка. |
| ID | ID задатка у структурној анализи посла. |

## <a name="staffing-attributes"></a>Атрибути запослених

Атрибутима ангажовања се приступа у пољу **Ресурси** у распореду. Можете потражити постојећи ресурс или изаберите **Креирај** и у окну **Брзо креирање** додајте члана пројектног тима као нови ресурс.

Поља **Улога**, **Јединица за обезбеђивање ресурса** и **Назив позиције** се користе за описивање потреба за ангажовањем ресурса на задатку. Ови атрибути ангажовања, заједно са распоредом задатака, користе се за проналажење доступних ресурса за обављање овог задатка.

   - **Улога**: Наведите врсту ресурса који је потребан за извршавање задатка.
   - **Јединица за обезбеђивање ресурса**: Наведите јединицу из које треба доделити ресурсе за задатак. Овај атрибут утиче на процену трошкова и продаје за задатак ако су стопе трошкови и наплате за ресурс подешене на основу јединица за обезбеђивање ресурса.
   - **Назив позиције**: Унесите име за генерички ресурс које служи као чувар места за ресурс који ће на крају обавити посао.

Поље **Ресурси** садржи назив позиције генеричког ресурса или именованог ресурса када га неко пронађе.

Поље **Категорија** садржи вредности које указују на шири тип посла у који се задатак може груписати. Ово поље не утиче на заказивање нити обезбеђивање ресурса. Уместо тога, поље се користи само за извештавање.

## <a name="task-dependencies"></a>Зависности задатка

Распоред у услузи Project Operations можете да користите за креирање односа претходника између задатака. Поље **Претходни задатак** користи једну или више вредности како би означио задатке од којих задатак зависи. Када доделите претходне вредности задатку, задатак можете да покренете једино када довршите све претходне задатке. Због зависних елемената, планирани датум почетка задатка враћа се на датум када су претходни задаци завршени.

Режим задатка нема утицаја на ажурирања која се обављају на датум почетка и завршетка претходних/зависних задатака.

## <a name="accessibility-and-keyboard-shortcuts"></a>Приступачност и тастерске пречице

Мрежа **Распоред** је потпуно доступна и може се користити са читачима екрана као што су Narrator, JAWS или NVDA. Кроз област мреже можете се кретати помоћу тастера са стрелицама (као у програму Microsoft Excel), можете користити тастер Tab да бисте се кретали кроз интерактивне елементе корисничког интерфејса, а помоћу тастера са стрелицом надоле, тастера Enter или размакнице можете да изаберете и отворите падајуће меније.