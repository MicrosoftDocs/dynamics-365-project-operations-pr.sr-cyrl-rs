---
title: Додељивање генеричких ресурса који се могу резервисати задатку и пројектном тиму
description: Ова тема пружа информације о резервисању генеричких ресурса за задатке и тимове пројекта.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: 5b4c47513b96310745fd2cdb296988a57df0e966
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291412"
---
# <a name="assign-generic-bookable-resources-to-a-task-and-generate-resource-requirements"></a><span data-ttu-id="e528b-103">Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима</span><span class="sxs-lookup"><span data-stu-id="e528b-103">Assign generic bookable resources to a task and generate resource requirements</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e528b-104">Поред резервисања и додељивања именованих или стварних ресурса пројекту, можете да доделите генеричке ресурсе пројектним задацима.</span><span class="sxs-lookup"><span data-stu-id="e528b-104">In addition to booking and assigning named or real resources to your project, you can assign generic resources to project tasks.</span></span> <span data-ttu-id="e528b-105">Ти ресурси могу да послуже као чувари места за именоване ресурсе док не будете спремни да као ангажоване особе на пројекту користите именоване ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e528b-105">These resources can serve as placeholders for named resources until you are ready to staff your project with named resources.</span></span> 

1. <span data-ttu-id="e528b-106">У апликацији Project Service Automation (PSA) отворите страницу **Пројекат** и на картици **Распоред** унесите име улоге генеричког ресурса у ћелију распореда **Ресурс**.</span><span class="sxs-lookup"><span data-stu-id="e528b-106">In Project Service Automation (PSA), open the **Project** page and on the **Schedule** tab, enter the position name of the generic resource in the **Resource** cell of the schedule.</span></span> <span data-ttu-id="e528b-107">Можете и да кликнете на икону **Ресурс** у ћелији да бисте отворили бирач ресурса, а затим унели име генеричког ресурса који желите да креирате.</span><span class="sxs-lookup"><span data-stu-id="e528b-107">Or, click the **Resource** icon in the cell to open the resource picker and then enter the name of the generic resource that you want to create.</span></span>

![Креирање и додељивање генеричког члана тима](media/RM-how-to-9.png)

<span data-ttu-id="e528b-109">Тако ћете отворити таблу **Брзо креирање члана пројектног тима**.</span><span class="sxs-lookup"><span data-stu-id="e528b-109">This will open the **Quick Create: Project Team Member** panel.</span></span> 

2. <span data-ttu-id="e528b-110">Унесите улогу и организациону јединицу генеричког члана тима ресурса, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="e528b-110">Enter the role and organization unit of the generic resource team member and then click **Save**.</span></span>

![Брзо креирање генеричког члана тима](media/RM-how-to-10.png)

3. <span data-ttu-id="e528b-112">Након што сте креирали новог генеричког члана тима ресурса, он ће бити додељен задатку.</span><span class="sxs-lookup"><span data-stu-id="e528b-112">After you have created the new generic resource team member, it is assigned to the task.</span></span> <span data-ttu-id="e528b-113">Можете наставити да додељујете тај генерички ресурс другим задацима у распореду задатака.</span><span class="sxs-lookup"><span data-stu-id="e528b-113">You can continue to assign that generic resource to other tasks in the task schedule.</span></span>

![Додељивање постојећег генеричког члана тима задацима](media/RM-how-to-11.png)

4. <span data-ttu-id="e528b-115">Након што сте доделили генерички ресурс, можете да генеришете потребу за ресурсом и да је испуните директним резервисањем или прослеђивањем захтева за ресурс менаџеру ресурса.</span><span class="sxs-lookup"><span data-stu-id="e528b-115">After you have assigned the generic resource, you can generate a resource requirement and fulfill it by directly booking or submitting a resource request to a resource manager.</span></span>

![Генерисање захтева за генеричког члана тима](media/RM-how-to-12.png)

<span data-ttu-id="e528b-117">У мрежи за чланове тима, поред тога што можете да користите бирач ресурса као што је поменуто горе, моћи ћете директно да додате генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e528b-117">On the team member grid, in addition to being able to use the resource picker as mentioned above, you can add generic resources directly.</span></span> <span data-ttu-id="e528b-118">Ресурси се додају помоћу потреба за ресурсима које се заснивају на датуму почетка/завршетка и методи доделе која је наведена у табли **Брзо креирање члана пројектног тима**.</span><span class="sxs-lookup"><span data-stu-id="e528b-118">The resources are added with a resource requirement that is based on the start/end dates and allocation method specified in the **Quick Create: Project Team Member** panel.</span></span>

<span data-ttu-id="e528b-119">Можете видети разлику ако директно додате генеричког члана тима, а затим доделите још задатака генеричком ресурсу од броја сати које тај ресурс може да покрије.</span><span class="sxs-lookup"><span data-stu-id="e528b-119">You can see a difference if you add the generic team member directly and then assign more tasks to the generic resource than they have required hours to cover.</span></span> <span data-ttu-id="e528b-120">Кликните на **Генериши захтев** да бисте поново генерисали захтев и балансирали захтеване сате у односу на додељене задатке.</span><span class="sxs-lookup"><span data-stu-id="e528b-120">Click **Generate Requirement** to regenerate the requirement to balance the required hours against assignments.</span></span>

<span data-ttu-id="e528b-121">Такође можете да кликнете на везу **Потреба за ресурсом** у мрежи тима да бисте отворили захтев и додали вештине, жељене ресурсе итд.</span><span class="sxs-lookup"><span data-stu-id="e528b-121">You can also click the **Resource requirement** link in the team grid to open the requirement and add skills, preferred resources, etc.</span></span>

![Захтев за ресурсима](media/RM-how-to-13.png)



[!INCLUDE[footer-include](../includes/footer-banner.md)]