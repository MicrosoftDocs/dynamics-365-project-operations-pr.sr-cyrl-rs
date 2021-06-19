---
title: Подешавање трошкова и стопа продаје за производе из каталога – једноставно
description: Ова тема пружа информације о томе како да поставите стопе цена и продаје за ставке из каталога производа.
author: rumant
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4995859696c844e99593139f63dffbf86a52f2f0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004356"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="6df54-103">Подешавање трошкова и стопа продаје за производе из каталога – једноставно</span><span class="sxs-lookup"><span data-stu-id="6df54-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="6df54-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="6df54-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="6df54-105">Подешавање цена за ставке каталога производа у услузи Dynamics 365 Project Operations је исто као и у услузи Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="6df54-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="6df54-106">У услузи Project Operations, производи се не могу проценити ни користити у пројектима, тако да цене у каталогу производа не морају да се подешавају у ценовницима пројеката за понуде и уговоре.</span><span class="sxs-lookup"><span data-stu-id="6df54-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="6df54-107">Користите поље **Цена производа** понуде, уговора или налога да бисте подесили цене у каталогу производа.</span><span class="sxs-lookup"><span data-stu-id="6df54-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="6df54-108">Не подешавајте цене у каталогу производа у ценовнику пројекта.</span><span class="sxs-lookup"><span data-stu-id="6df54-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="6df54-109">Ценовници пројеката ексклузивни су за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6df54-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="6df54-110">Пословна логика специфична за апликацију копира ценовнике из понуде у уговор.</span><span class="sxs-lookup"><span data-stu-id="6df54-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="6df54-111">Резултат је ценовник пројекта специфичан за уговор.</span><span class="sxs-lookup"><span data-stu-id="6df54-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="6df54-112">Операција копирања може одложити поступак добијања понуде ако пројектни ценовник на понуди постане превелик.</span><span class="sxs-lookup"><span data-stu-id="6df54-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="6df54-113">Ценовници производа се не копирају да би се креирали прилагођени ценовници по уговорима.</span><span class="sxs-lookup"><span data-stu-id="6df54-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="6df54-114">Будући да није укључено копирање, то не утиче на перформансе процеса понуде.</span><span class="sxs-lookup"><span data-stu-id="6df54-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]