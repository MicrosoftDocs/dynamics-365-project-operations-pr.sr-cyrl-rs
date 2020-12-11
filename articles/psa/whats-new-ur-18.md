---
title: Шта је ново или промењено у издању 18 исправке за Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 18 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
ms.topic: article
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
ms.openlocfilehash: 3a6d3ee21ecf742b2253132f3d3cc1cb2b57af75
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119886"
---
# <a name="project-service-automation-update-release-18-v3"></a>Project Service Automation издање исправке 18, у верзији 3

Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Ово издање је компатибилно са услугом Dynamics 365 9.x. Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 18. Број израде ове верзије је V3.10.8.12 и углавном је доступна путем самосталног ажурирања у априлу 2020. године.

## <a name="update-release-18"></a>Издање исправке 18

### <a name="bug-fixes"></a>Исправке грешака

**Време и трошак**

- Поправљено: токови **Опозив**, **Захтев** и **Откажи одобрење** избацују изузетке са нејасним порукама о грешкама.
- Поправљено: Када **Откажи одобрење** не успе за трошак, не избацује се релевантна грешка изузетка.
- Поправљено: Мрежа ставке времена погрешно обрађује нерадне дане у Аустралији након пребацивања летњег времена (DST) у октобру.
- Поправљено: Неправилна логика подразумеваних вредности спречава подношење трошкова.
- Поправљено: Када одобрење ставке времена не успе, одобрење остаје у статусу **На чекању**.
- Поправљено: SQL грешке при масовним одобрењима (застој / истек времена).
- Поправљено: Значајни проблеми са перформансама у корисничком искуству изазвани ажурирањем чланова тима приликом одобравања уноса времена.

**Управљање пројектима**

- Поправљено: Обавештење о временској зони премештено је са приказа **Сравњење** на главни образац **Пројекат**.
- Поправљено: Предложак календара нема исправне подразумеване вредности када се отвори нови образац пројекта.
- Поправљено: За Chromium прегледаче, корисници не могу лако да изаберу претходне задатке које ће избрисати.
- Поправљено: Креирање или копирање **пројекта из празног предлошка** преузима неповезане доделе.
- Поправљено: У специфичним рубним случајевима, креирање новог задатка из мреже задатака доводи до стварања дупликата записа.
- Поправљено: У ручном режиму корисници не могу да ажурирају датуме почетка задатка да буду каснији од сачуваног тренутног датума.

**Управљање ресурсима**

- Поправљено: Ред подзбира у приказу **Сравњење** погрешно израчунава одступање резервација након продужења резервације.
- Поправљено: Приказ **Сравњење** погрешно приказује додељене ресурсе када ресурс који је могуће резервисати има календар који се не подудара са календаром пројекта.

**Sales**

- Поправљено: Када се ставке времена поново одобре (**Одобри > Откажи>** Поново одобри), креира се дупликат ненаплативе стварне вредности.