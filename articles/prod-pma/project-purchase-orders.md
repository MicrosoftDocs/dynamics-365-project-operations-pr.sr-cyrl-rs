---
title: Поруџбенице за пројекат
description: Овај чланак описује разне методе помоћу којих можете да креирате поруџбенице за пројекат. Начин који користите зависи од сврхе поруџбенице и од тога када се купљене ставке користе и наплаћују пројекту.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083960"
---
# <a name="purchase-orders-for-a-project"></a><span data-ttu-id="4dcaf-104">Поруџбенице за пројекат</span><span class="sxs-lookup"><span data-stu-id="4dcaf-104">Purchase orders for a project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="4dcaf-105">Овај чланак описује разне методе помоћу којих можете да креирате поруџбенице за пројекат.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-105">This article describes the various methods that you can use to create purchase orders for a project.</span></span> <span data-ttu-id="4dcaf-106">Начин који користите зависи од сврхе поруџбенице и од тога када се купљене ставке користе и наплаћују пројекту.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-106">The method that you use depends on the purpose of the purchase order, and when the purchased items are consumed and charged to a project.</span></span>

### <a name="methods-for-creating-a-purchase-order"></a><span data-ttu-id="4dcaf-107">Методе за креирање поруџбенице</span><span class="sxs-lookup"><span data-stu-id="4dcaf-107">Methods for creating a purchase order</span></span>

<span data-ttu-id="4dcaf-108">Можете да користите један од следећих метода за креирање поруџбенице у управљању пројектима и рачуноводству.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-108">You can use one of the following methods to create a purchase order in Project management and accounting.</span></span> <span data-ttu-id="4dcaf-109">Сврха поруџбенице одређује када се поруџбеница користи и, стога, када се ставке наплаћују пројекту.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-109">The purpose of the purchase order determines when the purchase order is consumed and, therefore, when items are charged to a project.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="4dcaf-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4dcaf-110">Method</span></span></th>
<th><span data-ttu-id="4dcaf-111">Сврха</span><span class="sxs-lookup"><span data-stu-id="4dcaf-111">Purpose</span></span></th>
<th><span data-ttu-id="4dcaf-112">Потрошња ставки</span><span class="sxs-lookup"><span data-stu-id="4dcaf-112">Consumption of items</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="4dcaf-113">Креирајте поруџбеницу директно из пројекта.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-113">Create a purchase order directly from a project.</span></span></td>
<td><span data-ttu-id="4dcaf-114">Ову методу користите за куповину ставки од спољног продавца за потрошњу на пројекту.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-114">Use this method to purchase items from an external vendor for consumption on a project.</span></span> <span data-ttu-id="4dcaf-115">Поруџбеницу можете креирати на два начина:</span><span class="sxs-lookup"><span data-stu-id="4dcaf-115">You can create the purchase order in two ways:</span></span>
<ul>
<li><span data-ttu-id="4dcaf-116">Из самог пројекта.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-116">From the project itself.</span></span> <span data-ttu-id="4dcaf-117">У овом случају, пројекат је већ дефинисан за поруџбеницу.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-117">In this case, the project is already defined for the purchase order.</span></span></li>
<li><span data-ttu-id="4dcaf-118">Навигацијом до поруџбенице за пројекат.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-118">By navigating to the project purchase order.</span></span> <span data-ttu-id="4dcaf-119">Морате изабрати продавца и пројекат за који ћете креирати поруџбеницу.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-119">You must select both the vendor and the project to create the purchase order for.</span></span></li>
</ul></td>
<td><span data-ttu-id="4dcaf-120">Ставке се користе када се фактура добављача ажурира.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-120">Items are consumed when the vendor invoice is updated.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="4dcaf-121">Креирајте поруџбеницу директно из улазне поруџбине.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-121">Create a purchase order from a sales order.</span></span></td>
<td><span data-ttu-id="4dcaf-122">Користите овај метод за куповину ставки када креирате улазну поруџбину из пројекта.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-122">Use this method to purchase items when you create a sales order from a project.</span></span></td>
<td><span data-ttu-id="4dcaf-123">Ставке се користе када се поруџбеница фактурише клијенту.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-123">Items are consumed when the sales order is invoiced to the customer.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="4dcaf-124">Креирајте поруџбеницу на основу захтева за ставку.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-124">Create a purchase order from an item requirement.</span></span></td>
<td><span data-ttu-id="4dcaf-125">Користите овај метод за куповину ставки када креирате захтев за ставку из пројекта.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-125">Use this method to purchase items when you create an item requirement from a project.</span></span></td>
<td><span data-ttu-id="4dcaf-126">Ставке се користе када се ажурира отпремница захтева.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-126">Items are consumed when the item requirement packing slip is updated.</span></span></td>
</tr>
</tbody>
</table>

> [!NOTE] 
> <span data-ttu-id="4dcaf-127">Када ажурирате фактуру добављача или отпремницу, од вас ће се затражити да ажурирате отпремницу према захтеву за ставку.</span><span class="sxs-lookup"><span data-stu-id="4dcaf-127">When you update the vendor invoice or packing slip, you're prompted to update the packing slip on the item requirement.</span></span>

<span data-ttu-id="4dcaf-128">За више информација погледајте [Пријем ставки по поруџбеници из захтева за ставку](tasks/receive-items-purchase-order-item-requirement.md).</span><span class="sxs-lookup"><span data-stu-id="4dcaf-128">For more information, see [Receive items on purchase order from item requirement](tasks/receive-items-purchase-order-item-requirement.md).</span></span>

