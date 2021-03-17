---
title: Процене трошкова
description: Ова тема пружа информације о дефинисању или процени трошкова заснованих на пројекту.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3f0429366c69346113003355679c055cd2c74ca3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287076"
---
# <a name="expense-estimates"></a><span data-ttu-id="a5b67-103">Процене трошкова</span><span class="sxs-lookup"><span data-stu-id="a5b67-103">Expense estimates</span></span>
<span data-ttu-id="a5b67-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="a5b67-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a5b67-105">Поред дефинисања процена заснованих на ресурсима, Dynamics 365 Project Operations омогућава менаџерима пројеката да дефинишу трошкове засноване на пројекту за сваки пројекат.</span><span class="sxs-lookup"><span data-stu-id="a5b67-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="a5b67-106">Свака ставка трошкова може бити повезана са одређеним пројектним задатком или категоријом трошкова.</span><span class="sxs-lookup"><span data-stu-id="a5b67-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="a5b67-107">Категорије трошкова се обично дефинишу на нивоу организације.</span><span class="sxs-lookup"><span data-stu-id="a5b67-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="a5b67-108">Одређивање цена за сваку категорију трошкова обично је дефинисано у следећој хијерархији:</span><span class="sxs-lookup"><span data-stu-id="a5b67-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="a5b67-109">Организација</span><span class="sxs-lookup"><span data-stu-id="a5b67-109">Organization</span></span>
- <span data-ttu-id="a5b67-110">Клијент</span><span class="sxs-lookup"><span data-stu-id="a5b67-110">Customer</span></span>
- <span data-ttu-id="a5b67-111">Понуда/уговор</span><span class="sxs-lookup"><span data-stu-id="a5b67-111">Quote/contract</span></span>

<span data-ttu-id="a5b67-112">Довршите следеће кораке за приказ, додавање или брисање трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="a5b67-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="a5b67-113">Идите на **Пројекти**, и изаберите пројекат на којем желите да радите.</span><span class="sxs-lookup"><span data-stu-id="a5b67-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="a5b67-114">Изаберите картицу **Пројектне процене** и погледајте листу трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="a5b67-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="a5b67-115">Изаберите **Нови трошак** да бисте додали трошак.</span><span class="sxs-lookup"><span data-stu-id="a5b67-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="a5b67-116">Или изаберите трошак који желите да избришете, а затим изаберите **Избриши трошак**.</span><span class="sxs-lookup"><span data-stu-id="a5b67-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="a5b67-117">Следећи атрибути су дефинисани за сваку ставку трошкова:</span><span class="sxs-lookup"><span data-stu-id="a5b67-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="a5b67-118">**Категорија**: Уобичајена груписања коришћена за описивање свих трошкова насталих на пројекту.</span><span class="sxs-lookup"><span data-stu-id="a5b67-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="a5b67-119">**Датум почетка**: Датум када се предвиђа да ће настати трошак.</span><span class="sxs-lookup"><span data-stu-id="a5b67-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="a5b67-120">**Количина**: Процењени број ставки трошкова за одређену категорију.</span><span class="sxs-lookup"><span data-stu-id="a5b67-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="a5b67-121">**Јединична цена коштања**: Јединична цена која се користи за израчунавање цене трошкова.</span><span class="sxs-lookup"><span data-stu-id="a5b67-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="a5b67-122">**Јединична продајна цена**: Јединична цена која се користи за израчунавање продајне цене трошкова.</span><span class="sxs-lookup"><span data-stu-id="a5b67-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]