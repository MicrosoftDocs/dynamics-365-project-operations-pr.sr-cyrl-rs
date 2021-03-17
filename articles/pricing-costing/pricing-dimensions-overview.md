---
title: Преглед димензија за одређивање цена
description: Ова тема пружа информације о димензијама за одређивање цена у услузи Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 11/30/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ff675823d84c6e2b83be1e313f881bd672e53981
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275421"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="b6d48-103">Преглед димензија за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="b6d48-103">Pricing dimensions overview</span></span>

<span data-ttu-id="b6d48-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="b6d48-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b6d48-105">Димензије које се користе у људским ресурсима за подешавање цена и трошкова спадају у две категорије:</span><span class="sxs-lookup"><span data-stu-id="b6d48-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="b6d48-106">Људи</span><span class="sxs-lookup"><span data-stu-id="b6d48-106">People</span></span>
- <span data-ttu-id="b6d48-107">Планирани рад</span><span class="sxs-lookup"><span data-stu-id="b6d48-107">Planned work</span></span>

<span data-ttu-id="b6d48-108">Због тога постоје две врсте вредности димензија за одређивање цена које су доступне:</span><span class="sxs-lookup"><span data-stu-id="b6d48-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="b6d48-109">**Скупови опција**: Димензије које представљају фиксна набрајања за скуп вредности.</span><span class="sxs-lookup"><span data-stu-id="b6d48-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="b6d48-110">**Вредности засноване на ентитетима**: Димензије које могу бити различит скуп вредности.</span><span class="sxs-lookup"><span data-stu-id="b6d48-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="b6d48-111">Димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="b6d48-111">Pricing dimensions</span></span>

<span data-ttu-id="b6d48-112">Dynamics 365 Project Operations обавља испоруку помоћу подразумеваног скупа димензија за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="b6d48-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="b6d48-113">Ове димензије за одређивање цена можете да их видите тако што ћете отићи на **Project Operations** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="b6d48-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="b6d48-114">У запису параметра, на картици **Димензије за одређивање цена засноване на износима** проверите да ли улога **msdyn_resourcecategory** и организациона јединица ресурса **msdyn_organizationalunit** имају поља **Применљиво на продају** и **Применљиво на трошкове** подешена на **Да**.</span><span class="sxs-lookup"><span data-stu-id="b6d48-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="b6d48-115">Када су ова поља омогућена, можете да подесите цену и трошак за сваку комбинацију улоге и организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="b6d48-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

![Снимак екрана Project Service параметара са маркираном ставком „Применљиво на продају“](media/PS-OOB-parameters.png)

<span data-ttu-id="b6d48-117">Ако је потребно да одредите цену или трошкове ресурса помоћу додатних атрибута, можете да креирате прилагођена поља, ентитете и димензије.</span><span class="sxs-lookup"><span data-stu-id="b6d48-117">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="b6d48-118">Погледајте следећи одељак за више информација.</span><span class="sxs-lookup"><span data-stu-id="b6d48-118">For more information, see the following topics.</span></span> 
  
  > [!NOTE]
  > <span data-ttu-id="b6d48-119">Поступци морају бити завршени како би били наведени.</span><span class="sxs-lookup"><span data-stu-id="b6d48-119">The procedures must be completed in the order they are listed.</span></span>

