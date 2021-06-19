---
title: Улазне поруџбине пројекта за пројекте времена и материјала
description: Ова тема објашњава како се креирају улазне поруџбине засноване на пројектима времена и материјала.
author: Yowelle
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: dec9bc700d18f71ec7c9e976b38cb8cbb41f21b5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009679"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="f9233-103">Улазне поруџбине пројекта за пројекте времена и материјала</span><span class="sxs-lookup"><span data-stu-id="f9233-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="f9233-104">Овај тема описује како се креира улазна поруџбина за пројекат.</span><span class="sxs-lookup"><span data-stu-id="f9233-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="f9233-105">Упазне поруџбине могу се креирати само за пројекте тог типа **време и материјал**.</span><span class="sxs-lookup"><span data-stu-id="f9233-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="f9233-106">Ако пројекат времена и материјала садржи више извора финансирања у уговору о пројекту, морате омогућити параметар **Дозволи улазне поруџбине за пројекте са више извора финансирања** на страници **Управљање пројектом и рачуноводствени параметри**.</span><span class="sxs-lookup"><span data-stu-id="f9233-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="f9233-107">Подршка за улазне поруџбине пројеката са више извора финансирања доступна је почев од издања апликације 10.0.2 и новије.</span><span class="sxs-lookup"><span data-stu-id="f9233-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="f9233-108">Параметар који ће омогућити подршку за улазне поруџбине пројеката са више извора финансирања уклониће се у таласу издања из априла 2020. године, након чега ће функционалност увек бити омогућена.</span><span class="sxs-lookup"><span data-stu-id="f9233-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="f9233-109">Улазне поруџбине засноване на пројекту можете креирати на два начина:</span><span class="sxs-lookup"><span data-stu-id="f9233-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="f9233-110">Идите на сам пројекат.</span><span class="sxs-lookup"><span data-stu-id="f9233-110">Go to the project itself.</span></span> <span data-ttu-id="f9233-111">У окну радњи изаберите **Управљање > Задаци предмета > Улазна поруџбина**.</span><span class="sxs-lookup"><span data-stu-id="f9233-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="f9233-112">Информације о пројекту подразумевано се стављају у улазну поруџбину из пројекта.</span><span class="sxs-lookup"><span data-stu-id="f9233-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="f9233-113">Ако уговор о пројекту има више извора финансирања, мораћете да изаберете извор финансирања да бисте поставили клијента за улазну поруџбину.</span><span class="sxs-lookup"><span data-stu-id="f9233-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="f9233-114">Ако постоји само један извор финансирања за пројекат, клијент ће бити аутоматски подешен.</span><span class="sxs-lookup"><span data-stu-id="f9233-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="f9233-115">Идите на страницу листе **Све улазне поруџбине** и креирајте нову улазну поруџбину.</span><span class="sxs-lookup"><span data-stu-id="f9233-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="f9233-116">За улазну поруџбину ћете морати да изаберете пројекат.</span><span class="sxs-lookup"><span data-stu-id="f9233-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="f9233-117">Када изаберете пројекат, клијент ће бити постављен из извора финансирања или ћете морати изабрати извор финансирања ако уговор о пројекту има више извора финансирања.</span><span class="sxs-lookup"><span data-stu-id="f9233-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]