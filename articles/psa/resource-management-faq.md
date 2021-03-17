---
title: Најчешћа питања о управљању ресурсима
description: Ова тема нуди одговоре на најчешћа питања о управљању ресурсима.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 20562b98ccc8451ab57dd42fb8c2f9f303811dbe
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283161"
---
# <a name="resource-management-faq"></a><span data-ttu-id="685d0-103">Најчешћа питања о управљању ресурсима</span><span class="sxs-lookup"><span data-stu-id="685d0-103">Resource management FAQ</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a><span data-ttu-id="685d0-104">Која је разлика између члана тима и потребе за ресурсом?</span><span class="sxs-lookup"><span data-stu-id="685d0-104">What is the difference between a team member and a resource requirement?</span></span>

<span data-ttu-id="685d0-105">Члан пројектног тима може бити додељен задацима, резервисан или пребукиран, као и подешен као давалац одобрења.</span><span class="sxs-lookup"><span data-stu-id="685d0-105">A project team member can be assigned to tasks, booked or overbooked, and set as an approver.</span></span> <span data-ttu-id="685d0-106">Потреба за ресурсом може постојати без члана пројектног тима, као радна верзија напомене о потражњи.</span><span class="sxs-lookup"><span data-stu-id="685d0-106">A resource requirement can exist without a project team member, as a draft note of demand.</span></span> 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a><span data-ttu-id="685d0-107">Која је разлика између предложених и условно резервираних сати?</span><span class="sxs-lookup"><span data-stu-id="685d0-107">What is the difference between proposed and soft-booked hours?</span></span>

<span data-ttu-id="685d0-108">Предложени сати и условно резервисани сати разликују се по видљивости.</span><span class="sxs-lookup"><span data-stu-id="685d0-108">Proposed hours and soft-booked hours differ in visibility.</span></span> <span data-ttu-id="685d0-109">Предложени сати су видљиви само менаџерима ресурса и менаџеру пројеката који су покренули потражњу користећи захтев за ресурс.</span><span class="sxs-lookup"><span data-stu-id="685d0-109">Proposed hours are visible only to resource managers and the project manager who initiated the demand by using a resource request.</span></span> <span data-ttu-id="685d0-110">Условно резервисани сати су видљиви свима који имају приступ табели распореда.</span><span class="sxs-lookup"><span data-stu-id="685d0-110">Soft-booked hours are visible to anyone who has access to the Schedule Board.</span></span>

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a><span data-ttu-id="685d0-111">Како могу да видим условно резервисане сате за ресурсе у тиму?</span><span class="sxs-lookup"><span data-stu-id="685d0-111">How can I see the soft-booked hours for resources on a team?</span></span>

<span data-ttu-id="685d0-112">Условне резервације можете да обавите када резервишете потребу за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="685d0-112">Soft bookings can made when you book a resource requirement.</span></span> <span data-ttu-id="685d0-113">Ресурси који су условно резервисани у пројектном тиму приказују се као чланови тима који имају условно резервисане сате.</span><span class="sxs-lookup"><span data-stu-id="685d0-113">Resources that are soft-booked on a project team appear as team members who have soft-booked hours.</span></span> <span data-ttu-id="685d0-114">Приказују се и на табели распореда.</span><span class="sxs-lookup"><span data-stu-id="685d0-114">They also appear on the Schedule Board.</span></span>

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a><span data-ttu-id="685d0-115">Како да променим захтеване сате, датум почетка и завршетка за (генерички или именовани) ресурс који је резервисан?</span><span class="sxs-lookup"><span data-stu-id="685d0-115">How do I change the required hours, and the start and end dates, for a resource (generic or named) that I booked?</span></span>

<span data-ttu-id="685d0-116">Након резервисања ресурса, изаберите **Одржавање резервација** да унесете промене које су неопходне.</span><span class="sxs-lookup"><span data-stu-id="685d0-116">After resources are booked, select **Maintain Bookings** to make any changes that are required.</span></span>

## <a name="what-resources-types-does-project-service-automation-support"></a><span data-ttu-id="685d0-117">Које врсте ресурса подржава Project Service Automation?</span><span class="sxs-lookup"><span data-stu-id="685d0-117">What resources types does Project Service Automation support?</span></span>

<span data-ttu-id="685d0-118">**Корисник** и **Контакт** су једине врсте ресурса које подржава Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="685d0-118">**User** and **Contact** are the only resource types that are supported in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="685d0-119">Иако можете да креирате друге врсте ресурса (на пример, **Опрема** и **Група**), ниједан случај њиховог комплетног коришћења није подржан.</span><span class="sxs-lookup"><span data-stu-id="685d0-119">Although you can create other types of resources (for example, **Equipment** and **Group**), no end-to-end use case is supported for them.</span></span>

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a><span data-ttu-id="685d0-120">Која је разлика између доделе и резервације?</span><span class="sxs-lookup"><span data-stu-id="685d0-120">What is the difference between an assignment and a booking?</span></span>

<span data-ttu-id="685d0-121">Доделе представљају додела ресурса пројектним задацима у распореду пројеката.</span><span class="sxs-lookup"><span data-stu-id="685d0-121">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="685d0-122">Ресурси могу бити стварни или генерички ресурси.</span><span class="sxs-lookup"><span data-stu-id="685d0-122">The resources can be either real or generic resources.</span></span> <span data-ttu-id="685d0-123">Резервације представљају фиксну или условну расподелу ресурса за пројекат.</span><span class="sxs-lookup"><span data-stu-id="685d0-123">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="685d0-124">Фиксне резервације троше капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="685d0-124">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="685d0-125">Идеално би било да се за стварне ресурсе слажу резервације и доделе, јер се не разликују.</span><span class="sxs-lookup"><span data-stu-id="685d0-125">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="685d0-126">Међутим, PSA не спроводи овај договор.</span><span class="sxs-lookup"><span data-stu-id="685d0-126">However, PSA doesn't enforce this agreement.</span></span> <span data-ttu-id="685d0-127">Приказ Усаглашеност показује менаџеру пројеката места где се резервације и доделе ресурса не слажу.</span><span class="sxs-lookup"><span data-stu-id="685d0-127">The Reconciliation view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]