---
title: Шта је ново или промењено у издању 15 исправке Project Service Automation верзије 3
description: У овој теми дате су информације о томе шта је ново у издању исправке 15 за Project Service Automation у верзији 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/27/2020
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
ms.openlocfilehash: 86aadca637939120d0ccd839e7c425e9e8d38aec
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006844"
---
# <a name="project-service-automation-update-release-15-v3"></a><span data-ttu-id="b71a5-103">Project Service Automation издање исправке 15, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="b71a5-103">Project Service Automation Update Release 15, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b71a5-104">Са задовољство најављујемо најновију исправку за апликацију Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="b71a5-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="b71a5-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="b71a5-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b71a5-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="b71a5-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b71a5-107">Да бисте ажурирали ово издање, посетите центар за администрацију за Dynamics 365 online и идите до странице са решењима како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="b71a5-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="b71a5-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="b71a5-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b71a5-109">У овој теми дате су функције и исправке које су нове или су промењене у решењу PSA у верзији 3, издање исправке 15.</span><span class="sxs-lookup"><span data-stu-id="b71a5-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 15.</span></span> <span data-ttu-id="b71a5-110">Ова верзија има број верзије V3.10.5.28 и опште је доступна путем само-исправке у јануару 2020. године.</span><span class="sxs-lookup"><span data-stu-id="b71a5-110">This version has a build number of V3.10.5.28 and is generally available through a self-update in January 2020.</span></span>

## <a name="update-release-15"></a><span data-ttu-id="b71a5-111">Издање исправке 15</span><span class="sxs-lookup"><span data-stu-id="b71a5-111">Update Release 15</span></span> 

### <a name="enhancements"></a><span data-ttu-id="b71a5-112">Побољшања</span><span class="sxs-lookup"><span data-stu-id="b71a5-112">Enhancements</span></span>

- <span data-ttu-id="b71a5-113">Управљање пројектима</span><span class="sxs-lookup"><span data-stu-id="b71a5-113">Project Management</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b71a5-114">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="b71a5-114">Bug fixes</span></span>

- <span data-ttu-id="b71a5-115">Време и трошак</span><span class="sxs-lookup"><span data-stu-id="b71a5-115">Time and Expense</span></span>

  - <span data-ttu-id="b71a5-116">Исправљено: додавање руковања грешком приликом учитавања у приказу усклађивања.</span><span class="sxs-lookup"><span data-stu-id="b71a5-116">Fixed: Add on-load error handling in the reconciliation view.</span></span>
  - <span data-ttu-id="b71a5-117">Исправљено: чвориште ресурса за пројекат: преименовање ставке **Износ** ради смањења двосмислености.</span><span class="sxs-lookup"><span data-stu-id="b71a5-117">Fixed: Project Resource Hub: Rename **Amount** to reduce ambiguity.</span></span>
  - <span data-ttu-id="b71a5-118">Исправљено: подешавање приказа **Копирање колона за ставку времена** тако да обухвата тип.</span><span class="sxs-lookup"><span data-stu-id="b71a5-118">Fixed: Adjust the view **Copy Time Entry Columns** to include the type.</span></span>
  - <span data-ttu-id="b71a5-119">Исправљено: уређивање трајања ставке времена у приказу мреже коришћењем децималних бројева резултира непознатом грешком код неких бројева.</span><span class="sxs-lookup"><span data-stu-id="b71a5-119">Fixed: Editing time entry duration in the grid view using decimal numbers results in unknown error for some numbers.</span></span>

- <span data-ttu-id="b71a5-120">Управљање пројектима</span><span class="sxs-lookup"><span data-stu-id="b71a5-120">Project Management</span></span>

  - <span data-ttu-id="b71a5-121">Исправљено: падајући мени за **Коришћење у приказу праћења** се сада проширује на основу ширине опција.</span><span class="sxs-lookup"><span data-stu-id="b71a5-121">Fixed: The drop-down menu for **Use in Tracking View** now expands based on the width of the options.</span></span>
  - <span data-ttu-id="b71a5-122">Исправљено: када управљате пројектима у временској зони +13, прорачуни задатака могу приказати нетачне резултате.</span><span class="sxs-lookup"><span data-stu-id="b71a5-122">Fixed: When managing projects in the +13 time zone, tasks calculations can display inaccurate results.</span></span>
  - <span data-ttu-id="b71a5-123">Исправљено: **Време завршетка члана тима** је исправљено када се користи календар од 24 сата.</span><span class="sxs-lookup"><span data-stu-id="b71a5-123">Fixed: **Team Member End Time** has been corrected when using a 24-hour calendar.</span></span>
  - <span data-ttu-id="b71a5-124">Исправљено: поново активиран **BPF** у главном обрасцу **msdyn_project**.</span><span class="sxs-lookup"><span data-stu-id="b71a5-124">Fixed: Re-activated the **BPF** in **msdyn_project** main form.</span></span>
  - <span data-ttu-id="b71a5-125">Исправљено: израчунавање задатака више не игнорише један дан.</span><span class="sxs-lookup"><span data-stu-id="b71a5-125">Fixed: Assignments calculation no longer ignores one day.</span></span>
  - <span data-ttu-id="b71a5-126">Исправљено: нови банер обавештења је додат у образац пројекта када се временска зона разликује између корисника и пројеката.</span><span class="sxs-lookup"><span data-stu-id="b71a5-126">Fixed: A new notification banner has been added to the project form when the time zone differs between user and project.</span></span>

- <span data-ttu-id="b71a5-127">Sales</span><span class="sxs-lookup"><span data-stu-id="b71a5-127">Sales</span></span>

  - <span data-ttu-id="b71a5-128">Исправљено: проналажење категорије процене трошкова може да се користи за филтрирање дупликата.</span><span class="sxs-lookup"><span data-stu-id="b71a5-128">Fixed: Expense estimate category lookup can be used to filter duplicates.</span></span>
  - <span data-ttu-id="b71a5-129">Исправљено: кôд у **PluginDomain.ExecuteInTryCatchBlock(..)** више не сакрива порекло изузетка.</span><span class="sxs-lookup"><span data-stu-id="b71a5-129">Fixed: Code in **PluginDomain.ExecuteInTryCatchBlock(..)** no longer hides the origin of the exception.</span></span>
  - <span data-ttu-id="b71a5-130">Исправљено: више се не добија порука о грешци у ставци **Проналажење пројекта** у обрасцу **Ставка понуде** када има преко 1000 пројеката.</span><span class="sxs-lookup"><span data-stu-id="b71a5-130">Fixed: No longer get an error message in **Project lookup** in the **Quote Line** form when there are more than 1000 projects.</span></span>
  - <span data-ttu-id="b71a5-131">Исправљено: Мрежа **Процене** за процене цене рада и цене трошкова сада приказује исправан симбол валуте.</span><span class="sxs-lookup"><span data-stu-id="b71a5-131">Fixed: **Estimates** grid for labor estimates and expense estimates now displays the correct currency symbol.</span></span>
  - <span data-ttu-id="b71a5-132">Исправљено: након што организација ажурира PSA са издања исправке 14 на издање исправке 15, картица **Распоред** се више не појављује као празна у обрасцу **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="b71a5-132">Fixed: After an organization updates PSA from Update Release 14 to Update Release 15, the **Schedule** tab no longer appears as blank on the **Project** form.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]