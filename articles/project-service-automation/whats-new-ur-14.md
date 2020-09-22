---
title: Шта је ново у издању исправке 14 за Project Service Automation у верзији 3
description: У овој теми дате су информације о томе шта је ново у издању исправке 14 за Project Service Automation у верзији 3.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c69eab3b-0bb9-4b52-b606-e8a96e893471
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 31134756a5f4bff3022fca7df8364c49217b9b55
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755374"
---
# <a name="project-service-automation-v3-update-release-14"></a><span data-ttu-id="29bdf-103">Project Service Automation у верзији 3, издање исправке 14</span><span class="sxs-lookup"><span data-stu-id="29bdf-103">Project Service Automation V3, Update Release 14</span></span>
<span data-ttu-id="29bdf-104">Са задовољство најављујемо најновију исправку за апликацију Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="29bdf-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="29bdf-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="29bdf-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="29bdf-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="29bdf-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="29bdf-107">Да бисте ажурирали ово издање, посетите центар за администрацију за Dynamics 365 online и идите до странице са решењима како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="29bdf-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="29bdf-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="29bdf-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="29bdf-109">У овој теми дате су функције које су нове или су промењене у решењу PSA у верзији 3, издање исправке 14.</span><span class="sxs-lookup"><span data-stu-id="29bdf-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="29bdf-110">Ова верзија има број верзије V3.10.4.21 и доступна је према следећем плану:</span><span class="sxs-lookup"><span data-stu-id="29bdf-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="29bdf-111">**Општа доступност (само-исправка):** јануар 2020. године</span><span class="sxs-lookup"><span data-stu-id="29bdf-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="29bdf-112">**Ауто-исправка:** фебруар 2020. године</span><span class="sxs-lookup"><span data-stu-id="29bdf-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="29bdf-113">Издање исправке 14</span><span class="sxs-lookup"><span data-stu-id="29bdf-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="29bdf-114">Побољшања</span><span class="sxs-lookup"><span data-stu-id="29bdf-114">Enhancements</span></span>

- <span data-ttu-id="29bdf-115">Sales</span><span class="sxs-lookup"><span data-stu-id="29bdf-115">Sales</span></span>

     - <span data-ttu-id="29bdf-116">Вредности из прилагођених поља из **Детаљи ставке понуде** се копирају у **Детаљи предмета уговора за пројекат** када се понуда исправи на **Затворена као добијена**.</span><span class="sxs-lookup"><span data-stu-id="29bdf-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="29bdf-117">Потврђени пројекти могу имати статус **Затворена као изгубљена**.</span><span class="sxs-lookup"><span data-stu-id="29bdf-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="29bdf-118">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="29bdf-118">Resource Management</span></span>

     - <span data-ttu-id="29bdf-119">Када продужавате резервације, од корисника ће бити затражено да у дијалогу за потврду резимирају резултате резервација и наведу везу до опције „Одржавање резервација“.</span><span class="sxs-lookup"><span data-stu-id="29bdf-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="29bdf-120">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="29bdf-120">Bug fixes</span></span>

- <span data-ttu-id="29bdf-121">Време и трошак</span><span class="sxs-lookup"><span data-stu-id="29bdf-121">Time and Expense</span></span>

     - <span data-ttu-id="29bdf-122">Исправљено: побољшано корисничко искуство када корисник није изабрао ниједну ставку коју треба исправити.</span><span class="sxs-lookup"><span data-stu-id="29bdf-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="29bdf-123">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="29bdf-123">Resource Management</span></span>

     - <span data-ttu-id="29bdf-124">Исправљено: резервација ресурса више пута прекорачује име ресурса који је могуће резервисати.</span><span class="sxs-lookup"><span data-stu-id="29bdf-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="29bdf-125">Sales</span><span class="sxs-lookup"><span data-stu-id="29bdf-125">Sales</span></span>

     - <span data-ttu-id="29bdf-126">Исправљено: укупна продајна цена се не израчунава све док корисник не унесе и цену коштања за процене трошкова за пројекат.</span><span class="sxs-lookup"><span data-stu-id="29bdf-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="29bdf-127">Исправљено: затварање понуде као **Освојена** не успева ако уговорни пројекат није у статусу **Радна верзија**.</span><span class="sxs-lookup"><span data-stu-id="29bdf-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>

