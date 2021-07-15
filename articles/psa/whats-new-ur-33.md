---
title: Шта је ново или промењено у издању 33 исправке услуге Project Service Automation верзије 3
description: У овој теми наведене су функције и исправке које су доступне у издању 33 исправке услуге Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334596"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="a387c-103">Шта је ново или промењено у издању 33 исправке услуге Project Service Automation верзије 3</span><span class="sxs-lookup"><span data-stu-id="a387c-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a387c-104">Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a387c-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="a387c-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="a387c-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a387c-106">Компатибилна је са системом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="a387c-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a387c-107">Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку.</span><span class="sxs-lookup"><span data-stu-id="a387c-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="a387c-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a387c-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a387c-109">У овој теми наведене су функције које су нове или промењене у издању 33 услуге Project Service Automation верзије 3.</span><span class="sxs-lookup"><span data-stu-id="a387c-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="a387c-110">Ова верзија има број верзије 3.10.54.98 и опште је доступна путем самосталног ажурирања у јулу 2021.</span><span class="sxs-lookup"><span data-stu-id="a387c-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="a387c-111">Издање исправке 33</span><span class="sxs-lookup"><span data-stu-id="a387c-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a387c-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="a387c-112">Bug fixes</span></span>

<span data-ttu-id="a387c-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="a387c-113">**Time and Expense**</span></span>

<span data-ttu-id="a387c-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="a387c-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="a387c-115">Два закључана поља, **msdyn_description** и **msdyn_externaldescription** могу се уређивати након прослеђивања.</span><span class="sxs-lookup"><span data-stu-id="a387c-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="a387c-116">Порука о грешци се јавља ако се креира трошак који није повезан са пројектом.</span><span class="sxs-lookup"><span data-stu-id="a387c-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="a387c-117">Када се креира ставка времена, улога ресурса је подразумевано неактивна.</span><span class="sxs-lookup"><span data-stu-id="a387c-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="a387c-118">Ставке у главној књизи повезане са опозваним и избрисаним трошковима се не бришу.</span><span class="sxs-lookup"><span data-stu-id="a387c-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="a387c-119">На **обрасцу за брзо креирање ставке времена**, ажурирајте приказ **Листа пројектних задатака** да бисте подразумевано приказани датум променили у датум почетка задатка.</span><span class="sxs-lookup"><span data-stu-id="a387c-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="a387c-120">Када креирате унос времена са картице **Повезано** ресурса који може да се резервише, ставка времена се погрешно креира за пријављеног корисника уместо за надређени ресурс који може да се резервише.</span><span class="sxs-lookup"><span data-stu-id="a387c-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="a387c-121">Нова поља се додају у дијалог **Групно одобравање MDD**.</span><span class="sxs-lookup"><span data-stu-id="a387c-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="a387c-122">**Планирање пројекта**</span><span class="sxs-lookup"><span data-stu-id="a387c-122">**Project planning**</span></span>

<span data-ttu-id="a387c-123">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="a387c-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="a387c-124">Споре перформансе креирања пројеката када се предлошци радног времена пројекта примењују са сложеним календарима.</span><span class="sxs-lookup"><span data-stu-id="a387c-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="a387c-125">Када је датум почетка већи од датума завршетка, на предлошку пројекта копирања приказује се грешка због разлика у временској компоненти сваког поља.</span><span class="sxs-lookup"><span data-stu-id="a387c-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="a387c-126">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="a387c-126">**Resource management**</span></span>

<span data-ttu-id="a387c-127">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="a387c-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="a387c-128">У упиту о укупној искоришћености ресурса користи се нетачан параметар, а XML доводи до нетачних резултата филтера на мрежи **Укупна искоришћеност ресурса**.</span><span class="sxs-lookup"><span data-stu-id="a387c-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="a387c-129">Потврда **Продужетак резервација** приказује нетачан датум завршетка за резервације.</span><span class="sxs-lookup"><span data-stu-id="a387c-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="a387c-130">**Продаја**</span><span class="sxs-lookup"><span data-stu-id="a387c-130">**Sales**</span></span>

<span data-ttu-id="a387c-131">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="a387c-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="a387c-132">Порука о грешци се јавља ако се креира цена категорије са вредностима које недостају.</span><span class="sxs-lookup"><span data-stu-id="a387c-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="a387c-133">Јавља се порука о грешци ако се креира контролна тачка ставке уговора без ставке поруџбине.</span><span class="sxs-lookup"><span data-stu-id="a387c-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
