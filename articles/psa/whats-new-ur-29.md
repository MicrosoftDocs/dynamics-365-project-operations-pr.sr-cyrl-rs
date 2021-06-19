---
title: Шта је ново или промењено у издању 29 исправке Project Service Automation верзије 3
description: У овој теми су наведене функције и исправке које су доступне у издању исправке 29 за Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 320f4f74cb5997e42e2dc9e1d8c8a5ab95ae6647
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010489"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="8bf73-103">Шта је ново или промењено у издању 29 исправке Project Service Automation верзије 3</span><span class="sxs-lookup"><span data-stu-id="8bf73-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="8bf73-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="8bf73-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="8bf73-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="8bf73-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="8bf73-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="8bf73-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="8bf73-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="8bf73-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="8bf73-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="8bf73-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="8bf73-109">У овој теми су наведене функције и исправке које су нове или промењене у издању исправке 29 за Project Service Automation верзије 3.</span><span class="sxs-lookup"><span data-stu-id="8bf73-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="8bf73-110">Ова верзија има број верзије V3.10.47.7 и генерално је доступна путем самосталног ажурирања у фебруаре 2021.</span><span class="sxs-lookup"><span data-stu-id="8bf73-110">This version has a build number of V3.10.47.7 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="8bf73-111">Издање исправке 29</span><span class="sxs-lookup"><span data-stu-id="8bf73-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="8bf73-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="8bf73-112">Bug fixes</span></span>

<span data-ttu-id="8bf73-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="8bf73-113">**Time and Expense**</span></span>

<span data-ttu-id="8bf73-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="8bf73-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="8bf73-115">Корисници не могу да виде радно време забележено нерадним данима у мрежи за унос времена.</span><span class="sxs-lookup"><span data-stu-id="8bf73-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="8bf73-116">Одобрени уноси трошкова могу се уређивати на мрежи.</span><span class="sxs-lookup"><span data-stu-id="8bf73-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="8bf73-117">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="8bf73-117">**Project Management**</span></span>

<span data-ttu-id="8bf73-118">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="8bf73-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="8bf73-119">Недостаје логика валидације да би се осигурало да сати ангажовања за доделу ресурса не могу бити негативни.</span><span class="sxs-lookup"><span data-stu-id="8bf73-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="8bf73-120">Прилагођена радња, **AssignResourcesForTask** ажурира сва поља, а не само промењена.</span><span class="sxs-lookup"><span data-stu-id="8bf73-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="8bf73-121">Када копирате пројекат у окружењу са додатним компонентама или токовима посла који су регистровани у догађају **CreateProject**, атрибут **msdyn_bulkgenerationstatus** се не ажурира ако је **CopyWBSToProject** неуспешан.</span><span class="sxs-lookup"><span data-stu-id="8bf73-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="8bf73-122">Када проширите календар пројекта, радни дани се не сортирају у растућем редоследу, што доводи до неуспеха ажурирања неких пројектних задатака.</span><span class="sxs-lookup"><span data-stu-id="8bf73-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="8bf73-123">Промена менаџера пројекта на постојећем пројекту покреће подразумевану логику организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="8bf73-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="8bf73-124">**Продаја**</span><span class="sxs-lookup"><span data-stu-id="8bf73-124">**Sales**</span></span>

<span data-ttu-id="8bf73-125">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="8bf73-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="8bf73-126">Картица **Извршење уговора** на страници **Уговор** без упозорења не успева током иницијализације када нема линија уговора.</span><span class="sxs-lookup"><span data-stu-id="8bf73-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>