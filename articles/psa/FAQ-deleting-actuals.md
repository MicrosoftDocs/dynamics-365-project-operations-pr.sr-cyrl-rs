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
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="82f83-103">Зато не могу да избришем записе из ентитета стварних вредности?</span><span class="sxs-lookup"><span data-stu-id="82f83-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="82f83-104">Project Service Automation (PSA) не допушта вам брисање стварних вредности јер оне служе као извор истине за трансакције које имају финансијске импликације на долазне системе, као што је главна књига.</span><span class="sxs-lookup"><span data-stu-id="82f83-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="82f83-105">Ако би се стварне вредности могле избрисати, могао би се довести у питање интегритет трансакција финансијског извештавања.</span><span class="sxs-lookup"><span data-stu-id="82f83-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="82f83-106">Да би успоставили евиденцију надгледања, клијенти би требало да користе дневнике за креирање трансакција компензације.</span><span class="sxs-lookup"><span data-stu-id="82f83-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

