---
title: Ставке производа засноване на обрачуну
description: Ова тема пружа информације о примени цене коштања на ставку понуде засноване на производу.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1fa7896e249abfefd3e93cba4bad789e67e14f31
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003469"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="5edd6-103">Ставке производа засноване на обрачуну</span><span class="sxs-lookup"><span data-stu-id="5edd6-103">Costing product-based quote lines</span></span>

<span data-ttu-id="5edd6-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="5edd6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="5edd6-105">Ставке понуде засноване на производу у услузи Dynamics 365 Project Operations такође имају поље **Цена коштања**.</span><span class="sxs-lookup"><span data-stu-id="5edd6-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="5edd6-106">Ово поље се користи за праћење цене коштања производа на ставци понуде и за последичне прорачуне профитабилности.</span><span class="sxs-lookup"><span data-stu-id="5edd6-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="5edd6-107">Када се ставка понуде заснована на производу креира за каталошки производ, подразумевани трошкови ставке понуде засноване на производу долазе из поља **Стандардна цена** у каталогу производа.</span><span class="sxs-lookup"><span data-stu-id="5edd6-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="5edd6-108">Поље стандардне цене у каталогу производа подешено је у основној валути организације.</span><span class="sxs-lookup"><span data-stu-id="5edd6-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="5edd6-109">Подразумевана јединична цена у ставци понуде засноване на производу претвара се у продајну валуту у понуди.</span><span class="sxs-lookup"><span data-stu-id="5edd6-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="5edd6-110">Јединична цена ставке понуде засноване на производу</span><span class="sxs-lookup"><span data-stu-id="5edd6-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="5edd6-111">Сврха постојања јединичне цене у ставци понуде засноване на производу је омогућавање различитих цена за производ за сваку продају.</span><span class="sxs-lookup"><span data-stu-id="5edd6-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="5edd6-112">То није типичан сценарио, али добављач понекад може да снизи цену производа у зависности од клијента коначне продаје.</span><span class="sxs-lookup"><span data-stu-id="5edd6-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="5edd6-113">На пример:</span><span class="sxs-lookup"><span data-stu-id="5edd6-113">For example:</span></span>

<span data-ttu-id="5edd6-114">Fabrikam Robotics инсталира роботске руке на производним тракама компаније A Datum Corporation.</span><span class="sxs-lookup"><span data-stu-id="5edd6-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="5edd6-115">Fabrikam пружа услуге уградње, али роботске руке су набављене од компаније Trey robotics.</span><span class="sxs-lookup"><span data-stu-id="5edd6-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="5edd6-116">Ако инсталација роботске руке у компанији A Datum Corporation отвори нову индустријску делатност за роботске руке компаније Trey, тада би компанија Trey могла дати посебан попуст за овај посао компанији Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="5edd6-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="5edd6-117">У овом случају, Fabrikam ће креирати ставку понуде засновану на производу за роботске руке и унеће посебну цену по јединици за ову понуду.</span><span class="sxs-lookup"><span data-stu-id="5edd6-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="5edd6-118">Та цена се разликује од стандардне цене роботске руке компаније Trey.</span><span class="sxs-lookup"><span data-stu-id="5edd6-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]