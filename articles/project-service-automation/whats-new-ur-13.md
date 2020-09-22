---
title: Шта је ново у издању исправке 13 за Project Service Automation у верзији 3
description: У овој теми дате су информације о томе шта је ново у издању исправке 13 за Project Service Automation у верзији 3.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c6f6a5b6-b5bb-467c-b7c7-7fb962504c6d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5f1b6b3879c94a77ab62082aad1e470a3ba66552
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755375"
---
# <a name="project-service-automation-v3-update-release-13"></a><span data-ttu-id="22861-103">Project Service Automation у верзији 3, издање исправке 13</span><span class="sxs-lookup"><span data-stu-id="22861-103">Project Service Automation V3, Update Release 13</span></span>
<span data-ttu-id="22861-104">Са задовољство најављујемо најновију исправку за апликацију Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="22861-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="22861-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="22861-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="22861-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="22861-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="22861-107">Да бисте ажурирали ово издање, посетите центар за администрацију за Dynamics 365 online и идите до странице са решењима како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="22861-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="22861-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="22861-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="22861-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 13.</span><span class="sxs-lookup"><span data-stu-id="22861-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="22861-110">Ова верзија има број верзије V3.10.3.18 и доступна је према следећем плану:</span><span class="sxs-lookup"><span data-stu-id="22861-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="22861-111">**Општа доступност (само-исправка):** новембар 2019. године</span><span class="sxs-lookup"><span data-stu-id="22861-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="22861-112">**аутоматска исправка:** децембар 2019. године</span><span class="sxs-lookup"><span data-stu-id="22861-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="22861-113">Издање исправке 13</span><span class="sxs-lookup"><span data-stu-id="22861-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="22861-114">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="22861-114">Bug fixes</span></span>

- <span data-ttu-id="22861-115">Време и трошак</span><span class="sxs-lookup"><span data-stu-id="22861-115">Time and Expense</span></span>

     - <span data-ttu-id="22861-116">Исправљено: функција претраге на страници **Одобрење трошкова** не ради приликом претраживања према сврси трошкова.</span><span class="sxs-lookup"><span data-stu-id="22861-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="22861-117">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="22861-117">Resource Management</span></span>

     - <span data-ttu-id="22861-118">Исправљено: бројеви у сравњењу су исправљени како би били поравнати удесно.</span><span class="sxs-lookup"><span data-stu-id="22861-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="22861-119">Исправљено: није могуће доделити именоване ресурсе задацима путем картице **Распоред**.</span><span class="sxs-lookup"><span data-stu-id="22861-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="22861-120">Управљање пројектима</span><span class="sxs-lookup"><span data-stu-id="22861-120">Project Management</span></span>

     - <span data-ttu-id="22861-121">Исправљено: Изузетак за референцу на вредност које нема приликом додељивања члана тима када за **TransactionType** недостају информације о подешавању за ентитете **Unit** и **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="22861-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="22861-122">Sales</span><span class="sxs-lookup"><span data-stu-id="22861-122">Sales</span></span>

     - <span data-ttu-id="22861-123">Исправљено: дуплирани записи типа трансакције враћају грешку када се креирају записи цене улоге.</span><span class="sxs-lookup"><span data-stu-id="22861-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="22861-124">Исправљено: додатна дугмад за **Нова могућност за пословање**, **Понуда**, **Ставка поруџбине** и **Додај производ** су видљива у командама за могућности за пословање, понуде, производе поруџбине и подформи редова заснованих на пројекту.</span><span class="sxs-lookup"><span data-stu-id="22861-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines sub-grid.</span></span>


