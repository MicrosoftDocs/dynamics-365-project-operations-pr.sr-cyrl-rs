---
title: Више давалаца одобрења на извештају о трошковима
description: Ова тема пружа информације о извештајима о трошковима за које је потребно одобрење више особа.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0fbe1c93c5359a6be493e3c4e1b27b06dbb48002
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271731"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="7397a-103">Више давалаца одобрења на извештају о трошковима</span><span class="sxs-lookup"><span data-stu-id="7397a-103">Multiple approvers on an expense report</span></span>

<span data-ttu-id="7397a-104">У зависности од смерница одобравања трошкова у вашој организацији, извештај о трошковима који је поднео неки запослени можда ће морати да одобри више особа.</span><span class="sxs-lookup"><span data-stu-id="7397a-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="7397a-105">Када успостављате процес тока посла за одобравање извештаја о трошковима, можете да додате елементе тока посла који укључују задатке или кораке за једног даваоца одобрења за извештај о трошковима или више њих.</span><span class="sxs-lookup"><span data-stu-id="7397a-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="7397a-106">На пример, можда ћете захтевати да све извештаје о трошковима прво одобри менаџер запосленог који је поднео извештај, а затим координатор за дуговања.</span><span class="sxs-lookup"><span data-stu-id="7397a-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="7397a-107">Ако одлучите да захтевате више давалаца одобрења за извештај о трошковима, можете да додате елементе тока посла на било који од следећих начина:</span><span class="sxs-lookup"><span data-stu-id="7397a-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="7397a-108">Додајте један елемент одобрења који има један корак.</span><span class="sxs-lookup"><span data-stu-id="7397a-108">Add one approval element that has one step.</span></span> <span data-ttu-id="7397a-109">На пример, корак може захтевати да се извештај о трошковима додели групи корисника и да га одобри 50% чланова групе корисника.</span><span class="sxs-lookup"><span data-stu-id="7397a-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="7397a-110">Додајте један елемент одобрења који има више корака.</span><span class="sxs-lookup"><span data-stu-id="7397a-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="7397a-111">На пример, елемент одобрења може имати следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="7397a-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="7397a-112">Директор запосленог који је поднео извештај о трошковима га одобрава.</span><span class="sxs-lookup"><span data-stu-id="7397a-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="7397a-113">Службеник за дуговања верификује признанице и ставке извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="7397a-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="7397a-114">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="7397a-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="7397a-115">Додајте више елемената одобрења, од којих сваки има један корак.</span><span class="sxs-lookup"><span data-stu-id="7397a-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="7397a-116">На пример, можете додати засебни елемент одобрења за сваки од следећих корака:</span><span class="sxs-lookup"><span data-stu-id="7397a-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="7397a-117">Менаџер запосленог одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="7397a-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="7397a-118">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="7397a-118">The budget owner approves the expense report.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]