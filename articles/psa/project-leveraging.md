---
title: Продајне процене и пројекти
description: Ова тема пружа информације о томе како искористити распоред и процене у процесу продаје.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: eafe60362003198a223026526f56261de414bb4a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083990"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="8964c-103">Продајне процене и пројекти</span><span class="sxs-lookup"><span data-stu-id="8964c-103">Sales estimates and projects</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8964c-104">Током процеса продаје можете креирати процене продаје повезујући пројекат с продајном понудом.</span><span class="sxs-lookup"><span data-stu-id="8964c-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="8964c-105">На овај начин, може да дође до детерминистичке процене током процеса продаје, како би се искористиле предности заказивања пројеката и процене.</span><span class="sxs-lookup"><span data-stu-id="8964c-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="8964c-106">Ако продаја прође, распоред који је коришћен за процену продаје може се користити као основа за даље прецизирање пројектног плана.</span><span class="sxs-lookup"><span data-stu-id="8964c-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="8964c-107">Повезивање пројекта са ставком понуде</span><span class="sxs-lookup"><span data-stu-id="8964c-107">Linking a project to a quote line</span></span>

<span data-ttu-id="8964c-108">Када креирате ставку понуде засновану на пројекту, можете да креирате нови пројекат или повежете постојећи пројекат на страници **Ставка пројекта**.</span><span class="sxs-lookup"><span data-stu-id="8964c-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![Образац ставке понуде](media/project-8.png)
 
<span data-ttu-id="8964c-110">Када креирате нови пројекат из детаља ставке понуде, можете искористити предлошке пројекта.</span><span class="sxs-lookup"><span data-stu-id="8964c-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="8964c-111">Предлошци пројеката су модели пројеката који представљају стандардне планове пројеката и финансијске процене типичне за организацију.</span><span class="sxs-lookup"><span data-stu-id="8964c-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="8964c-112">Такође могу представљати копије пројектних планова и процена из прошлих пројеката.</span><span class="sxs-lookup"><span data-stu-id="8964c-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![Детаљи ставке понуде](media/project-9.png)
  
<span data-ttu-id="8964c-114">Када креирате пројекат из понуде, пројекат се аутоматски повезује са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="8964c-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="8964c-115">Компоненте процена у пројекту</span><span class="sxs-lookup"><span data-stu-id="8964c-115">Components of estimates in a project</span></span>

<span data-ttu-id="8964c-116">Распоред вам омогућава да поделите посао на задатке, одржавате хијерархију задатака, одредите који су ресурси потребни за обављање задатка и доделите процену потребних активности за обављање задатка.</span><span class="sxs-lookup"><span data-stu-id="8964c-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="8964c-117">Можете дефинисати радне активности и процене распореда помоћу поља на картици **Распоред** у оквиру странице **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="8964c-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="8964c-118">Пошто је ценовник повезан са пројектом, финансијске процене се израчунавају коришћењем цене коштања и продајне цене које су дефинисане у ценовнику.</span><span class="sxs-lookup"><span data-stu-id="8964c-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="8964c-119">Увоз процена из пројекта у понуду</span><span class="sxs-lookup"><span data-stu-id="8964c-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="8964c-120">Након што дефинишете процене пројекта, можете их увести у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="8964c-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="8964c-121">На страници **Детаљи ставке понуде** изаберите **Увоз из процена** на траци да бисте резимирали процене пројекта према врсти трансакције, улози или нивоу задатка.</span><span class="sxs-lookup"><span data-stu-id="8964c-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>
