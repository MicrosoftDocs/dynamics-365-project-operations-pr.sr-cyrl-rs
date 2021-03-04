---
title: Конфигурисање подешавања додатних параметара
description: Како да конфигуришете подешавања додатних параметара у услузи Project Service
author: JohnPBurrows
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
ms.openlocfilehash: 73264845808e12950a48eea2b79e54c393d9c024
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5151586"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="cf383-103">Конфигурисање подешавања додатних параметара (Project Service)</span><span class="sxs-lookup"><span data-stu-id="cf383-103">Configure additional parameter settings (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="cf383-104">Када конфигуришете ставке у претходним темама, треба да подесите додатне параметре пројекта које ћете користити у пројектима.</span><span class="sxs-lookup"><span data-stu-id="cf383-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="cf383-105">Када сте први пут инсталирали [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], креирали сте подешавање параметара да прво креирате све записе потребне како би [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] функционисао.</span><span class="sxs-lookup"><span data-stu-id="cf383-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="cf383-106">Сада је време да се вратите и конфигуришете додатна поља за ова подешавања.</span><span class="sxs-lookup"><span data-stu-id="cf383-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="cf383-107">Мораћете да конфигуришете следећа подешавања:</span><span class="sxs-lookup"><span data-stu-id="cf383-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="cf383-108">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="cf383-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="cf383-109">Учесталост фактурисања</span><span class="sxs-lookup"><span data-stu-id="cf383-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="cf383-110">Предложак радног времена</span><span class="sxs-lookup"><span data-stu-id="cf383-110">Work hours template</span></span>  
  
-   <span data-ttu-id="cf383-111">Ценовник</span><span class="sxs-lookup"><span data-stu-id="cf383-111">Price list</span></span>  
 
<span data-ttu-id="cf383-112">У овом кораку ћете такође указати на тип доделе ресурса који желите:</span><span class="sxs-lookup"><span data-stu-id="cf383-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="cf383-113">**Централни**.</span><span class="sxs-lookup"><span data-stu-id="cf383-113">**Central**.</span></span> <span data-ttu-id="cf383-114">Само менаџери ресурса могу да додељују ресурсе пројектима.</span><span class="sxs-lookup"><span data-stu-id="cf383-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="cf383-115">**Хибридни**.</span><span class="sxs-lookup"><span data-stu-id="cf383-115">**Hybrid**.</span></span> <span data-ttu-id="cf383-116">Менаџери ресурса, менаџери пројекта и менаџери пословног контакта могу да додељују ресурсе пројектима.</span><span class="sxs-lookup"><span data-stu-id="cf383-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="cf383-117">Да бисте подесили параметре пројекта:</span><span class="sxs-lookup"><span data-stu-id="cf383-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="cf383-118">Идите на **Project Service > Параметри**.</span><span class="sxs-lookup"><span data-stu-id="cf383-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="cf383-119">Кликните на подешавање параметара које желите да конфигуришете (оне које сте креирали када сте први пут инсталирали [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]) или кликните на **Ново** да бисте креирате нови.</span><span class="sxs-lookup"><span data-stu-id="cf383-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="cf383-120">У области **Општи подаци**, подесите све опције за параметре пројекта.</span><span class="sxs-lookup"><span data-stu-id="cf383-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="cf383-121">У области **Ценовник** кликните на **+** да бисте додали ценовник, изаберите ценовник у падајућој листи **Ценовник параметара пројекта**, а затим кликните на **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="cf383-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="cf383-122">Кликните на дугме **Сачувај** у доњем десном углу екрана.</span><span class="sxs-lookup"><span data-stu-id="cf383-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="cf383-123">Запис параметра пројекта мора да се одржава како би Project Service правилно функционисао.</span><span class="sxs-lookup"><span data-stu-id="cf383-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="cf383-124">Овај запис не би требало брисати.</span><span class="sxs-lookup"><span data-stu-id="cf383-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="cf383-125">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="cf383-125">See Also</span></span>  
 [<span data-ttu-id="cf383-126">Подешавање ресурса</span><span class="sxs-lookup"><span data-stu-id="cf383-126">Set up resources</span></span>](../psa/set-up-resources.md)
