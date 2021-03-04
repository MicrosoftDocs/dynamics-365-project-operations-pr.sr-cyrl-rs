---
title: Резервације у односу на доделе
description: Ова тема пружа информације о разликама између резервисања ресурса и додељивања ресурса.
author: ruhercul
manager: Annbe
ms.date: 01/08/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 9e346766e6ccbb3dff59ef12072a1cd63f1e4231
ms.sourcegitcommit: 260ce052fed760bb44c514517806049ca13a5459
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 01/08/2021
ms.locfileid: "4841190"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="e4a68-103">Резервације у односу на доделе</span><span class="sxs-lookup"><span data-stu-id="e4a68-103">Bookings vs assignments</span></span>

<span data-ttu-id="e4a68-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="e4a68-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e4a68-105">Резервације представљају фиксну или условну расподелу ресурса за пројекат.</span><span class="sxs-lookup"><span data-stu-id="e4a68-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="e4a68-106">Фиксне резервације троше капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="e4a68-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="e4a68-107">Резервације представљају организационе концепте тимова како би могли да разумеју како ће се ресурси ангажовати на различитим пројектима.</span><span class="sxs-lookup"><span data-stu-id="e4a68-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="e4a68-108">Dynamics 365 Project Operations сматра резервације концептом на нивоу пројекта.</span><span class="sxs-lookup"><span data-stu-id="e4a68-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="e4a68-109">За разлику од резервација, доделе представљају обавезивање ресурса за пројектне задатке у распореду пројеката.</span><span class="sxs-lookup"><span data-stu-id="e4a68-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="e4a68-110">Ресурси могу бити именовани или генерички.</span><span class="sxs-lookup"><span data-stu-id="e4a68-110">The resources can be named or generic.</span></span>  <span data-ttu-id="e4a68-111">Када се захтев за ресурс изведе из доделе пројектног задатка, Project Operations користи контуре активности доделе ресурса за израду контура детаља о захтеву за ресурс.</span><span class="sxs-lookup"><span data-stu-id="e4a68-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="e4a68-112">Међутим, позивање на доделе ресурса се не одржава.</span><span class="sxs-lookup"><span data-stu-id="e4a68-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="e4a68-113">Ажурирања резервација изведених из захтева за ресурс не ажурирају ниједну доделу ресурса.</span><span class="sxs-lookup"><span data-stu-id="e4a68-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="e4a68-114">Уобичајено је да је збир резервација за ресурс једнак збиру додела ресурса за један или више задатака.</span><span class="sxs-lookup"><span data-stu-id="e4a68-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="e4a68-115">Међутим, Project Operations не спроводи овај договор.</span><span class="sxs-lookup"><span data-stu-id="e4a68-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="e4a68-116">Приказ **Усаглашеност** показује менаџеру пројеката места где се резервације и доделе ресурса не слажу.</span><span class="sxs-lookup"><span data-stu-id="e4a68-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>


