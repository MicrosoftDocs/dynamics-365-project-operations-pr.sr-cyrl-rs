---
title: Креирајте пројекат
description: Како да креирате пројекат у апликацији Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/13/2020
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
ms.openlocfilehash: 164dff56bb61f6d9bc4cf0b0678a25e0169a31ee
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285096"
---
# <a name="create-a-project-project-service"></a><span data-ttu-id="b3932-103">Креирање пројекта (Project Service)</span><span class="sxs-lookup"><span data-stu-id="b3932-103">Create a project (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="b3932-104">Креирајте пројекат помоћу могућности [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у систему [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] када желите да креирате могућност за пословање, понуду или уговор за услуге на основу пројекта.</span><span class="sxs-lookup"><span data-stu-id="b3932-104">Create a project using the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] when you want to create an opportunity, quote, or contract for project-based services.</span></span> <span data-ttu-id="b3932-105">Могућности [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] вам помажу да управљате пројектом од могућности за пословање до завршетка.</span><span class="sxs-lookup"><span data-stu-id="b3932-105">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities help you manage your project from opportunity through completion.</span></span> <span data-ttu-id="b3932-106">Када креирате пројекат, такође ћете креирати структурну анализу посла, што утиче на ваше понуде, процене трошкова и управљање ресурсима.</span><span class="sxs-lookup"><span data-stu-id="b3932-106">When you create a project, you’ll also create a work breakdown structure, which affects your quotes, cost estimates, and resource management.</span></span>  
  
1.  <span data-ttu-id="b3932-107">Идите на **Project Service > Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="b3932-107">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="b3932-108">Кликните на **Нови пројекат**.</span><span class="sxs-lookup"><span data-stu-id="b3932-108">Click **New Project**.</span></span>  
  
3.  <span data-ttu-id="b3932-109">У оквиру области **Резиме**, унесите име пројекта, а затим попуните онолико детаља као можете.</span><span class="sxs-lookup"><span data-stu-id="b3932-109">In the **Summary** area, enter a name for your project, and then fill in as many of the details as you can.</span></span> <span data-ttu-id="b3932-110">Обавезна поља означена су црвеном звездицом (\*).</span><span class="sxs-lookup"><span data-stu-id="b3932-110">Items marked with a red asterisk (\*) are required.</span></span>  
  
4.  <span data-ttu-id="b3932-111">Кликните на дугме **Сачувај** да бисте креирали пројекат како бисте могли и даље да га уређујете.</span><span class="sxs-lookup"><span data-stu-id="b3932-111">Click **Save** to create your project so you can continue editing it.</span></span>  
  
<span data-ttu-id="b3932-112">Следеће, креираћете структурну анализу посла за пројекат за дефинисање задатака, трајање и улоге ресурса потребне за пројекат.</span><span class="sxs-lookup"><span data-stu-id="b3932-112">Next, you’ll create a work breakdown structure for your project to define the tasks, timing, and resource roles needed for the project.</span></span>  

> [!NOTE]
> <span data-ttu-id="b3932-113">Приликом заказивања, Project Service Automation уважава временску зону примењеног предлошка **Радно време**.</span><span class="sxs-lookup"><span data-stu-id="b3932-113">When scheduling, Project Service Automation respects the time zone of the applied **Work Hour** template.</span></span> <span data-ttu-id="b3932-114">Међутим, приликом прегледа задатака распореда, датуми почетка и завршетка задатка биће приказани у временској зони корисника.</span><span class="sxs-lookup"><span data-stu-id="b3932-114">However, when viewing the schedule tasks, the start and end dates of a task will be displayed in the user's time zone.</span></span> <span data-ttu-id="b3932-115">Ово се односи на друге временски усмерене приказе у обрасцу **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="b3932-115">This applies to other time-phased views in the **Project** form.</span></span> <span data-ttu-id="b3932-116">Ако се временска зона корисника не подудара са временском зоном предлошка радног времена примењеног на пројекат, приказаће се упозорење које објашњава разлику.</span><span class="sxs-lookup"><span data-stu-id="b3932-116">If the user's time zone does not match the time zone of the work hour template applied to the project, a warning which explains the difference will occur.</span></span> 
  
### <a name="see-also"></a><span data-ttu-id="b3932-117">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="b3932-117">See Also</span></span>  
 [<span data-ttu-id="b3932-118">Водич за менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="b3932-118">Project Manager Guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]