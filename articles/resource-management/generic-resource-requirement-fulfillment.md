---
title: Испуњавање генеричких захтева за ресурсима
description: Ова тема пружа информације о томе како да резервишете именоване ресурсе у складу са потребама за генеричким ресурсима.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fef896ae12c196d5566ad54f3e15373020e4e28a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279606"
---
# <a name="generic-resource-requirement-fulfillment"></a><span data-ttu-id="19fc2-103">Испуњавање генеричких захтева за ресурсима</span><span class="sxs-lookup"><span data-stu-id="19fc2-103">Generic resource requirement fulfillment</span></span>

<span data-ttu-id="19fc2-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="19fc2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="19fc2-105">Можете резервисати именовани ресурс да бисте заменили генерички ресурс за којим постоји потреба.</span><span class="sxs-lookup"><span data-stu-id="19fc2-105">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="19fc2-106">На страници **Пројекти**, изаберите картицу **Тим**.</span><span class="sxs-lookup"><span data-stu-id="19fc2-106">On the **Projects** page, select the **Team** tab.</span></span>
2. <span data-ttu-id="19fc2-107">Са листе изаберите генерички ресурс за којим постоји потреба, а затим изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="19fc2-107">Select the generic resource that has a resource requirement from the list, and then select **Book**.</span></span> <span data-ttu-id="19fc2-108">Или отворите потребу за ресурсом, а затим изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="19fc2-108">Or, open the resource requirement and then select **Book**.</span></span>
3. <span data-ttu-id="19fc2-109">На страници **Помоћник за заказивање** изаберите именовани ресурс који ћете резервисати за пројектни тим, а затим изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="19fc2-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then select **Book**.</span></span>

<span data-ttu-id="19fc2-110">Када се резервација доврши и испуни је именовани ресурс, генерички ресурс се замењује именованим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="19fc2-110">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

<span data-ttu-id="19fc2-111">Доделе у распореду се ажурирају и именованим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="19fc2-111">The assignments on the schedule are updated with the named resource as well.</span></span>

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="19fc2-112">Попуњавање генеричког ресурса већим бројем именованих ресурса</span><span class="sxs-lookup"><span data-stu-id="19fc2-112">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="19fc2-113">Испуњавање захтева за генерички ресурс са више именованих ресурса је слично додељивању једног именованог ресурса.</span><span class="sxs-lookup"><span data-stu-id="19fc2-113">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="19fc2-114">На пример, постоји задатак са трајањем од пет дана и 120 сати труда.</span><span class="sxs-lookup"><span data-stu-id="19fc2-114">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="19fc2-115">Овај задатак не може да доврши један ресурс који ради са типичним осмочасовним радним даном у седмици од пет радних дана.</span><span class="sxs-lookup"><span data-stu-id="19fc2-115">This task can't be completed by one resource that works a typical eight-hour day over a five-day week.</span></span> 

<span data-ttu-id="19fc2-116">Захтев је за 120 сати инжењеринга роботике у току пет дана, што је 24 часа дневно.</span><span class="sxs-lookup"><span data-stu-id="19fc2-116">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

<span data-ttu-id="19fc2-117">Ово је пример када је потребно више именованих ресурса за испуњавање генеричког захтева за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="19fc2-117">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="19fc2-118">Биће потребно да резервишете више ресурса да бисте испунили тај захтев.</span><span class="sxs-lookup"><span data-stu-id="19fc2-118">You will need to book multiple resources to fulfill the requirement.</span></span>

<span data-ttu-id="19fc2-119">Главна разлика у овом сценарију је то што генерички ресурс остаје у тиму који је додељен задатку, а резервисани именовани чланови тима ресурса нису додељени као део позиције.</span><span class="sxs-lookup"><span data-stu-id="19fc2-119">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="19fc2-120">Менаџер пројекта може по потреби да додели посао именованим ресурсима.</span><span class="sxs-lookup"><span data-stu-id="19fc2-120">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="19fc2-121">Приказ **Усаглашеност** може да помогне менаџеру пројекта да подели резервације више ресурса на задатке за додељивање.</span><span class="sxs-lookup"><span data-stu-id="19fc2-121">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="19fc2-122">Ово се не ради аутоматски јер у сваком сценарију компликованијем од обичног примера датог изнад, на пример када имате скуп задатака који сачињавају захтев или када систем мора да претпостави како менаџер пројекта намерава да додели ресурсе.</span><span class="sxs-lookup"><span data-stu-id="19fc2-122">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement or the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="19fc2-123">Пошто систем не може да разуме намеру, претпоставке ће се вероватно разликовати од предвиђених, па ће доћи до нетачног или непредвидивог резултата.</span><span class="sxs-lookup"><span data-stu-id="19fc2-123">Because the system can't understand intent, it's likely that the assumptions will be different than intended and an incorrect or unpredictable result will occur.</span></span> <span data-ttu-id="19fc2-124">Предвидив исход је да генерички ресурс остаје додељен док менаџер пројекта намерно не креира доделе, уз помоћ приказа **Усаглашеност**.</span><span class="sxs-lookup"><span data-stu-id="19fc2-124">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]