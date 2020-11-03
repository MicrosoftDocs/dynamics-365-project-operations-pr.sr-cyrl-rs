---
title: Преглед димензија за одређивање цена
description: Ова тема пружа информације о димензија за одређивање цена у услузи Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 6b1ebdc97ec4704ba256acb521c0f2e7c474940b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084079"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="a3753-103">Преглед димензија за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="a3753-103">Pricing dimensions overview</span></span>

<span data-ttu-id="a3753-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="a3753-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a3753-105">Димензије које се користе у људским ресурсима за подешавање цена и трошкова спадају у две категорије:</span><span class="sxs-lookup"><span data-stu-id="a3753-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="a3753-106">Људи</span><span class="sxs-lookup"><span data-stu-id="a3753-106">People</span></span>
- <span data-ttu-id="a3753-107">Планирани рад</span><span class="sxs-lookup"><span data-stu-id="a3753-107">Planned work</span></span>

<span data-ttu-id="a3753-108">Због тога постоје две врсте вредности димензија за одређивање цена које су доступне:</span><span class="sxs-lookup"><span data-stu-id="a3753-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="a3753-109">**Скупови опција** : Димензије које представљају фиксна набрајања за скуп вредности.</span><span class="sxs-lookup"><span data-stu-id="a3753-109">**Option sets** : Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="a3753-110">**Вредности засноване на ентитетима** : Димензије које могу бити различит скуп вредности.</span><span class="sxs-lookup"><span data-stu-id="a3753-110">**Entity-based values** : Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="a3753-111">Димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="a3753-111">Pricing dimensions</span></span>

<span data-ttu-id="a3753-112">Dynamics 365 Project Operations се испоручује са подразумеваним скупом димензија за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="a3753-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="a3753-113">Ове димензије за одређивање цена можете да их видите тако што ћете отићи на **Project Operations** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="a3753-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="a3753-114">У запису параметра, на картици **Димензије за одређивање цена засноване на износима** проверите да ли улога **msdyn_resourcecategory** и организациона јединица ресурса **msdyn_organizationalunit** имају поља **Применљиво на продају** и **Применљиво на трошкове** подешена на **Да**.</span><span class="sxs-lookup"><span data-stu-id="a3753-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="a3753-115">Када су ова поља омогућена, можете да подесите цену и трошак за сваку комбинацију улоге и организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="a3753-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="a3753-116">Ако је потребно да одредите цену или трошкове ресурса помоћу додатних атрибута, можете да креирате прилагођена поља, ентитете и димензије.</span><span class="sxs-lookup"><span data-stu-id="a3753-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="a3753-117">Одређивање цене времена људског ресурса</span><span class="sxs-lookup"><span data-stu-id="a3753-117">Pricing human resource time</span></span>
<span data-ttu-id="a3753-118">Како организација одређује цену времена људског ресурса је често значајно стратешко питање које директно утиче на профитабилност организације.</span><span class="sxs-lookup"><span data-stu-id="a3753-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="a3753-119">Сарађујте са финансијским тимовима и будите мудри када ваша организација буде спремна да утврди како жели да подеси стопе наплате и трошкова за време људског ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3753-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="a3753-120">Друга питања која се тичу формирања цена подразумевају да ли поново да користите поља или ентитете који тренутно нису димензије за одређивање цена, али се примењују као димензија за одређивање цена у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="a3753-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="a3753-121">Поља као што су **Категорија трансакције** ( **msdyn_transactioncategory** ) и **Ресурс који може да се резервише** ( **bookableresource** ) су примери могућих димензија.</span><span class="sxs-lookup"><span data-stu-id="a3753-121">Fields like **Transaction Category** ( **msdyn_transactioncategory** ) and **Bookable Resource** ( **bookableresource** ) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="a3753-122">Размотрите и да ли ваша димензија за одређивање цена треба да буде табела или скуп опција.</span><span class="sxs-lookup"><span data-stu-id="a3753-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="a3753-123">Ако предвиђате промене вредности димензије које ће премашити 10 или 12, а потребни су вам додатни атрибути за ове вредности, можете да креирате ентитет, а не скуп опција.</span><span class="sxs-lookup"><span data-stu-id="a3753-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="a3753-124">Одржавање скуп опција, као што је додавање или уклањање вредности, захтева администратора или програмера, док већина корисника може да додаје нове редове у табелу.</span><span class="sxs-lookup"><span data-stu-id="a3753-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="a3753-125">Следећи пример приказује курсне стопе које су подешене на основу улоге и организационе јединице ресурса коме припада ресурс.</span><span class="sxs-lookup"><span data-stu-id="a3753-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="a3753-126">Стопе трошкова се обично заснивају на групи личних доходака запослених и организационој јединици којој припадају.</span><span class="sxs-lookup"><span data-stu-id="a3753-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="a3753-127">У овом примеру, табеле са стопама наплате и стопама трошкова ће изгледати овако:</span><span class="sxs-lookup"><span data-stu-id="a3753-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="a3753-128">**Примери стопа наплате**</span><span class="sxs-lookup"><span data-stu-id="a3753-128">**Sample bill rates**</span></span>

