---
title: Шта је ново или промењено у издању 24 исправке Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 24 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
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
ms.openlocfilehash: 6c8348e65307f63a251f97bf1ea17578e7026da8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083924"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="6bfdb-103">Project Service Automation издање 24 исправке верзије 3</span><span class="sxs-lookup"><span data-stu-id="6bfdb-103">Project Service Automation Update Release 24, V3</span></span>

<span data-ttu-id="6bfdb-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="6bfdb-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="6bfdb-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="6bfdb-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="6bfdb-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="6bfdb-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="6bfdb-109">У овој теми дате су функције и исправке које су нове или промењене у решењу Project Service Automation у верзији 3, издање исправке 24.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="6bfdb-110">Ова верзија има број V3.10.42.43 и опште је доступна путем самосталне исправке објављене октобра 2020.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="6bfdb-111">Издање исправке 24</span><span class="sxs-lookup"><span data-stu-id="6bfdb-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="6bfdb-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="6bfdb-112">Bug fixes</span></span>

<span data-ttu-id="6bfdb-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="6bfdb-113">**Sales**</span></span>

<span data-ttu-id="6bfdb-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="6bfdb-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="6bfdb-115">Проблем приликом постављања подразумеваног ценовника производа.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="6bfdb-116">Перформансе остварене понуде су споре због уграђеног ценовника и копија записа цена улога.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="6bfdb-117">**Уговор о пројекту / чвориште за продају** > **Ставка предмета производа / количина ставке поруџбине** аутоматски се заокружује на најближи цели број.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="6bfdb-118">Подигните системске привилегије приликом читања ценовника.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="6bfdb-119">Копирајте поља адресе клијента **address1_freighttermscode** и **address1_shippingmethodcode** за понуду/поруџбину.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="6bfdb-120">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="6bfdb-120">**Time and Expense**</span></span>

<span data-ttu-id="6bfdb-121">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="6bfdb-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="6bfdb-122">**Мрежа ставке времена** не подржава временско понашање **Само датум**.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="6bfdb-123">**Ставка времена** се не освежава аутоматски.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="6bfdb-124">Потребно је ручно освежавање.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-124">A manual refresh is required.</span></span>
- <span data-ttu-id="6bfdb-125">Није могуће увести ставке времена из задатка када постоји пауза (0 сати) у доделама ресурса.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="6bfdb-126">Када креирате ставку времена, подесите да почетак буде исти као **msdyn_date**.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="6bfdb-127">Поново омогућите групно уређивање за унос времена.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="6bfdb-128">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="6bfdb-128">**Resource Management**</span></span>

<span data-ttu-id="6bfdb-129">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="6bfdb-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="6bfdb-130">Покушај ажурирања статуса једнодневне резервације без захтева довешће до изузетка „null-ref“.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="6bfdb-131">Грешка при учитавању **приказа усаглашености**.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="6bfdb-132">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="6bfdb-132">**Project Management**</span></span>

<span data-ttu-id="6bfdb-133">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="6bfdb-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="6bfdb-134">У **Распореду пројекта** , при промени из **Ручно** у **Аутоматски** , аутоматско чување се не довршава.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-134">In the **Project Schedule** , when changing from **Manual** to **Auto** , auto save is not completing.</span></span>
- <span data-ttu-id="6bfdb-135">Трошкови трошкова не би требало да се рачунају према одступању у односу на **Мрежа за праћење пројеката**.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="6bfdb-136">Недоследно понашање за колоне **Ознака процене** током учитавања у односу на промену типа **Временска фаза**.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="6bfdb-137">Стварни трошкови пројекта можда неће одражавати укупне износе из **стварних вредности**.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="6bfdb-138">**Предвиђени датум завршетка** на картици **Резиме** се не подудара са **САП распоредом**.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="6bfdb-139">**Ажурирање стварних сати** при извлачењу не ради исправно.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="6bfdb-140">Менаџер пројекта изван основне **пословне јединице** не може да креира пројекат.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="6bfdb-141">Промене у задатку или категорији **процена трошкова** не остају сачуване.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="6bfdb-142">**Копија уговора** копира распореде фактура и статус покретања.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="6bfdb-143">Дугме **Освежи стварне вредности** погрешно израчунава резимиране задатке.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="6bfdb-144">Додатак за Microsoft Project: Исправљена је грешка референце „null“ ако било који члан тима има празну јединицу за обезбеђивање ресурса.</span><span class="sxs-lookup"><span data-stu-id="6bfdb-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>

