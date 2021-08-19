---
title: Зато не могу да избришем записе из ентитета стварних вредности?
description: Ова тема пружа информације о томе зашто не можете обрисати записе из ентитета стварних вредности.
author: JPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
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
ms.openlocfilehash: d60a3586fd1f0f688bcd2626d039ebc1aa6b0925c90d676f0e716400d8e8d6dd
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "7002889"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>Зато не могу да избришем записе из ентитета стварних вредности?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Project Service Automation (PSA) не допушта вам брисање стварних вредности јер оне служе као извор истине за трансакције које имају финансијске импликације на долазне системе, као што је главна књига. Ако би се стварне вредности могле избрисати, могао би се довести у питање интегритет трансакција финансијског извештавања. Да би успоставили евиденцију надгледања, клијенти би требало да користе дневнике за креирање трансакција компензације.



[!INCLUDE[footer-include](../includes/footer-banner.md)]