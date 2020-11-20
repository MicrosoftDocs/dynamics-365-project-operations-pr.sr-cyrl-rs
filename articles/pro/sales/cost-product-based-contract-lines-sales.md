---
title: Цена за предмете уговора засноване на производу – једноставно
description: Ова тема пружа информације о креирању
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0e961bcf32a5dd662b7cd27a23eb5f664c45c292
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177259"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="bc7ad-103">Цена за предмете уговора засноване на производу – једноставно</span><span class="sxs-lookup"><span data-stu-id="bc7ad-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="bc7ad-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="bc7ad-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="bc7ad-105">Предмети уговора засновани на производима у програму Dynamics 365 Project Operations укључују поље **Цена коштања**, у коме се чува цена коштања производа за прорачун профитабилности на нижем нивоу.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="bc7ad-106">Када се предмет уговора заснован на производу креира за каталошки производ, подразумевани трошкови предмета уговора заснованог на производу долазе из поља **Стандардна цена** у каталогу производа.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="bc7ad-107">Поље **Стандардна цена** у каталогу производа подешено је у основној валути организације.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="bc7ad-108">Када јединични трошак подразумева предмет уговора, он се претвара у валуту продаје на уговору.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="bc7ad-109">Јединична цена предмета уговора заснованог на производу</span><span class="sxs-lookup"><span data-stu-id="bc7ad-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="bc7ad-110">Постојање јединичне цене у предмету уговора заснованог на производу омогућава различите цене за производ за сваку продају јединице.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="bc7ad-111">Иако нису увек неопходни, постоје одређени сценарији у којима добављач може снизити трошкове производа за клијента.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="bc7ad-112">Размотрите следећи сценарио:</span><span class="sxs-lookup"><span data-stu-id="bc7ad-112">Consider the following scenario:</span></span>

<span data-ttu-id="bc7ad-113">Fabrikam Robotics инсталира роботске руке на производним тракама компаније Adatum Corporation.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="bc7ad-114">Fabrikam пружа услуге уградње, али роботске руке су набављене од компаније Trey Research.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="bc7ad-115">Ако инсталација роботске руке у компанији Adatum Corporation отвори нову индустријску делатност за роботске руке компаније Trey Research, тада би компанија Trey Research могла дати посебан попуст за овај посао компанији Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="bc7ad-116">У овом случају, Fabrikam креира предмет уговора заснован на производу за роботске руке и уноси јединични трошак за овај уговор који се разликује од стандардног трошка роботских руку компаније Trey Research.</span><span class="sxs-lookup"><span data-stu-id="bc7ad-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
