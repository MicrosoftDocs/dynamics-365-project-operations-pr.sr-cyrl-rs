---
title: Подешавање трошкова и стопа продаје за производе из каталога – једноставно
description: Ова тема пружа информације о томе како да поставите стопе цена и продаје за ставке из каталога производа.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5e851193df8151821e112e01a9f33df5afee7df7
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764579"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="acfad-103">Подешавање трошкова и стопа продаје за производе из каталога – једноставно</span><span class="sxs-lookup"><span data-stu-id="acfad-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="acfad-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="acfad-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="acfad-105">Подешавање цена за ставке каталога производа у услузи Dynamics 365 Project Operations је исто као и у услузи Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="acfad-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="acfad-106">У услузи Project Operations, производи се не могу проценити ни користити у пројектима, тако да цене у каталогу производа не морају да се подешавају у ценовницима пројеката за понуде и уговоре.</span><span class="sxs-lookup"><span data-stu-id="acfad-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="acfad-107">Користите поље **Цена производа** понуде, уговора или налога да бисте подесили цене у каталогу производа.</span><span class="sxs-lookup"><span data-stu-id="acfad-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="acfad-108">Не подешавајте цене у каталогу производа у ценовнику пројекта.</span><span class="sxs-lookup"><span data-stu-id="acfad-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="acfad-109">Ценовници пројеката ексклузивни су за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="acfad-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="acfad-110">Пословна логика специфична за апликацију копира ценовнике из понуде у уговор.</span><span class="sxs-lookup"><span data-stu-id="acfad-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="acfad-111">Резултат је ценовник пројекта специфичан за уговор.</span><span class="sxs-lookup"><span data-stu-id="acfad-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="acfad-112">Операција копирања може одложити поступак добијања понуде ако пројектни ценовник на понуди постане превелик.</span><span class="sxs-lookup"><span data-stu-id="acfad-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="acfad-113">Ценовници производа се не копирају да би се креирали прилагођени ценовници по уговорима.</span><span class="sxs-lookup"><span data-stu-id="acfad-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="acfad-114">Будући да није укључено копирање, то не утиче на перформансе процеса понуде.</span><span class="sxs-lookup"><span data-stu-id="acfad-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>
