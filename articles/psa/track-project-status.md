---
title: Пратите статус пројекта
description: Како да пратите статус пројекта у апликацији Project Service
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
ms.openlocfilehash: e9c8b594d468016264d0b4d9745597a35f55e50e
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149606"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="02fad-103">Праћење статуса пројекта (Project Service)</span><span class="sxs-lookup"><span data-stu-id="02fad-103">Track a project’s status (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="02fad-104">Користите [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] да бисте пратили ток пројекта за клијента.</span><span class="sxs-lookup"><span data-stu-id="02fad-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="02fad-105">Како ангажовање напредује, фазе пројекта се ажурирају тако да одражавају фазу ангажовања:</span><span class="sxs-lookup"><span data-stu-id="02fad-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="02fad-106">**Ново**</span><span class="sxs-lookup"><span data-stu-id="02fad-106">**New**</span></span>    | <span data-ttu-id="02fad-107">Када креирате пројекат, фаза се поставља на **Ново**.</span><span class="sxs-lookup"><span data-stu-id="02fad-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="02fad-108">Ако сте креирали пројекат од предлошка, у овој фази пројекат може имати распоред, процене и податке о тиму.</span><span class="sxs-lookup"><span data-stu-id="02fad-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="02fad-109">У супротном, он ће бити у нацрт пројекта и потребно је да ручно унесете остатак компонената пројекта.</span><span class="sxs-lookup"><span data-stu-id="02fad-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="02fad-110">**Понуда**</span><span class="sxs-lookup"><span data-stu-id="02fad-110">**Quote**</span></span>   |      <span data-ttu-id="02fad-111">Када повежете пројекат са понудом или га креирате од понуде, фаза пројекта се поставља на **Понуда**, а процењени датуми почетка и завршетка се такође ажурирају.</span><span class="sxs-lookup"><span data-stu-id="02fad-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="02fad-112">Када је пројекат је у фази понуде, детаљи понуде се приказују на картици **Sales** на страници **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="02fad-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="02fad-113">**План**</span><span class="sxs-lookup"><span data-stu-id="02fad-113">**Plan**</span></span>   |                                     <span data-ttu-id="02fad-114">Када вам буде одобрена понуда повезана са пројектом и када ангажовање напредује до фазе уговора, фаза пројекта се ажурира на **План**.</span><span class="sxs-lookup"><span data-stu-id="02fad-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="02fad-115">Детаљи о уговору се приказују на картици **Sales** на страници **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="02fad-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="02fad-116">**Довршено**</span><span class="sxs-lookup"><span data-stu-id="02fad-116">**Complete**</span></span> |                    <span data-ttu-id="02fad-117">Када се посао на пројекту заврши, можете да пребаците фазу на **Довршено**.</span><span class="sxs-lookup"><span data-stu-id="02fad-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="02fad-118">Када се за фазу пројекта подеси довршавање, сматра се да је посао довршен 100%, али пројекат остаје отворен ради завођења ставки времена или трошкова.</span><span class="sxs-lookup"><span data-stu-id="02fad-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="02fad-119">**Затворите**</span><span class="sxs-lookup"><span data-stu-id="02fad-119">**Close**</span></span>   |           <span data-ttu-id="02fad-120">Када све трансакције буду снимљене на пројекту и не очекујете више да се евидентирају, можете ручно да поставите фазу **Затварања**.</span><span class="sxs-lookup"><span data-stu-id="02fad-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="02fad-121">Када се пројекат постави на **Затварање** не можете више да заводите трансакције на пројекту и пројекат ће бити само за читање.</span><span class="sxs-lookup"><span data-stu-id="02fad-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="02fad-122">Праћење статуса пројекта</span><span class="sxs-lookup"><span data-stu-id="02fad-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="02fad-123">Идите на **Project Service > Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="02fad-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="02fad-124">Кликните на пројекат на коме желите да радите.</span><span class="sxs-lookup"><span data-stu-id="02fad-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="02fad-125">На траци у врху екрана изаберите стрелицу надоле поред назива пројекта, а затим кликните на **Праћење пројекта**.</span><span class="sxs-lookup"><span data-stu-id="02fad-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="02fad-126">Изаберите **Праћење ангажовања** или **Праћење трошкова** у падајућој листи изнад листе задатака.</span><span class="sxs-lookup"><span data-stu-id="02fad-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="02fad-127">Кликните двапут на било који задатак да бисте га уредили.</span><span class="sxs-lookup"><span data-stu-id="02fad-127">Double-click any task to edit it.</span></span> <span data-ttu-id="02fad-128">Такође можете преместити или променити величину трака у графикону Gantt да бисте променили време и ток задатка.</span><span class="sxs-lookup"><span data-stu-id="02fad-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="02fad-129">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="02fad-129">See Also</span></span>  
 [<span data-ttu-id="02fad-130">Водич за менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="02fad-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
