---
title: Копирање понуда заснованих на пројекту
description: Ова тема пружа информације о начину копирања понуда заснованих на пројекту у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d7234958d542dec4cba55cb0516f1222937389e1
ms.sourcegitcommit: f255b2cbf290973ce62fe2c1c121bd1df15a7392
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3928605"
---
# <a name="copy-project-based-quotes"></a>Копирање понуда заснованих на пројекту

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_

Можете лако креирати нову понуду за пројекат копирањем постојеће. 

- Да бисте копирали понуду за пројекат, на страници листе **Понуде за пројекат** или страници детаља **понуде за пројекат**, изаберите понуду за пројекат коју желите да копирате, а затим изаберите **Копирај**.

То ће отворити страницу дијалога на којој можете унети параметре копије. Следећа табела наводи поља која су укључена у страницу дијалога. У зависности од изабраних вредности, поступак копирања се може променити.

| **Поље** | **Релевантност, сврха и смернице** | **Последични утицај** |
| --- | --- | --- |
| Тема | Унесите одговарајућу тему или назив циљне понуде. Када се дијалог отвори, систем ће га подесити на тему изворне понуде са додатим суфиксом **-копија**. | |
| Потенцијални клијент | Упућивање на запис о компанији клијента или пословном контакту. Када се дијалог отвори, систем ће га поставити на пословни контакт у изворној понуди. | Ово поље је примарни клијент у понуди. |
| Јединица уговарања | Организациона јединица која је одговорна за испоруку пројеката повезаних са овом погодбом.
Када се дијалог отвори, систем ће га поставити на јединицу уговарања у изворној понуди. | Јединица уговарања је одељење предузећа које ће извршити пројекте након закључења погодбе. Свака јединица уговарања има валуту. Валута се користи за извештавање о процењеним и стварним трошковима насталим током извршења пројекта. |
| Валута | Ово је валута у којој се обављају трансакције у погодби. Када се дијалог отвори, систем ће га поставити на валуту изворне понуде. Ово се може изменити, а ако је то промена, поље **Копирај одређивање цена** је увек постављено на **Не**. То је зато што ценовници на изворној понуди више нису релевантни. | Валута се користи за подразумевани ценовник, за израду финансијске процене на понуди и на крају за фактурисање клијенту када се погодба оствари. |
| Захтевани датум испоруке | Ово је датум испоруке који захтева клијент. | Ово се користи као датум завршетка приликом креирања датума фактурисања дуж одређене фреквенције. |
| Копирање одређивања цене | Вредност Да/Не указује на то да ли би се одређивање цене на понуди морало копирати из изворне понуде. | Ако је изабрано **Да**, референце на ценовник пројекта и ценовник производа се копирају из изворне понуде у циљну понуду. Ако је изабрано **Не**, ценовници се подразумевано постављају на основу најновијих ценовника који су постављени у параметрима пословног контакта или пројекта. |

Када на страници дијалога изаберете **У реду**, систем креира копију понуде за пројекат на основу параметара изабраних у дијалогу. Отвара се нова понуда за пројекат. 

> [!NOTE]
> Следеће информације се не копирају из изворне у циљну понуду:
>
> - Распореди за фактурисање
> - Понуда и клијенти ставке понуде
> - Референца пројекта на ставкама понуде засноване на пројекту – Информације о буџету клијента
>
>Будући да су ове информације врло специфичне за сваку понуду, та поља и записи се не копирају. Копирају се ставке понуде за пројекте и производе, процене детаља ставки понуде и вредности које не смеју да премаше вредност на нивоу понуде. Подразумеване вредности цена и стопа трошкова зависе од опције **Копирање одређивања цена** изабране на страници дијалога **Копирање параметара**.
