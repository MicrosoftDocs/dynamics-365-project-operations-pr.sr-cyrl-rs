---
title: Предмети могућности за пословање засновани на производу
description: Ова тема пружа информације о ставкама предмета могућности за пословање заснованим на производу у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896254"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="d1d60-103">Предмети могућности за пословање засновани на производу</span><span class="sxs-lookup"><span data-stu-id="d1d60-103">Product-based opportunity lines</span></span>

<span data-ttu-id="d1d60-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="d1d60-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d1d60-105">Предмети могућности за пословање засновани на производу су ставке у могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="d1d60-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="d1d60-106">Ове ставке се испоручују клијенту као посебне ставке на евентуалној фактури без икаквих других услуга са додатом вредношћу.</span><span class="sxs-lookup"><span data-stu-id="d1d60-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="d1d60-107">Повезана потрошња и коришћење се не прате на задацима било којих повезаних пројеката.</span><span class="sxs-lookup"><span data-stu-id="d1d60-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="d1d60-108">Ставке засноване на производима могу бити артикли из каталога или ручно додати производи.</span><span class="sxs-lookup"><span data-stu-id="d1d60-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="d1d60-109">Већина функционалности предмета могућности за пословање заснованих на производу прати функционалност коју пружа апликација Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="d1d60-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="d1d60-110">За више информација о предметима могућности за пословање заснованим на производу, погледајте [Додавање производа у могућност за пословање](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="d1d60-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="d1d60-111">Један концепт о предметима могућности за пословање заснованим на производу који је специфичан за могућности за пословање засноване на пројектима јесте **Буџет клијента**.</span><span class="sxs-lookup"><span data-stu-id="d1d60-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="d1d60-112">Користите ово поље за праћење износа који је клијент спреман да плати за ставку поруџбине.</span><span class="sxs-lookup"><span data-stu-id="d1d60-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="d1d60-113">Ако је метода прихода резимеа могућности за пословање постављена на **Системски израчунато**, вредности буџета клијената у ставкама заснованим на производу и пројекту се сабирају како би се израчунао процењени приход.</span><span class="sxs-lookup"><span data-stu-id="d1d60-113">If the revenue method of the Opportunity summary is set to **System Calculated**, the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
