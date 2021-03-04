---
title: Шта је ново или промењено у издању 28 исправке Project Service Automation верзије 3
description: У овој теми су наведене функције и исправке које су доступне у издању исправке 28 за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 2c50d6bdc033836e1259a2fd12b78015280d8093
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150641"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a><span data-ttu-id="b7b07-103">Шта је ново или промењено у издању 28 исправке Project Service Automation верзије 3</span><span class="sxs-lookup"><span data-stu-id="b7b07-103">What's new or changed in Project Service Automation Update Release 28, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b7b07-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="b7b07-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b7b07-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="b7b07-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b7b07-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="b7b07-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b7b07-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="b7b07-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="b7b07-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="b7b07-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b7b07-109">У овој теми су наведене функције и исправке које су нове или промењене у издању исправке 28 за Project Service Automation верзије 3. Ова верзија има број верзије V3.10.46.32 и постала је опште доступна путем самосталне исправке у јануару 2021.</span><span class="sxs-lookup"><span data-stu-id="b7b07-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 28 This version has a build number of V3.10.46.32 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-28"></a><span data-ttu-id="b7b07-110">Издање исправке 28</span><span class="sxs-lookup"><span data-stu-id="b7b07-110">Update Release 28</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b7b07-111">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="b7b07-111">Bug fixes</span></span>

<span data-ttu-id="b7b07-112">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="b7b07-112">**Time and Expense**</span></span>

<span data-ttu-id="b7b07-113">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="b7b07-113">The following issues have been fixed:</span></span>

- <span data-ttu-id="b7b07-114">Корисници могу да користе **Масовно уређивање** за ажурирање записа времена који су одобрени и послати.</span><span class="sxs-lookup"><span data-stu-id="b7b07-114">Users can use **Bulk Edit** to update time entries that have been approved and submitted.</span></span>

<span data-ttu-id="b7b07-115">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="b7b07-115">**Project Management**</span></span>

<span data-ttu-id="b7b07-116">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="b7b07-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="b7b07-117">У случајевима када се GUID задатка тумачи као број, задаци се не могу отворити за уређивање помоћу опције **Уреди задатак** у траци на страници **Структурна анализа посла**.</span><span class="sxs-lookup"><span data-stu-id="b7b07-117">In cases where the task GUID is interpreted as a number, tasks can't be opened for edit using **Edit Task** in the ribbon on the **Work Breakdown Structure** page.</span></span>

<span data-ttu-id="b7b07-118">**Sales**</span><span class="sxs-lookup"><span data-stu-id="b7b07-118">**Sales**</span></span>

<span data-ttu-id="b7b07-119">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="b7b07-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="b7b07-120">Изузетак празне референце се генерише када се позива додатна компонента **GetEstimatesForProject**.</span><span class="sxs-lookup"><span data-stu-id="b7b07-120">A null reference exception is generated when the **GetEstimatesForProject** plug-in is invoked.</span></span>
- <span data-ttu-id="b7b07-121">**Означи као спремно за фактурисање** у мрежи контролних тачака само делимично ажурира атрибуте, осим атрибута **InvoiceStatus**, који се ажурира.</span><span class="sxs-lookup"><span data-stu-id="b7b07-121">**Mark ready to invoice** on the milestone grid only partially updates attributes, except for the **InvoiceStatus** attribute, which is updated.</span></span>

