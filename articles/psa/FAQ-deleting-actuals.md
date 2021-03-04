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
ms.openlocfilehash: 36cd241c7c7a2ff6ae018c94d691bc95d1f0c912
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148976"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="2873b-103">Зато не могу да избришем записе из ентитета стварних вредности?</span><span class="sxs-lookup"><span data-stu-id="2873b-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="2873b-104">Project Service Automation (PSA) не допушта вам брисање стварних вредности јер оне служе као извор истине за трансакције које имају финансијске импликације на долазне системе, као што је главна књига.</span><span class="sxs-lookup"><span data-stu-id="2873b-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="2873b-105">Ако би се стварне вредности могле избрисати, могао би се довести у питање интегритет трансакција финансијског извештавања.</span><span class="sxs-lookup"><span data-stu-id="2873b-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="2873b-106">Да би успоставили евиденцију надгледања, клијенти би требало да користе дневнике за креирање трансакција компензације.</span><span class="sxs-lookup"><span data-stu-id="2873b-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

