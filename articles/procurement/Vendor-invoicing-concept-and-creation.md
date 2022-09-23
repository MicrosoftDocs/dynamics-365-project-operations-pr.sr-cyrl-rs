---
title: Креирање фактура добављача
description: Овај чланак описује концепт фактура добављача и објашњава како да их креирате у корпорацији Мицрософт Dynamics 365 Project Operations.
author: suvaidya
ms.date: 9/12/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: suvaidya
ms.openlocfilehash: 7f6c1ec46f23b6823734b28755b80ced4e3f9325
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475483"
---
# <a name="create-vendor-invoices"></a>Креирање фактура добављача

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Да бисте користили функционалност описану у овом чланку, **морате омогућити да се омогући обрада стварних података подизвођача помоћу операција пројекта за сценарије засноване на ресурсима** у **радном простору за** управљање функцијама.

Фактурисање добављача у корпорацији Мицрософт Dynamics 365 Project Operations може се користити за записивање трошкова испорука услуга и/или материјала на пројекту који су довршили добављачи.

Када се сервиси и/или материјали подубеђују добављачу, подизвођач представља уговорни уговор са тим добављачем. Како добављач испоручује услуге или како се материјали примају и користе на пројектним задацима, трошкови се бележе на пројекту. Добављач затим периодично шаље фактуре. Те фактуре се проверавају и подударају са трошковима који су забележени на пројекту. Након завршетка процеса верификације, фактура добављача се потврђује и ослобађа за плаћање.

## <a name="scenarios-for-use"></a>Сценарији за употребу

Фактуре добављача у операцијама пројекта могу се користити за подршку два различита сценарија:

- Клијенти користе пуна искуства подизвођања.
- Клијенти не користе комплетна искуства подизвођања, али желе да имају јединствен приказ трошкова за пројекте у операцијама пројекта.

### <a name="customers-use-the-full-subcontracting-experiences"></a>Клијенти користе комплетна искуства подизвођања

Искуства са фактуром добављача обезбеђују начин провере временских ставки, коришћења материјала и ставки трошкова које референцују компоненте подизвођачима и упорећују их са редовима фактуре добављача. Овај процес се може користити за проверу тачности редова фактуре добављача. Након довршавања процеса верификације и потврде фактуре добављача, систем сторнира стварне ставке које су записане одобреним евиденцијама времена, трошкова и коришћења материјала, а затим креира нове стварне трошкове коришћењем редова фактуре добављача.

### <a name="customers-dont-use-the-full-subcontracting-experiences-but-want-to-have-a-unified-view-of-costs-on-projects-in-project-operations"></a>Клијенти не користе комплетна искуства подизвођања, али желе да имају јединствен приказ трошкова пројеката у пројектне операције

Ако пратите процес подизвођаче у систему независног произвођача, трошкове из тог система независних произвођача можете записати у операције пројекта креирањем фактура добављача које не упућују на подизвођаче. На тај начин менаџери пројеката могу да имају јединствен, обједињен приказ свих трошкова на датом пројекту.

## <a name="create-vendor-invoices-in-project-operations"></a>Креирање фактура добављача у пројектне операције

Фактуре добављача се креирају у Дyнамицс 365 Финанце, помоћу модула **"Конта за плаћање** ". Фактуре добављача не можете креирати директно у Dataverse.

### <a name="set-up-vendor-invoice-verification"></a>Подешавање провере фактуре добављача

Ако је фактура добављача намењена подизвођачима Dataverse у програму, **потребан је параметар Ручна верификација од стране премијера**. Поставка опције одређује да ли фактура добављача треба аутоматски да буде потврђена или Dataverse захтева ручну потврду. Заглавље сваке фактуре добављача пројекта укључује опцију истог имена. Подразумевано, опција у заглављу свих фактура добављача пројекта постављена је на вредност коју сте овде поставили. Међутим, вредност можете ажурирати по потреби у заглављу појединачних фактура добављача.

Ако је опција постављена на"Да", **фактура** добављача која је креирана у "Финансије" и синхронизована са статусом Dataverse "Радна верзија" има **статус "Радна** верзија". Фактура затим мора бити проверена и верификована од стране менаџера пројекта и потврђена, пре него што се обради и прокњижи на одређена конта пројекта и књиге у финансијама.

Ако је опција подешена на "Не **·** ", фактура добављача се аутоматски потврђује. Није потребна даља акција.

Да бисте подесили проверу фактуре добављача, следите ове кораке.

