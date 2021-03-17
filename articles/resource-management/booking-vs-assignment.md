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
ms.openlocfilehash: 3aaf8dcbae0a5762879c2b1223eba3bdc33af1a7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279921"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="886d2-103">Резервације у односу на доделе</span><span class="sxs-lookup"><span data-stu-id="886d2-103">Bookings vs assignments</span></span>

<span data-ttu-id="886d2-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="886d2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="886d2-105">Резервације представљају фиксну или условну расподелу ресурса за пројекат.</span><span class="sxs-lookup"><span data-stu-id="886d2-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="886d2-106">Фиксне резервације троше капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="886d2-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="886d2-107">Резервације представљају организационе концепте тимова како би могли да разумеју како ће се ресурси ангажовати на различитим пројектима.</span><span class="sxs-lookup"><span data-stu-id="886d2-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="886d2-108">Dynamics 365 Project Operations сматра резервације концептом на нивоу пројекта.</span><span class="sxs-lookup"><span data-stu-id="886d2-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="886d2-109">За разлику од резервација, доделе представљају обавезивање ресурса за пројектне задатке у распореду пројеката.</span><span class="sxs-lookup"><span data-stu-id="886d2-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="886d2-110">Ресурси могу бити именовани или генерички.</span><span class="sxs-lookup"><span data-stu-id="886d2-110">The resources can be named or generic.</span></span>  <span data-ttu-id="886d2-111">Када се захтев за ресурс изведе из доделе пројектног задатка, Project Operations користи контуре активности доделе ресурса за израду контура детаља о захтеву за ресурс.</span><span class="sxs-lookup"><span data-stu-id="886d2-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="886d2-112">Међутим, позивање на доделе ресурса се не одржава.</span><span class="sxs-lookup"><span data-stu-id="886d2-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="886d2-113">Ажурирања резервација изведених из захтева за ресурс не ажурирају ниједну доделу ресурса.</span><span class="sxs-lookup"><span data-stu-id="886d2-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="886d2-114">Уобичајено је да је збир резервација за ресурс једнак збиру додела ресурса за један или више задатака.</span><span class="sxs-lookup"><span data-stu-id="886d2-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="886d2-115">Међутим, Project Operations не спроводи овај договор.</span><span class="sxs-lookup"><span data-stu-id="886d2-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="886d2-116">Приказ **Усаглашеност** показује менаџеру пројеката места где се резервације и доделе ресурса не слажу.</span><span class="sxs-lookup"><span data-stu-id="886d2-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]