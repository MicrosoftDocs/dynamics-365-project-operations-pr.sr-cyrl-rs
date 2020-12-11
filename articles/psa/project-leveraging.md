---
title: Продајне процене и пројекти
description: Ова тема пружа информације о томе како искористити распоред и процене у процесу продаје.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: d8bb380519759659dc1b4151b62228a626ee7a26
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120696"
---
# <a name="sales-estimates-and-projects"></a>Продајне процене и пројекти

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Током процеса продаје можете креирати процене продаје повезујући пројекат с продајном понудом. На овај начин, може да дође до детерминистичке процене током процеса продаје, како би се искористиле предности заказивања пројеката и процене. Ако продаја прође, распоред који је коришћен за процену продаје може се користити као основа за даље прецизирање пројектног плана.

## <a name="linking-a-project-to-a-quote-line"></a>Повезивање пројекта са ставком понуде

Када креирате ставку понуде засновану на пројекту, можете да креирате нови пројекат или повежете постојећи пројекат на страници **Ставка пројекта**. 

> ![Образац ставке понуде](media/project-8.png)
 
Када креирате нови пројекат из детаља ставке понуде, можете искористити предлошке пројекта. Предлошци пројеката су модели пројеката који представљају стандардне планове пројеката и финансијске процене типичне за организацију. Такође могу представљати копије пројектних планова и процена из прошлих пројеката.

> ![Детаљи ставке понуде](media/project-9.png)
  
Када креирате пројекат из понуде, пројекат се аутоматски повезује са ставком понуде.

## <a name="components-of-estimates-in-a-project"></a>Компоненте процена у пројекту

Распоред вам омогућава да поделите посао на задатке, одржавате хијерархију задатака, одредите који су ресурси потребни за обављање задатка и доделите процену потребних активности за обављање задатка.

Можете дефинисати радне активности и процене распореда помоћу поља на картици **Распоред** у оквиру странице **Пројекат**. Пошто је ценовник повезан са пројектом, финансијске процене се израчунавају коришћењем цене коштања и продајне цене које су дефинисане у ценовнику.

## <a name="importing-estimates-from-a-project-into-a-quote"></a>Увоз процена из пројекта у понуду

Након што дефинишете процене пројекта, можете их увести у ставку понуде. На страници **Детаљи ставке понуде** изаберите **Увоз из процена** на траци да бисте резимирали процене пројекта према врсти трансакције, улози или нивоу задатка.