---
title: Подесите трошкове и стопе продаје за производе из каталога
description: Ова тема пружа информације о томе како да поставите стопе цена и продаје за ставке из каталога производа.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5178a9143536bf4b2573403125325017861cdd5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084039"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products"></a><span data-ttu-id="a8f6c-103">Подесите трошкове и стопе продаје за производе из каталога</span><span class="sxs-lookup"><span data-stu-id="a8f6c-103">Set up cost and sales rates for catalog products</span></span>

<span data-ttu-id="a8f6c-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="a8f6c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="a8f6c-105">Постављање цена за ставке каталога производа у програму Dynamics 365 Project Operations је исто као у програму Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="a8f6c-106">Будући да се производи не могу проценити или користити на пројектима у услузи Project Operations, нема потребе за постављањем цена каталога производа на ценовнике пројеката за понуде и уговоре.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="a8f6c-107">Цене каталога производа треба поставити у пољу **Цена производа** понуде, уговора или налога.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="a8f6c-108">Не постављајте цене каталога производа у ценовнике пројеката за ове ентитете.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="a8f6c-109">Ценовници пројеката ексклузивни су за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="a8f6c-110">Постоји специфична пословна логика која копира ценовнике из понуде у уговор.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="a8f6c-111">Резултат је ценовник пројекта специфичан за уговор.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="a8f6c-112">Операција копирања може одложити поступак добијања понуде ако пројектни ценовник на понуди постане превелик.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="a8f6c-113">Ценовници производа се не копирају да би се креирали прилагођени ценовници по уговорима.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="a8f6c-114">То значи да ценовници производа не утичу на перформансе процеса освајања понуда.</span><span class="sxs-lookup"><span data-stu-id="a8f6c-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
