---
title: Шта је ново или промењено у издању 17.5 исправке Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 17 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: 7ba685568692dafe117de42a71bb14d391cd7cc4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083928"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="7828d-103">Project Service Automation издање исправке 17, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="7828d-103">Project Service Automation Update Release 17, V3</span></span>

<span data-ttu-id="7828d-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7828d-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="7828d-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="7828d-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="7828d-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="7828d-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="7828d-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="7828d-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="7828d-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="7828d-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="7828d-109">У овој теми дате су функције и исправке које су нове или су промењене у решењу PSA верзије 3, издање исправке 17.</span><span class="sxs-lookup"><span data-stu-id="7828d-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="7828d-110">Ова верзија има број верзије V3.10.6.34 и опште је доступна путем само-исправке у марту 2020. године.</span><span class="sxs-lookup"><span data-stu-id="7828d-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="7828d-111">Издање исправке 17</span><span class="sxs-lookup"><span data-stu-id="7828d-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="7828d-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="7828d-112">Bug fixes</span></span>

<span data-ttu-id="7828d-113">**Општи проблеми**</span><span class="sxs-lookup"><span data-stu-id="7828d-113">**General**</span></span>

- <span data-ttu-id="7828d-114">Исправљено: ажурирајте Project Service Automation за спровођење лиценци за чланове тима (Чвориште ресурса за пројекат ће укључити 3.x метаподатке плана услуге за чланове тима)</span><span class="sxs-lookup"><span data-stu-id="7828d-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="7828d-115">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="7828d-115">**Time and Expense**</span></span>

- <span data-ttu-id="7828d-116">Исправљено: немогућност промене процене трошкова из цене различите од нуле у нулу (0).</span><span class="sxs-lookup"><span data-stu-id="7828d-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="7828d-117">Промена се игнорише.</span><span class="sxs-lookup"><span data-stu-id="7828d-117">The change is ignored.</span></span>

<span data-ttu-id="7828d-118">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="7828d-118">**Project Management**</span></span>

- <span data-ttu-id="7828d-119">Исправљено: додата је провера нултих вредности у име позиције члана тима.</span><span class="sxs-lookup"><span data-stu-id="7828d-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="7828d-120">Исправљено: поље **msdyn_userresourceid** поље у ентитету **msdyn_resourceassignment** није одобрено.</span><span class="sxs-lookup"><span data-stu-id="7828d-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="7828d-121">Исправљено: надоградња са 2.x на 3.x сада управља празним контурама ангажовања у доделама задатака.</span><span class="sxs-lookup"><span data-stu-id="7828d-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="7828d-122">**Sales**</span><span class="sxs-lookup"><span data-stu-id="7828d-122">**Sales**</span></span>

- <span data-ttu-id="7828d-123">Исправљено: **Invoice.PreValidateInvoiceUpdate** сада правилно управља сценаријем поновног додељивања власништва записа.</span><span class="sxs-lookup"><span data-stu-id="7828d-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="7828d-124">Исправљено: када је класа трансакције **Време** , **UnitGroup** не може да се уређује ни за један ентитет, укључујући **QuoteLineDetails** , **JournalLine** , **InvoiceLineDetail** и **ContractLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="7828d-124">Fixed: When the transaction class is **Time** , **UnitGroup** is non-editable for all entities including, **QuoteLineDetails** , **JournalLine** , **InvoiceLineDetail** , and **ContractLineDetails**.</span></span> <span data-ttu-id="7828d-125">Међутим, **Јединица** не може да се уређује само за **JournalLine** и **InvoiceLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="7828d-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>


