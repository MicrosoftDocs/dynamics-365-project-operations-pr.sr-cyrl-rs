---
title: Шта је ново или промењено у издању 30 исправке Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 30 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 1169ee13c42e982cb30a40d92df660f8933786a9
ms.sourcegitcommit: b4a05c7d5512d60abdb0d05bedd390e288e8adc9
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/02/2021
ms.locfileid: "5852891"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="540c4-103">Шта је ново или промењено у издању 30 исправке Project Service Automation верзије 3</span><span class="sxs-lookup"><span data-stu-id="540c4-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="540c4-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="540c4-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="540c4-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="540c4-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="540c4-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="540c4-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="540c4-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="540c4-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="540c4-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="540c4-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="540c4-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 30.</span><span class="sxs-lookup"><span data-stu-id="540c4-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="540c4-110">Број израде ове верзије је V3.10.51.61 и углавном је доступна путем самосталног ажурирања у априлу 2021. године.</span><span class="sxs-lookup"><span data-stu-id="540c4-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="540c4-111">Издање исправке 30</span><span class="sxs-lookup"><span data-stu-id="540c4-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="540c4-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="540c4-112">Bug fixes</span></span>

<span data-ttu-id="540c4-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="540c4-113">**Time and Expense**</span></span>

<span data-ttu-id="540c4-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="540c4-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="540c4-115">Долази до грешке када креирате и сачувате ставку времена на страници **Брзо креирање** ако је поље **Улога** уклоњено.</span><span class="sxs-lookup"><span data-stu-id="540c4-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="540c4-116">Филтер за ставку времена примењује погрешан оператор филтера.</span><span class="sxs-lookup"><span data-stu-id="540c4-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="540c4-117">Копирани временски листови се не приказују аутоматски када изаберете **Копирање седмице** на контроли ставке времена.</span><span class="sxs-lookup"><span data-stu-id="540c4-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="540c4-118">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="540c4-118">**Resource Management**</span></span>

<span data-ttu-id="540c4-119">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="540c4-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="540c4-120">Када продужите резервацију, статус резервације додељен фиксној резервацији је нетачан.</span><span class="sxs-lookup"><span data-stu-id="540c4-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="540c4-121">Продужењем резервације поштује се статус резервације дефинисан као **Додељено** у метаподацима подешавања резервације.</span><span class="sxs-lookup"><span data-stu-id="540c4-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="540c4-122">Када није наведен важећи статус резервације, порука о грешци није правилно локализована.</span><span class="sxs-lookup"><span data-stu-id="540c4-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="540c4-123">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="540c4-123">**Project Management**</span></span>

<span data-ttu-id="540c4-124">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="540c4-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="540c4-125">Пројекти се не могу креирати у једној валути, а да укључују повезане задатке у другој валути.</span><span class="sxs-lookup"><span data-stu-id="540c4-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="540c4-126">**Продаја**</span><span class="sxs-lookup"><span data-stu-id="540c4-126">**Sales**</span></span>

<span data-ttu-id="540c4-127">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="540c4-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="540c4-128">Када се копира ценовник, цене се не ажурирају.</span><span class="sxs-lookup"><span data-stu-id="540c4-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="540c4-129">Затварање понуде као остварене не успева када детаљ цене има вредност за порекло.</span><span class="sxs-lookup"><span data-stu-id="540c4-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="540c4-130">На ентитету **Пројектни задатак**, **Процењена цена** се преименује у **Планирана цена (основна)**.</span><span class="sxs-lookup"><span data-stu-id="540c4-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="540c4-131">Изузетак нулте референце се генерише када се фактуре креирају или избришу.</span><span class="sxs-lookup"><span data-stu-id="540c4-131">A null reference exception is generated when invoices are created or deleted.</span></span>
