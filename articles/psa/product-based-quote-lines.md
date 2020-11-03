---
title: Ставке понуда засноване на производу
description: Ова тема пружа информације о ставкама понуда заснованим на производу.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
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
ms.openlocfilehash: 55a5b5041a494892e6d96bf24e1bc132a26521dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084152"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="2d40b-103">Ставке понуда засноване на производу</span><span class="sxs-lookup"><span data-stu-id="2d40b-103">Product-based quote lines</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="2d40b-104">Можете креирати ставке понуде засноване на производу у апликацији Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="2d40b-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="2d40b-105">То могу да буду ставке за унос или ставке из каталога производа.</span><span class="sxs-lookup"><span data-stu-id="2d40b-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="2d40b-106">Каталог производа</span><span class="sxs-lookup"><span data-stu-id="2d40b-106">Product catalog</span></span>

<span data-ttu-id="2d40b-107">Производи у Dynamics 365 каталогу производа имају подразумевану јединицу и групу јединица.</span><span class="sxs-lookup"><span data-stu-id="2d40b-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="2d40b-108">Ако неколико производа дели исти скуп атрибута, можете да креирате групу производа која такође има те атрибуте.</span><span class="sxs-lookup"><span data-stu-id="2d40b-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="2d40b-109">Сви производи из једне групе производа насљеђују исти скуп атрибута.</span><span class="sxs-lookup"><span data-stu-id="2d40b-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="2d40b-110">На пример, компанија продаје лиценце за претплату на разни софтвер.</span><span class="sxs-lookup"><span data-stu-id="2d40b-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="2d40b-111">Сав софтвер за претплату има следећа два атрибута:</span><span class="sxs-lookup"><span data-stu-id="2d40b-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="2d40b-112">Број корисника</span><span class="sxs-lookup"><span data-stu-id="2d40b-112">Number of users</span></span> 
- <span data-ttu-id="2d40b-113">Трајање претплате (у месецима)</span><span class="sxs-lookup"><span data-stu-id="2d40b-113">Subscription duration (in months)</span></span>

<span data-ttu-id="2d40b-114">Добар начин за одржавање ове врсте каталога је креирање групе производа под именом **Софтвер за претплату** и са атрибутима **Број корисника** и **Трајање претплате**.</span><span class="sxs-lookup"><span data-stu-id="2d40b-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software** , and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="2d40b-115">Затим можете додати појединачне производе, као што су **Dynamics 365 Sales** или **Dynamics 365 Field Service** у групу производа **Софтвер за претплату**.</span><span class="sxs-lookup"><span data-stu-id="2d40b-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="2d40b-116">Додавање ставки из каталога производа у понуду за пројекат</span><span class="sxs-lookup"><span data-stu-id="2d40b-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="2d40b-117">Страница са понудом за пројекат и страница уговора имају одељке за две врсте ставки: ставке засноване на пројекту и ставке засноване на производу.</span><span class="sxs-lookup"><span data-stu-id="2d40b-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="2d40b-118">За ставке засноване на производу, Dynamics 365 се користи за додавање ставки из каталога производа у понуду.</span><span class="sxs-lookup"><span data-stu-id="2d40b-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="2d40b-119">Падајућа листа у оквиру ставке понуде или предмета уговора за пројекат укључује све производе и јединице у ценовнику производа који је приложен уз понуду или уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2d40b-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="2d40b-120">Такође можете да додате производе који нису део ценовника производа понуде.</span><span class="sxs-lookup"><span data-stu-id="2d40b-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="2d40b-121">Поред тога, можете одабрати производе из других ценовника или можете одабрати производе директно из каталога производа.</span><span class="sxs-lookup"><span data-stu-id="2d40b-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="2d40b-122">Када изаберете производе директно из каталога производа, користи се подразумевани ценовник тог производа да бисте добили продајну цену производа.</span><span class="sxs-lookup"><span data-stu-id="2d40b-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="2d40b-123">Ако подразумевани ценовник није подешен, цена се подешава на 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="2d40b-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="2d40b-124">Ако се ставка понуде темељи на каталогу производа, можете изменити продајну цену директно у ставци понуде.</span><span class="sxs-lookup"><span data-stu-id="2d40b-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="2d40b-125">Имајте на уму да ставка понуде у систему Dynamics 365 има поље **Одређивање цена**.</span><span class="sxs-lookup"><span data-stu-id="2d40b-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="2d40b-126">Доступне су две вредности:</span><span class="sxs-lookup"><span data-stu-id="2d40b-126">Two values are available:</span></span>

