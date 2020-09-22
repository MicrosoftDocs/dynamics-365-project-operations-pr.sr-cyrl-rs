---
title: Зато не могу да избришем записе из ентитета стварних вредности?
description: Ова тема пружа информације о томе зашто не можете обрисати записе из ентитета стварних вредности.
author: JPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.prod: Project Service
ms.technology: Applies to all versions of Project Service
ms.assetid: ff504c34-7337-474f-89e8-d8afdd1e0a98
ms.author: Jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5817940933c161dccac0fe549fabacbe57e7077a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755329"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="bfb93-103">Зато не могу да избришем записе из ентитета стварних вредности?</span><span class="sxs-lookup"><span data-stu-id="bfb93-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="bfb93-104">Project Service Automation (PSA) не допушта вам брисање стварних вредности јер оне служе као извор истине за трансакције које имају финансијске импликације на долазне системе, као што је главна књига.</span><span class="sxs-lookup"><span data-stu-id="bfb93-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="bfb93-105">Ако би се стварне вредности могле избрисати, могао би се довести у питање интегритет трансакција финансијског извештавања.</span><span class="sxs-lookup"><span data-stu-id="bfb93-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="bfb93-106">Да би успоставили евиденцију надгледања, клијенти би требало да користе дневнике за креирање трансакција компензације.</span><span class="sxs-lookup"><span data-stu-id="bfb93-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

