---
title: Потребе за условним резервисањем
description: Ова тема пружа информације о томе како да резервишете ресурсе према потребама за условним резервисањем.
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
ms.openlocfilehash: e753dd2f5635d1e9d0d6a02ea5d1d537879dd3a5
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124116"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="55c06-103">Потребе за условним резервисањем</span><span class="sxs-lookup"><span data-stu-id="55c06-103">Soft-book requirements</span></span>

<span data-ttu-id="55c06-104">Потреба за ресурсом може се фиксно резервисати.</span><span class="sxs-lookup"><span data-stu-id="55c06-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="55c06-105">Фиксна резервација креира предлог који троши капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="55c06-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="55c06-106">Предлог се затим враћа подносиоцу захтева на одобрење.</span><span class="sxs-lookup"><span data-stu-id="55c06-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="55c06-107">Условно резервисање привремено додаје ресурса у пројектни тим и има другачији статус у табели распореда, али не троши капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="55c06-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="55c06-108">Да бисте условно резервисали ресурс из табеле распореда, подесите поље **Статус резервације** на **Условна**.</span><span class="sxs-lookup"><span data-stu-id="55c06-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

![Статус резервације је подешен на Условна](media/Resource-Management-image77.png)

<span data-ttu-id="55c06-110">Када картица **Тим** има приказ **Именовани чланови тима**, ресурс се појављује тамо.</span><span class="sxs-lookup"><span data-stu-id="55c06-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="55c06-111">Условно резервисани сати се евидентирају у колони **Условно резервисани сати**.</span><span class="sxs-lookup"><span data-stu-id="55c06-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

![Условно резервисани сати у приказу Именовани чланови тима](media/Resource-Management-image78.png)

<span data-ttu-id="55c06-113">Условно резервисани чланови тима могу бити додељени задацима.</span><span class="sxs-lookup"><span data-stu-id="55c06-113">Soft-booked team members can be assigned to tasks.</span></span>

![Условно резервисан члан тима је додељен задатку](media/Resource-Management-image79.png)

<span data-ttu-id="55c06-115">На картици **Усаглашеност** нису приказане резервације условно резервисаног ресурса јер картица **Усаглашеност** узима у обзир само фиксне резервације.</span><span class="sxs-lookup"><span data-stu-id="55c06-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![Условно резервисан ресурс без резервација на картици Усаглашеност](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="55c06-117">Не можете условно да резервишете ресурс из потребе која је генерисана од генеричког члана тима.</span><span class="sxs-lookup"><span data-stu-id="55c06-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="55c06-118">На табели распореда употребљава се другачија боја за условне резервације ресурса.</span><span class="sxs-lookup"><span data-stu-id="55c06-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![Условне резервације у табели распореда](media/Resource-Management-image81.png)

<span data-ttu-id="55c06-120">Да бисте условну резервацију претворили у фиксну, у табели распореда кликните десним тастером миша на условна резервација, а затим изаберите **Промени статус** \> **Фиксна резервација** \> **Фиксна**.</span><span class="sxs-lookup"><span data-stu-id="55c06-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![Промена статуса резервације у Фиксна](media/Resource-Management-image82.png)

<span data-ttu-id="55c06-122">Резервација је промењена и статус се мења у табели распореда.</span><span class="sxs-lookup"><span data-stu-id="55c06-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="55c06-123">Пошто је статус резервације сада **Фиксна**, ресурс је приказан као резервисан, а његов капацитет и доступност су прилагођени.</span><span class="sxs-lookup"><span data-stu-id="55c06-123">Because the booking status is now **Hard**, the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="55c06-124">Можете употребити исти метод да откажете фиксну резервацију или условну резервацију у табели распореда.</span><span class="sxs-lookup"><span data-stu-id="55c06-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="55c06-125">Да бисте претворили ресурс који је условно резервисан у фиксно резервисан на картици пројекта **Тим**, изаберите ресурс, а затим изаберите **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="55c06-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![Команда за потврду](media/Resource-Management-image83.png)
