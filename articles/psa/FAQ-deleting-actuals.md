---
title: Зато не могу да избришем записе из ентитета стварних вредности?
description: Ова тема пружа информације о томе зашто не можете обрисати записе из ентитета стварних вредности.
author: JPBurrows
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: b9b45e3ae0cd9273af4d2a5cd9cce30502c0aa78
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127176"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>Зато не могу да избришем записе из ентитета стварних вредности?

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Project Service Automation (PSA) не допушта вам брисање стварних вредности јер оне служе као извор истине за трансакције које имају финансијске импликације на долазне системе, као што је главна књига. Ако би се стварне вредности могле избрисати, могао би се довести у питање интегритет трансакција финансијског извештавања. Да би успоставили евиденцију надгледања, клијенти би требало да користе дневнике за креирање трансакција компензације.

