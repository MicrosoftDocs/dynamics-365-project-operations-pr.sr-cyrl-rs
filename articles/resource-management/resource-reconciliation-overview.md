---
title: Преглед сравњења ресурса
description: Ова тема пружа информације о томе да ли су поравнате резервације ресурса и додељивања задацима у пројекту.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
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
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1b60ed9d15f51ff01f27bcc231f5db27513a838f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897469"
---
# <a name="resource-reconciliation-overview"></a>Преглед сравњења ресурса

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_

За чланове тима, резервације и доделе су лабаво повезани. Другим речима, ресурси могу имати доделе, али не и резервације или могу имати резервације, али не и доделе. У идеалном случају, резервације и доделе треба да се ускладе тако да ресурси имају потребан капацитет да изврше додељене задатке. Међутим, резервације се могу заснивати на доступности, а временски распоред задатака може се мењати током пројекта. Стога, лабава повезаност резервација и додела пружа флексибилност.

Картица **Усаглашеност** на обрасцу **Пројекат** омогућава менаџерима пројеката да усагласе резервације чланова тима и њихове доделе за пројектне тимове.

Картица **Усаглашеност** такође приказује резервације и доделе све до нивоа доделе појединачног задатка за сваког члана тима. Сати се приказују у ћелијама који представљају временске периоде, од месеци, па све до дана.

Картица такође приказује укупни нето износ пројекта, заједно са колоном **Укупна вредност**.

Картица за сваки ресурс израчунава разлику између резервација члана тима и укупног броја додељених задатака члана тима. У идеалном случају, та разлика би требало да буде 0 (нула). Другим речима, не би требало да постоји разлика између резервација и додела. Разлике су обојене и засенчене како би се скренула пажња на две појаве:

- **Недостатак резервација** - Недостатак резервација настаје када ресурс има више додела него резервација. Будући да овај капацитет није резервисан, менаџер пројекта може да коригује ту појаву проширивањем резервација ресурса како би покрио дефицит.
- **Прекомерне резервације** – Прекомерна резервација настаје када је ресурс резервисан за пројекат, али није додељен задацима. Та појава може бити прихватљива у случајевима када је ресурс резервисан за пројекат пре доделе задатка. Међутим, у другим случајевима се не планира додељивање ресурса задацима. У тим случајевима, менаџер пројекта треба да размотрити отказивање резервација ресурса, тако да се капацитет може користити за други пројекат.

У неким случајевима, када прегледате време на вишем нивоу од нивоа дана (на пример, на месечном нивоу), можда ћете видети укупну разлику која је нула за неки ресурс (другим речима, резервације = доделе). Међутим, ако прегледате време на нивоу недеље, можда ћете видети да постоје доделе од нула сати и резервације од 40 сати у првој недељи, али доделе од 40 сати и резервације од нула сати у другој недељи. Све у свему, резервације и доделе се усклађују, али се разликују од једне до друге недеље.

Када прегледате време на вишим нивоима, ћелије на картици **Усаглашеност** имају индикатор који ће вас обавестити да постоје разлике на нижим нивоима. Дуплим кликом на ћелију можете да је повећате како бисте видели разлику. Затим можете да кликните десним тастером миша да бисте је умањили. Ако одаберете ресурс, а затим користите контролу **Следећа разлика** на траци са алаткама мреже, можете прећи на следећу разлику између резервација и додела за тај ресурс. Затим можете да користите контролу **Претходна разлика** за повратак. Такође можете искључити индикатор разлике и понашање у навигацији у делу **Подешавања**.


Ако имате доделе задатака за ресурс, али нема резервација, на страници **Пројекти** на картици **Усаглашеност** изаберите недостатак резервација, а затим **Продужи резервацију**. Појављује се дијалог **Продужење резервације** и приказује резервацију која је потребна да се реши проблем са недостатком ресурса. Такође показује постојеће резервације ресурса за све пројекте или друге ентитете који се могу заказивати. Ако изаберете **У реду** да бисте креирали резервацију за ресурс, без обзира на доступност тог ресурса, можете проузроковати прекомерну резервацију.

Менаџер пројекта или менаџер ресурса тада може да користи табелу распореда како би управљао било којом ситуацијом у којој је ресурс прекомерно резервисан у односу на његов капацитет.

