---
title: Подесите стопе наплате за рад
description: Ова тема пружа информације о томе како поставити стопе наплате за рад у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 501458510efca6434a51577aacd1f09d1a4faa25
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180729"
---
# <a name="set-up-labor-bill-rates"></a>Подесите стопе наплате за рад

**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха

Сваки ценовник има скуп цена улога или стопа рада које ступају на снагу за контекст и ефективност датума наведених у заглављу ценовника. Стопе наплате за време у услузи Dynamics 365 Project Operations могу се поставити у само једној валути, која је валута у заглављу ценовника.

1. Да бисте поставили стопе наплате за рад за продајни ценовник, направите ценовник на основу заглавља ценовника. 
2. На картици **Улога цена**, у подформи одаберите **+ Нова цена улоге**. 
3. У окну **Брзо креирање** унесите комбинацију улоге и организационе јединице за коју треба да подесите стопу наплате.

   Следећа табела укључује поља на картици **Општи подаци** и окну **Брзо креирање** линије цена за улогу коју треба имати на уму док креирате цене улога на продајном ценовнику:

    | Поље | Локација | Опис | Последични утицај |
    | --- | --- | --- | --- |
    | Улога | Картица **Општи подаци** и окно **Брзо креирање** | Изаберите улогу за коју постављате стопу наплате. | Улога на долазној процени или тренутном стању ће се подударати са овом линијом како би се задала стопа наплате улоге. |
    | Предузеће које одређује ресурсе | Картица **Општи подаци** и окно **Брзо креирање** | Изаберите компанију или правно лице од којег потиче улога. На пример, програмер из компаније Fabrikam Индија или програмер из компаније Fabrikam САД. | Предузеће које одређује ресурсе на долазној процени или тренутном стању ће се подударати са овом линијом како би се задала стопа наплате улоге. |
    | Јединица за одређивање ресурса | Картица **Општи подаци** и окно **Брзо креирање** | Изаберите организациону јединицу или одељење компаније одакле потиче улога. На пример, програмер из одељења за роботику компаније Fabrikam Индија или програмер из одељења софтвера компаније Fabrikam САД. | Јединица која одређује ресурсе на долазној процени или тренутном стању ће се подударати са овом линијом како би се задала стопа наплате улоге. |
    | Цена | Картица **Општи подаци** и окно **Брзо креирање** | Поставите стопу наплате за улогу, предузеће које одређује ресурсе и комбинацију јединица за обезбеђивање ресурса. На пример, програмер из компаније Fabrikam India има стопу наплате 100 USD или програмер компаније Fabrikam USA има стопу наплате 150 USD. | Ова цена је подразумевана стопа наплате за цену по јединици долазне процене или стварне линије за класу трансакције време. |
    | Валута | Картица **Општи подаци** и окно **Брзо креирање**| Вредност валуте подразумевано потиче из валуте из заглавља ценовника продаје. На продајном ценовнику, валута се не може заменити. | Ова валута је подразумевана валуте за цену по јединици долазне стварне продаје за класу трансакције Време. |
    | Распоред јединица | Картица **Општи подаци** и окно **Брзо креирање** | Распоред јединица подразумевано има вредност Време и не може се променити у ентитету цене улога јер се користи експресна стопа по јединицама времена. | Нема последичног утицаја за ово поље. |
    | Јединица | Картица **Општи подаци** и окно **Брзо креирање** | Јединична вредност подразумевано потиче из поља **Јединица времена** у заглављу ценовника продаје. Али, вредност се може заменити. На пример, програмер из компаније Fabrikam India има стопу наплате 1000 USD по **дану у Индији**. Програмер из компаније Fabrikam USA има стопу наплате од 1500 USD по **дану у САД**. | Када се јединична цена подразумева из долазне процене или стварне линије, систем користи систем јединица и конверзију у основне јединице за израчунавање јединичне цене. На пример, процена је за посао од 10 **дана у Индији** за програмера из Индије, а јединица, дан у Индији се дефинише као 10 сати. Када одређује цену те линије процене, апликација израчунава јединичну цену на процени као 1000 USD/10 сати = 100 USD на сат. |

## <a name="transfer-pricing-or-set-up-bill-rates-for-resources-from-other-organizational-units-or-divisions"></a>Пренесите цене или поставите стопе наплате за ресурсе из других организационих јединица или одељења 

Пројектне компаније често користе запослене из различитих правних лица и различитих одељења унутар правног лица за рад на пројектима. Пројекте може извршити једно правно лице или одељење, али запослени или консултанти који раде на пројектима могу потицати из истог правног лица и одељења или из неког другог. Пројекат би такође могао да се састоји од комбинације људи из различитих правних лица и одељења. У програму Project Operations правно лице које је власник пројекта је **Предузеће-власник**, а одељење које је власник испоруке је **Јединица уговарања**. Сва остала правна лица која пружају ресурсе су **Предузећа која одређују ресурсе**, а одељења која пружају ресурсе су **Јединице за одређивање ресурса**. Због разлика у трошковима радне снаге у различитим географским подручјима и на тржиштима рада широм света, стопе наплате за рад такође су различито постављене за различите географске регије.

На пример, програмеру из одељења за роботику компаније Fabrikam India, који ради на америчком пројекту, наплаћује се стопа од 100 USD на сат. Програмеру из одељења за роботику компаније Fabrikam US, који ради на америчком пројекту, наплаћује се стопа од 150 USD на сат. 

### <a name="example-set-up-a-bill-rate"></a>Пример: Подесите стопу наплате 

1. Креирајте продајни ценовник под називом *Fabrikam US стопе наплате* и одредите датум ступања на снагу.
2. У продајни ценовник унесите следеће информације о цени:

    | Улога | Предузеће које обезбеђује ресурсе | Јединица за одређивање ресурса | Стопа наплате |
    | --- | --- | --- | --- |
    | Пројектант | Fabrikam India | Fabrikam India - Robotics | $100 |
    | Пројектант | Fabrikam Philippines | Fabrikam Philippines - Robotics | 90 USD |
    | Пројектант | Fabrikam US | Fabrikam US - Robotics | 150 USD |

3. Приложите продајни ценовник, **Fabrikam US стопе наплате** пројектном ценовнику пројектног уговора или на одређени налог.