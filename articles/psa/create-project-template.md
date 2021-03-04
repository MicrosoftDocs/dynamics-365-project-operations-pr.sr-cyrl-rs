---
title: Креирајте предложак пројекта
description: Како да креирате предложак за пројекат у апликацији Project Service
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
ms.openlocfilehash: efc404131208e1c971cb091cf174c1f4707552f0
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149381"
---
# <a name="create-a-project-template-project-service"></a><span data-ttu-id="77295-103">Креирање предлошка за пројекат (Project Service)</span><span class="sxs-lookup"><span data-stu-id="77295-103">Create a project template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="77295-104">Предлошци пројекта вам штеде време ако ваше предузеће редовно лицитира за сличне типове пројеката.</span><span class="sxs-lookup"><span data-stu-id="77295-104">Project templates save you time if your company regularly bids on similar types of projects.</span></span> <span data-ttu-id="77295-105">Они обезбеђују стандардни скуп улога и процењених часова за тип пројекта.</span><span class="sxs-lookup"><span data-stu-id="77295-105">They provide a standard set of roles and estimated hours for a type of project.</span></span> <span data-ttu-id="77295-106">Менаџери пословног контакта и менаџери пројекта могу да креирају пројекте на основу предлошка пројекта или могу да копирају предложак и направе свој сопствени.</span><span class="sxs-lookup"><span data-stu-id="77295-106">Account managers and project managers can create projects based on a project template, or they can copy the template and make one of their own.</span></span>  
  
## <a name="components-of-project-template"></a><span data-ttu-id="77295-107">Компоненте предлошка пројекта</span><span class="sxs-lookup"><span data-stu-id="77295-107">Components of project template</span></span>
 <span data-ttu-id="77295-108">Предложак пројекта се састоји од три компоненте:</span><span class="sxs-lookup"><span data-stu-id="77295-108">A project template consists of three components:</span></span>  
  
- <span data-ttu-id="77295-109">**Структурна анализа посла**: Структурна анализа посла у предлошку пројекта има исти скуп елемената као и пројекат.</span><span class="sxs-lookup"><span data-stu-id="77295-109">**Work breakdown structure**: A work breakdown structure in a project template has the same set of elements as in the project.</span></span> <span data-ttu-id="77295-110">Можете да креирате хијерархију задатка, повезујете улоге са задатком, дефинишете распоред атрибута, постављате зависности и прегледате све податке у гантограму.</span><span class="sxs-lookup"><span data-stu-id="77295-110">You can create a task hierarchy, associate roles to task, define schedule attributes, set dependencies and view all the data in the Gantt.</span></span> <span data-ttu-id="77295-111">Структурна анализа посла у предлошцима пројекта такође подржава режиме задатака за сваки задатак.</span><span class="sxs-lookup"><span data-stu-id="77295-111">The work breakdown structure in project templates also support task modes for each task.</span></span> <span data-ttu-id="77295-112">Нема разлике између предлошка пројекта и пројекта приликом креирања радног распореда.</span><span class="sxs-lookup"><span data-stu-id="77295-112">There is no difference between a project template and a project when creating work schedule.</span></span>  
  
- <span data-ttu-id="77295-113">**Процене за пројекат**: Процене за пројекат у предлошцима функционишу на исти начин као у пројектима, осим што су ценовници са подразумеваним ценама трошкова и продајним ценама увек подразумевани ценовници трошкова и продаје дефинисани у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] параметрима.</span><span class="sxs-lookup"><span data-stu-id="77295-113">**Project estimates**: Project estimates in templates work the same way as they do in projects, except the price lists for defaulting the cost and sales prices are always the default cost and sales price lists defined in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parameters.</span></span> <span data-ttu-id="77295-114">Остале функционалности су исте као у пројекту.</span><span class="sxs-lookup"><span data-stu-id="77295-114">The rest of the functionality is the same as in a project.</span></span>  
  
- <span data-ttu-id="77295-115">**Формирање пројектног тима**: Када формирате пројектни тим за предложак пројекта, не можете резервисати именовани ресурс у предлошку.</span><span class="sxs-lookup"><span data-stu-id="77295-115">**Project team formation**: When forming a project team for a project template, you can’t book a named resource in a template.</span></span> <span data-ttu-id="77295-116">Можете да користите **Генерисање пројектног тима** у структурној анализи посла да бисте генерисали скуп генеричких ресурса.</span><span class="sxs-lookup"><span data-stu-id="77295-116">You can use **Generate Project Team** in the work breakdown structure to generate a set of generic resources.</span></span> <span data-ttu-id="77295-117">Такође можете навести потребне вештине и стручности за генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="77295-117">You can also specify required skills and proficiencies for generic resources.</span></span> <span data-ttu-id="77295-118">У предлошцима пројекта није могуће заменити генерички ресурс ресурсом који може да се резервише.</span><span class="sxs-lookup"><span data-stu-id="77295-118">You can’t substitute a generic resource with a bookable resource in project templates.</span></span>  
  
