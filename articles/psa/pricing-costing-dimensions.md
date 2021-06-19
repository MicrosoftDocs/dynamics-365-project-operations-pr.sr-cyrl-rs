---
title: Матична страница за димензије одређивања цена и обрачуна трошкова
description: Ова тема обезбеђује преглед димензија за одређивање цена.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 9a2e2f7ed394229bbc553af9e616a6f322857195
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009274"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="367c0-103">Матична страница за димензије одређивања цена и обрачуна трошкова</span><span class="sxs-lookup"><span data-stu-id="367c0-103">Pricing and costing dimensions home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="367c0-104">На димензије које се користе за одређивање цена и трошкова рада у пројектним организацијама утичу следећи атрибути:</span><span class="sxs-lookup"><span data-stu-id="367c0-104">The dimensions used to set labor pricing and costing in project-based organizations are influenced by the following attributes:</span></span>

- <span data-ttu-id="367c0-105">Људи који раде посао сличан свом искуству, улози или географској локацији</span><span class="sxs-lookup"><span data-stu-id="367c0-105">People doing work similar to their experience, role, or geography</span></span>
- <span data-ttu-id="367c0-106">Посао који треба обавити, сличан по сложености или добу дана</span><span class="sxs-lookup"><span data-stu-id="367c0-106">Work to be performed similar to its complexity or time of day</span></span>

<span data-ttu-id="367c0-107">С обзиром на типичну природу ових атрибута посла и људи који су потребни за обављање посла, постоје две врсте вредности димензија цене које су доступне у услузи Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="367c0-107">Given the typical nature of these attrubutes of the work and the people required to perform the work, there are two types of pricing dimension values available in Project Service Automation:</span></span> 

- <span data-ttu-id="367c0-108">**Скупови опција** – Атрибути који представљају фиксна набрајања за скуп вредности.</span><span class="sxs-lookup"><span data-stu-id="367c0-108">**Option sets** - Attributes that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="367c0-109">**Вредности засноване на ентитетима** – Атрибути који могу имати различит скуп вредности које су коначне, али се временом могу мењати.</span><span class="sxs-lookup"><span data-stu-id="367c0-109">**Entity-based values** - Attributes that can have a varied set of values that are finite but can change over time.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="367c0-110">Димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="367c0-110">Pricing dimensions</span></span>

