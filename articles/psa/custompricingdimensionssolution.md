---
title: Креирање прилагођених решења за димензије цене
description: У овој теми се објашњава како се креира прилагођено решење приликом креирања прилагођених димензија цене.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 3e437fce5b9f1fb330a713788e24100a4fe02948
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083981"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="ced83-103">Креирање прилагођених решења за димензије цене</span><span class="sxs-lookup"><span data-stu-id="ced83-103">Create custom solutions for pricing dimensions</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ced83-104">Све промене прилагођених димензија цене треба да буду у засебном решењу.</span><span class="sxs-lookup"><span data-stu-id="ced83-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="ced83-105">Ова важна најбоља пракса пружа флексибилност у будућности за ажурирање или уклањање промена по потреби, помоћи ће при поновној употреби посла и олакшава прилагођавање ових промена другој инстанци.</span><span class="sxs-lookup"><span data-stu-id="ced83-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="ced83-106">Када унесете све потребне промене, извезите ово решење као **Комплетно решење** и увезите га у друге инстанце да бисте поново користили подешавање за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="ced83-106">After you make the required changes, export this solution as a **Managed solution** , and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="ced83-107">Изаберите **Подешавања** > **Решења** , а затим изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="ced83-107">Select **Settings** > **Solutions** , and then select **New**.</span></span> 
2. <span data-ttu-id="ced83-108">Именујте решење, **\<your organization name> димензије за одређивање цена** , унесите преостале захтеване информације, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="ced83-108">Name the solution, **\<your organization name> pricing dimensions** , enter the remaining required information, and then select **Save**.</span></span>

> ![Креирање прилагођеног решења за димензије за одређивање цена](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="ced83-110">Додајте све захтеване ентитете и сродне компоненте у решење за димензије цене</span><span class="sxs-lookup"><span data-stu-id="ced83-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="ced83-111">Мораћете да додате следеће Project Service ентитете у решење за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="ced83-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="ced83-112">Довршите кораке у овој процедури да бисте направили неке важне промене шема у решењу за одређивање цена, тако да ентитети постану свесни нових димензија цене.</span><span class="sxs-lookup"><span data-stu-id="ced83-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="ced83-113">Изаберите **Подешавања** > **Решења** , а затим двапут кликните на **\<your organization name> димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="ced83-113">Select **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="ced83-114">У левом окну за навигацију истраживача решења изаберите **Додај постојеће** > **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="ced83-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="ced83-115">У дијалогу **Компоненте решења** изаберите следеће ентитете:</span><span class="sxs-lookup"><span data-stu-id="ced83-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="ced83-116">Стварно</span><span class="sxs-lookup"><span data-stu-id="ced83-116">Actual</span></span>
- <span data-ttu-id="ced83-117">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="ced83-117">Bookable Resource</span></span>
- <span data-ttu-id="ced83-118">Ставка процене</span><span class="sxs-lookup"><span data-stu-id="ced83-118">Estimate Line</span></span>
- <span data-ttu-id="ced83-119">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="ced83-119">Project Task</span></span>
- <span data-ttu-id="ced83-120">Детаљ ставке фактуре</span><span class="sxs-lookup"><span data-stu-id="ced83-120">Invoice Line Detail</span></span>
- <span data-ttu-id="ced83-121">Ставка у главној књизи</span><span class="sxs-lookup"><span data-stu-id="ced83-121">Journal Line</span></span>
- <span data-ttu-id="ced83-122">Детаљ предмета уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="ced83-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="ced83-123">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="ced83-123">Project Team Member</span></span>
- <span data-ttu-id="ced83-124">Детаљ ставке понуде</span><span class="sxs-lookup"><span data-stu-id="ced83-124">Quote Line Detail</span></span>
- <span data-ttu-id="ced83-125">Провизија на цену улоге</span><span class="sxs-lookup"><span data-stu-id="ced83-125">Role Price Markup</span></span>
- <span data-ttu-id="ced83-126">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="ced83-126">Role Price</span></span> 
- <span data-ttu-id="ced83-127">Ставка времена</span><span class="sxs-lookup"><span data-stu-id="ced83-127">Time Entry</span></span> 

> ![Додавање постојећих ентитета у решење за димензије одређивања цена](media/Existing-entities-to-PD-solution.png)

> ![Изаберите компоненте решења](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="ced83-130">Обавезно укључите све обрасце и приказе за сваки од изабраних ентитета.</span><span class="sxs-lookup"><span data-stu-id="ced83-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="ced83-131">Када се од вас затражи да укључите зависне ентитете за изабране ентитете, изаберите **Не**.</span><span class="sxs-lookup"><span data-stu-id="ced83-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![Немојте да укључујете све повезане компоненте](media/Do-not-include-required.png)


