---
title: Ставке могућности за пословање засноване на пројекту – једноставно
description: Ова тема пружа информације о ставкама предмета могућности за пословање заснованим на производу у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fd32bedb94cf36f706c112a845f342d9dde19805
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176358"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="f5f0b-103">Ставке могућности за пословање засноване на пројекту – једноставно</span><span class="sxs-lookup"><span data-stu-id="f5f0b-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="f5f0b-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="f5f0b-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f5f0b-105">Предмети могућности за пословање засновани на производу су ставке у могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="f5f0b-106">Ове ставке се испоручују клијенту као посебне ставке на евентуалној фактури без икаквих других услуга са додатом вредношћу.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="f5f0b-107">Повезана потрошња и коришћење се не прате на задацима било којих повезаних пројеката.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="f5f0b-108">Ставке засноване на производима могу бити артикли из каталога или ручно додати производи.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="f5f0b-109">Већина функционалности предмета могућности за пословање заснованих на производу прати функционалност коју пружа апликација Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="f5f0b-110">За више информација о предметима могућности за пословање заснованим на производу, погледајте [Додавање производа у могућност за пословање](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="f5f0b-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="f5f0b-111">Један концепт о предметима могућности за пословање заснованим на производу који је специфичан за могућности за пословање засноване на пројектима јесте **Буџет клијента**.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="f5f0b-112">Користите ово поље за праћење износа који је клијент спреман да плати за ставку поруџбине.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="f5f0b-113">Ако је метода прихода резимеа могућности за пословање постављена на **Системски израчунато**, вредности буџета клијената у ставкама заснованим на производу и пројекту се сабирају како би се израчунао процењени приход.</span><span class="sxs-lookup"><span data-stu-id="f5f0b-113">If the revenue method of the Opportunity summary is set to **System Calculated**, the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
