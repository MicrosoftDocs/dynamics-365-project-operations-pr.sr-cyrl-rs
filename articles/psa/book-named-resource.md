---
title: Резервисање именованих ресурса из потребе за ресурсима
description: Ова тема пружа информације о резервисању именованих ресурса у складу са потребама за генеричким ресурсима.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: d7ff58ec08661adc702867c6c26805a74a3637c9
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125916"
---
# <a name="book-named-resources-from-resource-requirements"></a><span data-ttu-id="24ca1-103">Резервисање именованих ресурса из потребе за ресурсима</span><span class="sxs-lookup"><span data-stu-id="24ca1-103">Book named resources from resource requirements</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="24ca1-104">Можете резервисати именовани ресурс да бисте заменили генерички ресурс за којим постоји потреба.</span><span class="sxs-lookup"><span data-stu-id="24ca1-104">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="24ca1-105">У апликацији Project Service Automation (PSA), на страници **Пројекти** кликните на картицу **Тим**.</span><span class="sxs-lookup"><span data-stu-id="24ca1-105">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab.</span></span>
2. <span data-ttu-id="24ca1-106">Са листе изаберите генерички ресурс за којим постоји потреба, а затим кликните на **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="24ca1-106">Select the generic resource that has a resource requirement from the list and then click **Book**.</span></span> <span data-ttu-id="24ca1-107">Или отворите потребу за ресурсом, а затим кликните на **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="24ca1-107">Or, open the resource requirement and then click **Book**.</span></span>


![Резервисање генеричког члана тима](media/RM-how-to-14.png)


3. <span data-ttu-id="24ca1-109">На страници **Помоћник за заказивање** изаберите именовани ресурс који ћете резервисати за пројектни тим, а затим кликните на **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="24ca1-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then click **Book**.</span></span>

![Резервисање генеричког члана тима помоћу помоћника за заказивање](media/RM-how-to-15.png)

<span data-ttu-id="24ca1-111">Када се резервација доврши и испуни је именовани ресурс, генерички ресурс се замењује именованим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="24ca1-111">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

![Именовани члан тима који замењује генеричког члана тима](media/RM-how-to-16.png)

<span data-ttu-id="24ca1-113">Доделе у распореду се ажурирају и именованим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="24ca1-113">The assignments on the schedule are updated with the named resource as well.</span></span>

![Именовани члан тима додељен пројектним задацима](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="24ca1-115">Попуњавање генеричког ресурса већим бројем именованих ресурса</span><span class="sxs-lookup"><span data-stu-id="24ca1-115">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="24ca1-116">Испуњавање захтева за генерички ресурс са више именованих ресурса је слично додељивању једног именованог ресурса.</span><span class="sxs-lookup"><span data-stu-id="24ca1-116">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="24ca1-117">На пример, постоји задатак са трајањем од пет дана и 120 сати труда.</span><span class="sxs-lookup"><span data-stu-id="24ca1-117">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="24ca1-118">Овај задатак не може да доврши један ресурс који ради са типичним осмочасовним радним даном у седмици од пет радних дана.</span><span class="sxs-lookup"><span data-stu-id="24ca1-118">This task can't be completed by one resource that works a typical eight-hour day over a five day week.</span></span> 

![Задатак који треба 120 сати труда током периода од пет дана](media/RM-how-to-21.png)

<span data-ttu-id="24ca1-120">Захтев је за 120 сати инжењеринга роботике у току пет дана, што је 24 часа дневно.</span><span class="sxs-lookup"><span data-stu-id="24ca1-120">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

![Захтев по дану](media/RM-how-to-22.png)

<span data-ttu-id="24ca1-122">Ово је пример када је потребно више именованих ресурса за испуњавање генеричког захтева за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="24ca1-122">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="24ca1-123">Биће потребно да резервишете више ресурса да бисте испунили тај захтев.</span><span class="sxs-lookup"><span data-stu-id="24ca1-123">You will need to book multiple resources to fulfill the requirement.</span></span>

![Резервисање више ресурса ради испуњавања захтева](media/RM-how-to-23.png)

<span data-ttu-id="24ca1-125">Главна разлика у овом сценарију је то што генерички ресурс остаје у тиму који је додељен задатку, а резервисани именовани чланови тима ресурса нису додељени као део позиције.</span><span class="sxs-lookup"><span data-stu-id="24ca1-125">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="24ca1-126">Менаџер пројекта може по потреби да додели посао именованим ресурсима.</span><span class="sxs-lookup"><span data-stu-id="24ca1-126">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="24ca1-127">Приказ **Усаглашеност** може да помогне менаџеру пројекта да подели резервације више ресурса на задатке за додељивање.</span><span class="sxs-lookup"><span data-stu-id="24ca1-127">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="24ca1-128">Ово се не ради аутоматски јер у сваком сценарију компликованијем од обичног примера датог изнад, на пример када имате скуп задатака који сачињавају захтев, систем мора да претпостави како менаџер пројекта намерава да додели ресурсе.</span><span class="sxs-lookup"><span data-stu-id="24ca1-128">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement, the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="24ca1-129">Пошто систем не може да разуме намеру, постоје шансе да ће се претпоставке разликовати од предвиђених, па ће доћи до нетачног или непредвидивог резултата.</span><span class="sxs-lookup"><span data-stu-id="24ca1-129">Because the system can't understand intent, chances are that the assumptions will be different than intended and an incorrect or unpredictable result will happen.</span></span> <span data-ttu-id="24ca1-130">Предвидив исход је да генерички ресурс остаје додељен док менаџер пројекта намерно не креира доделе, уз помоћ приказа **Усаглашеност**.</span><span class="sxs-lookup"><span data-stu-id="24ca1-130">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>