<span data-ttu-id="367c0-111">PSA обавља испоруку помоћу подразумеваног скуп димензија за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="367c0-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="367c0-112">Можете да их видите тако што ћете отићи на **Project Service** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="367c0-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="367c0-113">У запису параметра, на картици **Димензије за одређивање цена засноване на износима** проверите да ли улога **msdyn_resourcecategory** и организациона јединица ресурса **msdyn_organizationalunit** имају поља **Применљиво на продају** и **Применљиво на трошкове** подешена на **Да**.</span><span class="sxs-lookup"><span data-stu-id="367c0-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="367c0-114">Ово ће вам омогућити подешавање цене и трошка за сваку комбинацију улоге и организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="367c0-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![Снимак екрана Project Service параметара са маркираном ставком „Применљиво на продају“](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="367c0-116">Ако сте користили унапред дефинисана поља улоге и организационих јединица као димензије за одређивање цена пре верзије 3 апликације PSA, неће бити никаквих приметних промена.</span><span class="sxs-lookup"><span data-stu-id="367c0-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="367c0-117">Можете да наставите да користите Project Service као и обично.</span><span class="sxs-lookup"><span data-stu-id="367c0-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="367c0-118">Ако је потребно да одредите цену или трошкове ресурса помоћу додатних атрибута, можете да креирате прилагођена поља, ентитете и димензије.</span><span class="sxs-lookup"><span data-stu-id="367c0-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="367c0-119">Да бисте добили више информација, погледајте следеће теме, али имајте на уму да морате да довршите процедуре по доленаведеном редоследу:</span><span class="sxs-lookup"><span data-stu-id="367c0-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="367c0-120">Креирање прилагођених поља и ентитета</span><span class="sxs-lookup"><span data-stu-id="367c0-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="367c0-121">Додавање прилагођених поља у подешавање цена и ентитете трансакције</span><span class="sxs-lookup"><span data-stu-id="367c0-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="367c0-122">Подешавање прилагођених поља као димензија за одређивање цена </span><span class="sxs-lookup"><span data-stu-id="367c0-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="367c0-123">Ажурирање атрибута додатних компоненти тако да укључују нове димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="367c0-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="367c0-124">Одређивање цене времена људског ресурса</span><span class="sxs-lookup"><span data-stu-id="367c0-124">Pricing human resource time</span></span>
<span data-ttu-id="367c0-125">Како организација одређује цену времена људског ресурса је често значајно стратешко питање које директно утиче на профитабилност организације.</span><span class="sxs-lookup"><span data-stu-id="367c0-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="367c0-126">Сарађујте са финансијским тимовима и будите мудри када ваша организација буде спремна да утврди како жели да подеси стопе наплате и трошкова за време људског ресурса.</span><span class="sxs-lookup"><span data-stu-id="367c0-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="367c0-127">Друга питања која се тичу формирања цена подразумевају да ли поново да користите поља или ентитете који тренутно нису димензије за одређивање цена, али се примењују као димензија за одређивање цена у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="367c0-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="367c0-128">Поља као што су **Категорија трансакције** (**msdyn_transactioncategory**) и **Ресурс који може да се резервише** (**bookableresource**) су примери могућих димензија.</span><span class="sxs-lookup"><span data-stu-id="367c0-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="367c0-129">Размотрите и да ли ваша димензија за одређивање цена треба да буде табела или скуп опција.</span><span class="sxs-lookup"><span data-stu-id="367c0-129">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="367c0-130">Ако предвиђате промене вредности димензије које ће премашити 10 или 12, а потребни су вам додатни атрибути за ове вредности, боље је да креирате ентитет него скуп опција.</span><span class="sxs-lookup"><span data-stu-id="367c0-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, create an entity rather than an option set.</span></span> <span data-ttu-id="367c0-131">Одржавање скуп опција, као што је додавање или уклањање вредности, захтева администратора или програмера, док већина пословних корисника може да додаје нове редове у табелу.</span><span class="sxs-lookup"><span data-stu-id="367c0-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most business users.</span></span>

<span data-ttu-id="367c0-132">Следећи пример приказује курсне стопе које су подешене на основу улоге и организационе јединице ресурса коме припада ресурс.</span><span class="sxs-lookup"><span data-stu-id="367c0-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="367c0-133">Стопе трошкова се обично заснивају на групи личних доходака запослених и организационој јединици којој припадају.</span><span class="sxs-lookup"><span data-stu-id="367c0-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="367c0-134">У овом примеру, табеле са стопама наплате и стопама трошкова ће изгледати овако:</span><span class="sxs-lookup"><span data-stu-id="367c0-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="367c0-135">**Примери стопа наплате**</span><span class="sxs-lookup"><span data-stu-id="367c0-135">**Sample bill rates**</span></span>

| <span data-ttu-id="367c0-136">Улога</span><span class="sxs-lookup"><span data-stu-id="367c0-136">Role</span></span>        | <span data-ttu-id="367c0-137">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="367c0-137">Org Unit</span></span>    |<span data-ttu-id="367c0-138">Јединица</span><span class="sxs-lookup"><span data-stu-id="367c0-138">Unit</span></span>      |<span data-ttu-id="367c0-139">Цена</span><span class="sxs-lookup"><span data-stu-id="367c0-139">Price</span></span>      |<span data-ttu-id="367c0-140">Валута</span><span class="sxs-lookup"><span data-stu-id="367c0-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="367c0-141">Програмер</span><span class="sxs-lookup"><span data-stu-id="367c0-141">Developer</span></span>   | <span data-ttu-id="367c0-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="367c0-142">Contoso US</span></span>  |<span data-ttu-id="367c0-143">Сат</span><span class="sxs-lookup"><span data-stu-id="367c0-143">Hour</span></span> | <span data-ttu-id="367c0-144">200</span><span class="sxs-lookup"><span data-stu-id="367c0-144">200</span></span>|<span data-ttu-id="367c0-145">USD решење</span><span class="sxs-lookup"><span data-stu-id="367c0-145">USD</span></span>     |
| <span data-ttu-id="367c0-146">Програмер</span><span class="sxs-lookup"><span data-stu-id="367c0-146">Developer</span></span>   | <span data-ttu-id="367c0-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="367c0-147">Contoso India</span></span> |<span data-ttu-id="367c0-148">Сат</span><span class="sxs-lookup"><span data-stu-id="367c0-148">Hour</span></span>|   <span data-ttu-id="367c0-149">112</span><span class="sxs-lookup"><span data-stu-id="367c0-149">112</span></span>|<span data-ttu-id="367c0-150">USD решење</span><span class="sxs-lookup"><span data-stu-id="367c0-150">USD</span></span>     |


<span data-ttu-id="367c0-151">**Примери стопа трошкова**</span><span class="sxs-lookup"><span data-stu-id="367c0-151">**Sample cost rates**</span></span>

| <span data-ttu-id="367c0-152">Група личних доходака</span><span class="sxs-lookup"><span data-stu-id="367c0-152">Salary Band</span></span>     | <span data-ttu-id="367c0-153">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="367c0-153">Org Unit</span></span>    |<span data-ttu-id="367c0-154">Јединица</span><span class="sxs-lookup"><span data-stu-id="367c0-154">Unit</span></span>      |<span data-ttu-id="367c0-155">Цена</span><span class="sxs-lookup"><span data-stu-id="367c0-155">Price</span></span>      |<span data-ttu-id="367c0-156">Валута</span><span class="sxs-lookup"><span data-stu-id="367c0-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="367c0-157">Моје предузеће_Прва група личних доходака</span><span class="sxs-lookup"><span data-stu-id="367c0-157">My company_Band1</span></span> | <span data-ttu-id="367c0-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="367c0-158">Contoso US</span></span>  |<span data-ttu-id="367c0-159">Сат</span><span class="sxs-lookup"><span data-stu-id="367c0-159">Hour</span></span> | <span data-ttu-id="367c0-160">145</span><span class="sxs-lookup"><span data-stu-id="367c0-160">145</span></span>|<span data-ttu-id="367c0-161">USD решење</span><span class="sxs-lookup"><span data-stu-id="367c0-161">USD</span></span>     |
| <span data-ttu-id="367c0-162">Моје предузеће_друга група личних доходака</span><span class="sxs-lookup"><span data-stu-id="367c0-162">My company_Band2</span></span> | <span data-ttu-id="367c0-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="367c0-163">Contoso India</span></span> |<span data-ttu-id="367c0-164">Сат</span><span class="sxs-lookup"><span data-stu-id="367c0-164">Hour</span></span>|   <span data-ttu-id="367c0-165">67</span><span class="sxs-lookup"><span data-stu-id="367c0-165">67</span></span>|<span data-ttu-id="367c0-166">USD решење</span><span class="sxs-lookup"><span data-stu-id="367c0-166">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]