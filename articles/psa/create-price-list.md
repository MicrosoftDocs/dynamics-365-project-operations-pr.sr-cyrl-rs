---
title: Креирање ценовника
description: Како да креирате ценовник у апликацији Project Service
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bf75286fd1837e27a9b6053ccb21b60771ee197d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084008"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="b0b84-103">Креирање ценовника (Project Service)</span><span class="sxs-lookup"><span data-stu-id="b0b84-103">Create a price list (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="b0b84-104">Ценовници менаџерима за пословне контакте пружају шаблон који могу користити за креирање понуда и пројеката, као и за успостављања трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="b0b84-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="b0b84-105">Они обезбеђују списак ставки предмета са улогама и трошковима, као и ценом коју ћете наплатити за сваку.</span><span class="sxs-lookup"><span data-stu-id="b0b84-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="b0b84-106">Можете да креирате више ценовника тако да можете да одржавате посебне структуре цена за различите регионе у којима продајете ваше производе или за различите канале продаје.</span><span class="sxs-lookup"><span data-stu-id="b0b84-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="b0b84-107">Било би добро да креирате барем један ценовник за сваку валуту у којој планирате да фактуришете клијентима.</span><span class="sxs-lookup"><span data-stu-id="b0b84-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="b0b84-108">Да бисте креирали финансијске процене за рад који ће бити обављен, уверите се да сваки пројекат има одговарајућу листу трошкова и ценовник продаје.</span><span class="sxs-lookup"><span data-stu-id="b0b84-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="b0b84-109">Подесите подразумевану листу трошкова и ценовник продаје који се примењује на све пројекте креиране у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="b0b84-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="b0b84-110">Ценовници се ослањају на улоге и категорије трошкова, тако да, пре него што креирате ценовник, уверите се да сте већ конфигурисали улоге и категорије трошкова које желите да користите приликом креирања ценовника.</span><span class="sxs-lookup"><span data-stu-id="b0b84-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="b0b84-111">Идите на **Project Service > Ценовници**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="b0b84-112">Кликните на дугме **Ново**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="b0b84-113">У опцији **Контекст** , изаберите да ли је овај ценовник за **Трошак** , **Куповину** или **Продају**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-113">In **Context** , select whether this price list is for **Cost** , **Purchase** , or **Sales**.</span></span>  
  
4.  <span data-ttu-id="b0b84-114">У опцији **Име** унесите име за ценовник.</span><span class="sxs-lookup"><span data-stu-id="b0b84-114">In **Name** , enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="b0b84-115">У опцији **Валута** изаберите валуту коју ћете да користите за наплату или успостављање трошкова.</span><span class="sxs-lookup"><span data-stu-id="b0b84-115">In **Currency** , select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="b0b84-116">У опцији **Јединица за време** , наведите временски период на који се цена примењује, као што су дан или час.</span><span class="sxs-lookup"><span data-stu-id="b0b84-116">In **Time Unit** , specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="b0b84-117">Попуните поља **Датум почетка** , **Датум завршетка** и **Опис** , а по потреби.</span><span class="sxs-lookup"><span data-stu-id="b0b84-117">Fill in the **Start Date** , **End Date** , and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="b0b84-118">Кликните на дугме **Сачувај** за креирање записа тако да можете да наставите га уређујете.</span><span class="sxs-lookup"><span data-stu-id="b0b84-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="b0b84-119">Да бисте додали цену улоге у ценовник, кликните на дугме **+** у оквиру **Цене улога**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="b0b84-120">Попуните поља у обрасцу **Цена улоге** и кликните на дугме **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="b0b84-121">Наставите да додајете цене улоге по потреби.</span><span class="sxs-lookup"><span data-stu-id="b0b84-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="b0b84-122">Када завршите, кликните на дугме **Сачувај** у доњем десном углу екрана.</span><span class="sxs-lookup"><span data-stu-id="b0b84-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="b0b84-123">Да бисте додали цену категорије трошка у ценовник, кликните на дугме **+** у оквиру **Цене категорија**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="b0b84-124">Попуните поља у обрасцу **Цена категорије трансакције** и кликните на дугме **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="b0b84-125">Наставите да додајете цене категорија по потреби.</span><span class="sxs-lookup"><span data-stu-id="b0b84-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="b0b84-126">Када завршите, кликните на дугме **Сачувај** у доњем десном углу екрана.</span><span class="sxs-lookup"><span data-stu-id="b0b84-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="b0b84-127">Да бисте додали ставке ценовника у ценовник, кликните на дугме **+** у оквиру **Ставке ценовника**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="b0b84-128">Попуните поља у окну **Ставка ценовника** и кликните на дугме **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="b0b84-129">Наставите да додајете ставке ценовника по потреби.</span><span class="sxs-lookup"><span data-stu-id="b0b84-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="b0b84-130">Када завршите, кликните на дугме **Сачувај** у доњем десном углу екрана.</span><span class="sxs-lookup"><span data-stu-id="b0b84-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="b0b84-131">Да бисте додали односе територије у ценовник, кликните на дугме **+** у оквиру **Односи територије**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="b0b84-132">Попуните поља у прозору **Нова веза** и кликните на дугме **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="b0b84-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="b0b84-133">Наставите додавање односа територије по потреби.</span><span class="sxs-lookup"><span data-stu-id="b0b84-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="b0b84-134">Када завршите, кликните на дугме **Сачувај** у доњем десном углу екрана.</span><span class="sxs-lookup"><span data-stu-id="b0b84-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="b0b84-135">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="b0b84-135">See Also</span></span>  
 [<span data-ttu-id="b0b84-136">Конфигуришите програм Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="b0b84-136">Configure Project Service Automation</span></span>](../psa/configure.md)
