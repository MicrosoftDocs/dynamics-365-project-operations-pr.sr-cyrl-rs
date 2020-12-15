---
title: Коришћење ресурса који може да се резервише као аспекта за одређивање цена
description: Ова тема пружа информације о томе како да користите ресурс који се може резервисати као димензије за одређивање цена.
author: Rumant
manager: tfehr
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b0c5cb85f7c43f7b2fd9c367d7f7ac9c3250e0a1
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643101"
---
# <a name="use-a-bookable-resource-as-a-pricing-dimension"></a><span data-ttu-id="45b41-103">Коришћење ресурса који може да се резервише као аспекта за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="45b41-103">Use a bookable resource as a pricing dimension</span></span>

 <span data-ttu-id="45b41-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="45b41-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

<span data-ttu-id="45b41-105">Ова тема пружа информације о томе како да користите ресурс који се може резервисати као димензије за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="45b41-105">This topic provides information about how to use a bookable resource as a pricing dimension.</span></span> <span data-ttu-id="45b41-106">Ако је ваша стратегија одређивања цена подешена тако да сваки ресурс који можете резервирати мора да има одређену цену или стопу трошкова, користите ресурс који можете резервирати као димензију формирања цена.</span><span class="sxs-lookup"><span data-stu-id="45b41-106">If your pricing strategy is set up so that each bookable resource must have a specific price or cost rate, use a bookable resource as a pricing dimension.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45b41-107">Предуслови</span><span class="sxs-lookup"><span data-stu-id="45b41-107">Prerequisites</span></span>
<span data-ttu-id="45b41-108">Пре него што довршите процедуре у овој теми, морате да имате ново решење димензије за формирање цена за организацију.</span><span class="sxs-lookup"><span data-stu-id="45b41-108">Before you complete the procedures in this topic, you must have a new pricing dimension solution for your organization.</span></span> <span data-ttu-id="45b41-109">Ако их већ нисте креирали, погледајте [Креирање прилагођених поља и ентитета](../pricing-costing/create-custom-fields-entities-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="45b41-109">If you haven't already created one, see [Create custom fields and entities](../pricing-costing/create-custom-fields-entities-pricing-dimensions.md).</span></span>

## <a name="add-the-bookable-resource-field-to-forms-and-views"></a><span data-ttu-id="45b41-110">Додавање поља Ресурс који се може резервисати у обрасце и приказе</span><span class="sxs-lookup"><span data-stu-id="45b41-110">Add the Bookable Resource field to forms and views</span></span>
<span data-ttu-id="45b41-111">Да би поље **Ресурс који се може резервисати** било видљиво у решењу димензија формирања цена, морате да додате поље свим обрасцима и приказима као ентитет.</span><span class="sxs-lookup"><span data-stu-id="45b41-111">To make the **Bookable Resource** field visible in the pricing dimension solution, you need to add the field to all the forms and views as an entity.</span></span>

<span data-ttu-id="45b41-112">Следећа табела наводи све готове обрасце и приказе по ентитетима.</span><span class="sxs-lookup"><span data-stu-id="45b41-112">The following table lists all of the out-of-the box forms and views, by entity.</span></span> <span data-ttu-id="45b41-113">Такође ћете морати да додате ново поље у све додатне обрасце или приказе у вашим прилагођеним ентитетима.</span><span class="sxs-lookup"><span data-stu-id="45b41-113">You will also need to add the new field to any additional forms or views in your customized entities.</span></span>

|   <span data-ttu-id="45b41-114">Entity</span><span class="sxs-lookup"><span data-stu-id="45b41-114">Entity</span></span>        | <span data-ttu-id="45b41-115">Обрасци</span><span class="sxs-lookup"><span data-stu-id="45b41-115">Forms</span></span>   |<span data-ttu-id="45b41-116">Прикази</span><span class="sxs-lookup"><span data-stu-id="45b41-116">Views</span></span>        |
| ------------------------------|---------------------------------|----------------------------------|
|  <span data-ttu-id="45b41-117">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="45b41-117">Role Price</span></span>| <span data-ttu-id="45b41-118">Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-118">Information</span></span> | <span data-ttu-id="45b41-119">- Активне цене категорија ресурса</span><span class="sxs-lookup"><span data-stu-id="45b41-119">- Active Resource Category Prices</span></span><br> <span data-ttu-id="45b41-120">- Везано за цену категорије ресурса</span><span class="sxs-lookup"><span data-stu-id="45b41-120">- Resource Category Price Associated</span></span> |
|  <span data-ttu-id="45b41-121">Провизија на цену улоге</span><span class="sxs-lookup"><span data-stu-id="45b41-121">Role Price Markup</span></span>| <span data-ttu-id="45b41-122">Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-122">Information</span></span>| <span data-ttu-id="45b41-123">- Активне провизије на цену улоге</span><span class="sxs-lookup"><span data-stu-id="45b41-123">- Active Role Price Markup</span></span><br><span data-ttu-id="45b41-124">- Везано за провизију на цену улоге</span><span class="sxs-lookup"><span data-stu-id="45b41-124">- Role Price Markup Associated</span></span> |
|  <span data-ttu-id="45b41-125">Детаљ ставке понуде</span><span class="sxs-lookup"><span data-stu-id="45b41-125">Quote line detail</span></span>| <span data-ttu-id="45b41-126">- Информације о пројекту</span><span class="sxs-lookup"><span data-stu-id="45b41-126">- Project Information</span></span><br><span data-ttu-id="45b41-127">- Брзо креирање пројекта</span><span class="sxs-lookup"><span data-stu-id="45b41-127">- Project Quick Create</span></span>| <span data-ttu-id="45b41-128">- Активни детаљ ставке понуде</span><span class="sxs-lookup"><span data-stu-id="45b41-128">- Active Quote Line Detail</span></span><br><span data-ttu-id="45b41-129">- Комбиновани детаљи ставке понуде</span><span class="sxs-lookup"><span data-stu-id="45b41-129">- Combined Quote Line Details</span></span><br><span data-ttu-id="45b41-130">- Везано за детаље ставки понуде</span><span class="sxs-lookup"><span data-stu-id="45b41-130">- Quote Line Detail Associated</span></span> |
|  <span data-ttu-id="45b41-131">Детаљ предмета уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="45b41-131">Project Contract line detail</span></span>| <span data-ttu-id="45b41-132">- Информације о пројекту</span><span class="sxs-lookup"><span data-stu-id="45b41-132">- Project Information</span></span><br><span data-ttu-id="45b41-133">- Брзо креирање пројекта</span><span class="sxs-lookup"><span data-stu-id="45b41-133">- Project Quick Create</span></span>| <span data-ttu-id="45b41-134">- Комбиновани детаљи предмета уговора</span><span class="sxs-lookup"><span data-stu-id="45b41-134">- Combined Contract Line Details</span></span><br><span data-ttu-id="45b41-135">- Активни детаљи предмета уговора</span><span class="sxs-lookup"><span data-stu-id="45b41-135">- Active Contract Line Details</span></span><br><span data-ttu-id="45b41-136">- Везано за детаље предмета уговора</span><span class="sxs-lookup"><span data-stu-id="45b41-136">- Contract Line Detail Associated</span></span> |
|  <span data-ttu-id="45b41-137">Пројектни задатак</span><span class="sxs-lookup"><span data-stu-id="45b41-137">Project Task</span></span>| <span data-ttu-id="45b41-138">- Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-138">- Information</span></span><br><span data-ttu-id="45b41-139">- Нови образац</span><span class="sxs-lookup"><span data-stu-id="45b41-139">- New Form</span></span>| &nbsp; |
|  <span data-ttu-id="45b41-140">Члан пројектног тима</span><span class="sxs-lookup"><span data-stu-id="45b41-140">Project Team Member</span></span>| <span data-ttu-id="45b41-141">- Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-141">- Information</span></span><br><span data-ttu-id="45b41-142">- Нови образац</span><span class="sxs-lookup"><span data-stu-id="45b41-142">- New Form</span></span>| <span data-ttu-id="45b41-143">- Активни чланови пројектног тима</span><span class="sxs-lookup"><span data-stu-id="45b41-143">- Active Project Team Members</span></span><br><span data-ttu-id="45b41-144">- Чланови пројектног тима</span><span class="sxs-lookup"><span data-stu-id="45b41-144">- Project Team Members</span></span><br><span data-ttu-id="45b41-145">- Везани чланови пројектног тима</span><span class="sxs-lookup"><span data-stu-id="45b41-145">- Project Team members Associated</span></span> |
|  <span data-ttu-id="45b41-146">Ставка времена</span><span class="sxs-lookup"><span data-stu-id="45b41-146">Time Entry</span></span>| <span data-ttu-id="45b41-147">- Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-147">- Information</span></span><br><span data-ttu-id="45b41-148">- Креирање ставке времена</span><span class="sxs-lookup"><span data-stu-id="45b41-148">- Create Time Entry</span></span>| <span data-ttu-id="45b41-149">- Моје ставке времена према датуму</span><span class="sxs-lookup"><span data-stu-id="45b41-149">- My Time Entries By Date</span></span><br><span data-ttu-id="45b41-150">- Моје ставке времена за ову седмицу</span><span class="sxs-lookup"><span data-stu-id="45b41-150">- My Time Entries for this Week</span></span><br><span data-ttu-id="45b41-151">- Ставке времена за одобрење</span><span class="sxs-lookup"><span data-stu-id="45b41-151">- Time Entries for Approval</span></span>|
|  <span data-ttu-id="45b41-152">Ставка у главној књизи</span><span class="sxs-lookup"><span data-stu-id="45b41-152">Journal Line</span></span>| <span data-ttu-id="45b41-153">- Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-153">- Information</span></span><br><span data-ttu-id="45b41-154">- Брзо креирање</span><span class="sxs-lookup"><span data-stu-id="45b41-154">- Quick Create</span></span>| <span data-ttu-id="45b41-155">- Активне ставке у главној књизи</span><span class="sxs-lookup"><span data-stu-id="45b41-155">- Active Journal Lines</span></span><br><span data-ttu-id="45b41-156">- Везано за ставку у главној књизи</span><span class="sxs-lookup"><span data-stu-id="45b41-156">- Journal Line Associated</span></span> |
|  <span data-ttu-id="45b41-157">Детаљ ставке фактуре</span><span class="sxs-lookup"><span data-stu-id="45b41-157">Invoice Line Detail</span></span>| <span data-ttu-id="45b41-158">- Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-158">- Information</span></span><br><span data-ttu-id="45b41-159">- Брзо креирање</span><span class="sxs-lookup"><span data-stu-id="45b41-159">- Quick Create</span></span>| <span data-ttu-id="45b41-160">- Активни детаљ ставке фактуре</span><span class="sxs-lookup"><span data-stu-id="45b41-160">- Active Invoice Line Details</span></span><br><span data-ttu-id="45b41-161">- Наплативе трансакције фактуре</span><span class="sxs-lookup"><span data-stu-id="45b41-161">- Chargeable Invoice Transactions</span></span><br><span data-ttu-id="45b41-162">- Бесплатне трансакције фактуре</span><span class="sxs-lookup"><span data-stu-id="45b41-162">- Complimentary Invoice Transactions</span></span><br><span data-ttu-id="45b41-163">- Везано за детаље ставки фактуре</span><span class="sxs-lookup"><span data-stu-id="45b41-163">- Invoice Line Detail Associated</span></span> <br><span data-ttu-id="45b41-164">- Ненаплативе трансакције фактуре</span><span class="sxs-lookup"><span data-stu-id="45b41-164">- Non-Chargeable Invoice Transactions</span></span>|
|  <span data-ttu-id="45b41-165">Стварно</span><span class="sxs-lookup"><span data-stu-id="45b41-165">Actual</span></span>| <span data-ttu-id="45b41-166">- Информација</span><span class="sxs-lookup"><span data-stu-id="45b41-166">- Information</span></span><br><span data-ttu-id="45b41-167">- Активне стварне вредности</span><span class="sxs-lookup"><span data-stu-id="45b41-167">- Active Actuals</span></span>| <span data-ttu-id="45b41-168">Везане стварне вредности</span><span class="sxs-lookup"><span data-stu-id="45b41-168">Actual Associated</span></span> |

## <a name="set-up-a-bookable-resource-as-a-pricing-dimension"></a><span data-ttu-id="45b41-169">Подешавање ресурса који се може резервисати као димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="45b41-169">Set up a bookable resource as a pricing dimension</span></span>
<span data-ttu-id="45b41-170">Да бисте подесили ресурс који се може резервисати као димензије за одређивање цена, пратите ове кораке:</span><span class="sxs-lookup"><span data-stu-id="45b41-170">To set up a bookable resource as a pricing dimension, follow these steps:</span></span>

1. <span data-ttu-id="45b41-171">Идите на **Подешавања** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="45b41-171">Go to **Settings** > **Parameters**.</span></span> 
2. <span data-ttu-id="45b41-172">На страници **Параметар**, на картици **Димензије за одређивање цена засноване на износима**, потврдите да ли мрежа приказује записе у ентитету **Димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="45b41-172">On the **Parameter** page, on the **Amount-Based Pricing Dimensions** tab, verify that the grid shows the records in the **Pricing Dimensions** entity.</span></span> 
2. <span data-ttu-id="45b41-173">Додајте **Ресурс који се може резервисати** на ову листу димензија за одређивање цена као **msdyn_bookableresource**.</span><span class="sxs-lookup"><span data-stu-id="45b41-173">Add **Bookable Resource** to this list of pricing dimensions as **msdyn_bookableresource**.</span></span> 
3. <span data-ttu-id="45b41-174">У **Применљиво на трошкове** и **Применљиво на продају**, изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="45b41-174">In **Applicable to cost** and **Applicable to sales**, select a value.</span></span>
4. <span data-ttu-id="45b41-175">У **Врста димензије**, изаберите **Засновано на износу**.</span><span class="sxs-lookup"><span data-stu-id="45b41-175">In **Dimension Type**, select **Amount-based**.</span></span> 
5. <span data-ttu-id="45b41-176">Изаберите приоритет за трошкове и продају за ресурс који се може резервисати.</span><span class="sxs-lookup"><span data-stu-id="45b41-176">Select the cost and sales priority for the bookable resource.</span></span> <span data-ttu-id="45b41-177">Типично, ресурс који се може резервисати има највећи приоритет када је укључен као димензија формирања цена.</span><span class="sxs-lookup"><span data-stu-id="45b41-177">Typically, a bookable resource has the highest priority when included as a pricing dimension.</span></span> <span data-ttu-id="45b41-178">Подесите приоритет на **1** (или **0** у зависности од тога како рачунате приоритет) како бисте осигурали ово понашање.</span><span class="sxs-lookup"><span data-stu-id="45b41-178">Set the priority to **1** (or **0** depending on how you count the priority) to ensure this behavior.</span></span>

## <a name="set-up-pricing-dimension-field-names"></a><span data-ttu-id="45b41-179">Подешавање имена поља за димензију одређивања цена</span><span class="sxs-lookup"><span data-stu-id="45b41-179">Set up pricing dimension field names</span></span>

<span data-ttu-id="45b41-180">Када се име поља димензије за одређивање цена у табели **Цена улоге** разликује од назива поља у било ком другом ентитету где се користи подразумевано одређивање цена, запис димензије за одређивање цена мора да буде упознат са различитим називима.</span><span class="sxs-lookup"><span data-stu-id="45b41-180">When the field name of a pricing dimension in the **Role Price** table is different from the field name in any of the other entities where the default price is used, the pricing dimension record must be notified of the different names.</span></span>  

<span data-ttu-id="45b41-181">За ресурс који може да се резервише, ентитет **Чланова пројектног тима** има мало другачији назив поља од онога како се зове у ентитету **Цена улоге**:</span><span class="sxs-lookup"><span data-stu-id="45b41-181">For a bookable resource, the **Project Team Members** entity has a slightly different field name from what it is called on the **Role Price** entity:</span></span> 

 - <span data-ttu-id="45b41-182">Ентитет **Чланови пројектног тима** = **msdyn_bookableresourceid**</span><span class="sxs-lookup"><span data-stu-id="45b41-182">**Project Team Members** entity = **msdyn_bookableresourceid**</span></span>
 - <span data-ttu-id="45b41-183">Ентитет **Цена улоге** = **msdyn_bookableresource**</span><span class="sxs-lookup"><span data-stu-id="45b41-183">**Role Price** entity = **msdyn_bookableresource**</span></span>

<span data-ttu-id="45b41-184">Запис димензије за одређивање цена за **msydn_bookableresource** мора да буде обавештен о овој разлици.</span><span class="sxs-lookup"><span data-stu-id="45b41-184">The pricing dimension record for **msydn_bookableresource** must be notified of this difference.</span></span>

1. <span data-ttu-id="45b41-185">Двапут кликните на ред у мрежи **Димензије за одређивање цена** да бисте отворили страницу димензије поља **msdyn_bookableresource**.</span><span class="sxs-lookup"><span data-stu-id="45b41-185">Double-click the row in the **Pricing Dimensions** grid to open the dimension page of **msdyn_bookableresource**.</span></span>
2. <span data-ttu-id="45b41-186">На страници димензије, на картици **Повезано** изаберите **Називи поља димензија за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="45b41-186">On dimension page, on the **Related** tab, select **Pricing Dimension Field Names**.</span></span>

  ![Картица Имена поља димензија за одређивање цена](media/PD-fieldname.png)

3. <span data-ttu-id="45b41-188">У везаном приказу који се отвара изаберите **Додај нови назив поља димензије за одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="45b41-188">In the associated view that opens, select **Add New Pricing Dimension Field Name**.</span></span>

  ![Додавање нових имена поља димензије за одређивање цена](media/Add-NewPD-fieldname.png)

  <span data-ttu-id="45b41-190">Овако отварате страницу **Ново име поља димензије за одређивање цена** за **msdyn_bookableresource**.</span><span class="sxs-lookup"><span data-stu-id="45b41-190">This opens the **New Pricing dimension field name** page for **msdyn_bookableresource**.</span></span> 

4. <span data-ttu-id="45b41-191">У страници **Нови назив поља димензије за одређивање цене**, додајте **msdyn_projectteam** у **Логички назив ентитета**.</span><span class="sxs-lookup"><span data-stu-id="45b41-191">On the **New Pricing Dimension Field Name** page, add **msdyn_projectteam** to **Entity Locigal Name**.</span></span>
5. <span data-ttu-id="45b41-192">Додајте **msdyn_bookableresourceid** у **Назив поља**.</span><span class="sxs-lookup"><span data-stu-id="45b41-192">Add  **msdyn_bookableresourceid** to **Field Name**.</span></span>

 ![Образац за ново име поља димензије за одређивање цена](media/PD-fieldname-Added.png)