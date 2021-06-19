---
title: Шта је ново или промењено у издању 32 исправке услуге Project Service Automation верзије 3
description: У овој теми наведене су функције и исправке које су доступне у издању 32 исправке услуге Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 11bf451ef4f24e2301ffde4f86a556a8a4fe30b0
ms.sourcegitcommit: 886102894244887d72e5a6213071e8d8a52c9d48
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/01/2021
ms.locfileid: "6129684"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a><span data-ttu-id="2033b-103">Шта је ново или промењено у издању 32 исправке услуге Project Service Automation верзије 3</span><span class="sxs-lookup"><span data-stu-id="2033b-103">What's new or changed in Project Service Automation Update Release 32, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2033b-104">Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="2033b-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="2033b-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="2033b-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="2033b-106">Компатибилна је са системом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="2033b-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="2033b-107">Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку.</span><span class="sxs-lookup"><span data-stu-id="2033b-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="2033b-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="2033b-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="2033b-109">У овој теми наведене су функције које су нове или промењене у издању 32 исправке услуге Project Service Automation верзије 3.</span><span class="sxs-lookup"><span data-stu-id="2033b-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 32.</span></span> <span data-ttu-id="2033b-110">Ова верзија има број верзије 3.10.53.108 и опште је доступна путем самосталног ажурирања у јуну 2021.</span><span class="sxs-lookup"><span data-stu-id="2033b-110">This version has a build number of V3.10.53.108 and is generally available through a self-update in June 2021.</span></span>

## <a name="update-release-32"></a><span data-ttu-id="2033b-111">Издање исправке 32</span><span class="sxs-lookup"><span data-stu-id="2033b-111">Update Release 32</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="2033b-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="2033b-112">Bug fixes</span></span>

#### <a name="general"></a><span data-ttu-id="2033b-113">Опште</span><span class="sxs-lookup"><span data-stu-id="2033b-113">General</span></span>

- <span data-ttu-id="2033b-114">Када главна надоградња не успе, треба блокирати само главне улазне тачке апликације како би се осигурало да дељени ентитети и даље буду доступни.</span><span class="sxs-lookup"><span data-stu-id="2033b-114">When a major upgrade fails, only the main application entry points should be blocked, to ensure that shared entities are still accessible.</span></span>

#### <a name="time-and-expense"></a><span data-ttu-id="2033b-115">Време и трошак</span><span class="sxs-lookup"><span data-stu-id="2033b-115">Time and Expense</span></span>

<span data-ttu-id="2033b-116">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="2033b-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="2033b-117">**TimeEntriesImportFromResourceAssignment** не одржава времена почетка и завршетка исечака контуре доделе ресурса.</span><span class="sxs-lookup"><span data-stu-id="2033b-117">**TimeEntriesImportFromResourceAssignment** doesn't maintain the start and end times of the resource assignment contour slice.</span></span>
- <span data-ttu-id="2033b-118">Када изаберете **Отвори ставку** на мрежи **Ставка времена**, можда ћете бити спречени да изаберете друге обрасце.</span><span class="sxs-lookup"><span data-stu-id="2033b-118">When you select **Open Entry** on the **Time Entry** grid, you might be prevented from selecting other forms.</span></span>
- <span data-ttu-id="2033b-119">Док увозите задатке у ставке времена, упит клијентског кода може да генерише дугу URL адресу која не успева у упиту.</span><span class="sxs-lookup"><span data-stu-id="2033b-119">While you import assignments to time entries, the client code query could generate a long URL that fails the query.</span></span>
- <span data-ttu-id="2033b-120">У мрежи **Ставка времена**, када се вредност избрише из ћелије, фокус не остаје у мрежи.</span><span class="sxs-lookup"><span data-stu-id="2033b-120">In the **Time Entry** grid, after a value is deleted from a cell, the focus doesn't remain in the grid.</span></span>
- <span data-ttu-id="2033b-121">Дугме **Одбаци** је уклоњено из приказа **Одобрења обраде** за модерна одобрења.</span><span class="sxs-lookup"><span data-stu-id="2033b-121">The **Reject** button has been removed from the **Processing approvals** view for modern approvals.</span></span>
- <span data-ttu-id="2033b-122">На стабилност и перформансе групног одобравања ставке времена утичу застоји и неуспех у одговарајућем руковању прилагођавањима која су повезана са ентитетом **Ставка времена**.</span><span class="sxs-lookup"><span data-stu-id="2033b-122">The stability and performance of time entry bulk approval are affected by deadlocks and a failure to appropriately handle customizations that are related to the **Time Entry** entity.</span></span>

