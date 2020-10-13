---
title: Преглед режима управљања ресурсима
description: Ова тема пружа информације о функционалности управљања ресурсима у услузи Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4a8e605109e48b50da68abeee989f8ac8d3d659c
ms.sourcegitcommit: cf79185c8c84c55fbae55f9cfc1b17840e072b49
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3930109"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="61fe9-103">Преглед режима управљања ресурсима</span><span class="sxs-lookup"><span data-stu-id="61fe9-103">Resource management modes overview</span></span>

<span data-ttu-id="61fe9-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="61fe9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="61fe9-105">Dynamics 365 Project Operations подржава два режима како бисте извршили укупан ток резервације.</span><span class="sxs-lookup"><span data-stu-id="61fe9-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="61fe9-106">Режим управљања дефинисан је као параметар пројекта и може се изменити ако ваше пословање треба променити.</span><span class="sxs-lookup"><span data-stu-id="61fe9-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="61fe9-107">Централни режим</span><span class="sxs-lookup"><span data-stu-id="61fe9-107">Central mode</span></span>
<span data-ttu-id="61fe9-108">За организације које централизују додељивање ресурса пројектима, централни режим пружа начин да менаџери пројеката могу да дефинишу захтеве за ресурсима на нивоу пројекта.</span><span class="sxs-lookup"><span data-stu-id="61fe9-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="61fe9-109">Испуњавање захтева за ресурсима делегира се менаџеру ресурса.</span><span class="sxs-lookup"><span data-stu-id="61fe9-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="61fe9-110">Менаџери пројеката могу прихватити или одбити ресурсе које предложи менаџер ресурса.</span><span class="sxs-lookup"><span data-stu-id="61fe9-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Централни режим](./media/resource-management-central.png)

<span data-ttu-id="61fe9-112">Да бисте управљали ресурсима у централном режиму, погледајте:</span><span class="sxs-lookup"><span data-stu-id="61fe9-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="61fe9-113">Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима</span><span class="sxs-lookup"><span data-stu-id="61fe9-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="61fe9-114">Резервисање именованих ресурса из потребе за ресурсима</span><span class="sxs-lookup"><span data-stu-id="61fe9-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="61fe9-115">Прослеђивање захтева за ресурсом</span><span class="sxs-lookup"><span data-stu-id="61fe9-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="61fe9-116">Испуњавање захтева за ресурсима</span><span class="sxs-lookup"><span data-stu-id="61fe9-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="61fe9-117">Прихватање или одбацивање предложеног ресурса пројекта у захтеву за ресурс</span><span class="sxs-lookup"><span data-stu-id="61fe9-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="61fe9-118">Хибридни режим</span><span class="sxs-lookup"><span data-stu-id="61fe9-118">Hybrid mode</span></span>
<span data-ttu-id="61fe9-119">За организације којима је потребна флексибилност у расподели ресурса, хибридни режим омогућава менаџерима пројеката и менаџерима ресурса могућност да резервишу ресурсе.</span><span class="sxs-lookup"><span data-stu-id="61fe9-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Хибридни режим](./media/resource-management-hybrid.png)

<span data-ttu-id="61fe9-121">Поред подржаног процеса централног режима, погледајте следеће теме да бисте управљали свим осталим подржаним токовима резервација у хибридном режиму:</span><span class="sxs-lookup"><span data-stu-id="61fe9-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="61fe9-122">Резервисање ресурса директно у пројекту:</span><span class="sxs-lookup"><span data-stu-id="61fe9-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="61fe9-123">Резервисање именованих ресурса које је могуће резервисати за пројектни тим и додељивање задатака</span><span class="sxs-lookup"><span data-stu-id="61fe9-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="61fe9-124">Резервисање ресурса из захтева за ресурсима:</span><span class="sxs-lookup"><span data-stu-id="61fe9-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="61fe9-125">Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима</span><span class="sxs-lookup"><span data-stu-id="61fe9-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="61fe9-126">Резервисање именованих ресурса из потребе за ресурсима</span><span class="sxs-lookup"><span data-stu-id="61fe9-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
