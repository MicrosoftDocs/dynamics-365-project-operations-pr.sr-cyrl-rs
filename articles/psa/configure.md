---
title: Конфигуришите програм Project Service Automation
description: Кораци за конфигурисање апликације Project Service
author: ruhercul
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
ms.openlocfilehash: ef1724bb92e62ae21472e133fff0978c4faeeffa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002866"
---
# <a name="configure-project-service"></a><span data-ttu-id="7bd26-103">Конфигурисање апликације Project Service</span><span class="sxs-lookup"><span data-stu-id="7bd26-103">Configure Project Service</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="7bd26-104">Пре него што будете могли да користите могућности аутоматизовања [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у систему [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] за управљање пословним контактима, пројектима и ресурсима, морате да довршите неколико конфигурационих корака да бисте обезбедили да се решење [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] подудара са потребама организације.</span><span class="sxs-lookup"><span data-stu-id="7bd26-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="7bd26-105">У ове кораке спада следеће:</span><span class="sxs-lookup"><span data-stu-id="7bd26-105">These steps include:</span></span>  
  
-   <span data-ttu-id="7bd26-106">[Подесите временске јединице](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="7bd26-107">Конфигуришите јединице времена у каталогу производа које ћете користити као основу за планирање и наплату пројеката.</span><span class="sxs-lookup"><span data-stu-id="7bd26-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="7bd26-108">[Подесите валуте и девизне курсеве](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="7bd26-109">Подесите валуте које ћете користити за пројекте.</span><span class="sxs-lookup"><span data-stu-id="7bd26-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="7bd26-110">[Креирајте организационе јединице](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="7bd26-111">Подесите групе које ваше предузеће користи за поделу пословања, било по географији, пословној функцији или другој логичкој подели.</span><span class="sxs-lookup"><span data-stu-id="7bd26-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="7bd26-112">[Подесите учесталости фактурисања](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="7bd26-113">Подесите временске периоде које желите да користите за наплату клијентима.</span><span class="sxs-lookup"><span data-stu-id="7bd26-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="7bd26-114">[Конфигуришите категорије трансакција](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="7bd26-115">Подесите категорије трансакција за које ваши саветници могу да зарачунају наплативе и ненаплативе трошкове.</span><span class="sxs-lookup"><span data-stu-id="7bd26-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="7bd26-116">[Креирајте категорије трошкова](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="7bd26-117">Подесите категорије за које ваши саветници могу да зарачунају наплативе и ненаплативе трошкове.</span><span class="sxs-lookup"><span data-stu-id="7bd26-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="7bd26-118">[Креирајте ставке каталога производа](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="7bd26-119">Додајте производе које продајете, као што су софтверске лиценце, у каталог производа.</span><span class="sxs-lookup"><span data-stu-id="7bd26-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="7bd26-120">[Креирајте ценовник](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="7bd26-121">Конфигуришите различите ценовнике, у зависности од тога колико желите да наплатите клијентима за сваку улогу коју њихов пројекат захтева.</span><span class="sxs-lookup"><span data-stu-id="7bd26-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="7bd26-122">[Подесите ресурсе](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="7bd26-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="7bd26-123">Додајте вештине, стручности, улоге ресурса и остале информације о ресурсима које вам требају за пројекте.</span><span class="sxs-lookup"><span data-stu-id="7bd26-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="7bd26-124">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="7bd26-124">See Also</span></span>  
 <span data-ttu-id="7bd26-125">[Преглед услуге Project Service Automation](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="7bd26-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="7bd26-126">[Конфигуришите програм Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="7bd26-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="7bd26-127">[Водич за менаџера за пословне контакте](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="7bd26-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="7bd26-128">[Водич за менаџера пројекта](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="7bd26-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="7bd26-129">[Водич за менаџера ресурса](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="7bd26-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="7bd26-130">Водич за време, трошак и сарадњу</span><span class="sxs-lookup"><span data-stu-id="7bd26-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]