---
title: Матична страница за димензије одређивања цена и обрачуна трошкова
description: Ова тема обезбеђује преглед димензија за одређивање цена.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 425d7bb8-9015-4f67-b9c9-cf3602e9afe8
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 2379d0d2e038f28a1a8df87a851e9bf7db7fe33f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755357"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="31aa9-103">Матична страница за димензије одређивања цена и обрачуна трошкова</span><span class="sxs-lookup"><span data-stu-id="31aa9-103">Pricing and costing dimensions home page</span></span>

<span data-ttu-id="31aa9-104">Димензије које се користе у људским ресурсима за подешавање цена и трошкова спадају у две категорије:</span><span class="sxs-lookup"><span data-stu-id="31aa9-104">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="31aa9-105">Људи</span><span class="sxs-lookup"><span data-stu-id="31aa9-105">People</span></span>
- <span data-ttu-id="31aa9-106">Планирани рад</span><span class="sxs-lookup"><span data-stu-id="31aa9-106">Planned work</span></span>

<span data-ttu-id="31aa9-107">Због тога постоје две врсте вредности димензија за одређивање цена које су доступне у апликацији Project Service Automation (PSA):</span><span class="sxs-lookup"><span data-stu-id="31aa9-107">Because of this, there are two types of pricing dimension values available in Project Service Automation (PSA):</span></span> 

- <span data-ttu-id="31aa9-108">**Скупови опција** - Димензије које представљају фиксна набрајања за скуп вредности.</span><span class="sxs-lookup"><span data-stu-id="31aa9-108">**Option sets** - Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="31aa9-109">**Вредности засноване на ентитетима** - Димензије које могу бити различит скуп вредности.</span><span class="sxs-lookup"><span data-stu-id="31aa9-109">**Entity-based values** - Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="31aa9-110">Димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="31aa9-110">Pricing dimensions</span></span>

