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
ms.openlocfilehash: e3122c5d9495b3ff9a683f477e719ce0c228a84d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286086"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="ea575-103">Зато не могу да избришем записе из ентитета стварних вредности?</span><span class="sxs-lookup"><span data-stu-id="ea575-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ea575-104">Project Service Automation (PSA) не допушта вам брисање стварних вредности јер оне служе као извор истине за трансакције које имају финансијске импликације на долазне системе, као што је главна књига.</span><span class="sxs-lookup"><span data-stu-id="ea575-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="ea575-105">Ако би се стварне вредности могле избрисати, могао би се довести у питање интегритет трансакција финансијског извештавања.</span><span class="sxs-lookup"><span data-stu-id="ea575-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="ea575-106">Да би успоставили евиденцију надгледања, клијенти би требало да користе дневнике за креирање трансакција компензације.</span><span class="sxs-lookup"><span data-stu-id="ea575-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]