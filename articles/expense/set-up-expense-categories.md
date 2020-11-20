---
title: Подешавање категорија трошкова
description: Ова тема пружа информације о томе како да поставите категорије трошкова и дељене категорије за извештаје о трошковима.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 13e72e4b852fd0edac5ad35d5162e74b016bce33
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123801"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="73a7b-103">Подешавање категорија трошкова</span><span class="sxs-lookup"><span data-stu-id="73a7b-103">Set up expense categories</span></span>

<span data-ttu-id="73a7b-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="73a7b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="73a7b-105">Када запослени креирају извештаје о трошковима, сваки трошак који евидентирају мора бити повезан са категоријом трошкова.</span><span class="sxs-lookup"><span data-stu-id="73a7b-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="73a7b-106">Категорије трошкова су изведене из дељених категорија које се могу делити између правних лица у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="73a7b-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="73a7b-107">У зависности од тога како је ваша организација дефинисана, ове категорије трошкова могу се делити и у другим областима.</span><span class="sxs-lookup"><span data-stu-id="73a7b-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="73a7b-108">На основу дефиниције ваше организације и смерница тима за примену, морате да одредите да ли ће се категорије које се користе у управљању трошковима користити само у управљању трошковима или треба да се деле у другим областима.</span><span class="sxs-lookup"><span data-stu-id="73a7b-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="73a7b-109">Ове категорије се могу делити између управљања пројектима и рачуноводства и управљања трошковима или између управљања пројектима и рачуноводства и производње.</span><span class="sxs-lookup"><span data-stu-id="73a7b-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="73a7b-110">Међутим, они не могу да се деле између трошкова управљања и производње.</span><span class="sxs-lookup"><span data-stu-id="73a7b-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="73a7b-111">Пре него што започнете поступак подешавања, за сваку категорију трошкова морају се донети следеће одлуке:</span><span class="sxs-lookup"><span data-stu-id="73a7b-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="73a7b-112">Шта је то категорија трошкова?</span><span class="sxs-lookup"><span data-stu-id="73a7b-112">What is the expense category?</span></span> <span data-ttu-id="73a7b-113">Примери укључују категорије за летове, хотеле или километражу.</span><span class="sxs-lookup"><span data-stu-id="73a7b-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="73a7b-114">Може ли се категорија трошкова такође користити у управљању пројектима и рачуноводству?</span><span class="sxs-lookup"><span data-stu-id="73a7b-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="73a7b-115">Ако може, морате донети и следеће одлуке:</span><span class="sxs-lookup"><span data-stu-id="73a7b-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="73a7b-116">Који рачуни трошкова ће се користити за следеће трошкове?</span><span class="sxs-lookup"><span data-stu-id="73a7b-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="73a7b-117">Цена</span><span class="sxs-lookup"><span data-stu-id="73a7b-117">Cost</span></span>
        - <span data-ttu-id="73a7b-118">Расподела зарада</span><span class="sxs-lookup"><span data-stu-id="73a7b-118">Payroll allocation</span></span>
        - <span data-ttu-id="73a7b-119">Приходи у току – вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="73a7b-119">WIP-cost value</span></span>
        - <span data-ttu-id="73a7b-120">Ставка трошкова</span><span class="sxs-lookup"><span data-stu-id="73a7b-120">Cost-item</span></span>
        - <span data-ttu-id="73a7b-121">Приходи у току – вредност трошкова – ставка</span><span class="sxs-lookup"><span data-stu-id="73a7b-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="73a7b-122">Обрачунати губитак</span><span class="sxs-lookup"><span data-stu-id="73a7b-122">Accrued loss</span></span>
        - <span data-ttu-id="73a7b-123">Приходи у току – обрачунати губитак</span><span class="sxs-lookup"><span data-stu-id="73a7b-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="73a7b-124">Који рачуни прихода ће се користити за следеће изворе прихода?</span><span class="sxs-lookup"><span data-stu-id="73a7b-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="73a7b-125">Фактурисани приход</span><span class="sxs-lookup"><span data-stu-id="73a7b-125">Invoiced revenue</span></span>
        - <span data-ttu-id="73a7b-126">Обрачунати приход – Вредност продаје</span><span class="sxs-lookup"><span data-stu-id="73a7b-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="73a7b-127">Приходи у току – вредност продаје</span><span class="sxs-lookup"><span data-stu-id="73a7b-127">WIP-sales value</span></span>
        - <span data-ttu-id="73a7b-128">Обрачунати приход – производња</span><span class="sxs-lookup"><span data-stu-id="73a7b-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="73a7b-129">Приходи у току – производња</span><span class="sxs-lookup"><span data-stu-id="73a7b-129">WIP-production</span></span>
        - <span data-ttu-id="73a7b-130">Обрачунати приход – профит</span><span class="sxs-lookup"><span data-stu-id="73a7b-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="73a7b-131">Приходи у току – профит</span><span class="sxs-lookup"><span data-stu-id="73a7b-131">WIP-profit</span></span>
        - <span data-ttu-id="73a7b-132">Обрачунати приход – претплата</span><span class="sxs-lookup"><span data-stu-id="73a7b-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="73a7b-133">Приходи у току – претплата</span><span class="sxs-lookup"><span data-stu-id="73a7b-133">WIP-subscription</span></span>

- <span data-ttu-id="73a7b-134">Шта је то тип трошка?</span><span class="sxs-lookup"><span data-stu-id="73a7b-134">What is the expense type?</span></span>
- <span data-ttu-id="73a7b-135">Који је подразумевани начин плаћања за категорију трошка?</span><span class="sxs-lookup"><span data-stu-id="73a7b-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="73a7b-136">Морају ли се детаљно делити трошкови у категорији трошкова?</span><span class="sxs-lookup"><span data-stu-id="73a7b-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="73a7b-137">Који је главни подразумевани рачун за категорију трошка?</span><span class="sxs-lookup"><span data-stu-id="73a7b-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="73a7b-138">Која је подразумевана група пореза на промет производа за категорију трошкова?</span><span class="sxs-lookup"><span data-stu-id="73a7b-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="73a7b-139">Да ли су дозвољени додатни начини плаћања за категорију трошкова?</span><span class="sxs-lookup"><span data-stu-id="73a7b-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="73a7b-140">Ако јесу, који су то?</span><span class="sxs-lookup"><span data-stu-id="73a7b-140">If so, what are they?</span></span>
- <span data-ttu-id="73a7b-141">Постоје ли поткатегорије у овој категорији трошкова?</span><span class="sxs-lookup"><span data-stu-id="73a7b-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="73a7b-142">Ако постоје поткатегорије, морате донети и следеће одлуке:</span><span class="sxs-lookup"><span data-stu-id="73a7b-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="73a7b-143">Да ли је нека од поткатегорија изузета од повраћаја пореза?</span><span class="sxs-lookup"><span data-stu-id="73a7b-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="73a7b-144">Која је група пореза на промет производа за поткатегорије?</span><span class="sxs-lookup"><span data-stu-id="73a7b-144">What is the item sales tax group of the subcategories?</span></span>
