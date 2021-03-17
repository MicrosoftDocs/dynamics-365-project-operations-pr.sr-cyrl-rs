---
title: Креирање решења за прилагођене димензије одређивања цена
description: Ова тема пружа информације о томе како да креирате решења за прилагођене димензије одређивања цена.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3e3f688b0147974ef252a0ee00be20c4669d7165
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278436"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="c42ec-103">Креирање решења за прилагођене димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="c42ec-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="c42ec-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="c42ec-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="c42ec-105">Све промене прилагођених димензија цене треба да буду у засебном решењу.</span><span class="sxs-lookup"><span data-stu-id="c42ec-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="c42ec-106">Ова важна најбоља пракса омогућава флексибилност за ажурирање или уклањање промена по потреби, помаже при поновној употреби посла и олакшава прилагођавање ових промена другим инстанцама.</span><span class="sxs-lookup"><span data-stu-id="c42ec-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="c42ec-107">Након што унесете све потребне промене, извезите ово решење као **Комплетно** решење, па га увезете у друге инстанце да бисте га поново користили.</span><span class="sxs-lookup"><span data-stu-id="c42ec-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="c42ec-108">Креирање решења за прилагођене димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="c42ec-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="c42ec-109">Изаберите **Подешавања** > **Решења**, а затим изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="c42ec-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="c42ec-110">Именујте решење, *<your organization name> димензије за одређивање цена*.</span><span class="sxs-lookup"><span data-stu-id="c42ec-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="c42ec-111">Унесите преостале потребне информације, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="c42ec-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![Креирање решења за прилагођене димензије за одређивање цена](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="c42ec-113">Додајте све захтеване ентитете и сродне компоненте у решење за димензије цене</span><span class="sxs-lookup"><span data-stu-id="c42ec-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="c42ec-114">Додајте следеће Project Service ентитете у своје решење за одређивање цена да бисте унели важне промене у шеми у решењу за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="c42ec-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="c42ec-115">Након што завршите овај поступак, ентитети ће препознати нове димензије за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="c42ec-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="c42ec-116">Изаберите **Подешавања** > **Решења**, а затим кликните двапут на **<*назив ваше организације*> димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="c42ec-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="c42ec-117">У левом окну за навигацију истраживача решења изаберите **Додај постојеће** > **Ентитети**.</span><span class="sxs-lookup"><span data-stu-id="c42ec-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="c42ec-118">У дијалогу **Компоненте решења** изаберите следеће ентитете:</span><span class="sxs-lookup"><span data-stu-id="c42ec-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="c42ec-119">**Стварно**</span><span class="sxs-lookup"><span data-stu-id="c42ec-119">**Actual**</span></span>
   - <span data-ttu-id="c42ec-120">**Ресурс који може да се резервише**</span><span class="sxs-lookup"><span data-stu-id="c42ec-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="c42ec-121">**Ставка процене**</span><span class="sxs-lookup"><span data-stu-id="c42ec-121">**Estimate Line**</span></span>
   - <span data-ttu-id="c42ec-122">**Пројектни задатак**</span><span class="sxs-lookup"><span data-stu-id="c42ec-122">**Project Task**</span></span>
   - <span data-ttu-id="c42ec-123">**Детаљ ставке фактуре**</span><span class="sxs-lookup"><span data-stu-id="c42ec-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="c42ec-124">**Ставка у главној књизи**</span><span class="sxs-lookup"><span data-stu-id="c42ec-124">**Journal Line**</span></span>
   - <span data-ttu-id="c42ec-125">**Детаљ предмета уговора за пројекат**</span><span class="sxs-lookup"><span data-stu-id="c42ec-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="c42ec-126">**Члан пројектног тима**</span><span class="sxs-lookup"><span data-stu-id="c42ec-126">**Project Team Member**</span></span>
   - <span data-ttu-id="c42ec-127">**Детаљ ставке понуде**</span><span class="sxs-lookup"><span data-stu-id="c42ec-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="c42ec-128">**Провизија на цену улоге**</span><span class="sxs-lookup"><span data-stu-id="c42ec-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="c42ec-129">**Цена улоге**</span><span class="sxs-lookup"><span data-stu-id="c42ec-129">**Role Price**</span></span>
   - <span data-ttu-id="c42ec-130">**Ставка времена**</span><span class="sxs-lookup"><span data-stu-id="c42ec-130">**Time Entry**</span></span>
 
   ![Додавање решења са прилагођеном димензијом одређивања цена постојећим ентитетима](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="c42ec-132">За сваки ентитет, прегледајте компоненте које се додају и коначну листу средстава ентитета за сваки ентитет.</span><span class="sxs-lookup"><span data-stu-id="c42ec-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="c42ec-133">Укључите све обрасце и приказе за сваки од изабраних ентитета.</span><span class="sxs-lookup"><span data-stu-id="c42ec-133">Include all forms and views for each of the selected entities.</span></span>

  ![Додати ентитети](./media/solution-component-selection.png)


5.  <span data-ttu-id="c42ec-135">Када се од вас затражи да укључите било који зависни ентитет за изабране ентитете, изаберите **Не, не укључуј обавезне компоненте.**</span><span class="sxs-lookup"><span data-stu-id="c42ec-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![Укључивање зависних ентитета](./media/Do-not-include-required.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]