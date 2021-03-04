---
title: Цена за предмете уговора засноване на производу – једноставно
description: Ова тема пружа информације о креирању
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a81c972f36179621f0547c24fc53d294485f638c
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764477"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="33512-103">Цена за предмете уговора засноване на производу – једноставно</span><span class="sxs-lookup"><span data-stu-id="33512-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="33512-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="33512-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="33512-105">Предмети уговора заснованих на производима у услузи Dynamics 365 Project Operations укључују поље **Цена коштања** у коме се чува цена коштања производа за прорачуне профитабилности дистрибуције.</span><span class="sxs-lookup"><span data-stu-id="33512-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="33512-106">Када се за производ из каталога креира предмет уговора заснована на производу, трошкови у реду се подразумевано подешавају из поља **Стандардни трошкови** у каталогу производа.</span><span class="sxs-lookup"><span data-stu-id="33512-106">When a product-based contract line is created for a catalog product, the cost of the line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="33512-107">Поље **Стандардна цена** у каталогу производа подешено је у основној валути организације.</span><span class="sxs-lookup"><span data-stu-id="33512-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="33512-108">Када јединични трошак подразумева предмет уговора, он се претвара у валуту продаје на уговору.</span><span class="sxs-lookup"><span data-stu-id="33512-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="33512-109">Јединична цена предмета уговора заснованог на производу</span><span class="sxs-lookup"><span data-stu-id="33512-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="33512-110">Постојање јединичне цене у предмету уговора заснованог на производу омогућава различите цене за производ за сваку продају јединице.</span><span class="sxs-lookup"><span data-stu-id="33512-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="33512-111">Иако нису увек неопходни, постоје одређени сценарији у којима добављач може снизити трошкове производа за клијента.</span><span class="sxs-lookup"><span data-stu-id="33512-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="33512-112">Размотрите следећи сценарио:</span><span class="sxs-lookup"><span data-stu-id="33512-112">Consider the following scenario:</span></span>

<span data-ttu-id="33512-113">Fabrikam Robotics инсталира роботске руке на производним тракама компаније Adatum Corporation.</span><span class="sxs-lookup"><span data-stu-id="33512-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="33512-114">Fabrikam пружа услуге уградње, али руке робота су из компаније Trey Research.</span><span class="sxs-lookup"><span data-stu-id="33512-114">Fabrikam provides installation services but the robotic arms are from Trey Research.</span></span> <span data-ttu-id="33512-115">Ако инсталација роботске руке у компанији Adatum Corporation отвори нову индустријску делатност за роботске руке компаније Trey Research, тада би компанија Trey Research могла дати посебан попуст за овај посао компанији Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="33512-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="33512-116">У овом случају, Fabrikam креира предмет уговора заснован на производу за руке робота.</span><span class="sxs-lookup"><span data-stu-id="33512-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms.</span></span> <span data-ttu-id="33512-117">За овај уговор се уноси цена по јединици.</span><span class="sxs-lookup"><span data-stu-id="33512-117">A per unit cost is entered for this contract.</span></span> <span data-ttu-id="33512-118">Цена се разликује од цене за руке робота компаније Trey Research.</span><span class="sxs-lookup"><span data-stu-id="33512-118">The cost is different from the cost of robotic arms from Trey Research.</span></span>
