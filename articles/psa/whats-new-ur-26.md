---
title: Шта је ново или промењено у издању 26 исправке Project Service Automation верзије 3
description: У овој теми су наведене функције и исправке које су доступне у издању исправке 26 за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: 669b3ca4601bdac483db4e1d7f55a8bf5b3d9661
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948842"
---
# <a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="d2061-103">Project Service Automation издање исправке 26, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="d2061-103">Project Service Automation Update Release 26, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="d2061-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="d2061-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="d2061-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="d2061-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="d2061-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="d2061-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="d2061-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="d2061-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="d2061-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="d2061-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="d2061-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 26.</span><span class="sxs-lookup"><span data-stu-id="d2061-109">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="d2061-110">Ова верзија има број верзије V3.10.44.59 и генерално је доступна путем самосталног ажурирања у децембру 2020.</span><span class="sxs-lookup"><span data-stu-id="d2061-110">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

## <a name="update-release-26"></a><span data-ttu-id="d2061-111">Издање исправке 26</span><span class="sxs-lookup"><span data-stu-id="d2061-111">Update Release 26</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="d2061-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="d2061-112">Bug fixes</span></span>

<span data-ttu-id="d2061-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="d2061-113">**Time and Expense**</span></span>

<span data-ttu-id="d2061-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="d2061-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="d2061-115">Корисници могу да промене задатак на ставци времена која је одобрена/поднета.</span><span class="sxs-lookup"><span data-stu-id="d2061-115">Users are able to change the task on a time entry that has been approved/submitted.</span></span>
- <span data-ttu-id="d2061-116">Грешка „Референца објекта није подешена“ приликом чувања ставке времена.</span><span class="sxs-lookup"><span data-stu-id="d2061-116">"Object Reference Not Set" error when saving time entry.</span></span>
- <span data-ttu-id="d2061-117">Увоз ставке времена из додељивања ресурса креира ставке времена са нетачним вредностима датума и времена.</span><span class="sxs-lookup"><span data-stu-id="d2061-117">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>
- <span data-ttu-id="d2061-118">Када су инсталиране апликације Project Service Automation и Field Service, дугме **Ново** се приказује два пута на командној траци за ставке времена у апликацији Field Service.</span><span class="sxs-lookup"><span data-stu-id="d2061-118">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>
- <span data-ttu-id="d2061-119">Ћелије **Дозволи ажурирања јединице** и **групе јединица** сада раде у мрежи **Процене трошкова**.</span><span class="sxs-lookup"><span data-stu-id="d2061-119">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>
- <span data-ttu-id="d2061-120">Образац **Ажурирај уређивање ставке времена** укључује **Временску осу**.</span><span class="sxs-lookup"><span data-stu-id="d2061-120">**Update Time Entry Edit** form includes **Timeline**.</span></span>
- <span data-ttu-id="d2061-121">Одобрење времена за ставке времена које се не односе на пројекат блокирају систем приликом претраге за улогу одобраваоца пројекта.</span><span class="sxs-lookup"><span data-stu-id="d2061-121">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="d2061-122">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="d2061-122">**Resource Management**</span></span>

<span data-ttu-id="d2061-123">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="d2061-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="d2061-124">Додата је валидација у додатној компоненти **PostProjectCreate** за проверу примарног захтева пре његовог креирања.</span><span class="sxs-lookup"><span data-stu-id="d2061-124">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>
- <span data-ttu-id="d2061-125">Образац за брзо креирање **Члан пројектног тима** даје изузетак празне референце ако се поља уклоне из обрасца.</span><span class="sxs-lookup"><span data-stu-id="d2061-125">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>
- <span data-ttu-id="d2061-126">Генерирање захтева за 12 сати током 1 године неће успети.</span><span class="sxs-lookup"><span data-stu-id="d2061-126">Generate requirements for 12 hours over 1 year will fail.</span></span>
- <span data-ttu-id="d2061-127">Побољшана порука о грешци за изузетак празне референце током креирања захтева за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="d2061-127">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="d2061-128">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="d2061-128">**Project Management**</span></span>

<span data-ttu-id="d2061-129">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="d2061-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="d2061-130">Побољшана валидација за одговор на изузетак празне референце генерисане у додатној компоненти **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="d2061-130">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>
- <span data-ttu-id="d2061-131">Пројекти објављени у програмском додатку за рачунаре услуге Microsoft Project бришу нераспоређене задатке.</span><span class="sxs-lookup"><span data-stu-id="d2061-131">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>
- <span data-ttu-id="d2061-132">Додата је нова валидација када референца пројекта задатка није важећа због изузетка празне референце у додатној компоненти **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="d2061-132">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>
- <span data-ttu-id="d2061-133">Мрежа члана тима не приказује различите задатке у запису члана тима.</span><span class="sxs-lookup"><span data-stu-id="d2061-133">Team Member grid does not show distinct assignments on the team member record.</span></span>
- <span data-ttu-id="d2061-134">Додате су нове поруке за проверу ваљаности и поруке грешке због изузетка празне референце у додатној компоненти **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="d2061-134">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="d2061-135">**Sales**</span><span class="sxs-lookup"><span data-stu-id="d2061-135">**Sales**</span></span>

<span data-ttu-id="d2061-136">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="d2061-136">The following issues have been fixed:</span></span>

- <span data-ttu-id="d2061-137">Приликом избора ставке засноване на пројекту у понуду или уговору, дугме **Предлог** би требало да буде видљиво само при одабиру линије засноване на производу повезане са постојећим производом.</span><span class="sxs-lookup"><span data-stu-id="d2061-137">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>
- <span data-ttu-id="d2061-138">Поделите привилегију **Create_Product** из привилегије **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="d2061-138">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>
- <span data-ttu-id="d2061-139">Брисање ставке у фактору доводи до неуспеле празне референце на **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="d2061-139">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]