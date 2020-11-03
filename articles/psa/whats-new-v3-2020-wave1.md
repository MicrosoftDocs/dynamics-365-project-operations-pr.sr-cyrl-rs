---
title: Шта је ново или промењено у апликацији Project Service Automation у верзији 3.x таласу 1 за 2020. годину
description: У овој теми дате су информације о томе шта је ново и шта се променило у решењу Project Service Automation у верзији 3 таласу 1 за 2020.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/15/2020
ms.topic: article
author: stsporen
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 16b51995f863d9ee54172625dacbf081c51c8556
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083918"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="f3eb0-103">Шта је ново или промењено у апликацији Project Service Automation у верзији 3 таласу 1 за 2020. годину</span><span class="sxs-lookup"><span data-stu-id="f3eb0-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="f3eb0-104">Тема истиче кључне чињенице које треба узети у обзир приликом надоградње када прелазите на најновије издање решења Project Service Automation (PSA) верзије 3.x таласа 1 за 2020.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="f3eb0-105">Ставка времена</span><span class="sxs-lookup"><span data-stu-id="f3eb0-105">Time entry</span></span>
<span data-ttu-id="f3eb0-106">Искуство ставке времена је проширено како би испоручило могућности продужетка ставке времена у више сценарија клијената.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="f3eb0-107">Ово обухвата могућност додавања типова ставки, који сада покрећу одређено понашање на основу назива плана поља **Подешавања ставке времена** , приказано као **Извор времена**.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings** , displayed as **Time Source**.</span></span> <span data-ttu-id="f3eb0-108">Ново решење, под називом „Time, Expense, Statusing, and Approvals“ (TESA) је додат како би била подржана ова функционалност.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-108">A new solution, called Time, Expense, Statusing, and Approvals (TESA) has been added to support this functionality.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="f3eb0-109">Чињеница коју треба узети у обзир приликом надоградње</span><span class="sxs-lookup"><span data-stu-id="f3eb0-109">Upgrade consideration</span></span>
<span data-ttu-id="f3eb0-110">Како би ова функционалност била подржана, улоге у оквиру решења PSA су ажурирана тако да обухватају нове привилегије.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-110">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="f3eb0-111">Ове привилегије омогућавају приступ за читање новом ентитету, **Подешавања ставке времена**.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-111">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="f3eb0-112">Корисницима који захтевају могућност евидентирања времена би поред постојећих улога требало доделити корисничку улогу **Корисник ставке времена**.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-112">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="f3eb0-113">Ова улога укључује нову функционалност и обезбеђује да ставка времена и даље ради.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-113">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

<span data-ttu-id="f3eb0-114">Поред тога, ако имате прилагођене модуле апликација који садрже све обрасце за ентитет уноса времена, мораћете да уклоните **TESA образац за брзо креирање ставке времена** из модула.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-114">Additionally, if you have any custom app modules that include all forms for the time entry entity, you will be required to remove the **TESA time Entry Quick Create Form** from the module.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="f3eb0-115">Тренутно промењене проширене ставке времена</span><span class="sxs-lookup"><span data-stu-id="f3eb0-115">Currently extended time entry changes</span></span>
<span data-ttu-id="f3eb0-116">Како би се смањио утицај на тренутне кориснике ставке времена, ова промена улоге је једини суштински захтев који је неопходан како би се и даље користила ставка времена.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-116">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="f3eb0-117">Ако сте креирали прилагођене приказе или одвојена искуства ставки времена, морате подесити поља **Подешавање ставке времена** на исправну PSA вредност.</span><span class="sxs-lookup"><span data-stu-id="f3eb0-117">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
