---
title: Креирање предлошка за радне сате
description: Ова тема описује како да креирате предлошке за радне сате у апликацији Project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 525f601ad6fee902cb6d5c128b596cc2d33f30c4
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981273"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="50820-103">Креирање предлошка радних сати (Project Service)</span><span class="sxs-lookup"><span data-stu-id="50820-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="50820-104">Да бисте креирали и управљали пројектом, на њега морате применити шаблон календара.</span><span class="sxs-lookup"><span data-stu-id="50820-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="50820-105">Предложак календара дефинише следеће атрибуте пројекта:</span><span class="sxs-lookup"><span data-stu-id="50820-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="50820-106">Радно време, укључујући време почетка и завршетка</span><span class="sxs-lookup"><span data-stu-id="50820-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="50820-107">Радни дани</span><span class="sxs-lookup"><span data-stu-id="50820-107">Working days</span></span>
- <span data-ttu-id="50820-108">Изузеци из календара као што су нерадни дани</span><span class="sxs-lookup"><span data-stu-id="50820-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="50820-109">Шаблон календара који се примењује на пројекат је копија шаблона календара дефинисаног у подешавањима ваше организације.</span><span class="sxs-lookup"><span data-stu-id="50820-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="50820-110">Ако промените шаблон календара, те промене се неће пренети на радно време пројекта.</span><span class="sxs-lookup"><span data-stu-id="50820-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="50820-111">Да бисте променили радно време пројекта, мора се применити нови образац.</span><span class="sxs-lookup"><span data-stu-id="50820-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="50820-112">Да бисте креирали шаблон календара за своју организацију, постоје два кључна захтева:</span><span class="sxs-lookup"><span data-stu-id="50820-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="50820-113">Дефинишите жељено радно време шаблона помоћу новог или постојећег ресурса који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="50820-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="50820-114">Направите нови шаблон календара и повежите га са ресурсом који можете резервирати.</span><span class="sxs-lookup"><span data-stu-id="50820-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="50820-115">**Дефинишите радно време шаблона**</span><span class="sxs-lookup"><span data-stu-id="50820-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="50820-116">Идите на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="50820-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="50820-117">Направите нови ресурс за референцу у предлошку календара или одаберите постојећи.</span><span class="sxs-lookup"><span data-stu-id="50820-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="50820-118">Изаберите картицу ресурса **Радно време** и довршите упутства у [Поставите радно време за ресурс](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) за конфигурисање правила календара.</span><span class="sxs-lookup"><span data-stu-id="50820-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="50820-119">**Креирајте нови предложак календара**</span><span class="sxs-lookup"><span data-stu-id="50820-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="50820-120">Идите на **Подешавања** \> **Шаблон календара**.</span><span class="sxs-lookup"><span data-stu-id="50820-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="50820-121">Изаберите **Ново** и унесите име, опис и ресурс шаблона.</span><span class="sxs-lookup"><span data-stu-id="50820-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="50820-122">Када се на ресурс наводи шаблон календара, копија календара ресурса придружује се шаблону календара.</span><span class="sxs-lookup"><span data-stu-id="50820-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="50820-123">Ако промените радно време копираног шаблона, те промене се неће пренети на радно време календара.</span><span class="sxs-lookup"><span data-stu-id="50820-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="50820-124">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="50820-124">See Also</span></span>  
 [<span data-ttu-id="50820-125">Подешавање ресурса</span><span class="sxs-lookup"><span data-stu-id="50820-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
