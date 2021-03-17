---
title: Преглед ставки понуде засноване на производу – једноставно
description: Ова тема пружа информације о раду са ставкама понуде заснованим на производу.
author: rumant
manager: Annbe
ms.date: 10/30/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 29d82637c6c8bb5b5cde7707d181d5b3d3b235c4
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272586"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="4004c-103">Преглед ставки понуде засноване на производу – једноставно</span><span class="sxs-lookup"><span data-stu-id="4004c-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="4004c-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="4004c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4004c-105">Можете креирати ставке понуде засноване на производу у апликацији Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="4004c-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="4004c-106">Ставке понуде засноване на производу можете додати ручно или то могу да буду ставке из каталога производа.</span><span class="sxs-lookup"><span data-stu-id="4004c-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="4004c-107">Каталог производа</span><span class="sxs-lookup"><span data-stu-id="4004c-107">Product catalog</span></span>

<span data-ttu-id="4004c-108">Сваки производ у каталогу производа има подразумевану јединицу и групу јединица.</span><span class="sxs-lookup"><span data-stu-id="4004c-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="4004c-109">Ако више производа дели исти скуп атрибута, можете да креирате групу производа која такође дели те атрибуте.</span><span class="sxs-lookup"><span data-stu-id="4004c-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="4004c-110">На пример, компанија продаје лиценце за претплату на разне врсте софтвера.</span><span class="sxs-lookup"><span data-stu-id="4004c-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="4004c-111">Сав софтвер за претплату има следећа два атрибута:</span><span class="sxs-lookup"><span data-stu-id="4004c-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="4004c-112">Број корисника</span><span class="sxs-lookup"><span data-stu-id="4004c-112">Number of users</span></span>
- <span data-ttu-id="4004c-113">Трајање претплате, мерено у месецима</span><span class="sxs-lookup"><span data-stu-id="4004c-113">A subscription duration measured in months</span></span>

<span data-ttu-id="4004c-114">Да бисте одржавали ову врсту каталога, креирајте породицу производа под именом **Софтвер за претплату** и додајте број корисника и трајање претплате као атрибуте.</span><span class="sxs-lookup"><span data-stu-id="4004c-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="4004c-115">Затим можете да додате појединачне производе у породицу производа **Софтвер за претплату**.</span><span class="sxs-lookup"><span data-stu-id="4004c-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="4004c-116">Додавање ставки из каталога производа у понуду за пројекат</span><span class="sxs-lookup"><span data-stu-id="4004c-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="4004c-117">Странице **Понуда за пројекат** и **Уговор за пројекат** имају одељке за ставке засноване на пројекту и ставке засноване на производу.</span><span class="sxs-lookup"><span data-stu-id="4004c-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="4004c-118">За ставке засноване на производу, падајућа листа у оквиру ставке понуде или предмета уговора за пројекат укључује све производе и јединице у ценовнику производа.</span><span class="sxs-lookup"><span data-stu-id="4004c-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="4004c-119">Такође можете да додате производе који нису део ценовника производа.</span><span class="sxs-lookup"><span data-stu-id="4004c-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="4004c-120">Поред тога, можете одабрати производе из других ценовника или директно из каталога производа.</span><span class="sxs-lookup"><span data-stu-id="4004c-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="4004c-121">Када изаберете производе директно из каталога производа, користи се подразумевани ценовник тог производа да бисте добили продајну цену производа.</span><span class="sxs-lookup"><span data-stu-id="4004c-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="4004c-122">Ако подразумевани ценовник није подешен, цена се подешава на нула (0).</span><span class="sxs-lookup"><span data-stu-id="4004c-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="4004c-123">Када се ставка понуде заснива на каталогу производа, можете изменити продајну цену директно у ставци понуде.</span><span class="sxs-lookup"><span data-stu-id="4004c-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="4004c-124">Ставка понуде у пољу **Одређивање цене** са две доступне вредности:</span><span class="sxs-lookup"><span data-stu-id="4004c-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="4004c-125">**Измена начина одређивања цена**</span><span class="sxs-lookup"><span data-stu-id="4004c-125">**Override Pricing**</span></span>
- <span data-ttu-id="4004c-126">**Користи подразумевано**</span><span class="sxs-lookup"><span data-stu-id="4004c-126">**Use Default**</span></span>

<span data-ttu-id="4004c-127">Ако изаберете **Измена начина одређивања цена**, подразумевана цена се не поставља.</span><span class="sxs-lookup"><span data-stu-id="4004c-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="4004c-128">Уместо тога, морате да унесете цену производа у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="4004c-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="4004c-129">Ако изаберете **Користи подразумевано**, користи се подразумевана продајна цена и поље се закључава за уређивање.</span><span class="sxs-lookup"><span data-stu-id="4004c-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="4004c-130">Подразумеване продајне цене се уносе у ставке засноване на производима у оквиру понуде.</span><span class="sxs-lookup"><span data-stu-id="4004c-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="4004c-131">Поље **Одређивање цена** се тада подешава на **Измени начин одређивања цена** тако да можете да уредите подразумевану цену у ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="4004c-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="4004c-132">Ово је понашање специфично за Project Operations при измени ставки заснованих на производима у услузи Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="4004c-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]