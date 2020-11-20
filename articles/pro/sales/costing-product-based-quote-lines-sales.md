---
title: Ставке производа засноване на обрачуну
description: Ова тема пружа информације о примени цене коштања на ставку понуде засноване на производу.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d21ab159294cac66ffeb8abcf0943b4babd7b360
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4118944"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="c1f42-103">Ставке производа засноване на обрачуну</span><span class="sxs-lookup"><span data-stu-id="c1f42-103">Costing product-based quote lines</span></span>

<span data-ttu-id="c1f42-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="c1f42-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c1f42-105">Ставке понуде засноване на производу у услузи Dynamics 365 Project Operations такође имају поље **Цена коштања**.</span><span class="sxs-lookup"><span data-stu-id="c1f42-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="c1f42-106">Ово поље се користи за праћење цене коштања производа на ставци понуде и за последичне прорачуне профитабилности.</span><span class="sxs-lookup"><span data-stu-id="c1f42-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="c1f42-107">Када се ставка понуде заснована на производу креира за каталошки производ, подразумевани трошкови ставке понуде засноване на производу долазе из поља **Стандардна цена** у каталогу производа.</span><span class="sxs-lookup"><span data-stu-id="c1f42-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="c1f42-108">Поље стандардне цене у каталогу производа подешено је у основној валути организације.</span><span class="sxs-lookup"><span data-stu-id="c1f42-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="c1f42-109">Подразумевана јединична цена у ставци понуде засноване на производу претвара се у продајну валуту у понуди.</span><span class="sxs-lookup"><span data-stu-id="c1f42-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="c1f42-110">Јединична цена ставке понуде засноване на производу</span><span class="sxs-lookup"><span data-stu-id="c1f42-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="c1f42-111">Сврха постојања јединичне цене у ставци понуде засноване на производу је омогућавање различитих цена за производ за сваку продају.</span><span class="sxs-lookup"><span data-stu-id="c1f42-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="c1f42-112">То није типичан сценарио, али добављач понекад може да снизи цену производа у зависности од клијента коначне продаје.</span><span class="sxs-lookup"><span data-stu-id="c1f42-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="c1f42-113">На пример:</span><span class="sxs-lookup"><span data-stu-id="c1f42-113">For example:</span></span>

<span data-ttu-id="c1f42-114">Fabrikam Robotics инсталира роботске руке на производним тракама компаније A Datum Corporation.</span><span class="sxs-lookup"><span data-stu-id="c1f42-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="c1f42-115">Fabrikam пружа услуге уградње, али роботске руке су набављене од компаније Trey robotics.</span><span class="sxs-lookup"><span data-stu-id="c1f42-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="c1f42-116">Ако инсталација роботске руке у компанији A Datum Corporation отвори нову индустријску делатност за роботске руке компаније Trey, тада би компанија Trey могла дати посебан попуст за овај посао компанији Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="c1f42-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="c1f42-117">У овом случају, Fabrikam ће креирати ставку понуде засновану на производу за роботске руке и унеће посебну цену по јединици за ову понуду.</span><span class="sxs-lookup"><span data-stu-id="c1f42-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="c1f42-118">Та цена се разликује од стандардне цене роботске руке компаније Trey.</span><span class="sxs-lookup"><span data-stu-id="c1f42-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>
