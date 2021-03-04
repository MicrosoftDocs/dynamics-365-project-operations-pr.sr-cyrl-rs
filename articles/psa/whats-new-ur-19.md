---
title: Шта је ново или промењено у Project Service Automation издању исправке 19 у верзији 3
description: У овој теми дате су функције и исправке које су доступне у Project Service Automation издању исправке 19 у верзији 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: 8a73a6acd4ce4c9559cdf4591ede735a613f4d52
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143669"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="6bf8a-103">Project Service Automation издање исправке 19, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="6bf8a-103">Project Service Automation Update Release 19, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="6bf8a-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="6bf8a-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="6bf8a-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="6bf8a-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="6bf8a-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="6bf8a-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="6bf8a-109">У овој теми дате су функције и исправке које су нове или су промењене у решењу PSA у верзији 3, издање исправке 19.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="6bf8a-110">Број израде ове верзије је V3.10.30.41 и углавном је доступна путем самосталног ажурирања у мају 2020. године.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="6bf8a-111">Издање исправке 19</span><span class="sxs-lookup"><span data-stu-id="6bf8a-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="6bf8a-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="6bf8a-112">Bug fixes</span></span>

<span data-ttu-id="6bf8a-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="6bf8a-113">**Time and Expense**</span></span>

<span data-ttu-id="6bf8a-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="6bf8a-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="6bf8a-115">Грешке настале приликом увоза у ставки времена се не појављују исправно.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="6bf8a-116">Мрежа ставке времена не подржава понашање поља **Само датум**.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="6bf8a-117">Ресурси пројекта не могу да креирају трошак са пројектом.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="6bf8a-118">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="6bf8a-118">**Project Management**</span></span>

<span data-ttu-id="6bf8a-119">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="6bf8a-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="6bf8a-120">Другостепени подређени задатак узрокује погрешну процену залагања током израчунавања завршетка (EAC).</span><span class="sxs-lookup"><span data-stu-id="6bf8a-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="6bf8a-121">**Sales**</span><span class="sxs-lookup"><span data-stu-id="6bf8a-121">**Sales**</span></span>

<span data-ttu-id="6bf8a-122">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="6bf8a-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="6bf8a-123">Радња **Поновно израчунавање** не функционише са детаљима о трошковима предмета уговора или детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="6bf8a-124">**Ажурирање цена** недостаје за процене трошкова.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="6bf8a-125">Клијенти не могу да изаберу прилагођене разлоге статуса уговора са странице **Пројектни уговор**.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="6bf8a-126">Клијенти имају смањене перформансе када креирају прилагођени ценовник из понуде.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="6bf8a-127">Клијенти доживљавају недоследност са подразумеваним вредностима за **јединицу** на страницама **Детаљи ставке понуде** и **Детаљи предмета уговора**.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="6bf8a-128">Додавање ставки из категорије ненаплативих трансакција у наплативи предмет уговора неће се поштовати тип обрачуна **Није наплативо** категорије трансакције.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="6bf8a-129">Клијенти не могу да користе новододате улоге и категорију на претходно креираним уговорима.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="6bf8a-130">Клијенти имају смањене перформансе Непотребног умањења у PreValidateProjectTeamMemberUpdate.cs</span><span class="sxs-lookup"><span data-stu-id="6bf8a-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="6bf8a-131">Улоге које су подешене као ненаплативе на листи **Категорије ресурса** требају бити додате на картицу **Наплативе улоге** као **Ненаплативе** на предмету уговора за пројекат.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="6bf8a-132">Клијенти могу имати смањене перформансе приликом креирања пројекта јер **GetBookableResourceIdFromUser** прибавља све колоне ресурса који могу да се резервишу уместо само примарни ID.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="6bf8a-133">Ентитету **Тип трансакције** недостаје додатна компонента за претходну валидацију да спречи кориснике да уносе **Јединице** и **UnitGroups** које нису важеће за типове трансакција.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="6bf8a-134">Корак **Уклони** не ради за увоз ставке времена.</span><span class="sxs-lookup"><span data-stu-id="6bf8a-134">The **Remove** step does not work for time entry import.</span></span>
