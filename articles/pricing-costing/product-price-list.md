---
title: Ценовници производа
description: Ова тема пружа информације о ценовницима у каталошким ценама који се користе за понуде за пројекат и уговоре.
author: rumant
manager: AnnBe
ms.date: 04/05/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e37f0bf9eef946ab4ebd658cef4e1269cbaf686d
ms.sourcegitcommit: ac90be6106592f883a0de39a75836fb40255d65a
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/09/2021
ms.locfileid: "5877508"
---
# <a name="product-price-lists"></a><span data-ttu-id="eec11-103">Ценовници производа</span><span class="sxs-lookup"><span data-stu-id="eec11-103">Product price lists</span></span>

<span data-ttu-id="eec11-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="eec11-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

 <span data-ttu-id="eec11-105">У услузи Project Operations, **ценовници производа** и повезани ентитети ставке ценовника подржавају функционалност одређивања цена производа према понуди заснованој на производима и предметима уговора.</span><span class="sxs-lookup"><span data-stu-id="eec11-105">In Project Operations, **Product price lists** and related price list item entities support functionality for pricing products on product-based quote and contract lines.</span></span> <span data-ttu-id="eec11-106">За производе који се користе на пројектима, користе се записи ставки ценовника за ценовнике пројеката.</span><span class="sxs-lookup"><span data-stu-id="eec11-106">For products used on projects, the price list item records for project price lists are used.</span></span> 

<span data-ttu-id="eec11-107">Производи треба да буду подешени тако да у каталогу производа имају подразумеване трошкове и ценовнике.</span><span class="sxs-lookup"><span data-stu-id="eec11-107">Products should be set up so that they have default cost and price lists in the product catalog.</span></span> <span data-ttu-id="eec11-108">Користите ценовник, стандардну цену и тренутну цену да бисте конфигурисали подразумевану цену и ценовник.</span><span class="sxs-lookup"><span data-stu-id="eec11-108">Use the list price, standard cost, and current cost to configure default cost and list prices.</span></span> <span data-ttu-id="eec11-109">Подразумеване цене на листи користе се у ставци понуде или предмету уговора о пројекту само када систем не може да пронађе ставку ценовника за тај производ у ценовнику производа за понуду или уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="eec11-109">The default list prices are used on a quote line or a project contract line only when the system can't find a price list line for that product in the product price list for the quote or project contract.</span></span>

<span data-ttu-id="eec11-110">Цена коштања ставки каталога производа може се мењати између понуда.</span><span class="sxs-lookup"><span data-stu-id="eec11-110">The cost price of product catalog lines can be changed between quotes.</span></span> <span data-ttu-id="eec11-111">Ова могућност је важна, јер ако не пратите тачно трошкове, не можете да одредите оперативни профит од пројектних ангажманима.</span><span class="sxs-lookup"><span data-stu-id="eec11-111">This capability is important, because if you don't accurately track costs, you can't determine operational profits on project engagements.</span></span> <span data-ttu-id="eec11-112">Стандардна цена производа се подразумевано користи као цена коштања.</span><span class="sxs-lookup"><span data-stu-id="eec11-112">By default, the standard cost of the product is used as the cost price.</span></span> <span data-ttu-id="eec11-113">Међутим, подразумевана цена коштања може се ажурирати у ставци понуде ако за ту понуду постоји другачија цена.</span><span class="sxs-lookup"><span data-stu-id="eec11-113">However, the default cost price can be updated on the quote line if there's a different cost price for that quote.</span></span>

## <a name="price-list-items"></a><span data-ttu-id="eec11-114">Ставке ценовника</span><span class="sxs-lookup"><span data-stu-id="eec11-114">Price list items</span></span>

<span data-ttu-id="eec11-115">Можете да додате производе из каталога производа у различите ценовнике.</span><span class="sxs-lookup"><span data-stu-id="eec11-115">You can add products from a product catalog to different price lists.</span></span> <span data-ttu-id="eec11-116">Ставке ценовника за производе увијек упућују на одређену јединицу.</span><span class="sxs-lookup"><span data-stu-id="eec11-116">Price list lines for products always reference a specific unit.</span></span> <span data-ttu-id="eec11-117">Цене производа у ставкама ценовника се могу конфигурисати као износ валуте.</span><span class="sxs-lookup"><span data-stu-id="eec11-117">Pricing for a product on price list items can be configured as a currency amount.</span></span> <span data-ttu-id="eec11-118">Алтернативно, могу се конфигурисати као функција ценовника, тренутне цене или стандардне цене.</span><span class="sxs-lookup"><span data-stu-id="eec11-118">Alternatively, it can be configured as a function of the list price, current cost, or standard cost.</span></span>

