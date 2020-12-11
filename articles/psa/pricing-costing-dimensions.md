---
title: Матична страница за димензије одређивања цена и обрачуна трошкова
description: Ова тема обезбеђује преглед димензија за одређивање цена.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 515a2e2e518614884b414ca43702e8bfea2c6919
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084013"
---
# <a name="pricing-and-costing-dimensions-home-page"></a>Матична страница за димензије одређивања цена и обрачуна трошкова

На димензије које се користе за одређивање цена и трошкова рада у пројектним организацијама утичу следећи атрибути:

- Људи који раде посао сличан свом искуству, улози или географској локацији
- Посао који треба обавити, сличан по сложености или добу дана

С обзиром на типичну природу ових атрибута посла и људи који су потребни за обављање посла, постоје две врсте вредности димензија цене које су доступне у услузи Project Service Automation: 

- **Скупови опција** – Атрибути који представљају фиксна набрајања за скуп вредности.
- **Вредности засноване на ентитетима** – Атрибути који могу имати различит скуп вредности које су коначне, али се временом могу мењати.

## <a name="pricing-dimensions"></a>Димензије за одређивање цена

PSA обавља испоруку помоћу подразумеваног скуп димензија за одређивање цена. Можете да их видите тако што ћете отићи на **Project Service** > **Параметри**. У запису параметра, на картици **Димензије за одређивање цена засноване на износима** проверите да ли улога **msdyn_resourcecategory** и организациона јединица ресурса **msdyn_organizationalunit** имају поља **Применљиво на продају** и **Применљиво на трошкове** подешена на **Да**. Ово ће вам омогућити подешавање цене и трошка за сваку комбинацију улоге и организационе јединице.

![Снимак екрана Project Service параметара са маркираном ставком „Применљиво на продају“](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> Ако сте користили унапред дефинисана поља улоге и организационих јединица као димензије за одређивање цена пре верзије 3 апликације PSA, неће бити никаквих приметних промена. Можете да наставите да користите Project Service као и обично. 

Ако је потребно да одредите цену или трошкове ресурса помоћу додатних атрибута, можете да креирате прилагођена поља, ентитете и димензије. Да бисте добили више информација, погледајте следеће теме, али имајте на уму да морате да довршите процедуре по доленаведеном редоследу:

- [Креирање прилагођених поља и ентитета](create-custom-fields-entities.md)
- [Додавање прилагођених поља у подешавање цена и ентитете трансакције](field-references.md)
- [Подешавање прилагођених поља као димензија за одређивање цена ](set-up-pricing-dimensions.md)
- [Ажурирање атрибута додатних компоненти тако да укључују нове димензије за одређивање цена](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a>Одређивање цене времена људског ресурса
Како организација одређује цену времена људског ресурса је често значајно стратешко питање које директно утиче на профитабилност организације. Сарађујте са финансијским тимовима и будите мудри када ваша организација буде спремна да утврди како жели да подеси стопе наплате и трошкова за време људског ресурса.

Друга питања која се тичу формирања цена подразумевају да ли поново да користите поља или ентитете који тренутно нису димензије за одређивање цена, али се примењују као димензија за одређивање цена у вашој организацији. Поља као што су **Категорија трансакције** ( **msdyn_transactioncategory** ) и **Ресурс који може да се резервише** ( **bookableresource** ) су примери могућих димензија. 

Размотрите и да ли ваша димензија за одређивање цена треба да буде табела или скуп опција. Ако предвиђате промене вредности димензије које ће премашити 10 или 12, а потребни су вам додатни атрибути за ове вредности, боље је да креирате ентитет него скуп опција. Одржавање скуп опција, као што је додавање или уклањање вредности, захтева администратора или програмера, док већина пословних корисника може да додаје нове редове у табелу.

Следећи пример приказује курсне стопе које су подешене на основу улоге и организационе јединице ресурса коме припада ресурс. Стопе трошкова се обично заснивају на групи личних доходака запослених и организационој јединици којој припадају. У овом примеру, табеле са стопама наплате и стопама трошкова ће изгледати овако:

**Примери стопа наплате**

| Улога        | Организациона јединица    |Јединица      |Цена      |Валута  |
| ------------|-------------|----------|----------:|----------|
| Програмер   | Contoso US  |Hour | 200|USD     |
| Програмер   | Contoso India |Hour|   112.|USD     |


**Примери стопа трошкова**

| Група личних доходака     | Организациона јединица    |Јединица      |Цена      |Валута  |
| ----------------|-------------|----------|----------:|----------|
| Моје предузеће_Прва група личних доходака | Contoso US  |Hour | 145.|USD     |
| Моје предузеће_друга група личних доходака | Contoso India |Hour|   67.|USD     |