- <span data-ttu-id="2d40b-127">Измена начина одређивања цена</span><span class="sxs-lookup"><span data-stu-id="2d40b-127">Override pricing</span></span>  
- <span data-ttu-id="2d40b-128">Користи подразумеване цене</span><span class="sxs-lookup"><span data-stu-id="2d40b-128">Use default</span></span>

<span data-ttu-id="2d40b-129">Ако ово поље подесите на **Измена начина одређивања цена** , Dynamics 365 не подешава подразумевану цену.</span><span class="sxs-lookup"><span data-stu-id="2d40b-129">If you set this field to **Override pricing** , Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="2d40b-130">Морате да унесете цену производа у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="2d40b-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="2d40b-131">Ако ово поље подесите на **Користи подразумеване цене** , Dynamics 365 користи подразумеване продајне цене и закључава поље ради спречавања уређивања.</span><span class="sxs-lookup"><span data-stu-id="2d40b-131">If you set this field to **Use default** , Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="2d40b-132">Након што инсталирате PSA, подразумеване продајне цене се уносе у ставке засноване на производима у оквиру понуде.</span><span class="sxs-lookup"><span data-stu-id="2d40b-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="2d40b-133">Поље **Одређивање цена** се тада подешава на **Измени начин одређивања цена** тако да можете да уредите подразумевану цену у ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="2d40b-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![Подешавање измене начина одређивања цена](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="2d40b-135">Количински фактори производа</span><span class="sxs-lookup"><span data-stu-id="2d40b-135">Quantity factors for products</span></span>

<span data-ttu-id="2d40b-136">PSA користи количинске факторе да подржи продају производа заснованих на претплати.</span><span class="sxs-lookup"><span data-stu-id="2d40b-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="2d40b-137">За производе засноване на претплати, количина ставци понуде или предмету уговора о пројекту изражена је као број корисничких месеци.</span><span class="sxs-lookup"><span data-stu-id="2d40b-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="2d40b-138">Обично се цена софтвера за претплату чува у каталогу као цена по кориснику месечно.</span><span class="sxs-lookup"><span data-stu-id="2d40b-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="2d40b-139">Међутим, уместо тога можете користити описе других периода.</span><span class="sxs-lookup"><span data-stu-id="2d40b-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="2d40b-140">Током процеса продаје, цена у ставци понуде је обично цена по кориснику, месечно, до које се дошло преговорима и попустима од стране ИТ агента продаје.</span><span class="sxs-lookup"><span data-stu-id="2d40b-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="2d40b-141">Свака погодба има различит број корисника и различит број месеци претплате.</span><span class="sxs-lookup"><span data-stu-id="2d40b-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="2d40b-142">Количина која се користи за израчунавање количине ставке понуде је производ броја корисника и броја месеци претплате.</span><span class="sxs-lookup"><span data-stu-id="2d40b-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="2d40b-143">Да би подржао ову врсту продаје, PSA је увео концепт фактора количине.</span><span class="sxs-lookup"><span data-stu-id="2d40b-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="2d40b-144">Количински фактори се ослањају на атрибуте производа у систему Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="2d40b-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="2d40b-145">Када конфигуришете одређене особине производа, PSA вам омогућава да означите подскуп тих својстава или сва својства као факторе количине.</span><span class="sxs-lookup"><span data-stu-id="2d40b-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="2d40b-146">PSA потврђује да се као фактори количине означавају само нумеричка својства или својства производа која имају нумерички тип података.</span><span class="sxs-lookup"><span data-stu-id="2d40b-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="2d40b-147">Када се производ за који су конфигурисани фактори количине дода у ставку понуде, поље **Количина** у ставци понуде постаје поље само за читање.</span><span class="sxs-lookup"><span data-stu-id="2d40b-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="2d40b-148">Након што унесете вредности за својства производа која су количински фактори, PSA израчунава количину ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="2d40b-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="2d40b-149">На пример, Dynamics 365 може имати следећа својства:</span><span class="sxs-lookup"><span data-stu-id="2d40b-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="2d40b-150">**Бр. корисника** - Број корисника</span><span class="sxs-lookup"><span data-stu-id="2d40b-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="2d40b-151">**Бр. месеца** - Број месеци претплате</span><span class="sxs-lookup"><span data-stu-id="2d40b-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="2d40b-152">**Product SKU**</span><span class="sxs-lookup"><span data-stu-id="2d40b-152">**Product SKU**</span></span> 

<span data-ttu-id="2d40b-153">Својства **Бр. корисника** и **Бр. месеци** се могу означити као фактори количине, уређивањем својстава у ставци производа.</span><span class="sxs-lookup"><span data-stu-id="2d40b-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![Означавање броја корисника и броја месеци као фактора квалитета](media/basic-guide-11.png)
 
