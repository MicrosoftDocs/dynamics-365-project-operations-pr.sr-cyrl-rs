---
title: Преглед предмета уговора заснованих на производу – једноставно
description: Ова тема пружа информације о предметима уговора заснованим на производу.
author: rumant
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f248865287cdd3b1fdb3bbc40ad1c48b5302c2c0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994559"
---
# <a name="product-based-contract-lines-overview---lite"></a><span data-ttu-id="10a27-103">Преглед предмета уговора заснованих на производу – једноставно</span><span class="sxs-lookup"><span data-stu-id="10a27-103">Product-based contract lines overview - lite</span></span>

<span data-ttu-id="10a27-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="10a27-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="10a27-105">Можете креирати предмете уговора засноване на производу у апликацији Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="10a27-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="10a27-106">То могу да буду ручно креиране ставке или ставке из каталога производа.</span><span class="sxs-lookup"><span data-stu-id="10a27-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="10a27-107">Каталог производа</span><span class="sxs-lookup"><span data-stu-id="10a27-107">Product catalog</span></span>

<span data-ttu-id="10a27-108">Производи у каталогу производа имају подразумевану јединицу и групу јединица.</span><span class="sxs-lookup"><span data-stu-id="10a27-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="10a27-109">Ако неколико производа дели исти скуп атрибута, можете да креирате групу производа која такође има те атрибуте.</span><span class="sxs-lookup"><span data-stu-id="10a27-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="10a27-110">Сви производи из једне групе производа насљеђују исти скуп атрибута.</span><span class="sxs-lookup"><span data-stu-id="10a27-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="10a27-111">На пример, компанија продаје лиценце за претплату на разне врсте софтвера.</span><span class="sxs-lookup"><span data-stu-id="10a27-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="10a27-112">Сав софтвер за претплату има следећа два атрибута:</span><span class="sxs-lookup"><span data-stu-id="10a27-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="10a27-113">Број корисника</span><span class="sxs-lookup"><span data-stu-id="10a27-113">Number of users</span></span>
- <span data-ttu-id="10a27-114">Трајање претплате (у месецима)</span><span class="sxs-lookup"><span data-stu-id="10a27-114">Subscription duration (in months)</span></span>

<span data-ttu-id="10a27-115">Да бисте одржали ову врсту каталога, креирајте породицу производа која носи име **Софтвер за претплату**.</span><span class="sxs-lookup"><span data-stu-id="10a27-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="10a27-116">Додајте атрибуте, **Број корисника** и **Трајање претплате** породици производа.</span><span class="sxs-lookup"><span data-stu-id="10a27-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="10a27-117">Затим додајте појединачне производе у породицу производа **Софтвер за претплату**.</span><span class="sxs-lookup"><span data-stu-id="10a27-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="10a27-118">Додавање ставки из каталога производа у уговор</span><span class="sxs-lookup"><span data-stu-id="10a27-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="10a27-119">Уговори пројеката имају одељке за две врсте ставки, ставке засноване на пројекту и ставке засноване на производу.</span><span class="sxs-lookup"><span data-stu-id="10a27-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="10a27-120">Ставке засноване на производу укључују све производе и јединице у ценовнику производа на уговору.</span><span class="sxs-lookup"><span data-stu-id="10a27-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="10a27-121">Можете да додате производе који нису део ценовника производа уговора.</span><span class="sxs-lookup"><span data-stu-id="10a27-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="10a27-122">Можете одабрати производе из других ценовника или директно из каталога производа.</span><span class="sxs-lookup"><span data-stu-id="10a27-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="10a27-123">Када изаберете производе директно из каталога производа, користи се подразумевани ценовник тог производа за продајну цену производа.</span><span class="sxs-lookup"><span data-stu-id="10a27-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="10a27-124">Ако подразумевани ценовник није подешен, цена се подешава на 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="10a27-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="10a27-125">Ако се предмет уговора темељи на каталогу производа, можете изменити продајну цену директно у предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="10a27-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="10a27-126">Предмет уговора садржи поље **Цене** са две вредности:</span><span class="sxs-lookup"><span data-stu-id="10a27-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="10a27-127">**Измена начина одређивања цена**</span><span class="sxs-lookup"><span data-stu-id="10a27-127">**Override pricing**</span></span>
- <span data-ttu-id="10a27-128">**Користи подразумевано**</span><span class="sxs-lookup"><span data-stu-id="10a27-128">**Use default**</span></span>

<span data-ttu-id="10a27-129">Ако поље **Цене** подесите на **Измена начина одређивања цена**, подразумевана цена се не подешава.</span><span class="sxs-lookup"><span data-stu-id="10a27-129">If you set the **Pricing** field to **Override pricing**, the default price isn't set.</span></span> <span data-ttu-id="10a27-130">Унесите цену за производ у предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="10a27-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="10a27-131">Ако поље поставите на **Користи подразумеване вредности**, користи се подразумевана продајна цена и поље се не може уређивати.</span><span class="sxs-lookup"><span data-stu-id="10a27-131">If you set the field to **Use default**, the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="10a27-132">Након што инсталирате Project Operations, подразумеване продајне цене се уносе у ставке засноване на производима у оквиру уговора.</span><span class="sxs-lookup"><span data-stu-id="10a27-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="10a27-133">Поље **Одређивање цена** се подешава на **Измени начин одређивања цена** тако да можете да уредите подразумевану цену у предметима уговора.</span><span class="sxs-lookup"><span data-stu-id="10a27-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="10a27-134">Ово је измена понашања ставки заснованих на производима специфична за Project Operations у услузи Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="10a27-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]