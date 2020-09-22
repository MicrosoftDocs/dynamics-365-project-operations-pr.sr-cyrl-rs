---
title: Предлошци пројеката
description: Ова тема пружа информације о томе како користити предлошке пројекта за брзо подешавање пројекта.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: f0161bf9-af4c-4a21-b767-ac20a8e30688
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5a3112c2eef9525946314bdb587c44904557fa52
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755349"
---
# <a name="project-templates"></a><span data-ttu-id="b52b7-103">Предлошци пројеката</span><span class="sxs-lookup"><span data-stu-id="b52b7-103">Project templates</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b52b7-104">Предложак пројекта је унапред дефинисан оквир који вам помаже да брзо и лако покренете пројекат.</span><span class="sxs-lookup"><span data-stu-id="b52b7-104">A project template is a predefined framework that helps you quickly and easily start a project.</span></span> <span data-ttu-id="b52b7-105">Можете да користите унапред дефинисани предложак за креирање новог пројекта једним кликом.</span><span class="sxs-lookup"><span data-stu-id="b52b7-105">You can use a predefined template to create a new project with a single click.</span></span> <span data-ttu-id="b52b7-106">Што се тиче пројеката, морате дефинисати предуслове за предлошке пројеката.</span><span class="sxs-lookup"><span data-stu-id="b52b7-106">As for projects, you must define the prerequisites for project templates.</span></span> <span data-ttu-id="b52b7-107">Морате дефинисати календар пројекта за сваки предложак пројекта, а улоге и ценовници морају бити унапред дефинисани у организацији како би компоненте предлошка имале корисне податке.</span><span class="sxs-lookup"><span data-stu-id="b52b7-107">You must define a project calendar for each project template, and roles and price lists must be predefined in the organization, so that the components of the template have useful data.</span></span>

<span data-ttu-id="b52b7-108">Предложак пројекта састоји се од три компоненте: распоред, процене пројекта и чланови пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="b52b7-108">A project template consists of three components: a schedule, project estimates, and project team members.</span></span>

## <a name="schedule"></a><span data-ttu-id="b52b7-109">Распоред</span><span class="sxs-lookup"><span data-stu-id="b52b7-109">Schedule</span></span>

<span data-ttu-id="b52b7-110">Распоред у предлошку пројекта има исти скуп елемената као и распоред у пројекту.</span><span class="sxs-lookup"><span data-stu-id="b52b7-110">A schedule in a project template has the same set of elements as a schedule in a project.</span></span> <span data-ttu-id="b52b7-111">Можете да креирате хијерархију задатка, повезујете улоге са задацима, дефинишете распоред атрибута и подешавате зависне елементе.</span><span class="sxs-lookup"><span data-stu-id="b52b7-111">You can create a task hierarchy, associate roles with tasks, define schedule attributes, and set dependencies.</span></span> <span data-ttu-id="b52b7-112">Распоред у предлошку пројекта такође подржава режиме задатака за сваки задатак.</span><span class="sxs-lookup"><span data-stu-id="b52b7-112">A schedule in a project template also supports task modes for each task.</span></span> <span data-ttu-id="b52b7-113">Стога подржава и систем за заказивање.</span><span class="sxs-lookup"><span data-stu-id="b52b7-113">Therefore, it supports the scheduling engine.</span></span> <span data-ttu-id="b52b7-114">Морате повезати календар пројекта са пројектом.</span><span class="sxs-lookup"><span data-stu-id="b52b7-114">You must associate a project calendar with the project.</span></span> <span data-ttu-id="b52b7-115">Када креирате радни распоред, нема разлике између предлошка пројекта и пројекта.</span><span class="sxs-lookup"><span data-stu-id="b52b7-115">When you create a work schedule, there is no difference between a project template and a project.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="b52b7-116">Процене за пројекат</span><span class="sxs-lookup"><span data-stu-id="b52b7-116">Project estimates</span></span>

<span data-ttu-id="b52b7-117">Процене пројекта у обрасцу пројекта функционишу на исти начин као процене пројекта у пројекту.</span><span class="sxs-lookup"><span data-stu-id="b52b7-117">Project estimates in a project template work the same way as project estimates in a project.</span></span> <span data-ttu-id="b52b7-118">Међутим, цене трошкова и продајне цене се преузимају из подразумеваних ценовника трошкова и продајних ценовника које су дефинисани у параметрима.</span><span class="sxs-lookup"><span data-stu-id="b52b7-118">However, the cost and sales prices are pulled from the default cost and sales price lists that are defined in the parameters.</span></span>

## <a name="creating-a-project-from-a-template"></a><span data-ttu-id="b52b7-119">Креирање пројекта из предлошка</span><span class="sxs-lookup"><span data-stu-id="b52b7-119">Creating a project from a template</span></span>
 
<span data-ttu-id="b52b7-120">Постоји неколико начина за креирање пројекта из предлошка пројекта:</span><span class="sxs-lookup"><span data-stu-id="b52b7-120">There are several ways to create a project from a project template:</span></span>

- <span data-ttu-id="b52b7-121">Када креирате пројекат из понуде, можете одабрати предложак пројекта у дијалогу за **брзо креирање пројекта**.</span><span class="sxs-lookup"><span data-stu-id="b52b7-121">When you create a project from a quote, you can select a project template in the **Quick Create: Project** dialog box.</span></span>

