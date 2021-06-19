---
title: Управљање сложеним јединицама за предмете уговора засноване на производима – једноставно
description: Ова тема пружа информације о подршци продаји производа заснованих на претплати.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 86da5a96919438e883b56fc8ecfe765f70a789ff
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003199"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a><span data-ttu-id="2e824-103">Управљање сложеним јединицама за предмете уговора засноване на производима – једноставно</span><span class="sxs-lookup"><span data-stu-id="2e824-103">Manage complex units for product-based contract lines - lite</span></span>

<span data-ttu-id="2e824-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="2e824-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2e824-105">Dynamics 365 Project Operations користи количинске факторе да подржи продају производа заснованих на претплати.</span><span class="sxs-lookup"><span data-stu-id="2e824-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="2e824-106">За производе засноване на претплати, количина уговору или предмету уговора о пројекту изражена је као број корисничких месеци.</span><span class="sxs-lookup"><span data-stu-id="2e824-106">For subscription-based products, the quantity on the contract or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="2e824-107">Цена софтвера за претплату се чува у каталогу као цена по кориснику месечно.</span><span class="sxs-lookup"><span data-stu-id="2e824-107">The price of subscription software is stored in the catalog as the price per-user, per-month.</span></span> <span data-ttu-id="2e824-108">Током процеса продаје, цена у предмету уговора је обично цена по кориснику месечно, до које се дошло преговорима и попустима од стране агента продаје.</span><span class="sxs-lookup"><span data-stu-id="2e824-108">During the sales process, the price on the contract line is usually the per-user, per-month price that was negotiated and discounted by the sales agent.</span></span> <span data-ttu-id="2e824-109">Свака погодба има различит број корисника и различит број месеци претплате.</span><span class="sxs-lookup"><span data-stu-id="2e824-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="2e824-110">Количина која се користи за израчунавање износа предмета уговора је производ броја корисника и броја месеци претплате.</span><span class="sxs-lookup"><span data-stu-id="2e824-110">The quantity used to calculate the amount of the contract line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="2e824-111">Да би подржао ову врсту продаје, Project Operations подржава концепт *фактора количине*.</span><span class="sxs-lookup"><span data-stu-id="2e824-111">To support this type of sale, Project Operations supports the concept of *quantity factors*.</span></span> <span data-ttu-id="2e824-112">Количински фактори се ослањају на атрибуте производа.</span><span class="sxs-lookup"><span data-stu-id="2e824-112">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="2e824-113">Када конфигуришете одређене особине производа, можете да означите подскуп тих својстава или сва својства као факторе количине.</span><span class="sxs-lookup"><span data-stu-id="2e824-113">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="2e824-114">Project Operations потврђује да се као фактори количине означавају само нумеричка својства или својства производа која имају нумерички тип података.</span><span class="sxs-lookup"><span data-stu-id="2e824-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="2e824-115">Када се производ са конфигурисаним факторима количине дода предмету уговора, поље **Количина** постаје само за читање.</span><span class="sxs-lookup"><span data-stu-id="2e824-115">When a product with configured quantity factors is added to a contract line, the **Quantity** field  becomes read-only.</span></span> <span data-ttu-id="2e824-116">Када унесете вредности за својства производа која су количински фактори, Project Operations израчунава количину предмета уговора.</span><span class="sxs-lookup"><span data-stu-id="2e824-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the contract line.</span></span>

<span data-ttu-id="2e824-117">На пример, Dynamics 365 Sales може имати следећа својства:</span><span class="sxs-lookup"><span data-stu-id="2e824-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="2e824-118">**Бр. корисника**: број корисника.</span><span class="sxs-lookup"><span data-stu-id="2e824-118">**No of users**: The number of users.</span></span>
- <span data-ttu-id="2e824-119">**Бр. месеци**: број месеци претплате.</span><span class="sxs-lookup"><span data-stu-id="2e824-119">**No of Months**: The number of subscription months.</span></span>
- <span data-ttu-id="2e824-120">**SKU производа**: Јединица за чување залиха (SKU) за производ.</span><span class="sxs-lookup"><span data-stu-id="2e824-120">**Product SKU**: The stock keeping unit (SKU) for the product.</span></span>

<span data-ttu-id="2e824-121">Својства **Бр. корисника** и **Бр. месеци** се могу означити као фактори количине, уређивањем својстава у ставци производа.</span><span class="sxs-lookup"><span data-stu-id="2e824-121">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="2e824-122">Да бисте креирали факторе количине из својстава производа, обавите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="2e824-122">To create quantity factors from product properties, complete the following steps.</span></span>

1. <span data-ttu-id="2e824-123">У услузи **Project Operations** изаберите **Продаја-производи**.</span><span class="sxs-lookup"><span data-stu-id="2e824-123">On the **Project Operations**, select **Sales-Products**.</span></span>
2. <span data-ttu-id="2e824-124">Отворите производ за који треба да подесите факторе количине.</span><span class="sxs-lookup"><span data-stu-id="2e824-124">Open the product for which you need to set up quantity factors.</span></span> <span data-ttu-id="2e824-125">Уверите се да производ има својства која су већ подешена.</span><span class="sxs-lookup"><span data-stu-id="2e824-125">Make sure that the product has properties already set up.</span></span>
3. <span data-ttu-id="2e824-126">На страници **Информације о пројекту** изаберите картицу **Фактори количине**.</span><span class="sxs-lookup"><span data-stu-id="2e824-126">On the **Project Information** page, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="2e824-127">У подформи изаберите **Нови обрачун поља**.</span><span class="sxs-lookup"><span data-stu-id="2e824-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="2e824-128">Унесите назив **фактора количине** и изаберите вредност својства које се мапира у обрачун поља.</span><span class="sxs-lookup"><span data-stu-id="2e824-128">Enter the name of the **Quantity Factor** and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="2e824-129">Сачувајте и затворите образац.</span><span class="sxs-lookup"><span data-stu-id="2e824-129">Save and close the form.</span></span>
7. <span data-ttu-id="2e824-130">Поновите кораке 2–6 за сва својства која ће заједно чинити количину за предмет уговора заснован на производу.</span><span class="sxs-lookup"><span data-stu-id="2e824-130">Repeat steps 2-6 for all the properties that together will make up the quantity for the product-based contract line.</span></span>

<span data-ttu-id="2e824-131">Када се поставе фактори количине, када корисник креира предмет уговора за овај производ, количина предмета уговора се закључава.</span><span class="sxs-lookup"><span data-stu-id="2e824-131">With quantity factors set up, when the user creates a contract line for this product, the quantity of the contract line is locked.</span></span> <span data-ttu-id="2e824-132">Количина се затим израчунава као производ вредности својства за тај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="2e824-132">The quantity is then calculated as a product of the property values for that contract line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]