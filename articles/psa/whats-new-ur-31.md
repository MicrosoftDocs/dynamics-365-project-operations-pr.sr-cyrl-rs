---
title: Шта је ново или промењено у издању 31 исправке Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 31 исправке за Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: 160187ba7b96547e85a7a4ec4bf84c86d8fd8257
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999149"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="a431c-103">Шта је ново или промењено у издању 31 исправке Project Service Automation верзије 3</span><span class="sxs-lookup"><span data-stu-id="a431c-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a431c-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a431c-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a431c-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="a431c-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a431c-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="a431c-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a431c-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="a431c-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="a431c-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a431c-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a431c-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 31.</span><span class="sxs-lookup"><span data-stu-id="a431c-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="a431c-110">Број израде ове верзије је V3.10.52.77 и углавном је доступна путем самосталног ажурирања у мају 2021. године.</span><span class="sxs-lookup"><span data-stu-id="a431c-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="a431c-111">Издање исправке 31</span><span class="sxs-lookup"><span data-stu-id="a431c-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a431c-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="a431c-112">Bug fixes</span></span>

<span data-ttu-id="a431c-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="a431c-113">**Time and Expense**</span></span>

<span data-ttu-id="a431c-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="a431c-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="a431c-115">Командна дугмад за контролу уноса времена на страници **Ресурс који може да се резервише** су збуњивала кориснике.</span><span class="sxs-lookup"><span data-stu-id="a431c-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="a431c-116">Нулти изузетак референце је генерисан у **Project.SetTrackingFields** приликом одобравања уноса времена.</span><span class="sxs-lookup"><span data-stu-id="a431c-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="a431c-117">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="a431c-117">**Resource Management**</span></span>

<span data-ttu-id="a431c-118">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="a431c-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="a431c-119">**Направите члана тима** не приказује исправно подешавање метаподатака за подешавање резервације за **Подразумевани статус послате резервације**.</span><span class="sxs-lookup"><span data-stu-id="a431c-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="a431c-120">Приликом надоградње са PSA 1.X to 3.X, процес надоградње не успева на **UpgradeResourceRequirements**.</span><span class="sxs-lookup"><span data-stu-id="a431c-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="a431c-121">**Продаја**</span><span class="sxs-lookup"><span data-stu-id="a431c-121">**Sales**</span></span>

<span data-ttu-id="a431c-122">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="a431c-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="a431c-123">Стварни приход претвара износе у валуту пројекта у мрежи за праћење.</span><span class="sxs-lookup"><span data-stu-id="a431c-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="a431c-124">Задана валута није јасна приликом креирања редова дневника, цитата и линија уговора у сценаријима када се основна валута организације разликује од валуте пројекта.</span><span class="sxs-lookup"><span data-stu-id="a431c-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="a431c-125">Упит **валидације дневника исправки на чекању** се не филтрира према пројекту.</span><span class="sxs-lookup"><span data-stu-id="a431c-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="a431c-126">Преостала продаја се на пројекту погрешно израчунава.</span><span class="sxs-lookup"><span data-stu-id="a431c-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="a431c-127">Понуде засноване на контакту не успевају када се креирају без ценовника.</span><span class="sxs-lookup"><span data-stu-id="a431c-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="a431c-128">Када одаберете **Потврдите фактуру**, не приказује се знак обраде.</span><span class="sxs-lookup"><span data-stu-id="a431c-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="a431c-129">Када одаберете **Креирај фактуру**, не приказује се знак обраде.</span><span class="sxs-lookup"><span data-stu-id="a431c-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="a431c-130">Затварање понуде као изгубљене не отказује резервације.</span><span class="sxs-lookup"><span data-stu-id="a431c-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







