---
title: Управљање сложеним јединицама, као што су ставке понуде засноване на производу по кориснику месечно – једноставно
description: Ова тема пружа информације о управљању сложеним јединицама за ставке понуде засноване на производу.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b4a075ae5a7329f241cc31afceab0e085c771f72
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272901"
---
# <a name="managing-complex-units-such-as-per-user-per-month-for-product-based-quote-lines---lite"></a><span data-ttu-id="f86fb-103">Управљање сложеним јединицама, као што су ставке понуде засноване на производу по кориснику месечно – једноставно</span><span class="sxs-lookup"><span data-stu-id="f86fb-103">Managing complex units such as per-user, per-month for product-based quote lines - lite</span></span>

<span data-ttu-id="f86fb-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="f86fb-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f86fb-105">Dynamics 365 Project Operations користи количинске факторе да подржи продају производа заснованих на претплати.</span><span class="sxs-lookup"><span data-stu-id="f86fb-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="f86fb-106">За производе засноване на претплати, количина ставки понуде или предмета уговора о пројекту изражава се као број корисник-месеци.</span><span class="sxs-lookup"><span data-stu-id="f86fb-106">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="f86fb-107">Обично се цена софтвера за претплату чува у каталогу као цена по кориснику месечно.</span><span class="sxs-lookup"><span data-stu-id="f86fb-107">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="f86fb-108">Током процеса продаје, цена у ставци понуде је обично цена по кориснику, месечно, до које се дошло преговорима и попустима од стране ИТ агента продаје.</span><span class="sxs-lookup"><span data-stu-id="f86fb-108">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="f86fb-109">Свака погодба има различит број корисника и различит број месеци претплате.</span><span class="sxs-lookup"><span data-stu-id="f86fb-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="f86fb-110">Количина се користи за израчунавање ставке понуде је производ броја корисника и броја месеци претплате.</span><span class="sxs-lookup"><span data-stu-id="f86fb-110">The quantity used to compute the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="f86fb-111">Да би подржала ову врсту продаје, услуга Project Operations уводи концепт фактора количине.</span><span class="sxs-lookup"><span data-stu-id="f86fb-111">To support this type of sale, Project Operations introduced the concept of quantity factors.</span></span> <span data-ttu-id="f86fb-112">Количински фактори се ослањају на атрибуте производа у систему Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f86fb-112">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="f86fb-113">Када конфигуришете одређене особине производа, Project Operations вам омогућава да означите подскуп тих својстава или сва својства као факторе количине.</span><span class="sxs-lookup"><span data-stu-id="f86fb-113">When you configure specific properties for a product, Project Operations lets you flag a subset, or all of the properties, as quantity factors.</span></span>

<span data-ttu-id="f86fb-114">Project Operations потврђује да се као фактори количине означавају само нумеричка својства или својства производа која имају нумерички тип података.</span><span class="sxs-lookup"><span data-stu-id="f86fb-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="f86fb-115">Када у ред понуде додате производ са факторима количине, поље **Количина** постаје само за читање.</span><span class="sxs-lookup"><span data-stu-id="f86fb-115">When you add a product with quantity factors to a quote line, the **Quantity** field becomes read-only.</span></span> <span data-ttu-id="f86fb-116">Када унесете вредности за својства производа која су количински фактори, Project Operations израчунава количину ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f86fb-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the quote line.</span></span>

<span data-ttu-id="f86fb-117">На пример, Dynamics 365 Sales може имати следећа својства:</span><span class="sxs-lookup"><span data-stu-id="f86fb-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="f86fb-118">**Бр. корисника**: број корисника</span><span class="sxs-lookup"><span data-stu-id="f86fb-118">**No of users**: The number of users</span></span>
- <span data-ttu-id="f86fb-119">**Бр. месеци**: број месеци претплате</span><span class="sxs-lookup"><span data-stu-id="f86fb-119">**No of Months**: The number of subscription months</span></span>
- <span data-ttu-id="f86fb-120">**Product SKU**</span><span class="sxs-lookup"><span data-stu-id="f86fb-120">**Product SKU**</span></span>

<span data-ttu-id="f86fb-121">Можете означити **Број корисника** и **Број месеци** као факторе количине, уређивањем својстава у ставци производа.</span><span class="sxs-lookup"><span data-stu-id="f86fb-121">You can flag the **No of Users** and **No of Months** properties as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="f86fb-122">Да бисте креирали факторе количине из својстава производа, следите ове кораке:</span><span class="sxs-lookup"><span data-stu-id="f86fb-122">To create Quantity factors from Product properties, follow these steps:</span></span>

1. <span data-ttu-id="f86fb-123">У левом окну за навигацију услуге Project Operations идите на **Продаја** > **Производи**.</span><span class="sxs-lookup"><span data-stu-id="f86fb-123">On the Project Operations left navigation pane, go to **Sales** > **Products**.</span></span>
2. <span data-ttu-id="f86fb-124">Отворите производ за који треба да конфигуришете факторе количине.</span><span class="sxs-lookup"><span data-stu-id="f86fb-124">Open the product for which you need to configure quantity factors.</span></span> <span data-ttu-id="f86fb-125">Уверите се да производ има својства која су већ конфигурисана.</span><span class="sxs-lookup"><span data-stu-id="f86fb-125">Make sure the product has properties already configured.</span></span>
3. <span data-ttu-id="f86fb-126">На страници **Информације о пројекту** за Производ, изаберите картицу **Фактори количине**.</span><span class="sxs-lookup"><span data-stu-id="f86fb-126">On the **Project Information** page for the Product, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="f86fb-127">У подформи изаберите **Нови обрачун поља**.</span><span class="sxs-lookup"><span data-stu-id="f86fb-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="f86fb-128">Унесите назив фактора количине и изаберите вредност својства које се мапира у обрачун поља.</span><span class="sxs-lookup"><span data-stu-id="f86fb-128">Enter the name of the Quantity factor and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="f86fb-129">Сачувајте и затворите образац.</span><span class="sxs-lookup"><span data-stu-id="f86fb-129">Save and close the form.</span></span> <span data-ttu-id="f86fb-130">Поновите ове кораке за сва својства која ћете користити за израчунавање количине за ставку понуде засновану на производу.</span><span class="sxs-lookup"><span data-stu-id="f86fb-130">Repeat these steps for all properties to use for computing the quantity for the product-based quote line.</span></span>

<span data-ttu-id="f86fb-131">Када за производ креирате ставку понуде засноване на производу, количина ставке понуде ће бити закључана.</span><span class="sxs-lookup"><span data-stu-id="f86fb-131">When you create a product-based quote line for a product, the quantity of the quote line will be locked.</span></span> <span data-ttu-id="f86fb-132">Количина ће се израчунати као производ вредности својства које сте унели за ту ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="f86fb-132">The quantity will be computed as a product of the property values that you input for that quote line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]