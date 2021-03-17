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
ms.openlocfilehash: 5f3f5d196e0d7db4a6d8c4cfe834a335f4ef737c
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289207"
---
# <a name="purchase-orders-for-a-project"></a><span data-ttu-id="1eb25-104">Поруџбенице за пројекат</span><span class="sxs-lookup"><span data-stu-id="1eb25-104">Purchase orders for a project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1eb25-105">Овај чланак описује разне методе помоћу којих можете да креирате поруџбенице за пројекат.</span><span class="sxs-lookup"><span data-stu-id="1eb25-105">This article describes the various methods that you can use to create purchase orders for a project.</span></span> <span data-ttu-id="1eb25-106">Начин који користите зависи од сврхе поруџбенице и од тога када се купљене ставке користе и наплаћују пројекту.</span><span class="sxs-lookup"><span data-stu-id="1eb25-106">The method that you use depends on the purpose of the purchase order, and when the purchased items are consumed and charged to a project.</span></span>

### <a name="methods-for-creating-a-purchase-order"></a><span data-ttu-id="1eb25-107">Методе за креирање поруџбенице</span><span class="sxs-lookup"><span data-stu-id="1eb25-107">Methods for creating a purchase order</span></span>

<span data-ttu-id="1eb25-108">Можете да користите један од следећих метода за креирање поруџбенице у управљању пројектима и рачуноводству.</span><span class="sxs-lookup"><span data-stu-id="1eb25-108">You can use one of the following methods to create a purchase order in Project management and accounting.</span></span> <span data-ttu-id="1eb25-109">Сврха поруџбенице одређује када се поруџбеница користи и, стога, када се ставке наплаћују пројекту.</span><span class="sxs-lookup"><span data-stu-id="1eb25-109">The purpose of the purchase order determines when the purchase order is consumed and, therefore, when items are charged to a project.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1eb25-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1eb25-110">Method</span></span></th>
<th><span data-ttu-id="1eb25-111">Сврха</span><span class="sxs-lookup"><span data-stu-id="1eb25-111">Purpose</span></span></th>
<th><span data-ttu-id="1eb25-112">Потрошња ставки</span><span class="sxs-lookup"><span data-stu-id="1eb25-112">Consumption of items</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1eb25-113">Креирајте поруџбеницу директно из пројекта.</span><span class="sxs-lookup"><span data-stu-id="1eb25-113">Create a purchase order directly from a project.</span></span></td>
<td><span data-ttu-id="1eb25-114">Ову методу користите за куповину ставки од спољног продавца за потрошњу на пројекту.</span><span class="sxs-lookup"><span data-stu-id="1eb25-114">Use this method to purchase items from an external vendor for consumption on a project.</span></span> <span data-ttu-id="1eb25-115">Поруџбеницу можете креирати на два начина:</span><span class="sxs-lookup"><span data-stu-id="1eb25-115">You can create the purchase order in two ways:</span></span>
<ul>
<li><span data-ttu-id="1eb25-116">Из самог пројекта.</span><span class="sxs-lookup"><span data-stu-id="1eb25-116">From the project itself.</span></span> <span data-ttu-id="1eb25-117">У овом случају, пројекат је већ дефинисан за поруџбеницу.</span><span class="sxs-lookup"><span data-stu-id="1eb25-117">In this case, the project is already defined for the purchase order.</span></span></li>
<li><span data-ttu-id="1eb25-118">Навигацијом до поруџбенице за пројекат.</span><span class="sxs-lookup"><span data-stu-id="1eb25-118">By navigating to the project purchase order.</span></span> <span data-ttu-id="1eb25-119">Морате изабрати продавца и пројекат за који ћете креирати поруџбеницу.</span><span class="sxs-lookup"><span data-stu-id="1eb25-119">You must select both the vendor and the project to create the purchase order for.</span></span></li>
</ul></td>
<td><span data-ttu-id="1eb25-120">Ставке се користе када се фактура добављача ажурира.</span><span class="sxs-lookup"><span data-stu-id="1eb25-120">Items are consumed when the vendor invoice is updated.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1eb25-121">Креирајте поруџбеницу директно из улазне поруџбине.</span><span class="sxs-lookup"><span data-stu-id="1eb25-121">Create a purchase order from a sales order.</span></span></td>
<td><span data-ttu-id="1eb25-122">Користите овај метод за куповину ставки када креирате улазну поруџбину из пројекта.</span><span class="sxs-lookup"><span data-stu-id="1eb25-122">Use this method to purchase items when you create a sales order from a project.</span></span></td>
<td><span data-ttu-id="1eb25-123">Ставке се користе када се поруџбеница фактурише клијенту.</span><span class="sxs-lookup"><span data-stu-id="1eb25-123">Items are consumed when the sales order is invoiced to the customer.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1eb25-124">Креирајте поруџбеницу на основу захтева за ставку.</span><span class="sxs-lookup"><span data-stu-id="1eb25-124">Create a purchase order from an item requirement.</span></span></td>
<td><span data-ttu-id="1eb25-125">Користите овај метод за куповину ставки када креирате захтев за ставку из пројекта.</span><span class="sxs-lookup"><span data-stu-id="1eb25-125">Use this method to purchase items when you create an item requirement from a project.</span></span></td>
<td><span data-ttu-id="1eb25-126">Ставке се користе када се ажурира отпремница захтева.</span><span class="sxs-lookup"><span data-stu-id="1eb25-126">Items are consumed when the item requirement packing slip is updated.</span></span></td>
</tr>
</tbody>
</table>

> [!NOTE] 
> <span data-ttu-id="1eb25-127">Када ажурирате фактуру добављача или отпремницу, од вас ће се затражити да ажурирате отпремницу према захтеву за ставку.</span><span class="sxs-lookup"><span data-stu-id="1eb25-127">When you update the vendor invoice or packing slip, you're prompted to update the packing slip on the item requirement.</span></span>

<span data-ttu-id="1eb25-128">За више информација погледајте [Пријем ставки по поруџбеници из захтева за ставку](tasks/receive-items-purchase-order-item-requirement.md).</span><span class="sxs-lookup"><span data-stu-id="1eb25-128">For more information, see [Receive items on purchase order from item requirement](tasks/receive-items-purchase-order-item-requirement.md).</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]