1. У области Финансије идите на Управљање пројектима **и рачуноводствено подешавање** \> **пројекта** \> **управљања и рачуноводствених параметара.**
1. На картици **"** Финансије" поставите **опцију "Ручно верификација од стране премијера** **·** " ако смернице предузећа захтевају верификацију фактура добављача подизвођача. Ако верификација од стране менаџера пројекта није обавезна, оставите Dataverse поруку скуп опција на "Не **"**. Поставка ће подразумевано бити коришћена на страници фактуре добављача **на чекању**.

> [!NOTE]
> Фактуре добављача које су креиране за подизвођача Dataverse могу се исправно обрадити само ако **је опција "Ручно верификација од стране премијера** " подешена на "Да **"**. Стварне временске, материјалне и трошковне трошкове које креирају подизвођачи могу се ручно подударати са редовима фактуре добављача од стране менаџера пројекта само ако је ова опција подешена на "Да **"**.

### <a name="set-up-a-procurement-integration-account-for-vendor-invoices"></a>Подешавање конта интеграције набавке за фактуре добављача

Када се фактура добављача прокњижи у "Финансије за пројектне операције " – Интегрисано окружење (ненапуштено), финансије се књиже на конто интеграције са набавкама. Систем генерише стварне ствари за прокњижену Dataverse фактуру. Ове стварне ствари се књиже у "Финансије" коришћењем налога за интеграцију пројеката. Књижење налога интеграције пројекта књижи стварни трошак и сторни конто интеграције са набавкама.

Да бисте подесили конто интеграције набавке за фактуре добављача, следите ове кораке.

1. У области Финансије идите на Управљање пројектима **и рачуноводствено подешавање** \> **пројекта** \> **управљања и рачуноводствених параметара.**
1. На картици **Пројектне операције на Дyнамицс 365 картици ангажовање купаца** изаберите конто **интеграције** \> **набавки материјала.**

### <a name="create-and-post-subcontract-vendor-invoices"></a>Креирање и књижење фактура добављача подизвођачи

Када службеник који плаћа рачуне прими фактуру од подизвођача, нова фактура се креира у области "Финансије".

1. У области "Финансије" идите на фактуре **за исплате** \> **на чекању.** \> **·**
1. У окну **за радње** изаберите ставку Ново **да** бисте креирали фактуру добављача.
1. У заглављу фактуре, у пољу Конто **фактуре** изаберите ставку **Подизвођач**.
1. Изаберите датум фактуре.
1. На картици **"** Заглавље" поставите опцију **"Ручно верификација од стране** премијера" на опцију "Да **"**. Подразумевана поставка ове опције потиче са странице "Управљање **пројектима и рачуноводственим параметрима** ". Међутим, она се може променити на нивоу фактуре добављача.
1. На брзој **картици Ред** фактуре изаберите ставку Додај **ред да бисте** креирали ред фактуре добављача.
1. Изаберите категорију набавке која је креирана за редове подизвођачи и унесите јединичну цену, јединицу мере и количину.
1. У одељку Редови фактуре добављача, на **картици** Пројекат изаберите пројекат у који подизвођач дели фактуру подизвођача.
1. Изаберите категорију пројекта. Може бити било које врсте ставке "Артикал **", "** Трошкови **", "** Материјали **"** или "Часови **"**.
1. Изаберите улогу само ако је изабрана категорија пројекта типа "Сат **·** ".
1. Кликните на **дугме Прокњижи** да бисте прокњижили фактуру добављача.

Друга могућност је да креирате фактуру добављача тако што ћете ићи на фактуре **за плаћање** \> **·** \> **Отворити фактуре добављача** и изабрати ставку **Ново.**

Када се фактура добављача прокњижи, она постаје доступна за Dataverse проверу и обраду менаџера пројекта.

## <a name="vendor-invoice-processing-in-dataverse"></a>Обрада фактуре добављача у Dataverse

У фактури добављача која је креирана у Dataverse програму, неке вредности поља потииу из фактуре добављача која је записана у "Финансије". Друге вредности су подразумеване вредности које потииу из подизвораиа.

Следећа поља и сродни записи биће копирани из подизвођача у заглавље фактуре добављача:

- Валута
- Јединица уговарања
- Услови плаћања

У редовима фактуре добављача, операције пројекта користе следеће вредности поља да би унели подразумевану референцу реда подизвођачи и подизвођачи:

- Класа трансакције
- Улога
- Категорија трансакције
- Поља производа
- Project
- Задатак

> [!NOTE]
> Редови подизвођања фиксне цене нису подржани у операцијама пројекта.

[!INCLUDE[footer-include](../includes/footer-banner.md)]