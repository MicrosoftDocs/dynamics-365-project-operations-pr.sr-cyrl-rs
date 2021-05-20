---
title: Шта је ново или промењено у издању 12 исправке Project Service Automation верзије 3
description: У овој теми дате су информације о томе шта је ново у издању исправке 12 за Project Service Automation у верзији 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: 58a12ded135712d8194499ce4a9ba9e4e2aa99bd
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949517"
---
# <a name="project-service-automation-update-release-12-v3"></a><span data-ttu-id="199c7-103">Project Service Automation издање исправке 12, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="199c7-103">Project Service Automation Update Release 12, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="199c7-104">Са задовољство најављујемо најновију исправку за апликацију Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="199c7-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="199c7-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="199c7-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="199c7-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="199c7-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="199c7-107">Да бисте ажурирали ово издање, посетите центар за администрацију за Dynamics 365 online и идите до странице са решењима како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="199c7-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="199c7-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="199c7-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="199c7-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 12.</span><span class="sxs-lookup"><span data-stu-id="199c7-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 12.</span></span> <span data-ttu-id="199c7-110">Ова верзија има број верзије V3.10.2.34 и опште је доступна путем само-исправке у октобру 2019. године.</span><span class="sxs-lookup"><span data-stu-id="199c7-110">This version has a build number of V3.10.2.34 and is generally available through a self-update in October 2019.</span></span>

## <a name="update-release-12"></a><span data-ttu-id="199c7-111">Издање исправке 12</span><span class="sxs-lookup"><span data-stu-id="199c7-111">Update Release 12</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="199c7-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="199c7-112">Bug fixes</span></span>

- <span data-ttu-id="199c7-113">Време и трошак</span><span class="sxs-lookup"><span data-stu-id="199c7-113">Time and Expense</span></span>

    - <span data-ttu-id="199c7-114">Исправљено: Поруке о грешкама за ставку времена су исправљене са релевантнијим контекстом.</span><span class="sxs-lookup"><span data-stu-id="199c7-114">Fixed: Time entry error messaging has been updated with more relevant context.</span></span>
    - <span data-ttu-id="199c7-115">Исправљено: Мрежа ставке времена и распоред исправно приказују вертикалну траку за листање када је то потребно.</span><span class="sxs-lookup"><span data-stu-id="199c7-115">Fixed: Time entry grid and schedule correctly displays the vertical scrollbar when required.</span></span>
    - <span data-ttu-id="199c7-116">Исправљено: није могуће одобрити прослеђене ставке трошкова и времена.</span><span class="sxs-lookup"><span data-stu-id="199c7-116">Fixed: Submitted expense and time entries can be approved.</span></span>
    - <span data-ttu-id="199c7-117">Исправљено: порука дијалога потврде отказивања одобрења је исправљена и одражава статус одобрења када се промени из **Одобрено** у **Прослеђено**.</span><span class="sxs-lookup"><span data-stu-id="199c7-117">Fixed: Cancel approval confirmation dialog message has been corrected to reflect the status of the approval when changed from **Approved** to **Submitted**.</span></span>
    - <span data-ttu-id="199c7-118">Исправљено: поља **Цена**, **Јединица** и **Количина** су сада закључана у запису трошка након што је одобрен.</span><span class="sxs-lookup"><span data-stu-id="199c7-118">Fixed: **Price**, **Unit**, and **Quantity** fields are now locked on the Expense record after it is has been approved.</span></span>

- <span data-ttu-id="199c7-119">Управљање пројектима</span><span class="sxs-lookup"><span data-stu-id="199c7-119">Project Management</span></span>

    - <span data-ttu-id="199c7-120">Исправљено: радња **Ново** на главном обрасцу **Члан тима** је уклоњена.</span><span class="sxs-lookup"><span data-stu-id="199c7-120">Fixed: **New** action on **Team member** main form has been removed.</span></span>
    - <span data-ttu-id="199c7-121">Исправљено: доделе ресурса су исправљене како би се узеле у обзир грешке у непрецизном заокруживању, које доводе до померања датума завршетка задатка.</span><span class="sxs-lookup"><span data-stu-id="199c7-121">Fixed: Resource assignments have been updated to account for inaccurate rounding errors, which lead to a shift in a task’s end date.</span></span>
    - <span data-ttu-id="199c7-122">Исправљено: у мрежи задатака кориснику ће се приказати релевантне грешке на страни сервера.</span><span class="sxs-lookup"><span data-stu-id="199c7-122">Fixed: In the task grid, relevant server-side errors will be surfaced to the user.</span></span>
    - <span data-ttu-id="199c7-123">Исправљено: име члана тима сада се приказује у задатку бирача особа уместо назива положаја.</span><span class="sxs-lookup"><span data-stu-id="199c7-123">Fixed: The team member’s name now renders in the task people picker instead of the position name.</span></span>

- <span data-ttu-id="199c7-124">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="199c7-124">Resource Management</span></span>

    - <span data-ttu-id="199c7-125">Исправљено: детаљи о захтевима за ресурсима за пројекте креиране из предлошка сада користе календар пројеката.</span><span class="sxs-lookup"><span data-stu-id="199c7-125">Fixed: Resource requirement details for projects created from a template now use the project calendar.</span></span>
    - <span data-ttu-id="199c7-126">Исправљено: вештине и компетенције сада подразумевано потичу из основних података улоге у захтев за ресурсом који је креиран за ту улогу.</span><span class="sxs-lookup"><span data-stu-id="199c7-126">Fixed: Skills and competencies now default from role master data to the resource requirement created for that role.</span></span>

- <span data-ttu-id="199c7-127">Sales</span><span class="sxs-lookup"><span data-stu-id="199c7-127">Sales</span></span>

    - <span data-ttu-id="199c7-128">Исправљено: дуплирани ID-ови објекта пронађени на главном обрасцу **Уговор**.</span><span class="sxs-lookup"><span data-stu-id="199c7-128">Fixed: Duplicate object IDs found on the **Contract main** form.</span></span>
    - <span data-ttu-id="199c7-129">Исправљено: логика је исправљена како би картица **Анализа понуде** била видљива тако да приказује подешавање метаподатака картице.</span><span class="sxs-lookup"><span data-stu-id="199c7-129">Fixed: Logic has been updated to make the **Quote Analysis** tab visible so that it displays the metadata setup of the tab.</span></span>
    - <span data-ttu-id="199c7-130">Исправљено: рачуноводствени датум на стварном запису сада потиче од датума уноса времена/трошка, а не од датума одобрења.</span><span class="sxs-lookup"><span data-stu-id="199c7-130">Fixed: Accounting date on the actual record now comes from the date of the time/expense entry date and not the date of the approval.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]