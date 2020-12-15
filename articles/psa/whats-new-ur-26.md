---
title: Шта је ново или промењено у издању 26 исправке Project Service Automation верзије 3
ms.openlocfilehash: 849e7288ee91d3e9360c0b03f6b8b37ff29338e7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643281"
---
<a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="ee43d-102">Project Service Automation издање исправке 26, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="ee43d-102">Project Service Automation Update Release 26, V3</span></span>
================================================

<span data-ttu-id="ee43d-103">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="ee43d-103">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="ee43d-104">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="ee43d-104">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="ee43d-105">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="ee43d-105">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="ee43d-106">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="ee43d-106">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="ee43d-107">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="ee43d-107">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="ee43d-108">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 26.</span><span class="sxs-lookup"><span data-stu-id="ee43d-108">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="ee43d-109">Ова верзија има број верзије V3.10.44.59 и генерално је доступна путем самосталног ажурирања у децембру 2020.</span><span class="sxs-lookup"><span data-stu-id="ee43d-109">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

<a name="update-release-26"></a><span data-ttu-id="ee43d-110">Издање исправке 26</span><span class="sxs-lookup"><span data-stu-id="ee43d-110">Update Release 26</span></span>
-----------------

### <a name="bug-fixes"></a><span data-ttu-id="ee43d-111">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="ee43d-111">Bug fixes</span></span>

<span data-ttu-id="ee43d-112">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="ee43d-112">**Time and Expense**</span></span>

<span data-ttu-id="ee43d-113">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="ee43d-113">The following issues have been fixed:</span></span>

-   <span data-ttu-id="ee43d-114">Корисници могу да промене задатак на ставци времена која је одобрена/поднета.</span><span class="sxs-lookup"><span data-stu-id="ee43d-114">Users are able to change the task on a time entry that has been approved/submitted.</span></span>

-   <span data-ttu-id="ee43d-115">Грешка „Референца објекта није подешена“ приликом чувања ставке времена.</span><span class="sxs-lookup"><span data-stu-id="ee43d-115">"Object Reference Not Set" error when saving time entry.</span></span>

-   <span data-ttu-id="ee43d-116">Увоз ставке времена из додељивања ресурса креира ставке времена са нетачним вредностима датума и времена.</span><span class="sxs-lookup"><span data-stu-id="ee43d-116">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>

-   <span data-ttu-id="ee43d-117">Када су инсталиране апликације Project Service Automation и Field Service, дугме **Ново** се приказује два пута на командној траци за ставке времена у апликацији Field Service.</span><span class="sxs-lookup"><span data-stu-id="ee43d-117">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>

-   <span data-ttu-id="ee43d-118">Ћелије **Дозволи ажурирања јединице** и **групе јединица** сада раде у мрежи **Процене трошкова**.</span><span class="sxs-lookup"><span data-stu-id="ee43d-118">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>

-   <span data-ttu-id="ee43d-119">Образац **Ажурирај уређивање ставке времена** укључује **Временску осу**.</span><span class="sxs-lookup"><span data-stu-id="ee43d-119">**Update Time Entry Edit** form includes **Timeline**.</span></span>

-   <span data-ttu-id="ee43d-120">Одобрење времена за ставке времена које се не односе на пројекат блокирају систем приликом претраге за улогу одобраваоца пројекта.</span><span class="sxs-lookup"><span data-stu-id="ee43d-120">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="ee43d-121">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="ee43d-121">**Resource Management**</span></span>

<span data-ttu-id="ee43d-122">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="ee43d-122">The following issues have been fixed:</span></span>

-   <span data-ttu-id="ee43d-123">Додата је валидација у додатној компоненти **PostProjectCreate** за проверу примарног захтева пре његовог креирања.</span><span class="sxs-lookup"><span data-stu-id="ee43d-123">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>

-   <span data-ttu-id="ee43d-124">Образац за брзо креирање **Члан пројектног тима** даје изузетак празне референце ако се поља уклоне из обрасца.</span><span class="sxs-lookup"><span data-stu-id="ee43d-124">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>

-   <span data-ttu-id="ee43d-125">Генерирање захтева за 12 сати током 1 године неће успети.</span><span class="sxs-lookup"><span data-stu-id="ee43d-125">Generate requirements for 12 hours over 1 year will fail.</span></span>

-   <span data-ttu-id="ee43d-126">Побољшана порука о грешци за изузетак празне референце током креирања захтева за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="ee43d-126">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="ee43d-127">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="ee43d-127">**Project Management**</span></span>

<span data-ttu-id="ee43d-128">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="ee43d-128">The following issues have been fixed:</span></span>

-   <span data-ttu-id="ee43d-129">Побољшана валидација за одговор на изузетак празне референце генерисане у додатној компоненти **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="ee43d-129">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>

-   <span data-ttu-id="ee43d-130">Пројекти објављени у програмском додатку за рачунаре услуге Microsoft Project бришу нераспоређене задатке.</span><span class="sxs-lookup"><span data-stu-id="ee43d-130">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>

-   <span data-ttu-id="ee43d-131">Додата је нова валидација када референца пројекта задатка није важећа због изузетка празне референце у додатној компоненти **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="ee43d-131">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>

-   <span data-ttu-id="ee43d-132">Мрежа члана тима не приказује различите задатке у запису члана тима.</span><span class="sxs-lookup"><span data-stu-id="ee43d-132">Team Member grid does not show distinct assignments on the team member record.</span></span>

-   <span data-ttu-id="ee43d-133">Додате су нове поруке за проверу ваљаности и поруке грешке због изузетка празне референце у додатној компоненти **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="ee43d-133">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="ee43d-134">**Sales**</span><span class="sxs-lookup"><span data-stu-id="ee43d-134">**Sales**</span></span>

<span data-ttu-id="ee43d-135">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="ee43d-135">The following issues have been fixed:</span></span>

-   <span data-ttu-id="ee43d-136">Приликом избора ставке засноване на пројекту у понуду или уговору, дугме **Предлог** би требало да буде видљиво само при одабиру линије засноване на производу повезане са постојећим производом.</span><span class="sxs-lookup"><span data-stu-id="ee43d-136">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>

-   <span data-ttu-id="ee43d-137">Поделите привилегију **Create_Product** из привилегије **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="ee43d-137">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>

-   <span data-ttu-id="ee43d-138">Брисање ставке у фактору доводи до неуспеле празне референце на **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="ee43d-138">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
