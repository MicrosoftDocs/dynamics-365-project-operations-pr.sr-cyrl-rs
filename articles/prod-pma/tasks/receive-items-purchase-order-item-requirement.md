---
title: Пријем ставки по наруџбеници из захтева за ставку
description: Овај тема објашњава како да примите ставке на наруџбеници из захтева за ставку.
author: Yowelle
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 0e0c4a75f1d86538cc773af1f7c0ae3c83ef0ad5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6011704"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="ea4e7-103">Пријем ставки по наруџбеници из захтева за ставку</span><span class="sxs-lookup"><span data-stu-id="ea4e7-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="ea4e7-104">Овај тема објашњава како да примите ставке на наруџбеници из захтева за ставку.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="ea4e7-105">Коришћењем захтева за ставку уместо трансакције са ставком, можете да планирате испоруку непосредно пре него што се ставка стварно користи, креирате наруџбеницу, ставку укључите у оквир трговинског споразума и укључите захтев за ставку у планирање производње.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="ea4e7-106">Овај задатке користи USSI скуп података.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="ea4e7-107">У окну за навигацију, идите на **Модули > Управљање пројектима и рачуноводство > Пројекти > Сви пројекти**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="ea4e7-108">На листи, изаберите везу у жељеном реду.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="ea4e7-109">У окну радњи, изаберите **План**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="ea4e7-110">Изаберите **Захтеви за ставку**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="ea4e7-111">Изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-111">Select **New**.</span></span>
6. <span data-ttu-id="ea4e7-112">У новом реду унесите или изаберите вредност у пољу **Број ставке**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="ea4e7-113">У поље **Количина** унесите број.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="ea4e7-114">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-114">Select **Save**.</span></span>
9. <span data-ttu-id="ea4e7-115">У окну радњи изаберите **Управљај**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="ea4e7-116">Изаберите **Функције**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-116">Select **Functions**.</span></span>
11. <span data-ttu-id="ea4e7-117">Изаберите **Креирање поруџбенице**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="ea4e7-118">Изаберите поље за потврду **Укључи све**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="ea4e7-119">У пољу **Пословни контакт продавца** унесите или изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="ea4e7-120">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-120">Select **OK**.</span></span>
15. <span data-ttu-id="ea4e7-121">У окну за навигацију идите на **Модули > Дуговања > Поруџбенице > Све поруџбенице**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="ea4e7-122">На листи, изаберите везу у жељеном реду.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="ea4e7-123">У окну радњи изаберите **Купи**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="ea4e7-124">Изаберите **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="ea4e7-125">У окну радњи изаберите **Пријем**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="ea4e7-126">Изаберите **Пријем производа**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="ea4e7-127">У пољу **Пријем производа**, откуцајте вредност.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="ea4e7-128">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-128">Select **OK**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]