---
title: Преглед режима управљања ресурсима
description: У овој теми дате су информације о функцији управљања ресурсима у услузи Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4d132bcbef5421202d2f4899091f0dc75166dd66
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949967"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="3fd3e-103">Преглед режима управљања ресурсима</span><span class="sxs-lookup"><span data-stu-id="3fd3e-103">Resource management modes overview</span></span>

<span data-ttu-id="3fd3e-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="3fd3e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="3fd3e-105">Dynamics 365 Project Operations подржава два режима како бисте извршавали укупан ток резервације.</span><span class="sxs-lookup"><span data-stu-id="3fd3e-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="3fd3e-106">Режим управљања дефинисан је као параметар пројекта и може се изменити ако ваше пословање треба променити.</span><span class="sxs-lookup"><span data-stu-id="3fd3e-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="3fd3e-107">Централни режим</span><span class="sxs-lookup"><span data-stu-id="3fd3e-107">Central mode</span></span>
<span data-ttu-id="3fd3e-108">За организације које централизују додељивање ресурса пројектима, централни режим пружа начин да менаџери пројеката могу да дефинишу захтеве за ресурсима на нивоу пројекта.</span><span class="sxs-lookup"><span data-stu-id="3fd3e-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="3fd3e-109">Испуњавање захтева за ресурсима делегира се менаџеру ресурса.</span><span class="sxs-lookup"><span data-stu-id="3fd3e-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="3fd3e-110">Менаџери пројеката могу прихватити или одбити ресурсе које предложи менаџер ресурса.</span><span class="sxs-lookup"><span data-stu-id="3fd3e-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Централни режим](./media/resource-management-central.png)

<span data-ttu-id="3fd3e-112">Да бисте управљали ресурсима у централном режиму, погледајте:</span><span class="sxs-lookup"><span data-stu-id="3fd3e-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="3fd3e-113">Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима</span><span class="sxs-lookup"><span data-stu-id="3fd3e-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="3fd3e-114">Резервисање именованих ресурса из потребе за ресурсима</span><span class="sxs-lookup"><span data-stu-id="3fd3e-114">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="3fd3e-115">Прослеђивање захтева за ресурсом</span><span class="sxs-lookup"><span data-stu-id="3fd3e-115">Submit a resource request</span></span>](/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="3fd3e-116">Испуњавање захтева за ресурсима</span><span class="sxs-lookup"><span data-stu-id="3fd3e-116">Fulfill a resource request</span></span>](/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="3fd3e-117">Прихватање или одбацивање предложеног ресурса пројекта у захтеву за ресурс</span><span class="sxs-lookup"><span data-stu-id="3fd3e-117">Accept or reject a proposed project resource from a resource request</span></span>](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="3fd3e-118">Хибридни режим</span><span class="sxs-lookup"><span data-stu-id="3fd3e-118">Hybrid mode</span></span>
<span data-ttu-id="3fd3e-119">За организације којима је потребна флексибилност у расподели ресурса, хибридни режим омогућава менаџерима пројеката и менаџерима ресурса могућност да резервишу ресурсе.</span><span class="sxs-lookup"><span data-stu-id="3fd3e-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Хибридни режим](./media/resource-management-hybrid.png)

<span data-ttu-id="3fd3e-121">Поред подржаног процеса централног режима, погледајте следеће теме да бисте управљали свим осталим подржаним токовима резервација у хибридном режиму:</span><span class="sxs-lookup"><span data-stu-id="3fd3e-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="3fd3e-122">Резервисање ресурса директно у пројекту:</span><span class="sxs-lookup"><span data-stu-id="3fd3e-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="3fd3e-123">Резервисање именованих ресурса које је могуће резервисати за пројектни тим и додељивање задатака</span><span class="sxs-lookup"><span data-stu-id="3fd3e-123">Book named bookable resources to a project team and assign tasks</span></span>](/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="3fd3e-124">Резервисање ресурса из захтева за ресурсима:</span><span class="sxs-lookup"><span data-stu-id="3fd3e-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="3fd3e-125">Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима</span><span class="sxs-lookup"><span data-stu-id="3fd3e-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="3fd3e-126">Резервисање именованих ресурса из потребе за ресурсима</span><span class="sxs-lookup"><span data-stu-id="3fd3e-126">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]