| <span data-ttu-id="a3753-129">Улога</span><span class="sxs-lookup"><span data-stu-id="a3753-129">Role</span></span>        | <span data-ttu-id="a3753-130">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="a3753-130">Org Unit</span></span>    |<span data-ttu-id="a3753-131">Јединица</span><span class="sxs-lookup"><span data-stu-id="a3753-131">Unit</span></span>      |<span data-ttu-id="a3753-132">Цена</span><span class="sxs-lookup"><span data-stu-id="a3753-132">Price</span></span>      |<span data-ttu-id="a3753-133">Валута</span><span class="sxs-lookup"><span data-stu-id="a3753-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="a3753-134">Програмер</span><span class="sxs-lookup"><span data-stu-id="a3753-134">Developer</span></span>   | <span data-ttu-id="a3753-135">Contoso US</span><span class="sxs-lookup"><span data-stu-id="a3753-135">Contoso US</span></span>  |<span data-ttu-id="a3753-136">Hour</span><span class="sxs-lookup"><span data-stu-id="a3753-136">Hour</span></span> | <span data-ttu-id="a3753-137">200</span><span class="sxs-lookup"><span data-stu-id="a3753-137">200</span></span>|<span data-ttu-id="a3753-138">USD</span><span class="sxs-lookup"><span data-stu-id="a3753-138">USD</span></span>     |
| <span data-ttu-id="a3753-139">Програмер</span><span class="sxs-lookup"><span data-stu-id="a3753-139">Developer</span></span>   | <span data-ttu-id="a3753-140">Contoso India</span><span class="sxs-lookup"><span data-stu-id="a3753-140">Contoso India</span></span> |<span data-ttu-id="a3753-141">Hour</span><span class="sxs-lookup"><span data-stu-id="a3753-141">Hour</span></span>|   <span data-ttu-id="a3753-142">112.</span><span class="sxs-lookup"><span data-stu-id="a3753-142">112</span></span>|<span data-ttu-id="a3753-143">USD</span><span class="sxs-lookup"><span data-stu-id="a3753-143">USD</span></span>     |


<span data-ttu-id="a3753-144">**Примери стопа трошкова**</span><span class="sxs-lookup"><span data-stu-id="a3753-144">**Sample cost rates**</span></span>

| <span data-ttu-id="a3753-145">Група личних доходака</span><span class="sxs-lookup"><span data-stu-id="a3753-145">Salary Band</span></span>     | <span data-ttu-id="a3753-146">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="a3753-146">Org Unit</span></span>    |<span data-ttu-id="a3753-147">Јединица</span><span class="sxs-lookup"><span data-stu-id="a3753-147">Unit</span></span>      |<span data-ttu-id="a3753-148">Цена</span><span class="sxs-lookup"><span data-stu-id="a3753-148">Price</span></span>      |<span data-ttu-id="a3753-149">Валута</span><span class="sxs-lookup"><span data-stu-id="a3753-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="a3753-150">Моје предузеће_Прва група личних доходака</span><span class="sxs-lookup"><span data-stu-id="a3753-150">My company_Band1</span></span> | <span data-ttu-id="a3753-151">Contoso US</span><span class="sxs-lookup"><span data-stu-id="a3753-151">Contoso US</span></span>  |<span data-ttu-id="a3753-152">Hour</span><span class="sxs-lookup"><span data-stu-id="a3753-152">Hour</span></span> | <span data-ttu-id="a3753-153">145.</span><span class="sxs-lookup"><span data-stu-id="a3753-153">145</span></span>|<span data-ttu-id="a3753-154">USD</span><span class="sxs-lookup"><span data-stu-id="a3753-154">USD</span></span>     |
| <span data-ttu-id="a3753-155">Моје предузеће_друга група личних доходака</span><span class="sxs-lookup"><span data-stu-id="a3753-155">My company_Band2</span></span> | <span data-ttu-id="a3753-156">Contoso India</span><span class="sxs-lookup"><span data-stu-id="a3753-156">Contoso India</span></span> |<span data-ttu-id="a3753-157">Hour</span><span class="sxs-lookup"><span data-stu-id="a3753-157">Hour</span></span>|   <span data-ttu-id="a3753-158">67.</span><span class="sxs-lookup"><span data-stu-id="a3753-158">67</span></span>|<span data-ttu-id="a3753-159">USD</span><span class="sxs-lookup"><span data-stu-id="a3753-159">USD</span></span>     |