<span data-ttu-id="31aa9-111">PSA обавља испоруку помоћу подразумеваног скуп димензија за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="31aa9-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="31aa9-112">Можете да их видите тако што ћете отићи на **Project Service** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="31aa9-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="31aa9-113">У запису параметра, на картици **Димензије за одређивање цена засноване на износима** проверите да ли улога **msdyn_resourcecategory** и организациона јединица ресурса **msdyn_organizationalunit** имају поља **Применљиво на продају** и **Применљиво на трошкове** подешена на **Да**.</span><span class="sxs-lookup"><span data-stu-id="31aa9-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="31aa9-114">Ово ће вам омогућити подешавање цене и трошка за сваку комбинацију улоге и организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="31aa9-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![Снимак екрана Project Service параметара са маркираном ставком „Применљиво на продају“](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="31aa9-116">Ако сте користили унапред дефинисана поља улоге и организационих јединица као димензије за одређивање цена пре верзије 3 апликације PSA, неће бити никаквих приметних промена.</span><span class="sxs-lookup"><span data-stu-id="31aa9-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="31aa9-117">Можете да наставите да користите Project Service као и обично.</span><span class="sxs-lookup"><span data-stu-id="31aa9-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="31aa9-118">Ако је потребно да одредите цену или трошкове ресурса помоћу додатних атрибута, можете да креирате прилагођена поља, ентитете и димензије.</span><span class="sxs-lookup"><span data-stu-id="31aa9-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="31aa9-119">Да бисте добили више информација, погледајте следеће теме, али имајте на уму да морате да довршите процедуре по доленаведеном редоследу:</span><span class="sxs-lookup"><span data-stu-id="31aa9-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="31aa9-120">Креирање прилагођених поља и ентитета</span><span class="sxs-lookup"><span data-stu-id="31aa9-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="31aa9-121">Додавање прилагођених поља у подешавање цена и ентитете трансакције</span><span class="sxs-lookup"><span data-stu-id="31aa9-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="31aa9-122">Подешавање прилагођених поља као димензија за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="31aa9-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="31aa9-123">Ажурирање атрибута додатних компоненти тако да укључују нове димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="31aa9-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="31aa9-124">Одређивање цене времена људског ресурса</span><span class="sxs-lookup"><span data-stu-id="31aa9-124">Pricing human resource time</span></span>
<span data-ttu-id="31aa9-125">Како организација одређује цену времена људског ресурса је често значајно стратешко питање које директно утиче на профитабилност организације.</span><span class="sxs-lookup"><span data-stu-id="31aa9-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="31aa9-126">Сарађујте са финансијским тимовима и будите мудри када ваша организација буде спремна да утврди како жели да подеси стопе наплате и трошкова за време људског ресурса.</span><span class="sxs-lookup"><span data-stu-id="31aa9-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="31aa9-127">Друга питања која се тичу формирања цена подразумевају да ли поново да користите поља или ентитете који тренутно нису димензије за одређивање цена, али се примењују као димензија за одређивање цена у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="31aa9-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="31aa9-128">Поља као што су **Категорија трансакције** (**msdyn_transactioncategory**) и **Ресурс који може да се резервише** (**bookableresource**) су примери могућих димензија.</span><span class="sxs-lookup"><span data-stu-id="31aa9-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="31aa9-129">Требало би да размотрите и да ли ваша димензија за одређивање цена треба да буде табела или скуп опција.</span><span class="sxs-lookup"><span data-stu-id="31aa9-129">You should also consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="31aa9-130">Ако предвиђате промене вредности димензије које ће премашити 10 или 12, а потребни су вам додатни атрибути за ове вредности, можете да креирате ентитет, а не скуп опција.</span><span class="sxs-lookup"><span data-stu-id="31aa9-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="31aa9-131">Одржавање скуп опција, као што је додавање или уклањање вредности, захтева администратора или програмера, док већина корисника може да додаје нове редове у табелу.</span><span class="sxs-lookup"><span data-stu-id="31aa9-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="31aa9-132">Следећи пример приказује курсне стопе које су подешене на основу улоге и организационе јединице ресурса коме припада ресурс.</span><span class="sxs-lookup"><span data-stu-id="31aa9-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="31aa9-133">Стопе трошкова се обично заснивају на групи личних доходака запослених и организационој јединици којој припадају.</span><span class="sxs-lookup"><span data-stu-id="31aa9-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="31aa9-134">У овом примеру, табеле са стопама наплате и стопама трошкова ће изгледати овако:</span><span class="sxs-lookup"><span data-stu-id="31aa9-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="31aa9-135">**Примери стопа наплате**</span><span class="sxs-lookup"><span data-stu-id="31aa9-135">**Sample bill rates**</span></span>

| <span data-ttu-id="31aa9-136">Улога</span><span class="sxs-lookup"><span data-stu-id="31aa9-136">Role</span></span>        | <span data-ttu-id="31aa9-137">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="31aa9-137">Org Unit</span></span>    |<span data-ttu-id="31aa9-138">Јединица</span><span class="sxs-lookup"><span data-stu-id="31aa9-138">Unit</span></span>      |<span data-ttu-id="31aa9-139">Цена</span><span class="sxs-lookup"><span data-stu-id="31aa9-139">Price</span></span>      |<span data-ttu-id="31aa9-140">Валута</span><span class="sxs-lookup"><span data-stu-id="31aa9-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="31aa9-141">Програмер</span><span class="sxs-lookup"><span data-stu-id="31aa9-141">Developer</span></span>   | <span data-ttu-id="31aa9-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="31aa9-142">Contoso US</span></span>  |<span data-ttu-id="31aa9-143">Hour</span><span class="sxs-lookup"><span data-stu-id="31aa9-143">Hour</span></span> | <span data-ttu-id="31aa9-144">200</span><span class="sxs-lookup"><span data-stu-id="31aa9-144">200</span></span>|<span data-ttu-id="31aa9-145">USD</span><span class="sxs-lookup"><span data-stu-id="31aa9-145">USD</span></span>     |
| <span data-ttu-id="31aa9-146">Програмер</span><span class="sxs-lookup"><span data-stu-id="31aa9-146">Developer</span></span>   | <span data-ttu-id="31aa9-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="31aa9-147">Contoso India</span></span> |<span data-ttu-id="31aa9-148">Hour</span><span class="sxs-lookup"><span data-stu-id="31aa9-148">Hour</span></span>|   <span data-ttu-id="31aa9-149">112.</span><span class="sxs-lookup"><span data-stu-id="31aa9-149">112</span></span>|<span data-ttu-id="31aa9-150">USD</span><span class="sxs-lookup"><span data-stu-id="31aa9-150">USD</span></span>     |


<span data-ttu-id="31aa9-151">**Примери стопа трошкова**</span><span class="sxs-lookup"><span data-stu-id="31aa9-151">**Sample cost rates**</span></span>

| <span data-ttu-id="31aa9-152">Група личних доходака</span><span class="sxs-lookup"><span data-stu-id="31aa9-152">Salary Band</span></span>     | <span data-ttu-id="31aa9-153">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="31aa9-153">Org Unit</span></span>    |<span data-ttu-id="31aa9-154">Јединица</span><span class="sxs-lookup"><span data-stu-id="31aa9-154">Unit</span></span>      |<span data-ttu-id="31aa9-155">Цена</span><span class="sxs-lookup"><span data-stu-id="31aa9-155">Price</span></span>      |<span data-ttu-id="31aa9-156">Валута</span><span class="sxs-lookup"><span data-stu-id="31aa9-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="31aa9-157">Моје предузеће_Прва група личних доходака</span><span class="sxs-lookup"><span data-stu-id="31aa9-157">My company_Band1</span></span> | <span data-ttu-id="31aa9-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="31aa9-158">Contoso US</span></span>  |<span data-ttu-id="31aa9-159">Hour</span><span class="sxs-lookup"><span data-stu-id="31aa9-159">Hour</span></span> | <span data-ttu-id="31aa9-160">145.</span><span class="sxs-lookup"><span data-stu-id="31aa9-160">145</span></span>|<span data-ttu-id="31aa9-161">USD</span><span class="sxs-lookup"><span data-stu-id="31aa9-161">USD</span></span>     |
| <span data-ttu-id="31aa9-162">Моје предузеће_друга група личних доходака</span><span class="sxs-lookup"><span data-stu-id="31aa9-162">My company_Band2</span></span> | <span data-ttu-id="31aa9-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="31aa9-163">Contoso India</span></span> |<span data-ttu-id="31aa9-164">Hour</span><span class="sxs-lookup"><span data-stu-id="31aa9-164">Hour</span></span>|   <span data-ttu-id="31aa9-165">67.</span><span class="sxs-lookup"><span data-stu-id="31aa9-165">67</span></span>|<span data-ttu-id="31aa9-166">USD</span><span class="sxs-lookup"><span data-stu-id="31aa9-166">USD</span></span>     |
