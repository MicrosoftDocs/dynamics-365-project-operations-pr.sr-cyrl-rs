---
title: Редови фактуре добављача за прекретнице
description: Овај тема објашњава како се креирају редови фактуре добављача за прекретнице у подизвођачи.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 4fa11e2a4f459016b3ce141b03fe97e55c9a2759
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/14/2022
ms.locfileid: "8590640"
---
# <a name="vendor-invoice-lines-for-milestones"></a>Редови фактуре добављача за прекретнице

[!include [banner](../../includes/dataverse-preview.md)]

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Фактура добављача у корпорацији Мицрософт Dynamics 365 Project Operations може имати редове фактуре добављача за прекретнице које су дефинисане у реду подизвођачи. Менаџери пројекта могу да користе редове фактуре добављача за прекретнице да би записали трошкове услуга који се набављају као трошкове засноване на прекретници који настављају на услугама или производима који се набављају за пројекат.

Редови фактуре добављача за прекретнице увек морају да упућују на ред подизвођаче који има метод фактурисања фиксне цене. Када ред фактуре добављача за прекретнице упућује на ред подизвођаче, менаџери пројекта ће моћи да се подударају и верификују основне трошкове времена, трошкова или материјала који референцују на ред подизвођаче у односу на прекретницу коју фактурише добављач.

Следећа табела пружа информације о пољима у редовима фактуре добављача за прекретнице.

| Поље | Опис | Функционални утицај |
| --- | --- | --- |
| Именуј | Име реда фактуре добављача, да бисте помогли у идентификацији. | Ово име ће бити приказано као прва колона у свим проналажењем која се заснива на редовима фактуре добављача. |
| Опис | Кратак опис услуга које добављач фактурише у реду фактуре добављача. | Ниједно |
| Подуговор | Подизвођачи на који су услуге првобитно наручене. | Када је за фактуру добављача изабран подизвођаи, сви редови у фактури добављача же наследити тај избор. Фактура добављача не може имати редове фактуре добављача који упућују на различите подизвођачи. |
| Ред подизвођачи | Ред подизвођаче на којем су услуге наручене. Листа редова подизвођака који се могу изабрати ограничена је на редове изабраног подизвођака. | Када је ред подизвођача изабран у реду фактуре добављача за прекретнице, **поља категорија "Улога** **" и "Трансакција** " и поља повезана са производом су небитна и нису доступна. Поља **"Количина", "** Јединица **"** и "Група **јединица" такође** нису релевантна за редове фактуре добављача засноване на прекретници. |
| Датум трансакције | Датум када ће трошак стварног реда фактуре добављача бити записан у пројекат. | Ниједно |
| Класа трансакције | Изаберите **ставку** Прекретница да бисте записали фактуру добављача за довршену прекретницу која је дефинисана у реду подизвођач. | Ниједно |
| Контролна тачка | Изаберите прекретницу која је дефинисана у повезаном реду подизвођачи који је означен као "Спремно **за фактурисање"**. | Прекретнице у реду подизвођања које имају статус "Спремно **за фактурисање** " могу бити изабране у реду фактуре добављача. |
| Project | Коришћено је име пројекта на којем су коришћене услуге које се фактурише. | Ово поље је обавезно и не може остати празно. |
| Задатак | Коришћено је име пројектног задатка на којем су коришћене услуге које се фактурише. Ово поље је доступно само ако је изабран пројекат. Избор пројектног задатка је опционалан. | Ако ово поље остане празно, менаџер пројекта може да упореди ред фактуре добављача са класом трансакција у повезаном реду подизвођач који је записан на било ком задатку пројекта. Ако ред фактуре добављача не упућује на ред подизвођача, а ово поље остане празно, стварни трошак који је креирао ред фактуре добављача неће бити повезан ни са једном необличаваном стварном продајом. У овом случају, ако је наплата заснована на задатку подешена, трошкови можда неће моћи да се фактуришу крајњем купцу. |
| Износ контролне тачке | Унесите вредност прекретнице која је дефинисана у реду подизвођачи који је спреман за фактурисање. | Ниједно |
| Порез на промет | Унесите износ пореза на промет. | Ниједно |
| Укупан износ | Укупан износ реда фактуре добављача, укључујући порезе. Ово поље се израчунава као порез на *промет у износу* + *прекретнице*. | Ниједно |

> [!NOTE]
> Када се креира ред фактуре добављача који упућује на прекретницу реда подизвођања, статус прекретнице подизвођања се ажурира у креирану **фактуру добављача**. Затим, када је та фактура добављача потврђена, статус прекретнице реда подизвођачи се ажурира у фактуру **добављача потврђен.**

[!INCLUDE[footer-include](../../includes/footer-banner.md)]