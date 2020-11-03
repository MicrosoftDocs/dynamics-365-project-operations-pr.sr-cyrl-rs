---
title: Процене ресурса
description: Ова тема пружа информације о томе како се израчунавају процене ресурса у услузи Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083892"
---
# <a name="resource-estimates"></a><span data-ttu-id="cdaa3-103">Процене ресурса</span><span class="sxs-lookup"><span data-stu-id="cdaa3-103">Resource estimates</span></span>

<span data-ttu-id="cdaa3-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="cdaa3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cdaa3-105">Процене ресурса потичу из ангажовања у времену које је дефинисано у структурној анализи посла заједно са применљивим димензијама за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="cdaa3-106">Типично, прорачун је **сатница за сваку улогу x број сати.**</span><span class="sxs-lookup"><span data-stu-id="cdaa3-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="cdaa3-107">Ангажовање у времену за сваки ресурс ускладиштено је у запису о додели ресурса.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="cdaa3-108">Одређивање цена се складишти у унапред дефинисаном ценовнику.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="cdaa3-109">Конверзија јединица примењује се на основу важећег ценовника.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-109">Unit conversion is applied based on the applicable price list.</span></span>

![Процене ресурса](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="cdaa3-111">Подразумевана цена коштања и валута трошкова</span><span class="sxs-lookup"><span data-stu-id="cdaa3-111">Default cost price and cost currency</span></span>

<span data-ttu-id="cdaa3-112">Цене трошкова подразумевано долазе из организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="cdaa3-113">Подразумевана стопа наплате и продајна валута</span><span class="sxs-lookup"><span data-stu-id="cdaa3-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="cdaa3-114">Продајне цене се примењују једном по погодби.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="cdaa3-115">Хијерархија продајног ценовника подразумевано је следећа:</span><span class="sxs-lookup"><span data-stu-id="cdaa3-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="cdaa3-116">Организација</span><span class="sxs-lookup"><span data-stu-id="cdaa3-116">Organization</span></span>
2. <span data-ttu-id="cdaa3-117">Клијент</span><span class="sxs-lookup"><span data-stu-id="cdaa3-117">Customer</span></span>
3. <span data-ttu-id="cdaa3-118">Понуда/уговор</span><span class="sxs-lookup"><span data-stu-id="cdaa3-118">Quote/contract</span></span>