## <a name="create-a-project-from-a-template"></a><span data-ttu-id="77295-119">Креирање пројекта из предлошка</span><span class="sxs-lookup"><span data-stu-id="77295-119">Create a project from a template</span></span>  
 <span data-ttu-id="77295-120">Пројекат из предлошка можете да креирате на следеће начине:</span><span class="sxs-lookup"><span data-stu-id="77295-120">You can create a project from a template in these following ways:</span></span>  
  
-   <span data-ttu-id="77295-121">Када креирате пројекат из понуде, можете одабрати предложак пројекта у обрасцу за брзо креирање пројекта.</span><span class="sxs-lookup"><span data-stu-id="77295-121">When creating a project from the quote, you can choose a project template in the project quick create form.</span></span>  
  
-   <span data-ttu-id="77295-122">Приликом креирања пројекта кликом на **Нови пројекат**, образац пројекта се приказује пре него што сачувате запис.</span><span class="sxs-lookup"><span data-stu-id="77295-122">When creating a project by clicking **New Project**, the project form displays before you save the record.</span></span> <span data-ttu-id="77295-123">Одавде, можете да кликнете на поље **Изаберите предложак** да бисте одабрали из листе унапред дефинисаних предложака пројеката у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="77295-123">From here, you can click **Pick a template** field to choose from the list of pre-defined project templates in your organization.</span></span>  
  
-   <span data-ttu-id="77295-124">Кликните на **Креирај пројекат из предлошка** на страници **Предложак пројекта** да бисте креирали пројекат из предлошка.</span><span class="sxs-lookup"><span data-stu-id="77295-124">Click **Create project from a template** on the **Project Template** page to create a project from the template.</span></span>  
  
## <a name="copying-components-of-a-template-to-a-project"></a><span data-ttu-id="77295-125">Креирање компоненти предлошка у пројекат</span><span class="sxs-lookup"><span data-stu-id="77295-125">Copying components of a template to a project</span></span>  
 <span data-ttu-id="77295-126">Када копирате компоненте предлошка у пројекат, има неколико ствари о којима би требало да знате.</span><span class="sxs-lookup"><span data-stu-id="77295-126">When you copy components of a template into a project, there are a few things you should know about.</span></span>  
  
 <span data-ttu-id="77295-127">**Копирање структурне анализе посла**: Када копирате структурну анализу посла из предлошка пројекта, ако пројекат има другачији календар пројекта него предложак, радни часови из календара пројекта ће бити примењени на распоред задатака.</span><span class="sxs-lookup"><span data-stu-id="77295-127">**Copying a work breakdown structure**: When you copy the work breakdown structure from a project template, if the project has a different project calendar than the template, the work hours from the project’s calendar will be applied to the schedule of tasks.</span></span> <span data-ttu-id="77295-128">Овим се распоред прилагођава календару који подржава пројекат.</span><span class="sxs-lookup"><span data-stu-id="77295-128">This adjusts the schedule to the backing project calendar.</span></span> <span data-ttu-id="77295-129">Слично, први задатак у структурној анализи посла почиње на датум почетка пројекта, тако да се остатак распореда хијерархије задатака ажурира на основу трајања и зависности наведене у структурној анализи посла за предложак.</span><span class="sxs-lookup"><span data-stu-id="77295-129">Similarly, the first task on the work breakdown structure takes the project’s start date, so the rest of the task hierarchy schedule is updated based on the duration and dependencies specified in the template’s work breakdown structure.</span></span>  
  
 <span data-ttu-id="77295-130">**Копирање процена за пројекат**: Када копирате у све ставке процене пројекта, ценовници се ажурирају на основу власничке јединице пројекта за ценовник трошкова и клијента за продајни ценовник.</span><span class="sxs-lookup"><span data-stu-id="77295-130">**Copying project estimates**: When you copy across project estimate lines, price lists are updated based on the owning unit of the project for the cost price list and customer for the sales price list.</span></span> <span data-ttu-id="77295-131">Трошкови по јединици и продајне цене се утврђују из ових ценовника на пројектима који су повезани са ентитетом продаје.</span><span class="sxs-lookup"><span data-stu-id="77295-131">The unit cost and sales prices are determined from these price lists on projects that are associated to a sales entity.</span></span>  
  
 <span data-ttu-id="77295-132">**Копирање пројектног тима**: Када копирате пројектни тим из предлошка у пројекат, копирају се сви генерички ресурси, заједно са вештинама и стручношћу дефинисаним у предлошку.</span><span class="sxs-lookup"><span data-stu-id="77295-132">**Copying a project team**: When you copy the project team from the template to a project, the generic resources are copied across, along with the skills and proficiencies defined in the template.</span></span> <span data-ttu-id="77295-133">Доделе генеричких ресурса такође се одржавају као предложак пројекта.</span><span class="sxs-lookup"><span data-stu-id="77295-133">Generic resource assignments are also maintained as in the project template.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="77295-134">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="77295-134">See Also</span></span>  
 [<span data-ttu-id="77295-135">Водич за менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="77295-135">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