#### <a name="project-planning"></a><span data-ttu-id="2033b-123">Планирање пројекта</span><span class="sxs-lookup"><span data-stu-id="2033b-123">Project Planning</span></span>

- <span data-ttu-id="2033b-124">Изузетак нулте референце се генерише када ажурирате пројекат који има нулту вредност у пољу **Јединица уговарања**.</span><span class="sxs-lookup"><span data-stu-id="2033b-124">A null reference exception is generated when you update a project that has a null value in the **Contracting Unit** field.</span></span>
- <span data-ttu-id="2033b-125">**Освежи укупне вредности пројеката** погрешно израчунава преостали трошак и преосталу продају у пројекту.</span><span class="sxs-lookup"><span data-stu-id="2033b-125">**Refresh Project Totals** incorrectly calculates the remaining cost and remaining sales on a project.</span></span>
- <span data-ttu-id="2033b-126">Прекомерни прорачуни цена утичу на перформансе повезане са ажурирањима на контурама доделе ресурса.</span><span class="sxs-lookup"><span data-stu-id="2033b-126">Redundant pricing calculations affect performance that is related to updates on resource assignment contours.</span></span>

#### <a name="resource-management"></a><span data-ttu-id="2033b-127">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="2033b-127">Resource Management</span></span>

<span data-ttu-id="2033b-128">Следећи проблем је исправљен:</span><span class="sxs-lookup"><span data-stu-id="2033b-128">The following issue has been fixed:</span></span>

- <span data-ttu-id="2033b-129">Када је капацитет календара ресурса који може да се резервише већи од 1, Project Service Automation погрешно препознаје капацитет као 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="2033b-129">When a bookable resource's calendar capacity is more than 1, Project Service Automation incorrectly recognizes the capacity as 0 (zero).</span></span> <span data-ttu-id="2033b-130">Стога се у приказу распореда јавља бесконачна петља.</span><span class="sxs-lookup"><span data-stu-id="2033b-130">Therefore, an infinite loop occurs in the schedule view.</span></span>

#### <a name="sales"></a><span data-ttu-id="2033b-131">Продаја</span><span class="sxs-lookup"><span data-stu-id="2033b-131">Sales</span></span>

<span data-ttu-id="2033b-132">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="2033b-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="2033b-133">Када се креира ставка у главној књизи која има прилагођени тип трансакције, јавља се следећи изузетак нулте референце: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span><span class="sxs-lookup"><span data-stu-id="2033b-133">When a journal line is created that has a custom transaction type, the following null reference exception occurs: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span></span>
- <span data-ttu-id="2033b-134">Улоге и категорије које су деактивиране пре копирања понуде не би требало додавати улогама које се наплаћују и категоријама новокопиране понуде.</span><span class="sxs-lookup"><span data-stu-id="2033b-134">Roles and categories that are inactivated before a quotation is copied should not be added to chargeable roles and categories of the newly copied quotation.</span></span>
- <span data-ttu-id="2033b-135">Датум документа и датум обрачуна нису усклађени са датумом почетка који је наведен у детаљима ставке фактуре која се креира директно на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="2033b-135">The document date and accounting date aren't aligned with the start date that is provided on an invoice line detail that is created directly on a draft invoice.</span></span>
- <span data-ttu-id="2033b-136">Изузеци од нулте референце се генеришу у сценаријима који су повезани са деактивацијом улога и категорија пре копирања понуде.</span><span class="sxs-lookup"><span data-stu-id="2033b-136">Null reference exceptions are generated in scenarios that are related to inactivation of roles and categories before a quotation is copied.</span></span>
- <span data-ttu-id="2033b-137">Радња **Ажурирање цена** на страници **Пројекти** не ажурира процене трошкова и процене материјала.</span><span class="sxs-lookup"><span data-stu-id="2033b-137">The **Update Prices** action on the **Projects** page doesn't update expense estimates and material estimates.</span></span>
