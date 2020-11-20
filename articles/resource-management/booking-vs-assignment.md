---
title: Резервације у односу на доделе
description: Ова тема пружа информације о разликама између резервисања ресурса и додељивања ресурса.
author: ruhercul
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8fe6937dfdfe137f28917c16da1d7dc6155284ae
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130236"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="14966-103">Резервације у односу на доделе</span><span class="sxs-lookup"><span data-stu-id="14966-103">Bookings vs assignments</span></span>

<span data-ttu-id="14966-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="14966-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="14966-105">Резервације представљају фиксну или условну расподелу ресурса за пројекат.</span><span class="sxs-lookup"><span data-stu-id="14966-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="14966-106">Фиксне резервације троше капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="14966-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="14966-107">Резервације представљају организационе концепте тимова како би могли да разумеју како ће се ресурси ангажовати на различитим пројектима.</span><span class="sxs-lookup"><span data-stu-id="14966-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="14966-108">Dynamics 365 Project Operations сматра резервације концептом на нивоу пројекта.</span><span class="sxs-lookup"><span data-stu-id="14966-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="14966-109">За разлику од резервација, доделе представљају обавезивање ресурса за пројектне задатке у распореду пројеката.</span><span class="sxs-lookup"><span data-stu-id="14966-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="14966-110">Ресурси могу бити именовани или генерички.</span><span class="sxs-lookup"><span data-stu-id="14966-110">The resources can be named or generic.</span></span> 

<span data-ttu-id="14966-111">Уобичајено је да је збир резервација за ресурс једнак збиру додела ресурса за један или више задатака.</span><span class="sxs-lookup"><span data-stu-id="14966-111">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="14966-112">Међутим, Project Operations не спроводи овај договор.</span><span class="sxs-lookup"><span data-stu-id="14966-112">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="14966-113">Приказ **Усаглашеност** показује менаџеру пројеката места где се резервације и доделе ресурса не слажу.</span><span class="sxs-lookup"><span data-stu-id="14966-113">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>
