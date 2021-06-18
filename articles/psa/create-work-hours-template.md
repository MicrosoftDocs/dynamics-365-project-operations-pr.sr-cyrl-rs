---
title: Креирање предлошка за радне сате
description: Ова тема описује како да креирате предлошке за радне сате у апликацији Project Service.
author: ruhercul
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
ms.openlocfilehash: 105e3cb2ef7b904e96dc21013906e0b7444e3b88
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997214"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="29296-103">Креирање предлошка радних сати (Project Service)</span><span class="sxs-lookup"><span data-stu-id="29296-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="29296-104">Да бисте креирали и управљали пројектом, на њега морате применити шаблон календара.</span><span class="sxs-lookup"><span data-stu-id="29296-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="29296-105">Предложак календара дефинише следеће атрибуте пројекта:</span><span class="sxs-lookup"><span data-stu-id="29296-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="29296-106">Радно време, укључујући време почетка и завршетка</span><span class="sxs-lookup"><span data-stu-id="29296-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="29296-107">Радни дани</span><span class="sxs-lookup"><span data-stu-id="29296-107">Working days</span></span>
- <span data-ttu-id="29296-108">Изузеци из календара као што су нерадни дани</span><span class="sxs-lookup"><span data-stu-id="29296-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="29296-109">Шаблон календара који се примењује на пројекат је копија шаблона календара дефинисаног у подешавањима ваше организације.</span><span class="sxs-lookup"><span data-stu-id="29296-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="29296-110">Ако промените шаблон календара, те промене се неће пренети на радно време пројекта.</span><span class="sxs-lookup"><span data-stu-id="29296-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="29296-111">Да бисте променили радно време пројекта, мора се применити нови образац.</span><span class="sxs-lookup"><span data-stu-id="29296-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="29296-112">Да бисте креирали шаблон календара за своју организацију, постоје два кључна захтева:</span><span class="sxs-lookup"><span data-stu-id="29296-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="29296-113">Дефинишите жељено радно време шаблона помоћу новог или постојећег ресурса који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="29296-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="29296-114">Направите нови шаблон календара и повежите га са ресурсом који можете резервирати.</span><span class="sxs-lookup"><span data-stu-id="29296-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="29296-115">**Дефинишите радно време шаблона**</span><span class="sxs-lookup"><span data-stu-id="29296-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="29296-116">Идите на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="29296-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="29296-117">Направите нови ресурс за референцу у предлошку календара или одаберите постојећи.</span><span class="sxs-lookup"><span data-stu-id="29296-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="29296-118">Изаберите картицу ресурса **Радно време** и довршите упутства у [Поставите радно време за ресурс](/dynamics365/field-service/set-work-hours-resource.md) за конфигурисање правила календара.</span><span class="sxs-lookup"><span data-stu-id="29296-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="29296-119">**Креирајте нови предложак календара**</span><span class="sxs-lookup"><span data-stu-id="29296-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="29296-120">Идите на **Подешавања** \> **Шаблон календара**.</span><span class="sxs-lookup"><span data-stu-id="29296-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="29296-121">Изаберите **Ново** и унесите име, опис и ресурс шаблона.</span><span class="sxs-lookup"><span data-stu-id="29296-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="29296-122">Када се на ресурс наводи шаблон календара, копија календара ресурса придружује се шаблону календара.</span><span class="sxs-lookup"><span data-stu-id="29296-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="29296-123">Ако промените радно време копираног шаблона, те промене се неће пренети на радно време календара.</span><span class="sxs-lookup"><span data-stu-id="29296-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="29296-124">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="29296-124">See Also</span></span>  
 [<span data-ttu-id="29296-125">Подешавање ресурса</span><span class="sxs-lookup"><span data-stu-id="29296-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
