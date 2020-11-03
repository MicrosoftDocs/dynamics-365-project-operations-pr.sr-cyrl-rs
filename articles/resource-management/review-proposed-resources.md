---
title: Преглед предложених ресурса
description: Ова тема пружа информације о томе како предложите ресурсе за пројекте.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: ad5cbdeb5fe05e6115eb024833a8d58b626ea4c9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083939"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="0a080-103">Преглед предложених ресурса</span><span class="sxs-lookup"><span data-stu-id="0a080-103">Review proposed resources</span></span>

<span data-ttu-id="0a080-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="0a080-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0a080-105">Менаџери ресурса могу да предложе ресурс менаџеру пројеката коришћењем захтева за ресурс.</span><span class="sxs-lookup"><span data-stu-id="0a080-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="0a080-106">Из мреже захтева или самог захтева изаберите **Пронађи ресурсе**.</span><span class="sxs-lookup"><span data-stu-id="0a080-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="0a080-107">На страници **Помоћник за заказивање** изаберите ресурс, а затим у окну **Креирање резервације ресурса** , у пољу **Статус резервације** , изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="0a080-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="0a080-108">Долази до следећих измена статуса:</span><span class="sxs-lookup"><span data-stu-id="0a080-108">The following status updates occur:</span></span>

- <span data-ttu-id="0a080-109">На страници **Помоћник за заказивање** индикатори статуса се ажурирају како би указали да је резервација предложена, а да ресурс није фиксно резервисан.</span><span class="sxs-lookup"><span data-stu-id="0a080-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="0a080-110">У захтеву за ресурс се статус мења у **Захтева преглед**.</span><span class="sxs-lookup"><span data-stu-id="0a080-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="0a080-111">На картици **Тим** у оквиру пројекта, вредност генеричког члана тима **Статус захтева** се мења у **Захтева преглед**.</span><span class="sxs-lookup"><span data-stu-id="0a080-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="0a080-112">Менаџер пројекта може предлог прихватити или одбацити.</span><span class="sxs-lookup"><span data-stu-id="0a080-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="0a080-113">Када менаџери ресурса обрађују захтеве за ресурсе, могу користити било који од следећих приступа:</span><span class="sxs-lookup"><span data-stu-id="0a080-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="0a080-114">Могу да предлажу више ресурса да би задовољили потражњу ако није доступан ниједан ресурс за испуњавање захтеваних сати.</span><span class="sxs-lookup"><span data-stu-id="0a080-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="0a080-115">Предложени сати се затим деле на више ресурса који могу да задовоље захтеване сате.</span><span class="sxs-lookup"><span data-stu-id="0a080-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="0a080-116">У овом сценарију, сати се не могу преклапати.</span><span class="sxs-lookup"><span data-stu-id="0a080-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="0a080-117">Могу да предлажу мање ресурса него што је потребно.</span><span class="sxs-lookup"><span data-stu-id="0a080-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="0a080-118">У овом сценарију, капацитет предложеног ресурса је мањи од захтеваних сати које је навео подносилац захтева.</span><span class="sxs-lookup"><span data-stu-id="0a080-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="0a080-119">Стога, када подносилац захтева прихвати предложене ресурсе, креира се потреба за неиспуњеним ресурсом да би се евидентирала преостала потражња.</span><span class="sxs-lookup"><span data-stu-id="0a080-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="0a080-120">Могу да резервишу више ресурса да би задовољили потражњу ако није доступан ниједан ресурс за обављање посла.</span><span class="sxs-lookup"><span data-stu-id="0a080-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="0a080-121">Могу да резервишу мање ресурса него што је потребно.</span><span class="sxs-lookup"><span data-stu-id="0a080-121">Book fewer resources than are required.</span></span> <span data-ttu-id="0a080-122">У овом сценарију, број резервисаних сати је мањи од броја захтеваних сати.</span><span class="sxs-lookup"><span data-stu-id="0a080-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="0a080-123">Систем вас упућује да предложите ресурсе уместо резервација, тако да подносилац захтева може да провери и прати преосталу потражњу.</span><span class="sxs-lookup"><span data-stu-id="0a080-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="0a080-124">Наплатива укупна искоришћеност</span><span class="sxs-lookup"><span data-stu-id="0a080-124">Billable utilization</span></span>

