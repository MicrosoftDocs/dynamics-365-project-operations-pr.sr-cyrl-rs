---
title: Коришћење постојећег поља у услузи Project Service као димензије за одређивање цена
description: Ова тема пружа информације о коришћењу постојећих Project Service поља као димензија за одређивање цена.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 09e565c91eda9dee6e0ec479a5c85d94d2591147
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6008104"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="8ee9d-103">Коришћење постојећег поља у услузи Project Service као димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="8ee9d-103">Use an existing field in Project Service as a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="8ee9d-104">Project Service Automation (PSA) има многа поља у ентитету **Стварне вредности** која се могу користити као димензије за одређивање цена засновано на ресурсима у организацијама које обављају пројекте.</span><span class="sxs-lookup"><span data-stu-id="8ee9d-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="8ee9d-105">На пример, једно уобичајено поље је **Ресурс који се може резервисати**.</span><span class="sxs-lookup"><span data-stu-id="8ee9d-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="8ee9d-106">Мања предузећа са мање од 20-30 наплативих ресурса могу да открију да је једноставнији приступ ако имају стопе наплате и трошкова специфичне за сваки ресурс.</span><span class="sxs-lookup"><span data-stu-id="8ee9d-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="8ee9d-107">Међутим, како се наплатива радна снага повећава, одређене стопе могу постати нереалне за одржавање пошто ће трошкови ресурса и стопе наплате почети да се разликују са унапређењем ресурса, стицањем већег искуства или различитог спектра вештина.</span><span class="sxs-lookup"><span data-stu-id="8ee9d-107">However, as the billable workforce grows, specific rates could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill set.</span></span> <span data-ttu-id="8ee9d-108">Будући да овај приступ још увек функционише за предузећа одређене величине, погледајте чланак [Коришћење ресурса који се може резервисати као димензије за одређивање цена](bookable-resource-pricing-dimension.md) да бисте разумели како се постојеће Project Service поље може користити као димензија за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="8ee9d-108">Because this approach still works for companies of a certain size, see [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="8ee9d-109">Други пример је категорија трансакције.</span><span class="sxs-lookup"><span data-stu-id="8ee9d-109">Another example is that of transaction category.</span></span> <span data-ttu-id="8ee9d-110">Клијенти и примењивачи су користили категорију трансакције у апликацији PSA да класификују посао и помоћу поља одређују цену и трошкове на основу категорије посла.</span><span class="sxs-lookup"><span data-stu-id="8ee9d-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="8ee9d-111">Више информација потражите у чланку [Коришћење категорије трансакције као димензије одређивања цена](transaction-category-pricing-dimension.md).</span><span class="sxs-lookup"><span data-stu-id="8ee9d-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]