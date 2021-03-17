---
title: Преглед предложених ресурса
description: Ова тема пружа информације о томе како предложите ресурсе за пројекте.
author: ruhercul
manager: AnnBe
ms.date: 11/05/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fa0515b9d6a0023c05c37d2bcfa6a403f48927cb
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279291"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="2d090-103">Преглед предложених ресурса</span><span class="sxs-lookup"><span data-stu-id="2d090-103">Review proposed resources</span></span>

<span data-ttu-id="2d090-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="2d090-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2d090-105">Менаџери ресурса могу да предложе ресурс менаџеру пројеката коришћењем захтева за ресурс.</span><span class="sxs-lookup"><span data-stu-id="2d090-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="2d090-106">Из мреже захтева или самог захтева изаберите **Пронађи ресурсе**.</span><span class="sxs-lookup"><span data-stu-id="2d090-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="2d090-107">На страници **Помоћник за заказивање** изаберите ресурс, а затим у окну **Креирање резервације ресурса**, у пољу **Статус резервације**, изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="2d090-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="2d090-108">Долази до следећих измена статуса:</span><span class="sxs-lookup"><span data-stu-id="2d090-108">The following status updates occur:</span></span>

- <span data-ttu-id="2d090-109">На страници **Помоћник за заказивање** индикатори статуса се ажурирају како би указали да је резервација предложена, а да ресурс није фиксно резервисан.</span><span class="sxs-lookup"><span data-stu-id="2d090-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="2d090-110">У захтеву за ресурс се статус мења у **Захтева преглед**.</span><span class="sxs-lookup"><span data-stu-id="2d090-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="2d090-111">На картици **Тим** у оквиру пројекта, вредност генеричког члана тима **Статус захтева** се мења у **Захтева преглед**.</span><span class="sxs-lookup"><span data-stu-id="2d090-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="2d090-112">Менаџер пројекта може предлог прихватити или одбацити.</span><span class="sxs-lookup"><span data-stu-id="2d090-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="2d090-113">Када менаџери ресурса обрађују захтеве за ресурсе, могу користити било који од следећих приступа:</span><span class="sxs-lookup"><span data-stu-id="2d090-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="2d090-114">Могу да предлажу више ресурса да би задовољили потражњу ако није доступан ниједан ресурс за испуњавање захтеваних сати.</span><span class="sxs-lookup"><span data-stu-id="2d090-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="2d090-115">Предложени сати се затим деле на више ресурса који могу да задовоље захтеване сате.</span><span class="sxs-lookup"><span data-stu-id="2d090-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="2d090-116">У овом сценарију, сати се не могу преклапати.</span><span class="sxs-lookup"><span data-stu-id="2d090-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="2d090-117">Могу да предлажу мање ресурса него што је потребно.</span><span class="sxs-lookup"><span data-stu-id="2d090-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="2d090-118">У овом сценарију, капацитет предложеног ресурса је мањи од захтеваних сати које је навео подносилац захтева.</span><span class="sxs-lookup"><span data-stu-id="2d090-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="2d090-119">Стога, када подносилац захтева прихвати предложене ресурсе, креира се потреба за неиспуњеним ресурсом да би се евидентирала преостала потражња.</span><span class="sxs-lookup"><span data-stu-id="2d090-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="2d090-120">Могу да резервишу више ресурса да би задовољили потражњу ако није доступан ниједан ресурс за обављање посла.</span><span class="sxs-lookup"><span data-stu-id="2d090-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="2d090-121">Могу да резервишу мање ресурса него што је потребно.</span><span class="sxs-lookup"><span data-stu-id="2d090-121">Book fewer resources than are required.</span></span> <span data-ttu-id="2d090-122">У овом сценарију, број резервисаних сати је мањи од броја захтеваних сати.</span><span class="sxs-lookup"><span data-stu-id="2d090-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="2d090-123">Систем вас упућује да предложите ресурсе уместо резервација, тако да подносилац захтева може да провери и прати преосталу потражњу.</span><span class="sxs-lookup"><span data-stu-id="2d090-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="2d090-124">Доступности ресурса</span><span class="sxs-lookup"><span data-stu-id="2d090-124">Resource availability</span></span>

<span data-ttu-id="2d090-125">Од пресудног је значаја да менаџери ресурса могу да прегледају доступност ресурса и ажурирају резервације.</span><span class="sxs-lookup"><span data-stu-id="2d090-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="2d090-126">У неким случајевима, не постоји формална потражња (захтев за ресурс), али менаџер ресурса мора да одговори на непланирану потражњу која долази преко канала попут е-поште, телефонског позива или тренутне поруке.</span><span class="sxs-lookup"><span data-stu-id="2d090-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="2d090-127">Менаџери ресурса користе таблу распореда за ажурирање ресурса и резервација.</span><span class="sxs-lookup"><span data-stu-id="2d090-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="2d090-128">Радно време ресурса користи се као основа за израчунавање доступности ресурса.</span><span class="sxs-lookup"><span data-stu-id="2d090-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="2d090-129">Резервације ресурса троше капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="2d090-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="2d090-130">Табела распореда користи боје и сенчења да би приказала резервације, доступност и пребукираност, као и статус резервација.</span><span class="sxs-lookup"><span data-stu-id="2d090-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="2d090-131">Поставка у подешавањима табеле распореда омогућава вам да прикажете легенду.</span><span class="sxs-lookup"><span data-stu-id="2d090-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="2d090-132">Ако се стрелица усмерена удесно појави поред појединачног ресурса који се може резервисати у табели распореда, ресурс се може проширити и показати детаље посла за који је ресурс резервисан.</span><span class="sxs-lookup"><span data-stu-id="2d090-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="2d090-133">Пошто Dynamics 365 Project Operations користи Universal Resource Scheduling механизам, ако сте инсталирали и Dynamics 365 Field Service, можете прегледати детаље о резервацијама ресурса за пројекте, радним налозима и било којим другим ентитетима за које сте проширили заказивање.</span><span class="sxs-lookup"><span data-stu-id="2d090-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="2d090-134">Да бисте видели више детаља о појединачном ресору, кликните десним тастером миша на ресурс да бисте отворили картицу ресурса.</span><span class="sxs-lookup"><span data-stu-id="2d090-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]