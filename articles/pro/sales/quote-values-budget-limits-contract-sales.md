---
title: Резиме информација о понуди пројекта (Продаја)
description: Ова тема пружа информације о информацијама и подешавањима који се односе на понуде за пројекте и утичу на њих. (Sales)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d050258ae457bb4392d5fa761442cfc7a444feb0
ms.sourcegitcommit: f6509f7d50de4d4ebb92c1bf2cfcdf09f17458eb
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/06/2020
ms.locfileid: "3966857"
---
# <a name="summary-information-on-a-project-quote-sales"></a>Резиме информација о понуди пројекта (Продаја)

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Овај чланак објашњава информације које се односе на понуду за пројекат. То укључује подешавања која утичу на све ставке понуде и информације о понуди које су сажете у свим ставкама за покретање KPI-ова понуде за пројекат.

Следећа табела наводи поља информација резимеа о понуди за пројект која су јединствена за Dynamics 365 Project Operations или имају неке важне промене у понашању из Dynamics 365 Sales понуда.

| **Поље** | **Локација** | **Релевантност, сврха и смернице** | **Последични утицај** |
| --- | --- | --- | --- |
| Тип | Картица са резимеом (скривена) | Ово поље скупа опција има следеће опције:</br>- Засновано на послу (доступно само када је инсталирана услуга Project Operations)</br>- Засновано на ставци (доступно само када су инсталиране услуге Project Operations и Sales)</br>- Засновано на сервисном одржавању (доступно када је инсталирана услуга Dynamics 365 Field Service) | Када користите апликацију Project Operations, вредност овог поља се аутоматски поставља на опцију **Засновано на послу**. То класификује понуду као понуду засновану на пројекту. Понуда треба да се заснива на пројекту како би се омогућила сва проширења и функције специфичне за пројекат. |
| Потенцијални клијент | Картица резимеа | Упућивање на запис о компанији клијента или пословном контакту. Када се креира понуда из могућности за пословање, ово поље се копира из одговарајућег поља у могућности за пословање. | Валута у понуди за пројекат се подразумевано заснива на валути клијента. Међутим, то може да се промени пре него што се понуда сачува. |
| Менаџер за пословне контакте | Картица резимеа | Име менаџера пословног контакта за ову погодбу. Када се креира понуда из могућности за пословање, ово поље се копира из одговарајућег поља у могућности за пословање. | Менаџер пословног контакта је одговоран за управљање односом са клијентом кроз завршетак овог пројекта. На основу записа ресурса који може да се резервише повезаног са менаџером пословног контакта, уговорна јединица се подразумева из понуде за пројекат. |
| Јединица уговарања | Картица резимеа | Организациона јединица која је одговорна за испоруку пројекта или пројеката повезаних са овом понудом. Када се креира понуда из могућности за пословање, ово поље се копира из одговарајућег поља у могућности за пословање. | Јединица уговарања је одељење предузећа које ће извршавати пројекте након закључења погодбе. Свака јединица уговарања има валуту и она се користи за извештавање о процењеним и стварним трошковима насталим током извршавања пројекта. |
| Ценовник производа | Картица резимеа | Ово је ценовник који се користи за одређивање подразумеваних цена у ставкама понуда заснованим на производима. Листа опција за ово поље приказује листу ценовника где се валута ценовника подудара са валутом у понуди. Када се креира понуда из могућности за пословање, ово поље се копира из одговарајућег поља у могућности за пословање. Ово поље у могућности за пословање се подразумева из записа пословног контакта, али се може променити. | Када се понуда оствари, вредност поље се копира у уговор о пројекту који се креира. |
| Валута | Картица резимеа | То указује на валуту која ће се користити за извештавање о вредности ове погодбе. То је такође валута у којој ће се клијенту фактурисати ако се оствари погодба. Када се креира понуда из могућности за пословање, ово поље се копира из одговарајућег поља у могућности за пословање. Ово поље у могућности за пословање се подразумева из записа пословног контакта, али корисник је може променити. | Када се понуда сачува, ово поље више није могуће уређивати. Ово се користи да се одреде подразумевани ценовници производа и пројекта у понуди. Валута у понуди се користи за подударање валуте са ценовником. |
| Ограничење које не сме да се прекорачи | Картица резимеа | Ово указује на договорено горње ограничење коначне вредности са којим се клијент слаже за овај посао. | Ово горње ограничење се процењује током извршења и применљиво је на све ставке и пројекте повезане са овом погодбом. |
| Захтевани датум испоруке | Картица резимеа | Када се креира понуда из могућности за пословање, ово поље се копира из одговарајућег поља у могућности за пословање. | Овај датум се користи као датум завршетка за генерисање распореда за фактурисање. |

У наставку су картице и KPI-ови доступни на понуди за пројект који су јединствени за Project Operations или имају неке важне промене у понашању из понуда за продају:

| **Поље** | **Локација** | **Релевантност, сврха и смернице** |
| --- | --- | --- |
| Анализа исплативости | Картица у понуди | Картица приказује следеће метрике:</br>- Укупни наплативи трошкови</br></br>- Укупни ненаплативи трошкови</br>- Укупан приход</br>- Укупни приход (основни)</br>- Бруто маржа</br>- Прилагођена бруто маржа|
| Поређење са очекивањима клијента | Картица у понуди | Ова картица приказује следеће метрике:</br>- Процењени завршетак</br>- Захтевани завршетак</br>- Буџет клијента</br>- Вредност понуде |
| Анализа понуде | Картица у понуди | Ова картица резимира следеће најважније KPI-ове за понуду за пројекат</br>- Поређење са очекивањима клијената за буџет и распоред</br>- Бруто маржа</br>- Прилагођена бруто маржа |