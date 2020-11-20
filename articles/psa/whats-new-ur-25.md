---
title: Шта је ново или промењено у издању 25 исправке Project Service Automation верзије 3
description: У овој теми су наведене функције и исправке које су доступне у издању 25 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: a5a81893c4a804deb09cf33e0ac3f1a25b8bca36
ms.sourcegitcommit: a2b810219d381716d3eedb14c4eb6cdefb5b5845
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/02/2020
ms.locfileid: "4183561"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a><span data-ttu-id="5b27c-103">Шта је ново или промењено у издању 25 исправке Project Service Automation верзије 3</span><span class="sxs-lookup"><span data-stu-id="5b27c-103">What's new or changed in Project Service Automation Update Release 25, V3</span></span>

<span data-ttu-id="5b27c-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5b27c-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="5b27c-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="5b27c-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="5b27c-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="5b27c-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="5b27c-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="5b27c-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="5b27c-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="5b27c-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="5b27c-109">У овој теми су наведене функције и исправке које су нове или промењене за Project Service Automation верзије 3, издање 25 исправке. Ова верзија има број верзије V 3.10.43.76 и постала је опште доступна путем самосталне исправке у октобру 2020.</span><span class="sxs-lookup"><span data-stu-id="5b27c-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 25 This version has a build number of V 3.10.43.76 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-25"></a><span data-ttu-id="5b27c-110">Издање исправке 25</span><span class="sxs-lookup"><span data-stu-id="5b27c-110">Update Release 25</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="5b27c-111">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="5b27c-111">Bug fixes</span></span>

<span data-ttu-id="5b27c-112">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="5b27c-112">**Time and Expense**</span></span>

<span data-ttu-id="5b27c-113">Следећи проблем је исправљен:</span><span class="sxs-lookup"><span data-stu-id="5b27c-113">The following issue has been fixed:</span></span>

- <span data-ttu-id="5b27c-114">Графикон ставке времена који приказује додатне податке на основу превеликог интервала који се преузима.</span><span class="sxs-lookup"><span data-stu-id="5b27c-114">Time entry chart showing additional data based on too large of an interval being retrieved.</span></span>

<span data-ttu-id="5b27c-115">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="5b27c-115">**Resource Management**</span></span>

<span data-ttu-id="5b27c-116">Следећи проблем је исправљен:</span><span class="sxs-lookup"><span data-stu-id="5b27c-116">The following issue has been fixed:</span></span>

- <span data-ttu-id="5b27c-117">Додат је Package Deployer кôд за прескакање увоза закрпе за услугу Universal Resource Scheduling ако закрпа више верзије већ постоји.</span><span class="sxs-lookup"><span data-stu-id="5b27c-117">Added package deployer code to skip the Universal Resource Scheduling patch import if a higher version patch already exists.</span></span>

<span data-ttu-id="5b27c-118">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="5b27c-118">**Project Management**</span></span>

<span data-ttu-id="5b27c-119">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="5b27c-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="5b27c-120">Исправљене су разлике у заокруживању и курсној листи које су доводиле до нетачних планираних трошкова у мрежи за праћење пројекта.</span><span class="sxs-lookup"><span data-stu-id="5b27c-120">Corrected rounding and exchange rate discrepancies resulting in incorrect planned cost in the project tracking grid.</span></span>
- <span data-ttu-id="5b27c-121">Подршка могућности приказивања две или више мрежа за реакције на обрасцу **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="5b27c-121">Support the ability to display two or more react grids on the **Project** form.</span></span>
- <span data-ttu-id="5b27c-122">Обезбеђена је валидација која решава проблем са могућношћу додељивања задатка након датума завршетка календара, што је доводило до неуспеле доделе ресурса.</span><span class="sxs-lookup"><span data-stu-id="5b27c-122">Provided validation to address the ability to assign a task past the calendar end date, which results in a failed resource assignment.</span></span>
- <span data-ttu-id="5b27c-123">Побољшано је руковање грешкама за решавање изузетка празне референце генерисане из следећег:</span><span class="sxs-lookup"><span data-stu-id="5b27c-123">Improved error handling to address Null Reference Exception generated from the following:</span></span>

    - <span data-ttu-id="5b27c-124">Додатна компонента **PreValidateProjectTeamMemberCreate**</span><span class="sxs-lookup"><span data-stu-id="5b27c-124">**PreValidateProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="5b27c-125">**PreValidateProjectTaskCreate** када се пројектни задатак креира без повезаног пројекта</span><span class="sxs-lookup"><span data-stu-id="5b27c-125">**PreValidateProjectTaskCreate** when a project task is created without an associated project</span></span>
    - <span data-ttu-id="5b27c-126">Додатна компонента **PreProjectTeamMemberCreate**</span><span class="sxs-lookup"><span data-stu-id="5b27c-126">**PreProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="5b27c-127">Додатна компонента **PostProjectTeamMemberDelete**</span><span class="sxs-lookup"><span data-stu-id="5b27c-127">**PostProjectTeamMemberDelete** plug-in</span></span>
    - <span data-ttu-id="5b27c-128">Додатна компонента **PreValidateProjectTaskDelete**</span><span class="sxs-lookup"><span data-stu-id="5b27c-128">**PreValidateProjectTaskDelete** plug-in</span></span>

<span data-ttu-id="5b27c-129">**Sales**</span><span class="sxs-lookup"><span data-stu-id="5b27c-129">**Sales**</span></span>

<span data-ttu-id="5b27c-130">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="5b27c-130">The following issues have been fixed:</span></span>

- <span data-ttu-id="5b27c-131">Побољшано је руковање грешкама за решавање проблема изузетка празне референце генерисане из **Копирање пројекта: Процене за HelperResource Management**.</span><span class="sxs-lookup"><span data-stu-id="5b27c-131">Improved error handling to address Null Reference Exceptions generated from **Copy Project: Estimates HelperResource Management**.</span></span>
- <span data-ttu-id="5b27c-132">**Није спремно за фактурисање** на страници **Неизвршавање наплате времена и материјала** не брише статус наплате.</span><span class="sxs-lookup"><span data-stu-id="5b27c-132">**Not ready to Invoice** on a **Time and Material Billing Backlog** doesn't clear the billing status.</span></span>
- <span data-ttu-id="5b27c-133">Исправљена су погрешно означена дугмад **Цене** на картицама **Цена улоге** и **Ставке каталога**.</span><span class="sxs-lookup"><span data-stu-id="5b27c-133">Corrected mislabeled **Prices** buttons on the **Role Price** and **Catalog Items** tab.</span></span>
