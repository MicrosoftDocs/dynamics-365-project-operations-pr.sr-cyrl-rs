---
title: Шта је ново или промењено у издању 23 исправке Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 23 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: eaae9cc62c449695cb2e999be48c57075aadbb21
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083919"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="bba84-103">Project Service Automation издање 23 исправке верзије 3</span><span class="sxs-lookup"><span data-stu-id="bba84-103">Project Service Automation Update Release 23, V3</span></span>

<span data-ttu-id="bba84-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="bba84-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="bba84-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="bba84-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="bba84-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="bba84-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="bba84-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="bba84-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="bba84-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="bba84-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="bba84-109">У овој теми дате су функције и исправке које су нове или промењене у решењу Project Service Automation у верзији 3, издање исправке 23.</span><span class="sxs-lookup"><span data-stu-id="bba84-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="bba84-110">Ова верзија има број V3.10.34.30 и опште је доступна путем самосталне исправке објављене августа 2020.</span><span class="sxs-lookup"><span data-stu-id="bba84-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="bba84-111">Издање исправке 23</span><span class="sxs-lookup"><span data-stu-id="bba84-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="bba84-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="bba84-112">Bug fixes</span></span>

<span data-ttu-id="bba84-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="bba84-113">**Time and Expense**</span></span>

<span data-ttu-id="bba84-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="bba84-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="bba84-115">Рукујте граничним случајем у функцији **Избриши члана пројектног тима** да бисте пружили смислен изузетак.</span><span class="sxs-lookup"><span data-stu-id="bba84-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="bba84-116">Увоз задатка резултира празним екраном за уклањање.</span><span class="sxs-lookup"><span data-stu-id="bba84-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="bba84-117">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="bba84-117">**Resource Management**</span></span>

<span data-ttu-id="bba84-118">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="bba84-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="bba84-119">**Картица ресурса мреже за укупну искоришћеност ресурса** приказује нетачне податке када је временска скала дужа од пет дана.</span><span class="sxs-lookup"><span data-stu-id="bba84-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="bba84-120">Када клијенти креирају ресурс који може да се резервише, додатна компонента повремено не успева аутоматски да дода ресурс у Microsoft Office 365 групу.</span><span class="sxs-lookup"><span data-stu-id="bba84-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="bba84-121">Приказ **Усаглашеност** нетачно приказује ручне контуре у приказу **Недеља** или **Месец**.</span><span class="sxs-lookup"><span data-stu-id="bba84-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="bba84-122">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="bba84-122">**Project Management**</span></span>

<span data-ttu-id="bba84-123">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="bba84-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="bba84-124">Прекомерни број ентитета **RetrieveMultiple за подешавања корисника** узрокују погоршане перформансе за одобравање пројеката и друге операције.</span><span class="sxs-lookup"><span data-stu-id="bba84-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="bba84-125">Проналажење ресурса мреже **Планирање задатака** ограничено је на приказивање до пет чланова тима из пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="bba84-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="bba84-126">Проналажење ресурса мреже **Планирање задатака** не филтрира неактивне ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bba84-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="bba84-127">Ручни режим не ради како се очекује у структурној анализи посла на планирању пројекта.</span><span class="sxs-lookup"><span data-stu-id="bba84-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="bba84-128">Мрежа **Планирање задатака** показује **Неактивне категорије трансакција**.</span><span class="sxs-lookup"><span data-stu-id="bba84-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="bba84-129">Мрежа **Додељивање ресурса** се неправилно заокружује када задатак има више додела.</span><span class="sxs-lookup"><span data-stu-id="bba84-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="bba84-130">Вредности заокруживања разликују се између планираних трошкова и стварних трошкова за један задатак.</span><span class="sxs-lookup"><span data-stu-id="bba84-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="bba84-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="bba84-131">**Sales**</span></span>

<span data-ttu-id="bba84-132">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="bba84-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="bba84-133">Дупли клик на **Преузми све категорије трансакција** креира више линија.</span><span class="sxs-lookup"><span data-stu-id="bba84-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>
