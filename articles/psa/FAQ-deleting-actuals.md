---
title: Зато не могу да избришем записе из ентитета стварних вредности?
description: Овај чланак пружа информације о томе зашто не можете обрисати записе из ентитета стварних вредности.
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
ms.reviewer: johnmichalak
ms.openlocfilehash: bd446961432a8f18895db45699d7a731d55235b5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925598"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>Зато не могу да избришем записе из ентитета стварних вредности?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Project Service Automation (PSA) не допушта вам брисање стварних вредности јер оне служе као извор истине за трансакције које имају финансијске импликације на долазне системе, као што је главна књига. Ако би се стварне вредности могле избрисати, могао би се довести у питање интегритет трансакција финансијског извештавања. Да би успоставили евиденцију надгледања, клијенти би требало да користе дневнике за креирање трансакција компензације.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
