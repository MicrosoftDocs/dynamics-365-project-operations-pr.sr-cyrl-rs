---
title: Конфигуришите програм Project Service Automation
description: Кораци за конфигурисање апликације Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 56ba0b8d-808c-48d6-965f-abd74b49c2b4
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 52be4705e6ef983dcf421df5d1bfb5c6de8e9a30
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755359"
---
# <a name="configure-project-service"></a><span data-ttu-id="02bce-103">Конфигурисање апликације Project Service</span><span class="sxs-lookup"><span data-stu-id="02bce-103">Configure Project Service</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="02bce-104">Пре него што будете могли да користите могућности аутоматизовања [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у систему [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] за управљање пословним контактима, пројектима и ресурсима, морате да довршите неколико конфигурационих корака да бисте обезбедили да се решење [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] подудара са потребама организације.</span><span class="sxs-lookup"><span data-stu-id="02bce-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="02bce-105">У ове кораке спада следеће:</span><span class="sxs-lookup"><span data-stu-id="02bce-105">These steps include:</span></span>  
  
-   <span data-ttu-id="02bce-106">[Подесите временске јединице](../project-service/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-106">[Set up time units](../project-service/set-up-time-units.md).</span></span> <span data-ttu-id="02bce-107">Конфигуришите јединице времена у каталогу производа које ћете користити као основу за планирање и наплату пројеката.</span><span class="sxs-lookup"><span data-stu-id="02bce-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="02bce-108">[Подесите валуте и девизне курсеве](../project-service/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-108">[Set up currencies and exchange rates](../project-service/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="02bce-109">Подесите валуте које ћете користити за пројекте.</span><span class="sxs-lookup"><span data-stu-id="02bce-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="02bce-110">[Креирајте организационе јединице](../project-service/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-110">[Create organizational units](../project-service/create-organizational-units.md).</span></span> <span data-ttu-id="02bce-111">Подесите групе које ваше предузеће користи за поделу пословања, било по географији, пословној функцији или другој логичкој подели.</span><span class="sxs-lookup"><span data-stu-id="02bce-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="02bce-112">[Подесите учесталости фактурисања](../project-service/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-112">[Set up invoice frequencies](../project-service/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="02bce-113">Подесите временске периоде које желите да користите за наплату клијентима.</span><span class="sxs-lookup"><span data-stu-id="02bce-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="02bce-114">[Конфигуришите категорије трансакција](../project-service/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-114">[Configure transaction categories](../project-service/configure-transaction-categories.md).</span></span> <span data-ttu-id="02bce-115">Подесите категорије трансакција за које ваши саветници могу да зарачунају наплативе и ненаплативе трошкове.</span><span class="sxs-lookup"><span data-stu-id="02bce-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="02bce-116">[Креирајте категорије трошкова](../project-service/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-116">[Configure expense categories](../project-service/configure-expense-categories.md).</span></span> <span data-ttu-id="02bce-117">Подесите категорије за које ваши саветници могу да зарачунају наплативе и ненаплативе трошкове.</span><span class="sxs-lookup"><span data-stu-id="02bce-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="02bce-118">[Креирајте ставке каталога производа](../project-service/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-118">[Create product catalog items](../project-service/create-product-catalog-items.md).</span></span> <span data-ttu-id="02bce-119">Додајте производе које продајете, као што су софтверске лиценце, у каталог производа.</span><span class="sxs-lookup"><span data-stu-id="02bce-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="02bce-120">[Креирајте ценовник](../project-service/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-120">[Create a price list](../project-service/create-price-list.md).</span></span> <span data-ttu-id="02bce-121">Конфигуришите различите ценовнике, у зависности од тога колико желите да наплатите клијентима за сваку улогу коју њихов пројекат захтева.</span><span class="sxs-lookup"><span data-stu-id="02bce-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="02bce-122">[Подесите ресурсе](../project-service/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="02bce-122">[Set up resources](../project-service/set-up-resources.md).</span></span> <span data-ttu-id="02bce-123">Додајте вештине, стручности, улоге ресурса и остале информације о ресурсима које вам требају за пројекте.</span><span class="sxs-lookup"><span data-stu-id="02bce-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="02bce-124">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="02bce-124">See Also</span></span>  
 <span data-ttu-id="02bce-125">[Преглед услуге Project Service Automation](../project-service/overview.md) </span><span class="sxs-lookup"><span data-stu-id="02bce-125">[Overview of Project Service Automation](../project-service/overview.md) </span></span>  
 <span data-ttu-id="02bce-126">[Конфигуришите програм Project Service Automation](../project-service/configure.md) </span><span class="sxs-lookup"><span data-stu-id="02bce-126">[Configure Project Service Automation](../project-service/configure.md) </span></span>  
 <span data-ttu-id="02bce-127">[Водич за менаџера за пословне контакте](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="02bce-127">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="02bce-128">[Водич за менаџера пројекта](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="02bce-128">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="02bce-129">[Водич за менаџера ресурса](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="02bce-129">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="02bce-130">Водич за време, трошак и сарадњу</span><span class="sxs-lookup"><span data-stu-id="02bce-130">Time, Expense, and Collaboration Guid</span></span>](../project-service/time-expense-collaboration-guide.md)