1. [<span data-ttu-id="b6d48-120">Креирање решења за прилагођене димензије одређивања цена</span><span class="sxs-lookup"><span data-stu-id="b6d48-120">Create a solution for custom pricing dimensions</span></span>](../sales/create-solution-custompd.md)
2. [<span data-ttu-id="b6d48-121">Креирање прилагођених поља и ентитета</span><span class="sxs-lookup"><span data-stu-id="b6d48-121">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md)
3. [<span data-ttu-id="b6d48-122">Додавање прилагођених поља у подешавање цена и ентитете трансакције </span><span class="sxs-lookup"><span data-stu-id="b6d48-122">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
4. [<span data-ttu-id="b6d48-123">Подешавање прилагођених поља као димензија за одређивање цена </span><span class="sxs-lookup"><span data-stu-id="b6d48-123">Set up custom fields as pricing dimensions</span></span>](set-up-custom-fields-pricing-dimensions.md)
5. [<span data-ttu-id="b6d48-124">Ажурирање атрибута додатних компоненти тако да укључују нове димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="b6d48-124">Update plug-in attributes to include new pricing dimensions</span></span>](update-plugin-attributes-pd.md)


## <a name="pricing-human-resource-time"></a><span data-ttu-id="b6d48-125">Одређивање цене времена људског ресурса</span><span class="sxs-lookup"><span data-stu-id="b6d48-125">Pricing human resource time</span></span>
<span data-ttu-id="b6d48-126">Како организација одређује цену времена људског ресурса је често значајно стратешко питање које директно утиче на профитабилност организације.</span><span class="sxs-lookup"><span data-stu-id="b6d48-126">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="b6d48-127">Сарађујте са финансијским тимовима и будите мудри када ваша организација буде спремна да утврди како жели да подеси стопе наплате и трошкова за време људског ресурса.</span><span class="sxs-lookup"><span data-stu-id="b6d48-127">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="b6d48-128">Друга питања која се тичу формирања цена подразумевају да ли поново да користите поља или ентитете који тренутно нису димензије за одређивање цена, али се примењују као димензија за одређивање цена у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="b6d48-128">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="b6d48-129">Поља као што су **Категорија трансакције** (**msdyn_transactioncategory**) и **Ресурс који може да се резервише** (**bookableresource**) су примери могућих димензија.</span><span class="sxs-lookup"><span data-stu-id="b6d48-129">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="b6d48-130">Размотрите и да ли ваша димензија за одређивање цена треба да буде табела или скуп опција.</span><span class="sxs-lookup"><span data-stu-id="b6d48-130">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="b6d48-131">Ако предвиђате промене вредности димензије које ће премашити 10 или 12, а потребни су вам додатни атрибути за ове вредности, можете да креирате ентитет, а не скуп опција.</span><span class="sxs-lookup"><span data-stu-id="b6d48-131">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="b6d48-132">Одржавање скуп опција, као што је додавање или уклањање вредности, захтева администратора или програмера, док већина корисника може да додаје нове редове у табелу.</span><span class="sxs-lookup"><span data-stu-id="b6d48-132">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="b6d48-133">Следећи пример приказује курсне стопе које су подешене на основу улоге и организационе јединице ресурса коме припада ресурс.</span><span class="sxs-lookup"><span data-stu-id="b6d48-133">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="b6d48-134">Стопе трошкова се обично заснивају на групи личних доходака запослених и организационој јединици којој припадају.</span><span class="sxs-lookup"><span data-stu-id="b6d48-134">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="b6d48-135">У овом примеру, табеле са стопама наплате и стопама трошкова ће изгледати овако:</span><span class="sxs-lookup"><span data-stu-id="b6d48-135">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="b6d48-136">**Примери стопа наплате**</span><span class="sxs-lookup"><span data-stu-id="b6d48-136">**Sample bill rates**</span></span>

| <span data-ttu-id="b6d48-137">Улога</span><span class="sxs-lookup"><span data-stu-id="b6d48-137">Role</span></span>        | <span data-ttu-id="b6d48-138">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="b6d48-138">Org Unit</span></span>    |<span data-ttu-id="b6d48-139">Јединица</span><span class="sxs-lookup"><span data-stu-id="b6d48-139">Unit</span></span>      |<span data-ttu-id="b6d48-140">Цена</span><span class="sxs-lookup"><span data-stu-id="b6d48-140">Price</span></span>      |<span data-ttu-id="b6d48-141">Валута</span><span class="sxs-lookup"><span data-stu-id="b6d48-141">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="b6d48-142">Програмер</span><span class="sxs-lookup"><span data-stu-id="b6d48-142">Developer</span></span>   | <span data-ttu-id="b6d48-143">Contoso US</span><span class="sxs-lookup"><span data-stu-id="b6d48-143">Contoso US</span></span>  |<span data-ttu-id="b6d48-144">Hour</span><span class="sxs-lookup"><span data-stu-id="b6d48-144">Hour</span></span> | <span data-ttu-id="b6d48-145">200</span><span class="sxs-lookup"><span data-stu-id="b6d48-145">200</span></span>|<span data-ttu-id="b6d48-146">USD</span><span class="sxs-lookup"><span data-stu-id="b6d48-146">USD</span></span>     |
| <span data-ttu-id="b6d48-147">Програмер</span><span class="sxs-lookup"><span data-stu-id="b6d48-147">Developer</span></span>   | <span data-ttu-id="b6d48-148">Contoso India</span><span class="sxs-lookup"><span data-stu-id="b6d48-148">Contoso India</span></span> |<span data-ttu-id="b6d48-149">Hour</span><span class="sxs-lookup"><span data-stu-id="b6d48-149">Hour</span></span>|   <span data-ttu-id="b6d48-150">112.</span><span class="sxs-lookup"><span data-stu-id="b6d48-150">112</span></span>|<span data-ttu-id="b6d48-151">USD</span><span class="sxs-lookup"><span data-stu-id="b6d48-151">USD</span></span>     |


<span data-ttu-id="b6d48-152">**Примери стопа трошкова**</span><span class="sxs-lookup"><span data-stu-id="b6d48-152">**Sample cost rates**</span></span>

| <span data-ttu-id="b6d48-153">Група личних доходака</span><span class="sxs-lookup"><span data-stu-id="b6d48-153">Salary Band</span></span>     | <span data-ttu-id="b6d48-154">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="b6d48-154">Org Unit</span></span>    |<span data-ttu-id="b6d48-155">Јединица</span><span class="sxs-lookup"><span data-stu-id="b6d48-155">Unit</span></span>      |<span data-ttu-id="b6d48-156">Цена</span><span class="sxs-lookup"><span data-stu-id="b6d48-156">Price</span></span>      |<span data-ttu-id="b6d48-157">Валута</span><span class="sxs-lookup"><span data-stu-id="b6d48-157">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="b6d48-158">Моје предузеће_Прва група личних доходака</span><span class="sxs-lookup"><span data-stu-id="b6d48-158">My company_Band1</span></span> | <span data-ttu-id="b6d48-159">Contoso US</span><span class="sxs-lookup"><span data-stu-id="b6d48-159">Contoso US</span></span>  |<span data-ttu-id="b6d48-160">Hour</span><span class="sxs-lookup"><span data-stu-id="b6d48-160">Hour</span></span> | <span data-ttu-id="b6d48-161">145.</span><span class="sxs-lookup"><span data-stu-id="b6d48-161">145</span></span>|<span data-ttu-id="b6d48-162">USD</span><span class="sxs-lookup"><span data-stu-id="b6d48-162">USD</span></span>     |
| <span data-ttu-id="b6d48-163">Моје предузеће_друга група личних доходака</span><span class="sxs-lookup"><span data-stu-id="b6d48-163">My company_Band2</span></span> | <span data-ttu-id="b6d48-164">Contoso India</span><span class="sxs-lookup"><span data-stu-id="b6d48-164">Contoso India</span></span> |<span data-ttu-id="b6d48-165">Hour</span><span class="sxs-lookup"><span data-stu-id="b6d48-165">Hour</span></span>|   <span data-ttu-id="b6d48-166">67.</span><span class="sxs-lookup"><span data-stu-id="b6d48-166">67</span></span>|<span data-ttu-id="b6d48-167">USD</span><span class="sxs-lookup"><span data-stu-id="b6d48-167">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]