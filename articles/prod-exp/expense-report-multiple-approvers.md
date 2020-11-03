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
ms.openlocfilehash: ce24b156a268f9f5aada35f9314d2d9c6607200b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084128"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="1553c-103">Више давалаца одобрења на извештају о трошковима</span><span class="sxs-lookup"><span data-stu-id="1553c-103">Multiple approvers on an expense report</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1553c-104">У зависности од смерница одобравања трошкова у вашој организацији, извештај о трошковима који је поднео неки запослени можда ће морати да одобри више особа.</span><span class="sxs-lookup"><span data-stu-id="1553c-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="1553c-105">Када успостављате процес тока посла за одобравање извештаја о трошковима, можете да додате елементе тока посла који укључују задатке или кораке за једног даваоца одобрења за извештај о трошковима или више њих.</span><span class="sxs-lookup"><span data-stu-id="1553c-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="1553c-106">На пример, можда ћете захтевати да све извештаје о трошковима прво одобри менаџер запосленог који је поднео извештај, а затим координатор за дуговања.</span><span class="sxs-lookup"><span data-stu-id="1553c-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="1553c-107">Ако одлучите да захтевате више давалаца одобрења за извештај о трошковима, можете да додате елементе тока посла на било који од следећих начина:</span><span class="sxs-lookup"><span data-stu-id="1553c-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="1553c-108">Додајте један елемент одобрења који има један корак.</span><span class="sxs-lookup"><span data-stu-id="1553c-108">Add one approval element that has one step.</span></span> <span data-ttu-id="1553c-109">На пример, корак може захтевати да се извештај о трошковима додели групи корисника и да га одобри 50% чланова групе корисника.</span><span class="sxs-lookup"><span data-stu-id="1553c-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="1553c-110">Додајте један елемент одобрења који има више корака.</span><span class="sxs-lookup"><span data-stu-id="1553c-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="1553c-111">На пример, елемент одобрења може имати следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="1553c-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="1553c-112">Директор запосленог који је поднео извештај о трошковима га одобрава.</span><span class="sxs-lookup"><span data-stu-id="1553c-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="1553c-113">Службеник за дуговања верификује признанице и ставке извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="1553c-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="1553c-114">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="1553c-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="1553c-115">Додајте више елемената одобрења, од којих сваки има један корак.</span><span class="sxs-lookup"><span data-stu-id="1553c-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="1553c-116">На пример, можете додати засебни елемент одобрења за сваки од следећих корака:</span><span class="sxs-lookup"><span data-stu-id="1553c-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="1553c-117">Менаџер запосленог одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="1553c-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="1553c-118">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="1553c-118">The budget owner approves the expense report.</span></span>
