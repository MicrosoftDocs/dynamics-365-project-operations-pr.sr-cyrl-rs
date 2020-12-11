---
title: Подешавање ценовника
description: Ова тема пружа информације о томе како да подесите цене и ценовнике.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 000c22944b187b6250f2e982d73020028093fde6
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180210"
---
# <a name="set-up-price-lists"></a>Подешавање ценовника

_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_

Ценовници у услузи Dynamics 365 Project Operations представљају каталог стопа. Стопе изражавају стопе цена, продаје и обрачуна. У зависности од тога да ли ценовник изражава стопе цена или продаје и обрачуна, контекст ценовника је **Продаја** или **Цена**.

Следећа проширења су специфична за Project Operations и примењују се на ценовнике из услуге Dynamics 365 Sales.

- **Контекст**: Ово поље има подржане вредности **Цена** и **Продаја**. Није подржана вредност **Куповина**. Поставите контекст на **Цена** да бисте направили ценовник трошкова или поставите контекст на **Продаја** за продајни ценовник. Ценовник трошкова одређује цену за врсту трошкова на проценама и стварним записима. Продајни ценовници одређују цену на проценама и стварним записима ненаплаћених и наплаћених типова продаје.
- **Јединица времена**: Ово је подразумевана јединица времена за коју се цена поставља у одговарајућој табели **Улога цена** за овај ценовник.
- **Ентитет ценовника**: Ово скривено поље служи да Project Operations разликује ценовнике који су специфични за понуду или уговор од оних који су стандардни и глобално применљиви.

## <a name="price-list-header"></a>Заглавље ценовника

Следећа табела укључује поља са картице **Општи подаци** ценовника која су јединствена за Project Operations или имају значајне промене у понашању у односу на ценовник у Продаји.

| Поље | Локација | Опис | Последични утицај |
| --- | --- | --- | --- |
| Именуј | Картица **Општи подаци** и обрасци **Брзо креирање** | Идентитет ценовника. | Ценовник је приказан са овом вредношћу на свим страницама листе и падајућим опцијама.|
| Контекст | Картица **Општи подаци** и обрасци **Брзо креирање** | Ово поље се може поставити на **Цена** или **Продаја**. | Ценовник подешен на **Трошак** користи се за тражење цене за процене трошкова и стварне трошкове. Ценовник подешен на **Продаја** користи се за тражење цене за процене продаје и стварне износе продаје. Само ценовници којима је контекст постављен на **Продаја** могу се приложити пројектним ценовницима за клијенте, пројектним понудама и пројектним уговорима. |
| Датум почетка | Картица **Општи подаци** и обрасци **Брзо креирање** | Датум почетка периода у коме је ценовник на снази. | Уз поље **Датум завршетка**, ово поље се користи да би се утврдило који ценовник је применљив за одређену процену или стварну линију. |
| Датум завршетка | Картица **Општи подаци** и обрасци **Брзо креирање** | Датум завршетка периода у коме је ценовник на снази. | Уз поље **Датум почетка**, ово поље се користи да би се утврдило који ценовник је применљив за одређену процену или стварну линију. |
| Валута | Картица **Општи подаци** и обрасци **Брзо креирање** | Ово поље се користи за задавање подразумеване валуте у свакој улози, категорији или ставци ценовника у вези са овим ценовником. | На ценовницима, улогама, категоријама или ставкама ценовника опције **Продаја** не могу се креирати линије ни у једној валути осим у овој. На ценовницима опције **Цена** можете креирати линију цена улога у било којој валути. Овде дефинисана валута се користи као подразумевана. Корисничко подешавање које је повезано са ценама улога може заменити ову вредност како би се омогућило подешавање стопе цене рада у било којој валути. Стопе цене категорија и цене ставки ценовника могу се поставити само у валути која је овде дефинисана. |
| Јединица времена | Картица **Општи подаци** и обрасци **Брзо креирање** | Ово поље се користи за задавање подразумеване временске јединице на свакој линији улоге у вези са овим ценовником. | Ова вредност поља се користи само за подешавање повезане цене улоге. На ценовницима опције **Цена** и **Продаја** можете креирати линију цена улога у било којој јединици времена. Овде дефинисана јединица времена се користи као подразумевана. Кориснички подешене повезане цене улога могу заменити ову вредност како би се омогућило подешавање стопе цене рада и обрачуна у било јединици времена. |
| Опис | Картица **Општи подаци** и обрасци **Брзо креирање** | Ово текстуално поље вам омогућава да наведете вишелинијски опис ценовника. | Ово поље је приказано у **Везаним** приказима на ценовнику у различитим ентитетима који имају повезане ценовнике. |