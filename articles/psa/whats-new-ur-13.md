---
title: Шта је ново или промењено у издању 13 исправке Project Service Automation верзије 3
description: У овој теми дате су информације о томе шта је ново у издању исправке 13 за Project Service Automation у верзији 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: dbdcb811bfeacf17e841d679f097c591c16cd4c0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281046"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="f4976-103">Project Service Automation издање исправке 13, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="f4976-103">Project Service Automation Update Release 13, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f4976-104">Са задовољство најављујемо најновију исправку за апликацију Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="f4976-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="f4976-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="f4976-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f4976-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f4976-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f4976-107">Да бисте ажурирали ово издање, посетите центар за администрацију за Dynamics 365 online и идите до странице са решењима како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="f4976-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="f4976-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f4976-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f4976-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 13.</span><span class="sxs-lookup"><span data-stu-id="f4976-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="f4976-110">Ова верзија има број верзије V3.10.3.18 и доступна је према следећем плану:</span><span class="sxs-lookup"><span data-stu-id="f4976-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="f4976-111">**Општа доступност (само-исправка):** новембар 2019. године</span><span class="sxs-lookup"><span data-stu-id="f4976-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="f4976-112">**аутоматска исправка:** децембар 2019. године</span><span class="sxs-lookup"><span data-stu-id="f4976-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="f4976-113">Издање исправке 13</span><span class="sxs-lookup"><span data-stu-id="f4976-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="f4976-114">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="f4976-114">Bug fixes</span></span>

- <span data-ttu-id="f4976-115">Време и трошак</span><span class="sxs-lookup"><span data-stu-id="f4976-115">Time and Expense</span></span>

     - <span data-ttu-id="f4976-116">Исправљено: функција претраге на страници **Одобрење трошкова** не ради приликом претраживања према сврси трошкова.</span><span class="sxs-lookup"><span data-stu-id="f4976-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="f4976-117">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="f4976-117">Resource Management</span></span>

     - <span data-ttu-id="f4976-118">Исправљено: бројеви у сравњењу су исправљени како би били поравнати удесно.</span><span class="sxs-lookup"><span data-stu-id="f4976-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="f4976-119">Исправљено: није могуће доделити именоване ресурсе задацима путем картице **Распоред**.</span><span class="sxs-lookup"><span data-stu-id="f4976-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="f4976-120">Управљање пројектима</span><span class="sxs-lookup"><span data-stu-id="f4976-120">Project Management</span></span>

     - <span data-ttu-id="f4976-121">Исправљено: Изузетак за референцу на вредност које нема приликом додељивања члана тима када за **TransactionType** недостају информације о подешавању за ентитете **Unit** и **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="f4976-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="f4976-122">Sales</span><span class="sxs-lookup"><span data-stu-id="f4976-122">Sales</span></span>

     - <span data-ttu-id="f4976-123">Исправљено: дуплирани записи типа трансакције враћају грешку када се креирају записи цене улоге.</span><span class="sxs-lookup"><span data-stu-id="f4976-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="f4976-124">Исправљено: Додатна дугмад за ставке **Нова могућност за пословање**, **Понуда**, **Ставка поруџбине** и **Додавање производа** су видљива у командама за могућности за пословање, понуде, наручивање производа и подформе за ставке засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="f4976-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines subgrid.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]