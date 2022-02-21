---
title: Предмети подуговора за категорије трошкова
description: Ова тема објашњава како евидентирати предмете подуговора за трошак и користити поља за бележење времена куповине од продаваца.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0c32bf2ac54de98a921d338e436ecd089e68a759
ms.sourcegitcommit: cd4e81f129681a12f2efe63ec2bb14e611cf88ba
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/20/2021
ms.locfileid: "7506117"
---
#  <a name="subcontract-lines-for-expense-categories"></a>Предмети подуговора за категорије трошкова

[!include [banner](../../includes/dataverse-preview.md)]

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Подуговор у услузи Dynamics 365 Project Operations може имати предмет за категорије трошкова. Предмети подуговора за категорије трошкова дозвољавају менаџеру пројекта да купује категорије услуга или производа од продаваца које могу да наплате на име пројекта.

Довршите следеће кораке да бисте креирали предмет подуговора за категорије трошкова у услузи Project Operations.

1. На страници навигације изаберите **Подуговори** и отворите подуговор са којим желите да радите.
2. На картици **Предмети подуговора** изаберите **Ново** за креирање новог предмета.
3. На страници **Брзо креирање**, у пољу **Класа трансакције** изаберите **Трошак** и унесите или изаберите било које друге потребне информације о пољу.

Следећа табела пружа информације о пољима на страници са детаљима **Предмет подуговора** и страници **Брзо креирање**.

| **Поље** | **Опис** | **Функционални утицај** |
| --- | --- | --- |
| Име | Назив ставке подуговора за помоћ при идентификацији. | Ово ће бити приказано као прва колона у свим претрагама заснованим на ставкама предмета подуговора. |
| Опис | Кратак опис категорија трошкова које се купују у ставци подуговора. | Ниједно |
|Тип предмета | Ово поље има подразумевану вредност **На основу количине**. |Ниједно |
| Начин наплате | Ово је скуп опција који представља два главна модела уговарања подржана у услузи Project Operations: **Фиксна цена** и **Време и материјал**. | Распоред фактура заснован на контролним тачкама је доступан за ставке подуговора када је изабран метод наплате по фиксној цени. |
| Класа трансакције | Ово поље има подразумевану вредност **Време**. Да бисте креирали предмете подуговора за куповину производа, подесите поље **Класа трансакције** на **Трошак**.  | Ово указује на то да се предмет подуговора користи за евидентирање куповине категорије трошкова који ће се користити на пројектима. |
| Категорија трансакције | Приказује листу активних категорија трансакција у систему. |Ниједно |
| Захтевани почетак | Унесите датум када категорије набавке морају да буду доступне код добављача. | Захтевано време почетка се користи за избор ценовника пројекта из ценовника пројекта који је приложен подуговору. Цена категорије на ставци подуговора потиче из тог ценовника. |
| Захтевани завршетак | Унесите датум када категорије набавке више неће бити потребне. | Ово ће се користити за приказивање упозорења када вођа пројекта повеже ову ставку подуговора са одређеним проценама трошкова на пројекту који су потребни након овог датума. |
| Поручена количина | Количина категорије која се купује од добављача. | Ово ће се користити за приказивање упозорења када вођа пројекта користи количину већу од ове.|
| Група јединица | Подразумевана вредност се заснива на подразумеваној групи јединица која је подешена за изабрану категорију. |Ниједно |
| Јединица | Подразумевана вредност се заснива на подразумеваној јединици која је подешена за изабрану категорију.  | Комбинација **Категорије** и **Јединице** користиће се као подразумевана вредност или ће бити израчуната за јединичну цену за предмет подуговора.  |
| Цена по јединици | Подразумевана вредност користи комбинацију **Категорије** и **Јединице** из цена категорија које су повезане са ценовником пројекта, што је применљиво за тражено време почетка за ставку подуговора. |Ниједно |
| Међуизнос | Ово је поље само за читање које се израчунава као „Количина“ X „Јединична цена“, ако су унете вредности за количину и јединичну цену. Ако су једно или оба поља празна, можете унети вредност у ово поље. |Ниједно |
| Порез на промет | Унесите износ пореза на промет. |Ниједно |
| Укупан износ | Укупан износ из предмета подуговора укључујући порез. Ово поље се рачуна као међузбир + порез на промет. |Ниједно |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]