<span data-ttu-id="0a080-125">Ресурси могу имати циљану наплативу укупну искоришћеност.</span><span class="sxs-lookup"><span data-stu-id="0a080-125">Resources can have a target billable utilization.</span></span> <span data-ttu-id="0a080-126">Она је дефинисана као атрибут подразумеване улоге ресурса или је подешена у запису појединачног ресурса који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="0a080-126">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="0a080-127">Израчунавање укупне искоришћености темељи се на стварним сатима које су ресурси пријавили коришћењем одобрених ставки времена.</span><span class="sxs-lookup"><span data-stu-id="0a080-127">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="0a080-128">Следеће формуле се користе за израчунавање укупне искоришћености:</span><span class="sxs-lookup"><span data-stu-id="0a080-128">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="0a080-129">Наплатива укупна искоришћеност = наплативи стварни сати ÷ капацитет ресурса</span><span class="sxs-lookup"><span data-stu-id="0a080-129">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="0a080-130">Ненаплатива укупна искоришћеност = Стварно време са ID-ом врсте наплате = Ненаплативо, допунско или недоступно ÷ Капацитет ресурса</span><span class="sxs-lookup"><span data-stu-id="0a080-130">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="0a080-131">Интерно = Стварно време без продајног уговора ÷ Капацитет ресурса</span><span class="sxs-lookup"><span data-stu-id="0a080-131">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="0a080-132">Капацитет ресурса = Радно време ресурса – Ван канцеларије – Нерадни дани</span><span class="sxs-lookup"><span data-stu-id="0a080-132">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="0a080-133">Можете пронаћи приказ **Укупна искоришћеност ресурса** у окну **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="0a080-133">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="0a080-134">Свака ћелија у мрежи представља проценат наплативе укупне искоришћености ресурса у неком периоду, као што је дан, недеља или месец.</span><span class="sxs-lookup"><span data-stu-id="0a080-134">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="0a080-135">Следеће формуле се користе за бојење ћелија:</span><span class="sxs-lookup"><span data-stu-id="0a080-135">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="0a080-136">**Зелена:** Наплатива укупна искоришћеност \>= циљна укупна искоришћеност ресурса</span><span class="sxs-lookup"><span data-stu-id="0a080-136">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="0a080-137">**Жута:** циљна укупна искоришћеност – 20 \<= наплатива укупна искоришћеност \< циљна укупна искоришћеност</span><span class="sxs-lookup"><span data-stu-id="0a080-137">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="0a080-138">**Црвена:** наплатива укупна искоришћеност \< циљна укупна искоришћеност – 20</span><span class="sxs-lookup"><span data-stu-id="0a080-138">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="0a080-139">Због тога што је приказ **Укупна искоришћеност ресурса** заснована на табли распореда, за филтрирање резултата можете користити могућности филтрирања табле распореда.</span><span class="sxs-lookup"><span data-stu-id="0a080-139">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="0a080-140">Мрежа захтева да подесите циљну укупну искоришћеност за улогу или појединачни ресурс.</span><span class="sxs-lookup"><span data-stu-id="0a080-140">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="0a080-141">Да бисте то подесили, идите на ставку **Ресурси** \> **Улоге ресурса**.</span><span class="sxs-lookup"><span data-stu-id="0a080-141">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="0a080-142">Уз то, сваком ресурсу који се може резервисати мора се доделити подразумевана улога.</span><span class="sxs-lookup"><span data-stu-id="0a080-142">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="0a080-143">Идите на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="0a080-143">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="0a080-144">На картици **Project Service** потврдите да је дефинисана улога ресурса и да је поље **Је подразумевано** за ту улогу подешено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="0a080-144">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="0a080-145">Ако **Је подразумевано = Не** , можете додати додатне улоге.</span><span class="sxs-lookup"><span data-stu-id="0a080-145">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="0a080-146">Улога где **Је подразумевано = Да** користи се за процену укупне искоришћености ресурса у односу на циљну искоришћеност за ту улогу.</span><span class="sxs-lookup"><span data-stu-id="0a080-146">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="0a080-147">На картици **Project Service** можете подесити и појединачну циљну укупну искоришћеност за ресурс.</span><span class="sxs-lookup"><span data-stu-id="0a080-147">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="0a080-148">Калкулација укупне искоришћености затим користи ту циљну укупну искоришћеност за процену циља ресурса уместо циља подразумеване улоге ресурса.</span><span class="sxs-lookup"><span data-stu-id="0a080-148">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="0a080-149">Укупна искоришћеност је приказана за ресурс само ако је тај ресурс одобрио наплативо време током периода који је приказан на мрежи.</span><span class="sxs-lookup"><span data-stu-id="0a080-149">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="0a080-150">Доступности ресурса</span><span class="sxs-lookup"><span data-stu-id="0a080-150">Resource availability</span></span>

<span data-ttu-id="0a080-151">Од пресудног је значаја да менаџери ресурса могу да прегледају доступност ресурса и ажурирају резервације.</span><span class="sxs-lookup"><span data-stu-id="0a080-151">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="0a080-152">У неким случајевима, не постоји формална потражња (захтев за ресурс), али менаџер ресурса мора да одговори на непланирану потражњу која долази преко канала попут е-поште, телефонског позива или тренутне поруке.</span><span class="sxs-lookup"><span data-stu-id="0a080-152">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="0a080-153">Менаџери ресурса користе таблу распореда за ажурирање ресурса и резервација.</span><span class="sxs-lookup"><span data-stu-id="0a080-153">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="0a080-154">Радно време ресурса користи се као основа за израчунавање доступности ресурса.</span><span class="sxs-lookup"><span data-stu-id="0a080-154">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="0a080-155">Резервације ресурса троше капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="0a080-155">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="0a080-156">Табела распореда користи боје и сенчења да би приказала резервације, доступност и пребукираност, као и статус резервација.</span><span class="sxs-lookup"><span data-stu-id="0a080-156">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="0a080-157">Поставка у подешавањима табеле распореда омогућава вам да прикажете легенду.</span><span class="sxs-lookup"><span data-stu-id="0a080-157">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="0a080-158">Ако се стрелица усмерена удесно појави поред појединачног ресурса који се може резервисати у табели распореда, ресурс се може проширити и показати детаље посла за који је ресурс резервисан.</span><span class="sxs-lookup"><span data-stu-id="0a080-158">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="0a080-159">Пошто Dynamics 365 Project Operations користи Universal Resource Scheduling механизам, ако сте инсталирали и Dynamics 365 Field Service, можете прегледати детаље о резервацијама ресурса за пројекте, радним налозима и било којим другим ентитетима за које сте проширили заказивање.</span><span class="sxs-lookup"><span data-stu-id="0a080-159">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="0a080-160">Да бисте видели више детаља о појединачном ресору, кликните десним тастером миша на ресурс да бисте отворили картицу ресурса.</span><span class="sxs-lookup"><span data-stu-id="0a080-160">To view more details about an individual resource, right-click it to open the resource card.</span></span>

