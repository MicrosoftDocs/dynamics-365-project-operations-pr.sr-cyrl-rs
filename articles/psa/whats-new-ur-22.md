---
title: Шта је ново или промењено у издању 22 исправке за Project Service Automation у верзији 3
description: У овој теми дате су функције и исправке које су доступне у издању 22 исправке за Project Service Automation у верзији 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
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
ms.openlocfilehash: 389897c2604974a0bf7f221758dd03e1748ffeb5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280596"
---
# <a name="project-service-automation-update-release-22-v3"></a><span data-ttu-id="29827-103">Project Service Automation издање исправке 22, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="29827-103">Project Service Automation Update Release 22, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="29827-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="29827-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="29827-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="29827-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="29827-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="29827-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="29827-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="29827-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="29827-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="29827-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="29827-109">У овој теми дате су функције које су нове или су промењене у издању 22 исправке за Project Service Automation у верзији 3.</span><span class="sxs-lookup"><span data-stu-id="29827-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 22.</span></span> <span data-ttu-id="29827-110">Број израде ове верзије је V 3.10.33.48 и углавном је доступна путем самосталног ажурирања у јуну 2020. године.</span><span class="sxs-lookup"><span data-stu-id="29827-110">This version has a build number of V 3.10.33.48 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-22"></a><span data-ttu-id="29827-111">Издање исправке 22</span><span class="sxs-lookup"><span data-stu-id="29827-111">Update Release 22</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="29827-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="29827-112">Bug fixes</span></span>



<span data-ttu-id="29827-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="29827-113">**Time and Expense**</span></span>

<span data-ttu-id="29827-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="29827-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="29827-115">**Ставке времена** се не додају аутоматски у распоред ставки времена након увоза.</span><span class="sxs-lookup"><span data-stu-id="29827-115">**Time entries** are not automatically added in the Time entries schedule after import.</span></span>
- <span data-ttu-id="29827-116">Алатка за бирање датума на мрежи у опцији **Ставке времена** не препознаје регионална подешавања корисника.</span><span class="sxs-lookup"><span data-stu-id="29827-116">The **Time Entry** grid date picker does not recognize a user's regional settings.</span></span>

<span data-ttu-id="29827-117">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="29827-117">**Resource Management**</span></span>

<span data-ttu-id="29827-118">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="29827-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="29827-119">У ручном режиму, промене у скицама **Додела ресурса** се не препознају при генерисању ставке **Захтеви за ресурсом**.</span><span class="sxs-lookup"><span data-stu-id="29827-119">In manual mode, changes to **Resource Assignment** contours are not recognized when generating **Resource Requirements**.</span></span>
- <span data-ttu-id="29827-120">**Захтеви за ресурсом** не подржавају статусе прилагођених захтева.</span><span class="sxs-lookup"><span data-stu-id="29827-120">**Resource Requests** do not support custom request statuses.</span></span>

<span data-ttu-id="29827-121">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="29827-121">**Project Management**</span></span>

<span data-ttu-id="29827-122">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="29827-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="29827-123">Двоструким кликом на EstimateGridControl неће се правилно рашчланити бројеви у холандском формату.</span><span class="sxs-lookup"><span data-stu-id="29827-123">Using double-click on EstimateGridControl will not correctly parse Dutch format numbers.</span></span>
- <span data-ttu-id="29827-124">Додељени сати се не ажурирају исправно када се доделе мењају помоћу програмског додатка за Microsoft Project десктоп клијент.</span><span class="sxs-lookup"><span data-stu-id="29827-124">Assigned hours do not update correctly when assignments are changed using the Microsoft Project desktop client add-in.</span></span>
- <span data-ttu-id="29827-125">Мреже за праћење и процене пројеката приказују погрешну шифру валуте продаје када је валута уговора другачија од валуте купца и ако је организација конфигурисана за приказивање шифара валута уместо симбола валуте.</span><span class="sxs-lookup"><span data-stu-id="29827-125">Project Tracking and Estimates grids display incorrect sales currency code when contract currency is different than customer currency and organization is configured to display currency codes instead of currency symbols.</span></span>
- <span data-ttu-id="29827-126">Датум завршетка члана тима додаће један дан ако је распоред радног времена 24 сата дневно.</span><span class="sxs-lookup"><span data-stu-id="29827-126">A Team member's finish date will add one day if the work hour schedule is 24-hours per day.</span></span>
- <span data-ttu-id="29827-127">У Распореду пројеката, додавање Категорије трансакције задатку не покреће аутоматско спремање.</span><span class="sxs-lookup"><span data-stu-id="29827-127">On the Project Schedule, adding a Transaction Category to a task does not trigger auto save.</span></span>
- <span data-ttu-id="29827-128">Следећа грешка се приказује приликом додавања члана тима у предложак пројекта: „Захтеви за ресурсима не могу бити повезани са предлошцима пројекта“.</span><span class="sxs-lookup"><span data-stu-id="29827-128">The following error is displayed when adding a team member to the Project Template: "Resource requirements cannot be associated with project templates".</span></span> 
- <span data-ttu-id="29827-129">Скрипта правила траке „msdyn.Approval.CanApproveOrReject“ приказује грешку временског ограничења.</span><span class="sxs-lookup"><span data-stu-id="29827-129">Ribbon rule script "msdyn.Approval.CanApproveOrReject" displays a timeout error.</span></span>

<span data-ttu-id="29827-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="29827-130">**Sales**</span></span>

<span data-ttu-id="29827-131">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="29827-131">The following issues have been fixed:</span></span>

- <span data-ttu-id="29827-132">Порука о грешци приликом провере није приказана када је у претраживању ценовника на обрасцу/ентитету „Нови ценовник понуде за пројекат“ изабран Ценовник трошкова.</span><span class="sxs-lookup"><span data-stu-id="29827-132">Validation error message not displayed when a Cost Price List is selected in Price List lookup on 'New Quote Project Price List' form/entity.</span></span>
- <span data-ttu-id="29827-133">Затварање добијене понуде не прелази на креирани уговор ако је BPF у прилогу понуде у завршној фази.</span><span class="sxs-lookup"><span data-stu-id="29827-133">Closing the quote as won does not navigate to the created contract if a BPF attached to the quote is in the final stage.</span></span>
- <span data-ttu-id="29827-134">Сторнирање **Ненаплаћена продаја** је повезано са првобитним трошком када се опозове унос времена.</span><span class="sxs-lookup"><span data-stu-id="29827-134">Reversing **Unbilled Sales** is linked to original cost when a time entry is recalled.</span></span>
- <span data-ttu-id="29827-135">Након одабира дугмета **Потврди**, статус фактуре се не мења у **Потврђено**, осим ако се фактура освежи.</span><span class="sxs-lookup"><span data-stu-id="29827-135">After selecting the **Confirm** button, the invoice status doesn't change to **Confirmed** unless the invoice is refreshed.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]