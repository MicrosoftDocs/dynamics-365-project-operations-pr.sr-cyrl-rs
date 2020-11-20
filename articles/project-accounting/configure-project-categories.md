---
title: Конфигурисање категорија пројекта
description: Ова тема пружа информације о подешавању категорија пројеката.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 3698b68b5dd0460343d26af0fcea5b9a56be4083
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131946"
---
# <a name="configure-project-categories"></a><span data-ttu-id="376f0-103">Конфигурисање категорија пројекта</span><span class="sxs-lookup"><span data-stu-id="376f0-103">Configure project categories</span></span>

<span data-ttu-id="376f0-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="376f0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="376f0-105">Услуга Project Operations нуди снажне могућности за категоризацију прихода и трошкова на пројектима.</span><span class="sxs-lookup"><span data-stu-id="376f0-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="376f0-106">Категорије пружају могућност извештавања о пројектним трансакцијама и спроводе књижење у главну књигу.</span><span class="sxs-lookup"><span data-stu-id="376f0-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="376f0-107">Следећи дијаграм илуструје корелацију између категорија трансакција, дељених категорија и категорија пројеката.</span><span class="sxs-lookup"><span data-stu-id="376f0-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="376f0-108">Категорије трансакција су основно груписање за пројектне трансакције.</span><span class="sxs-lookup"><span data-stu-id="376f0-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="376f0-109">Унутар те групације постоји скуп дељених категорија које се могу делити између апликација и модула.</span><span class="sxs-lookup"><span data-stu-id="376f0-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="376f0-110">Улазећи још даље у детаље, категорије пројеката су најосновнији ниво категорија.</span><span class="sxs-lookup"><span data-stu-id="376f0-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="376f0-111">Категорије пројеката су специфичне за правно лице, модул и апликацију.</span><span class="sxs-lookup"><span data-stu-id="376f0-111">Project categories are specific to legal entity, module, and application.</span></span>

![Корелација између категорија трансакција, дељених категорија и категорија пројеката](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="376f0-113">Категорије трансакција</span><span class="sxs-lookup"><span data-stu-id="376f0-113">Transaction categories</span></span>

<span data-ttu-id="376f0-114">Категорије трансакција представљају основно груписање за пројектне трансакције и нису специфичне за предузеће или тип трансакције.</span><span class="sxs-lookup"><span data-stu-id="376f0-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="376f0-115">На пример, Contoso Robotics користи категорије Дизајн, Путовање, Инсталација и Услужне трансакције за груписање пројектних трансакција.</span><span class="sxs-lookup"><span data-stu-id="376f0-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="376f0-116">Категорије трансакција дефинисане су у модулу услуге Project Operations.</span><span class="sxs-lookup"><span data-stu-id="376f0-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="376f0-117">Идите на **Подешавања** \> **Категорије трансакција** да отворите образац.</span><span class="sxs-lookup"><span data-stu-id="376f0-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="376f0-118">Креирајте нову категорију трансакција било избором **Нова** или избором **Увези из Excel табеле**.</span><span class="sxs-lookup"><span data-stu-id="376f0-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="376f0-119">Дељене категорије</span><span class="sxs-lookup"><span data-stu-id="376f0-119">Shared categories</span></span>

<span data-ttu-id="376f0-120">Dynamics 365 користи концепт дељених категорија за категоризацију трошкова у различитим апликацијама, као што су Dynamics 365 Finance, Dynamics 365 Supply Chain и Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="376f0-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="376f0-121">За сваку креирану категорију трансакција, Project Operations аутоматски креира четири повезане дељене категорије: Сати, Трошкови, Накнаде и Ставка.</span><span class="sxs-lookup"><span data-stu-id="376f0-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="376f0-122">Можете да прегледате и прилагодите дељене категорије тако што ћете отићи на **Управљање пројектима и рачуноводство** \> **Подешавање** \> **Категорије** \> **Дељене категорије**.</span><span class="sxs-lookup"><span data-stu-id="376f0-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="376f0-123">Категорије пројеката</span><span class="sxs-lookup"><span data-stu-id="376f0-123">Project categories</span></span>

<span data-ttu-id="376f0-124">Категорије пројеката представљају најосновнији ниво конфигурације категорија и морају се конфигурисати одвојено и за свако предузеће, по рачуновођи пројекта.</span><span class="sxs-lookup"><span data-stu-id="376f0-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="376f0-125">Идите на **Управљање пројектима и рачуноводство** \> **Подешавање** \> **Категорије** \> **Категорије пројеката**.</span><span class="sxs-lookup"><span data-stu-id="376f0-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="376f0-126">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="376f0-126">Select **New**.</span></span>
3. <span data-ttu-id="376f0-127">Изаберите **ID категорије** дељене категорије коју сте креирали у претходном одељку.</span><span class="sxs-lookup"><span data-stu-id="376f0-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="376f0-128">Project Operations омогућава употребу само оних заједничких категорија које су повезане са категоријама трансакција.</span><span class="sxs-lookup"><span data-stu-id="376f0-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="376f0-129">Изаберите групу категорија.</span><span class="sxs-lookup"><span data-stu-id="376f0-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="376f0-130">Групе категорија</span><span class="sxs-lookup"><span data-stu-id="376f0-130">Category groups</span></span>

<span data-ttu-id="376f0-131">Групе категорија користе се за дељење својстава, пре свега профила за књижење, између повезаних категорија пројекта.</span><span class="sxs-lookup"><span data-stu-id="376f0-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="376f0-132">За сваку врсту трансакције мора постојати најмање једна група категорија, а свакој категорији пројекта додељена је група.</span><span class="sxs-lookup"><span data-stu-id="376f0-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="376f0-133">Спецификације књижења у услузи Project Operations дефинисане су правилима профила трошкова и прихода пројекта, категоријама пројеката и групама категорија.</span><span class="sxs-lookup"><span data-stu-id="376f0-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="376f0-134">Можете да подесите групе категорија ако одете на **Управљање пројектима и рачуноводство** \> **Подешавање** \> **Категорије** \> **Групе категорија**.</span><span class="sxs-lookup"><span data-stu-id="376f0-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>
