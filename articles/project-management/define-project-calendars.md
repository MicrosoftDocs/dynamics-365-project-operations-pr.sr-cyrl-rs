---
title: Дефинисање календара пројеката
description: Ова тема пружа информације о коришћењу календара пројекта за праћење распореда пројеката.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
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
ms.openlocfilehash: 774399f2c02d8434c9c042c3a9f995792893bfce
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084146"
---
# <a name="define-project-calendars"></a><span data-ttu-id="ffff0-103">Дефинисање календара пројеката</span><span class="sxs-lookup"><span data-stu-id="ffff0-103">Define project calendars</span></span>

<span data-ttu-id="ffff0-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="ffff0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ffff0-105">Да бисте креирали распоред пројекта, креирајте предложак календара пројекта који дефинише број радних сати по дану и све прекиде пословних активности.</span><span class="sxs-lookup"><span data-stu-id="ffff0-105">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="ffff0-106">Да бисте креирали предложак календара пројекта, радни предложак повезујете са пољем **Предложак календара** за пројекат.</span><span class="sxs-lookup"><span data-stu-id="ffff0-106">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="ffff0-107">Следите ове кораке за креирање радног предлошка.</span><span class="sxs-lookup"><span data-stu-id="ffff0-107">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="ffff0-108">У левом окну за навигацију изаберите **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="ffff0-108">In the left navigation pane, select **Resources**.</span></span> 
2. <span data-ttu-id="ffff0-109">На страници листе **Ресурси** отворите запис корисника, а затим изаберите **Прикажи радно време**.</span><span class="sxs-lookup"><span data-stu-id="ffff0-109">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="ffff0-110">Обавезно дозволите искачуће прозоре на страници прегледача.</span><span class="sxs-lookup"><span data-stu-id="ffff0-110">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="ffff0-111">Ово вам омогућава да видите радно време подешено за ресурс.</span><span class="sxs-lookup"><span data-stu-id="ffff0-111">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="ffff0-112">На картици **Месечни приказ** изаберите **Подешавање**.</span><span class="sxs-lookup"><span data-stu-id="ffff0-112">On the **Monthly View** tab, select **Set Up**.</span></span> <span data-ttu-id="ffff0-113">Појавиће се листа са три опције:</span><span class="sxs-lookup"><span data-stu-id="ffff0-113">A list of three options appears:</span></span> 

  - <span data-ttu-id="ffff0-114">Нови седмични распоред</span><span class="sxs-lookup"><span data-stu-id="ffff0-114">New Weekly Schedule</span></span>
  - <span data-ttu-id="ffff0-115">Распоред посла за један дан</span><span class="sxs-lookup"><span data-stu-id="ffff0-115">Work Schedule for One Day</span></span>
  - <span data-ttu-id="ffff0-116">Одступање у времену</span><span class="sxs-lookup"><span data-stu-id="ffff0-116">Time Off</span></span>

4. <span data-ttu-id="ffff0-117">Изаберите **Нови седмични распоред** , а затим подесите опције за овај распоред ресурса.</span><span class="sxs-lookup"><span data-stu-id="ffff0-117">Select **New Weekly Schedule** , and then set the options for this resource schedule.</span></span> <span data-ttu-id="ffff0-118">Можете подесити периодични седмични распоред, параметре сата у дану, прекид пословних активности и још много тога.</span><span class="sxs-lookup"><span data-stu-id="ffff0-118">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="ffff0-119">Подесите опсег датума, изаберите **Сачувај** , а затим изаберите **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="ffff0-119">Set the date range, select **Save** , and then select **Close**.</span></span> 
6. <span data-ttu-id="ffff0-120">Вратите се на страницу листе **Ресурси** и одаберите ресурс за који сте одредили радно време.</span><span class="sxs-lookup"><span data-stu-id="ffff0-120">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="ffff0-121">Изаберите **Подесите календар као** да подесили радни предложак.</span><span class="sxs-lookup"><span data-stu-id="ffff0-121">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="ffff0-122">У дијалог **Радни предложак** унесите име радног предлошка, а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="ffff0-122">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="ffff0-123">Сада можете повезати радни предложак са предлошком календара пројекта.</span><span class="sxs-lookup"><span data-stu-id="ffff0-123">You can now associate the work template with a project calendar template.</span></span>
