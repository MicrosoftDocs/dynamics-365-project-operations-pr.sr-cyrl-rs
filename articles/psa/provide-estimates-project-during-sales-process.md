---
title: Обезбедите радне процене за пројекат током продајног процеса
description: Како да обезбедите радне процене за пројекат током продајног процеса у апликацији Project Service
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
ms.openlocfilehash: 7bd83b6872d437f1d074d6ea2336c751bdfdd9e6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120606"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a><span data-ttu-id="2c032-103">Обезбедите радне процене за пројекат током продајног процеса (Project Service)</span><span class="sxs-lookup"><span data-stu-id="2c032-103">Provide work estimates for a project during the sales process (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="2c032-104">Током процеса продаје, можете правити процене продаје одоздо нагоре са предметима понуде.</span><span class="sxs-lookup"><span data-stu-id="2c032-104">During the sales process, you can work out sales estimates from the ground up with quote lines.</span></span> <span data-ttu-id="2c032-105">Могућности [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у систему [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] пружају више научни и детерминистички начин за добијање процена продаје раздвајањем ставки посла и повезивањем релевантних атрибута који доприносе проценама за пројекат у структурној анализи посла.</span><span class="sxs-lookup"><span data-stu-id="2c032-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] provide a more scientific and deterministic way of coming up with sales estimates by breaking down work items and associating relevant attributes that contribute toward the estimates for the project in the work breakdown structure.</span></span>  
  
 <span data-ttu-id="2c032-106">Након што успете да продате, можете да користите повезану структурну анализу посла у плану пројекта, по потреби је прецизирајући ради успешног обављања пројекта.</span><span class="sxs-lookup"><span data-stu-id="2c032-106">Once you win the sale, you can use the associated work breakdown structure in your project plan, refining it as necessary for successful completion of your project.</span></span>  
  
## <a name="link-a-project-to-a-quote-line"></a><span data-ttu-id="2c032-107">Повезивање пројекта са ставком понуде</span><span class="sxs-lookup"><span data-stu-id="2c032-107">Link a project to a quote line</span></span>  
 <span data-ttu-id="2c032-108">Када креирате ставку понуде на основу пројекта, можете да креирате нови пројекат од ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="2c032-108">When creating a project-based quote line, you can create a new project from the quote line.</span></span> <span data-ttu-id="2c032-109">Затим можете да користите предлошке пројекта који су или унапред конфигурисани стандардни планови пројекта и финансијске процене уобичајене за вашу организацију или копије плана пројекта и процене из прошлог пројекта.</span><span class="sxs-lookup"><span data-stu-id="2c032-109">You can then use project templates, which are either pre-configured standard project plans and financial estimates common to your organization, or a copy of a project plan and estimates from a past project.</span></span> <span data-ttu-id="2c032-110">Када креирате пројекат, избор предлошка пројекта пружа основу за прецизирање плана пројекта, процена и захтева за ресурсима.</span><span class="sxs-lookup"><span data-stu-id="2c032-110">When you create a project, choosing a project template provides a basis to refine the project plan, estimates, and role requirements.</span></span> <span data-ttu-id="2c032-111">Креирањем пројекта из понуде, пројекат се аутоматски повезује са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="2c032-111">By creating your project from the quote, the project is automatically associated with the quote line.</span></span>  
  
## <a name="project-estimate-components"></a><span data-ttu-id="2c032-112">Компоненте процене за пројекат</span><span class="sxs-lookup"><span data-stu-id="2c032-112">Project estimate components</span></span>  
 <span data-ttu-id="2c032-113">Структурна анализа посла за пројекат обезбеђује начин да поделите рад у задатке, одржавате хијерархију задатака и доделите процену труда потребног да бисте довршили сваки задатак.</span><span class="sxs-lookup"><span data-stu-id="2c032-113">The work breakdown structure in a project provides a way to break down work into tasks, maintain a hierarchy of tasks, and assign an estimate of effort required to complete each task.</span></span> <span data-ttu-id="2c032-114">Такође можете да повежете улоге са задатком да бисте указали на процену типа ресурса који су потребни за довршење задатка и распореда.</span><span class="sxs-lookup"><span data-stu-id="2c032-114">You can also associate roles to a task to indicate an estimate of the type of resource required to complete a task and a schedule.</span></span>  
  
 <span data-ttu-id="2c032-115">Структурна анализа посла вам помаже да одредите процене рада и распореда.</span><span class="sxs-lookup"><span data-stu-id="2c032-115">The work breakdown structure helps you determine work effort and schedule estimates.</span></span> <span data-ttu-id="2c032-116">Подразумевано пројекат користи подразумеване ценовнике које сте раније дефинисали.</span><span class="sxs-lookup"><span data-stu-id="2c032-116">By default, the project uses default price lists that you defined earlier.</span></span> <span data-ttu-id="2c032-117">Цене трошкова и продаје дефинисане у ценовницима помажу у утврђивању финансијских процена за анализу посла за пројекат.</span><span class="sxs-lookup"><span data-stu-id="2c032-117">The cost and sales prices defined in the price lists help determine financial estimates for the project’s work breakdown.</span></span>  
  
 <span data-ttu-id="2c032-118">Ако је ваш пројекат повезан са понудом, а понуде има неки други ценовник од подразумеваног, ценовник понуде се користи за финансијске процене.</span><span class="sxs-lookup"><span data-stu-id="2c032-118">If your project is associated with a quote, and the quote has a different price list from the default, the quote’s price list is used for financial estimates.</span></span>  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="2c032-119">Увоз процена из пројекта у понуду</span><span class="sxs-lookup"><span data-stu-id="2c032-119">Import estimates from a project into a quote</span></span>  
 <span data-ttu-id="2c032-120">Када имате процене за пројекат у пројекту, можете увозити ове процене у ставке понуде:</span><span class="sxs-lookup"><span data-stu-id="2c032-120">Once you have project estimates in the project, you can import these estimates into the quote line:</span></span>  
  
-   <span data-ttu-id="2c032-121">У **Детаљи ставке понуде**, кликните на **Увези из процена**.</span><span class="sxs-lookup"><span data-stu-id="2c032-121">In **Quote Line Details**, click **Import from estimates**.</span></span> 

-   <span data-ttu-id="2c032-122">Изаберите да ли да увезете процене за пројекат груписане по типу трансакције, улози или нивоу чвора структурне анализе посла.</span><span class="sxs-lookup"><span data-stu-id="2c032-122">Select whether to import project estimates summarized by transaction type, role, or work breakdown structure node level.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="2c032-123">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="2c032-123">See Also</span></span>  
 [<span data-ttu-id="2c032-124">Водич за менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="2c032-124">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
