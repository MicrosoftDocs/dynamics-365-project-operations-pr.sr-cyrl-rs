---
title: Јединице и групе јединица
description: Ова тема пружа информације о томе како да креирате јединице и групе јединица у систему Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: ea5399368214a293ca7c10fabf21d82407b5c76f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898774"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="17cfa-103">Јединице и групе јединица</span><span class="sxs-lookup"><span data-stu-id="17cfa-103">Units and unit groups</span></span>

<span data-ttu-id="17cfa-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="17cfa-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="17cfa-105">Јединице су количине или мере у којима продајете производе или услуге.</span><span class="sxs-lookup"><span data-stu-id="17cfa-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="17cfa-106">На пример, ако продајете прибор за баштованство, можда продајете семе у јединицама пакета, кутија и палета.</span><span class="sxs-lookup"><span data-stu-id="17cfa-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="17cfa-107">Група јединица је колекција различитих јединица.</span><span class="sxs-lookup"><span data-stu-id="17cfa-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="17cfa-108">Да бисте довршили кораке у овој теми, уверите се да вам је додељена улога Администратор система или Менаџер за Sales Professional или да имате еквивалентне дозволе.</span><span class="sxs-lookup"><span data-stu-id="17cfa-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="17cfa-109">Креирање групе јединица</span><span class="sxs-lookup"><span data-stu-id="17cfa-109">Create a unit group</span></span>

1. <span data-ttu-id="17cfa-110">На мапи локације, изаберите **Јединице**.</span><span class="sxs-lookup"><span data-stu-id="17cfa-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="17cfa-111">Изаберите **Ново** и у дијалогу **Креирање групе јединица** унесите назив јединице.</span><span class="sxs-lookup"><span data-stu-id="17cfa-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="17cfa-112">У пољу **Примарна јединица** унесите најнижу заједничку мерну јединицу у којој ће се производ продавати.</span><span class="sxs-lookup"><span data-stu-id="17cfa-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="17cfa-113">На пример, можете унети „комад“ или „унца“.</span><span class="sxs-lookup"><span data-stu-id="17cfa-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="17cfa-114">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="17cfa-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="17cfa-115">Додавање јединица у групу јединица</span><span class="sxs-lookup"><span data-stu-id="17cfa-115">Add units to a unit group</span></span>

1. <span data-ttu-id="17cfa-116">Отворите групу јединица и на картици **Повезано** изаберите **Јединице**.</span><span class="sxs-lookup"><span data-stu-id="17cfa-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="17cfa-117">Видећете да је примарна јединица већ додата.</span><span class="sxs-lookup"><span data-stu-id="17cfa-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="17cfa-118">Изаберите **Додај нову јединицу** и на страници **Брзо креирање: јединица**, у пољу **Назив**, унесите назив јединице.</span><span class="sxs-lookup"><span data-stu-id="17cfa-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="17cfa-119">У пољу **Количина** унесите количину коју желите да јединица садржи.</span><span class="sxs-lookup"><span data-stu-id="17cfa-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="17cfa-120">На пример, ако кутија садржи два комада, унесите „2“.</span><span class="sxs-lookup"><span data-stu-id="17cfa-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="17cfa-121">У пољу **Основна јединица** изаберите основну јединицу да бисте успоставили најнижу мерну јединицу за јединицу.</span><span class="sxs-lookup"><span data-stu-id="17cfa-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="17cfa-122">На пример, можете одабрати „Комад“.</span><span class="sxs-lookup"><span data-stu-id="17cfa-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="17cfa-123">Изаберите **Сачувај**:</span><span class="sxs-lookup"><span data-stu-id="17cfa-123">Select **Save**:</span></span>