> ![Дијалог за брзо креирање пројекта](media/project-11.png)

- <span data-ttu-id="b52b7-123">Када креирате пројекат одабиром опције **Нови пројекат**, страница **Пројекат** се појављује пре него што се запис сачува.</span><span class="sxs-lookup"><span data-stu-id="b52b7-123">When you create a project by selecting **New Project**, the **Project** page appears before the record is saved.</span></span> <span data-ttu-id="b52b7-124">У пољу **Избор предлошка** изаберите један од унапред дефинисаних предложака пројеката у организацији.</span><span class="sxs-lookup"><span data-stu-id="b52b7-124">In the **Pick a Template** field, select one of the predefined project templates in the organization.</span></span>
- <span data-ttu-id="b52b7-125">Употребите **Креирање пројекта из предлошка** на страници **Ентитет предлошка**.</span><span class="sxs-lookup"><span data-stu-id="b52b7-125">Use **Create Project from a Template** on the **Template Entity** page.</span></span>

## <a name="copying-components-of-template-to-project"></a><span data-ttu-id="b52b7-126">Копирање компоненти предлошка у пројекат</span><span class="sxs-lookup"><span data-stu-id="b52b7-126">Copying components of template to project</span></span>

<span data-ttu-id="b52b7-127">Када копирате компоненте предлошка пројекта у пројекат, може се догодити неколико замена, зависно од подешавања у пројекту.</span><span class="sxs-lookup"><span data-stu-id="b52b7-127">When you copy the components of a project template to a project, a few overrides can occur, depending on the settings in the project.</span></span>

### <a name="copying-the-schedule"></a><span data-ttu-id="b52b7-128">Копирање распореда</span><span class="sxs-lookup"><span data-stu-id="b52b7-128">Copying the schedule</span></span>

<span data-ttu-id="b52b7-129">Када копирате распоред из предлошка пројекта, ако пројекат има другачији календар пројекта него предложак, радно време из календара пројекта се примењује на распоред задатака.</span><span class="sxs-lookup"><span data-stu-id="b52b7-129">When you copy the schedule from a project template, if the project has a different project calendar than the template, work hours from the project's calendar are applied to the task schedule.</span></span> <span data-ttu-id="b52b7-130">На овај начин се распоред прилагођава како би одговарао календару који подржава пројекат.</span><span class="sxs-lookup"><span data-stu-id="b52b7-130">In this way, the schedule is adjusted to match the backing project calendar.</span></span> <span data-ttu-id="b52b7-131">Слично, први задатак у распореду почиње на датум почетка пројекта, а остатак распореда хијерархије се ажурира на основу трајања и зависних елемената наведених у предлошку.</span><span class="sxs-lookup"><span data-stu-id="b52b7-131">Similarly, the first task on the schedule takes the project's start date, and the schedule of the rest of the hierarchy is updated based on the duration and dependencies that are specified in the template.</span></span> 

### <a name="copying-project-estimates"></a><span data-ttu-id="b52b7-132">Копирање процена пројекта</span><span class="sxs-lookup"><span data-stu-id="b52b7-132">Copying project estimates</span></span> 

<span data-ttu-id="b52b7-133">Када копирате више ставки процене пројеката, ценовници се ажурирају.</span><span class="sxs-lookup"><span data-stu-id="b52b7-133">When you copy across project estimate lines, the price lists are updated.</span></span> <span data-ttu-id="b52b7-134">У ценовнику трошкова, ове исправке су засноване на јединици која је власник пројекта.</span><span class="sxs-lookup"><span data-stu-id="b52b7-134">For the cost price list, these updates are based on the owning unit of the project.</span></span> <span data-ttu-id="b52b7-135">У ценовнику продаје засноване су на клијенту.</span><span class="sxs-lookup"><span data-stu-id="b52b7-135">For the sales price list, they are based on the customer.</span></span> <span data-ttu-id="b52b7-136">Када су у питању пројекти који су повезани са ентитетом продаје, трошкови по јединици и продајне цене се утврђују на основу ових ценовника.</span><span class="sxs-lookup"><span data-stu-id="b52b7-136">For projects that are associated with a sales entity, the unit cost and sales prices are determined based on these price lists.</span></span>

### <a name="copying-a-project-team"></a><span data-ttu-id="b52b7-137">Копирање пројектног тима</span><span class="sxs-lookup"><span data-stu-id="b52b7-137">Copying a project team</span></span>

<span data-ttu-id="b52b7-138">Када копирате пројектни тим из предлошка пројекта у пројекат, копирају се генерички ресурси, заједно са вештинама и стручношћу дефинисаним у предлошку.</span><span class="sxs-lookup"><span data-stu-id="b52b7-138">When a project team is copied from a project template to a project, the generic resources are copied, together with the skills and proficiencies that are defined in the template.</span></span> <span data-ttu-id="b52b7-139">Доделе генеричких ресурса такође се одржавају као у предлошку пројекта.</span><span class="sxs-lookup"><span data-stu-id="b52b7-139">Generic resource assignments are also maintained as they were in the project template.</span></span> <span data-ttu-id="b52b7-140">Именовани ресурси нису подржани у предлошцима пројеката.</span><span class="sxs-lookup"><span data-stu-id="b52b7-140">Named resources aren't supported in project templates.</span></span>