<span data-ttu-id="eec11-119">Функционалност одређивања цена подржава различите опције заокруживања када су цене производа конфигурисане као функција ценовника, стандардна цена или тренутна цена.</span><span class="sxs-lookup"><span data-stu-id="eec11-119">Pricing functionality supports various rounding options when product prices are configured as a function of the list price, standard cost, or current cost.</span></span> <span data-ttu-id="eec11-120">Поред тога што можете искористити више метода одређивања цена и могућности заокруживања, листе попуста можете повезати са ставкама ценовника.</span><span class="sxs-lookup"><span data-stu-id="eec11-120">In addition to taking advantage of multiple pricing methods and rounding options, you can associate discount lists with price list items.</span></span> 

 
## <a name="default-product-price-list"></a><span data-ttu-id="eec11-121">Подразумевани ценовник производа</span><span class="sxs-lookup"><span data-stu-id="eec11-121">Default product price list</span></span>
<span data-ttu-id="eec11-122">Сваки запис клијента има поље **Подразумевани ценовник**, где можете одредити ценовник који одговара валути клијента.</span><span class="sxs-lookup"><span data-stu-id="eec11-122">Each customer record has a **Default Price List** field, where you can specify a price list that matches the currency of the customer.</span></span> <span data-ttu-id="eec11-123">Подразумевана вредност се не уноси у ово поље аутоматски.</span><span class="sxs-lookup"><span data-stu-id="eec11-123">A default value isn't automatically entered in this field.</span></span> <span data-ttu-id="eec11-124">Када постоји прилагођени уговор о ценама са одређеним клијентом, ово поље можете користити да бисте повезали ценовник са тим клијентом.</span><span class="sxs-lookup"><span data-stu-id="eec11-124">When a custom pricing agreement with a specific customer exists, you can use this field to associate a price list with that customer.</span></span>

<span data-ttu-id="eec11-125">Ентитети Могућност за пословање, Понуда и Уговор о пројекту користе следећи редослед за уношење подразумеваних ценовника производа.</span><span class="sxs-lookup"><span data-stu-id="eec11-125">The Opportunity, Quote, and Project Contract entities use the following order to enter default product price lists.</span></span> <span data-ttu-id="eec11-126">Исти редослед се користи за ценовнике пројеката.</span><span class="sxs-lookup"><span data-stu-id="eec11-126">The same order is used for project price lists.</span></span>

1.  <span data-ttu-id="eec11-127">Понуда</span><span class="sxs-lookup"><span data-stu-id="eec11-127">Quote</span></span>
2.  <span data-ttu-id="eec11-128">Могућност за пословање</span><span class="sxs-lookup"><span data-stu-id="eec11-128">Opportunity</span></span>
3.  <span data-ttu-id="eec11-129">Клијент</span><span class="sxs-lookup"><span data-stu-id="eec11-129">Customer</span></span>
4.  <span data-ttu-id="eec11-130">Глобална подешавања</span><span class="sxs-lookup"><span data-stu-id="eec11-130">Global settings</span></span> 

<span data-ttu-id="eec11-131">Поље **Производ** у ставци понуде подразумевано наводи све активне производе у ценовнику производа за понуду.</span><span class="sxs-lookup"><span data-stu-id="eec11-131">By default, the **Product** field on the quote line lists all the active products in the product price list of the quote.</span></span> <span data-ttu-id="eec11-132">Ако производ није активиран или је радна верзија производа, он није наведен, чак и ако је у ценовнику.</span><span class="sxs-lookup"><span data-stu-id="eec11-132">If a product has been inactivated, or if it's a draft product, it isn't listed, even if it's in the price list.</span></span> 

<span data-ttu-id="eec11-133">Ставке каталога производа додају се као ставке фактуре на првој фактури која је креирана за уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="eec11-133">Product catalog lines are added as invoice lines on the first invoice that is created for a project contract.</span></span> <span data-ttu-id="eec11-134">У радној верзији фактуре те ставке фактуре могу се избрисати.</span><span class="sxs-lookup"><span data-stu-id="eec11-134">On a draft invoice, those invoice lines can be deleted.</span></span> <span data-ttu-id="eec11-135">У том случају, ставке ће се појавити на наредној фактури док се не фактуришу или док се фактура не пошаље клијенту.</span><span class="sxs-lookup"><span data-stu-id="eec11-135">In that case, the lines will appear on a subsequent invoice until they are invoiced, or until the invoice is sent to the customer.</span></span> <span data-ttu-id="eec11-136">Не можете фактурисати делимичну количину ставке фактуре за производ.</span><span class="sxs-lookup"><span data-stu-id="eec11-136">You can't invoice a partial quantity of a product invoice line.</span></span> <span data-ttu-id="eec11-137">Када се фактуришу ставке производа из пројектног уговора, креирају се стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="eec11-137">When the product lines from the project contract are invoiced, actuals are created.</span></span> <span data-ttu-id="eec11-138">Међутим, ове стварне вредности нису повезане са сродним ентитетом пројекта.</span><span class="sxs-lookup"><span data-stu-id="eec11-138">However, those actuals aren't linked to the related project entity.</span></span> <span data-ttu-id="eec11-139">Другим речима, предмети уговора засновани на производима не зависе ни од какве употребе засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="eec11-139">In other words, product-based project contract lines are independent of any project-based use.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
