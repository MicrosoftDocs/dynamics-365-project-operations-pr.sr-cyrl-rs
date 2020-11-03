---
title: Процене трошкова
description: Ова тема пружа информације о дефинисању или процени трошкова заснованих на пројекту.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2afe4ff2f84fc5426c409e6314da73b11a4de281
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083894"
---
# <a name="expense-estimates"></a><span data-ttu-id="bb639-103">Процене трошкова</span><span class="sxs-lookup"><span data-stu-id="bb639-103">Expense estimates</span></span>
<span data-ttu-id="bb639-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="bb639-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bb639-105">Заједно са дефинисањем процена заснованих на ресурсима, Dynamics 365 Project Operations омогућава менаџерима пројеката да дефинишу трошкове засноване на пројекту за сваки пројекат.</span><span class="sxs-lookup"><span data-stu-id="bb639-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="bb639-106">Свака ставка трошкова може бити повезана са одређеним пројектним задатком или категоријом трошкова.</span><span class="sxs-lookup"><span data-stu-id="bb639-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="bb639-107">Категорије трошкова се обично дефинишу на нивоу организације.</span><span class="sxs-lookup"><span data-stu-id="bb639-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="bb639-108">Одређивање цена за сваку категорију трошкова обично је дефинисано у следећој хијерархији:</span><span class="sxs-lookup"><span data-stu-id="bb639-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="bb639-109">Организација</span><span class="sxs-lookup"><span data-stu-id="bb639-109">Organization</span></span>
- <span data-ttu-id="bb639-110">Клијент</span><span class="sxs-lookup"><span data-stu-id="bb639-110">Customer</span></span>
- <span data-ttu-id="bb639-111">Понуда/уговор</span><span class="sxs-lookup"><span data-stu-id="bb639-111">Quote/contract</span></span>

<span data-ttu-id="bb639-112">Довршите следеће кораке за приказ, додавање или брисање трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="bb639-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="bb639-113">Идите на **Пројекти** , и изаберите пројекат на којем желите да радите.</span><span class="sxs-lookup"><span data-stu-id="bb639-113">Go to **Projects** , and select the project you want to work on.</span></span>
2. <span data-ttu-id="bb639-114">Изаберите картицу **Пројектне процене** и погледајте листу трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="bb639-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="bb639-115">Изаберите **Нови трошак** да бисте додали трошак.</span><span class="sxs-lookup"><span data-stu-id="bb639-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="bb639-116">Или изаберите трошак који желите да избришете, а затим изаберите **Избриши трошак**.</span><span class="sxs-lookup"><span data-stu-id="bb639-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="bb639-117">Следећи атрибути су дефинисани за сваку ставку трошкова:</span><span class="sxs-lookup"><span data-stu-id="bb639-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="bb639-118">**Категорија** : Уобичајена груписања коришћена за описивање свих трошкова насталих на пројекту.</span><span class="sxs-lookup"><span data-stu-id="bb639-118">**Category** : The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="bb639-119">**Датум почетка** : Датум када се предвиђа да ће настати трошак.</span><span class="sxs-lookup"><span data-stu-id="bb639-119">**Start Date** : The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="bb639-120">**Количина** : Процењени број ставки трошкова за одређену категорију.</span><span class="sxs-lookup"><span data-stu-id="bb639-120">**Quantity** : The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="bb639-121">**Јединична цена коштања** : Јединична цена која се користи за израчунавање цене трошкова.</span><span class="sxs-lookup"><span data-stu-id="bb639-121">**Unit Cost Price** : The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="bb639-122">**Јединична продајна цена** : Јединична цена која се користи за израчунавање продајне цене трошкова.</span><span class="sxs-lookup"><span data-stu-id="bb639-122">**Unit Sales Price** : The unit price used to calculate the sale prices of the expense.</span></span>

