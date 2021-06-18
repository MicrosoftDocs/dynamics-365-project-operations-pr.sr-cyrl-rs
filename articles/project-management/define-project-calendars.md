---
title: Дефинисање календара пројеката
description: Ова тема пружа информације о томе како применити шаблон календара на пројекат за праћење распореда пројеката.
author: ruhercul
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 0d1a2c4bd2d4022bbf79afcef79170eb482e6418
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999014"
---
# <a name="define-project-calendars"></a><span data-ttu-id="fba87-103">Дефинисање календара пројеката</span><span class="sxs-lookup"><span data-stu-id="fba87-103">Define project calendars</span></span>

<span data-ttu-id="fba87-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="fba87-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="fba87-105">Да бисте креирали и управљали пројектом, на њега морате применити шаблон календара.</span><span class="sxs-lookup"><span data-stu-id="fba87-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="fba87-106">Предложак календара дефинише следеће атрибуте пројекта:</span><span class="sxs-lookup"><span data-stu-id="fba87-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="fba87-107">Радно време, укључујући време почетка и завршетка</span><span class="sxs-lookup"><span data-stu-id="fba87-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="fba87-108">Радни дани</span><span class="sxs-lookup"><span data-stu-id="fba87-108">Working days</span></span>
- <span data-ttu-id="fba87-109">Изузеци из календара као што су нерадни дани</span><span class="sxs-lookup"><span data-stu-id="fba87-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="fba87-110">Шаблон календара који се примењује на пројекат је копија шаблона календара дефинисаног у подешавањима ваше организације.</span><span class="sxs-lookup"><span data-stu-id="fba87-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="fba87-111">Ако промените шаблон календара, те промене се неће пренети на радно време пројекта.</span><span class="sxs-lookup"><span data-stu-id="fba87-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="fba87-112">Да бисте променили радно време пројекта, мора се применити нови образац.</span><span class="sxs-lookup"><span data-stu-id="fba87-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="fba87-113">Да бисте креирали шаблон календара за своју организацију, постоје два кључна захтева:</span><span class="sxs-lookup"><span data-stu-id="fba87-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="fba87-114">Дефинишите жељено радно време шаблона помоћу новог или постојећег ресурса који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="fba87-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="fba87-115">Направите нови шаблон календара и повежите га са ресурсом који можете резервирати.</span><span class="sxs-lookup"><span data-stu-id="fba87-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="fba87-116">**Дефинишите радно време шаблона**</span><span class="sxs-lookup"><span data-stu-id="fba87-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="fba87-117">Идите на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="fba87-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="fba87-118">Направите нови ресурс за референцу у предлошку календара или одаберите постојећи.</span><span class="sxs-lookup"><span data-stu-id="fba87-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="fba87-119">Изаберите картицу ресурса **Радно време** и довршите упутства у [Поставите радно време за ресурс](/dynamics365/field-service/set-work-hours-resource.md) за конфигурисање правила календара.</span><span class="sxs-lookup"><span data-stu-id="fba87-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="fba87-120">**Креирајте нови предложак календара**</span><span class="sxs-lookup"><span data-stu-id="fba87-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="fba87-121">Идите на **Подешавања** \> **Шаблон календара**.</span><span class="sxs-lookup"><span data-stu-id="fba87-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="fba87-122">Изаберите **Ново** и унесите име, опис и ресурс шаблона.</span><span class="sxs-lookup"><span data-stu-id="fba87-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="fba87-123">Када се на ресурс наводи шаблон календара, копија календара ресурса придружује се шаблону календара.</span><span class="sxs-lookup"><span data-stu-id="fba87-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="fba87-124">Ако промените радно време копираног шаблона, те промене се неће пренети на радно време календара.</span><span class="sxs-lookup"><span data-stu-id="fba87-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="fba87-125">Сада можете повезати радни предложак са предлошком календара пројекта.</span><span class="sxs-lookup"><span data-stu-id="fba87-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

