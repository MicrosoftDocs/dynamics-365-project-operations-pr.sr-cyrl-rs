---
title: Шта је ново или промењено у издању 18 исправке за Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 18 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: bd6038b3594e8507c4a441b00ddc2eb240f796dc
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949202"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="a0562-103">Project Service Automation издање исправке 18, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="a0562-103">Project Service Automation Update Release 18, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a0562-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a0562-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a0562-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="a0562-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a0562-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="a0562-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a0562-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="a0562-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="a0562-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a0562-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a0562-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 18.</span><span class="sxs-lookup"><span data-stu-id="a0562-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="a0562-110">Број израде ове верзије је V3.10.8.12 и углавном је доступна путем самосталног ажурирања у априлу 2020. године.</span><span class="sxs-lookup"><span data-stu-id="a0562-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="a0562-111">Издање исправке 18</span><span class="sxs-lookup"><span data-stu-id="a0562-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a0562-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="a0562-112">Bug fixes</span></span>

<span data-ttu-id="a0562-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="a0562-113">**Time and Expense**</span></span>

- <span data-ttu-id="a0562-114">Поправљено: токови **Опозив**, **Захтев** и **Откажи одобрење** избацују изузетке са нејасним порукама о грешкама.</span><span class="sxs-lookup"><span data-stu-id="a0562-114">Fixed: **Recall**, **Request**, and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="a0562-115">Поправљено: Када **Откажи одобрење** не успе за трошак, не избацује се релевантна грешка изузетка.</span><span class="sxs-lookup"><span data-stu-id="a0562-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="a0562-116">Поправљено: Мрежа ставке времена погрешно обрађује нерадне дане у Аустралији након пребацивања летњег времена (DST) у октобру.</span><span class="sxs-lookup"><span data-stu-id="a0562-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="a0562-117">Поправљено: Неправилна логика подразумеваних вредности спречава подношење трошкова.</span><span class="sxs-lookup"><span data-stu-id="a0562-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="a0562-118">Поправљено: Када одобрење ставке времена не успе, одобрење остаје у статусу **На чекању**.</span><span class="sxs-lookup"><span data-stu-id="a0562-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="a0562-119">Поправљено: SQL грешке при масовним одобрењима (застој / истек времена).</span><span class="sxs-lookup"><span data-stu-id="a0562-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="a0562-120">Поправљено: Значајни проблеми са перформансама у корисничком искуству изазвани ажурирањем чланова тима приликом одобравања уноса времена.</span><span class="sxs-lookup"><span data-stu-id="a0562-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="a0562-121">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="a0562-121">**Project Management**</span></span>

- <span data-ttu-id="a0562-122">Поправљено: Обавештење о временској зони премештено је са приказа **Сравњење** на главни образац **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="a0562-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="a0562-123">Поправљено: Предложак календара нема исправне подразумеване вредности када се отвори нови образац пројекта.</span><span class="sxs-lookup"><span data-stu-id="a0562-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="a0562-124">Поправљено: За Chromium прегледаче, корисници не могу лако да изаберу претходне задатке које ће избрисати.</span><span class="sxs-lookup"><span data-stu-id="a0562-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="a0562-125">Поправљено: Креирање или копирање **пројекта из празног предлошка** преузима неповезане доделе.</span><span class="sxs-lookup"><span data-stu-id="a0562-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="a0562-126">Поправљено: У специфичним рубним случајевима, креирање новог задатка из мреже задатака доводи до стварања дупликата записа.</span><span class="sxs-lookup"><span data-stu-id="a0562-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="a0562-127">Поправљено: У ручном режиму корисници не могу да ажурирају датуме почетка задатка да буду каснији од сачуваног тренутног датума.</span><span class="sxs-lookup"><span data-stu-id="a0562-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="a0562-128">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="a0562-128">**Resource Management**</span></span>

- <span data-ttu-id="a0562-129">Поправљено: Ред подзбира у приказу **Сравњење** погрешно израчунава одступање резервација након продужења резервације.</span><span class="sxs-lookup"><span data-stu-id="a0562-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="a0562-130">Поправљено: Приказ **Сравњење** погрешно приказује додељене ресурсе када ресурс који је могуће резервисати има календар који се не подудара са календаром пројекта.</span><span class="sxs-lookup"><span data-stu-id="a0562-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="a0562-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="a0562-131">**Sales**</span></span>

- <span data-ttu-id="a0562-132">Поправљено: Када се ставке времена поново одобре (**Одобри > Откажи>** Поново одобри), креира се дупликат ненаплативе стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="a0562-132">Fixed: When time entries are re-approved (**Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]