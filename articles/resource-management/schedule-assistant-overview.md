---
title: Преглед помоћника за заказивање
description: Ова тема пружа информације о раду са помоћником за планирање ради резервисања ресурса.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: da551e805f395e466952df1dbb7d193bdddba358
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908552"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="24456-103">Преглед помоћника за заказивање</span><span class="sxs-lookup"><span data-stu-id="24456-103">Schedule assistant overview</span></span>

<span data-ttu-id="24456-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="24456-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="24456-105">Помоћник за планирање се користи за резервисање ресурса на основу захтева које је дефинисао менаџер пројекта.</span><span class="sxs-lookup"><span data-stu-id="24456-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="24456-106">Помоћник за планирање се ослања на параметре наведене у захтеву за ресурсом да би пронашао ресурс.</span><span class="sxs-lookup"><span data-stu-id="24456-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="24456-107">Помоћник за планирање препоручује ресурсе који одговарају релевантним захтевима, попут доступних времена или потребних вештина.</span><span class="sxs-lookup"><span data-stu-id="24456-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="24456-108">Када се идентификују одговарајући ресурси, менаџер ресурса или пројекта може резервисати ресурс за рад.</span><span class="sxs-lookup"><span data-stu-id="24456-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24456-109">Предуслови</span><span class="sxs-lookup"><span data-stu-id="24456-109">Prerequisites</span></span>

<span data-ttu-id="24456-110">Помоћник за планирање је део решења Universal Resource Scheduling.</span><span class="sxs-lookup"><span data-stu-id="24456-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="24456-111">Ово решење је укључено и инсталирано са услугама Dynamics 365 Project Operations, Dynamics 365 Field Service и Dynamics 365 Customer Service.</span><span class="sxs-lookup"><span data-stu-id="24456-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="24456-112">Захтеви и ресурси који се подударају</span><span class="sxs-lookup"><span data-stu-id="24456-112">Matching requirements and resources</span></span>

<span data-ttu-id="24456-113">Захтев за генерисаним ресурсом заснива се на детаљима као што су:</span><span class="sxs-lookup"><span data-stu-id="24456-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="24456-114">Карактеристике</span><span class="sxs-lookup"><span data-stu-id="24456-114">Characteristics</span></span>
-   <span data-ttu-id="24456-115">Улоге</span><span class="sxs-lookup"><span data-stu-id="24456-115">Roles</span></span>
-   <span data-ttu-id="24456-116">Пословне јединице</span><span class="sxs-lookup"><span data-stu-id="24456-116">Business units</span></span>
-   <span data-ttu-id="24456-117">Жељене поставке ресурса</span><span class="sxs-lookup"><span data-stu-id="24456-117">Resource preferences</span></span>
-   <span data-ttu-id="24456-118">Контуре ангажовања</span><span class="sxs-lookup"><span data-stu-id="24456-118">Effort contours</span></span>
-   <span data-ttu-id="24456-119">Временска зона</span><span class="sxs-lookup"><span data-stu-id="24456-119">Time zone</span></span>

<span data-ttu-id="24456-120">Помоћник за планирање користи ове детаље за филтрирање ресурса.</span><span class="sxs-lookup"><span data-stu-id="24456-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="24456-121">Покретање помоћника за планирање</span><span class="sxs-lookup"><span data-stu-id="24456-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="24456-122">Постоје два начина на које се покреће помоћник за планирање.</span><span class="sxs-lookup"><span data-stu-id="24456-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="24456-123">Ако користите хибридни режим, у мрежи члана тима можете да изаберете било ког члана тима са неиспуњеним захтевима за ресурсима, а затим изаберите **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="24456-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="24456-124">Ако користите централни режим, менаџер ресурса проналази и бира ресурс.</span><span class="sxs-lookup"><span data-stu-id="24456-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="24456-125">Филтер помоћника за планирање</span><span class="sxs-lookup"><span data-stu-id="24456-125">Schedule assistant filters</span></span>

<span data-ttu-id="24456-126">Након покретања помоћника за планирање, детаљи из захтева за ресурсом приказују се као филтриране вредности у левом окну.</span><span class="sxs-lookup"><span data-stu-id="24456-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="24456-127">Менаџер ресурса или менаџер пројеката могу прецизно подесити резултате прилагођавањем филтера како би удовољили потребама распореда.</span><span class="sxs-lookup"><span data-stu-id="24456-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="24456-128">Окно филтера приказује опције везане за посао, укључујући:</span><span class="sxs-lookup"><span data-stu-id="24456-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="24456-129">Почетак и завршетак посла</span><span class="sxs-lookup"><span data-stu-id="24456-129">Work start and end</span></span>
-   <span data-ttu-id="24456-130">Карактеристике</span><span class="sxs-lookup"><span data-stu-id="24456-130">Characteristics</span></span>
-   <span data-ttu-id="24456-131">Улоге</span><span class="sxs-lookup"><span data-stu-id="24456-131">Roles</span></span>
-   <span data-ttu-id="24456-132">Организационе јединице</span><span class="sxs-lookup"><span data-stu-id="24456-132">Organizational units</span></span>
-   <span data-ttu-id="24456-133">Предузеће које обезбеђује ресурсе</span><span class="sxs-lookup"><span data-stu-id="24456-133">Resourcing company</span></span>
-   <span data-ttu-id="24456-134">Типови ресурса</span><span class="sxs-lookup"><span data-stu-id="24456-134">Resource types</span></span>
-   <span data-ttu-id="24456-135">Жељени ресурси</span><span class="sxs-lookup"><span data-stu-id="24456-135">Preferred resources</span></span>
