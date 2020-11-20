---
title: Извештаји о трошковима и више одобравалаца
description: Ова тема пружа информације о извештајима о трошковима за које је потребно одобрење више особа.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: cfa8677f38e9468aa3236f587d2e9bd5af839054
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121011"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="e602a-103">Извештаји о трошковима и више одобравалаца</span><span class="sxs-lookup"><span data-stu-id="e602a-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="e602a-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="e602a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e602a-105">У зависности од смерница одобравања трошкова у вашој организацији, поднети извештај о трошковима ће можда морати да одобри више особа.</span><span class="sxs-lookup"><span data-stu-id="e602a-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="e602a-106">Када успостављате процес тока посла за одобравање извештаја о трошковима, можете да додате елементе тока посла који укључују задатке или кораке за једног даваоца одобрења за извештај о трошковима или више њих.</span><span class="sxs-lookup"><span data-stu-id="e602a-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="e602a-107">На пример, можда ћете захтевати да све извештаје о трошковима одобре две засебне особе, менаџер запосленог који је поднео извештај и координатор за дуговања.</span><span class="sxs-lookup"><span data-stu-id="e602a-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="e602a-108">Ако одлучите да захтевате више давалаца одобрења за извештај о трошковима, можете да додате елементе тока посла на било који од следећих начина:</span><span class="sxs-lookup"><span data-stu-id="e602a-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="e602a-109">Додајте један елемент одобрења који има један корак.</span><span class="sxs-lookup"><span data-stu-id="e602a-109">Add one approval element that has one step.</span></span> <span data-ttu-id="e602a-110">На пример, корак може захтевати да се извештај о трошковима додели групи корисника и да га одобри 50% чланова групе корисника.</span><span class="sxs-lookup"><span data-stu-id="e602a-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="e602a-111">Додајте један елемент одобрења који има више корака.</span><span class="sxs-lookup"><span data-stu-id="e602a-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="e602a-112">На пример, елемент одобрења може имати следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="e602a-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="e602a-113">Директор запосленог који је поднео извештај о трошковима га одобрава.</span><span class="sxs-lookup"><span data-stu-id="e602a-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="e602a-114">Службеник за дуговања верификује признанице и ставке извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="e602a-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="e602a-115">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="e602a-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="e602a-116">Додајте више елемената одобрења, од којих сваки има један корак.</span><span class="sxs-lookup"><span data-stu-id="e602a-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="e602a-117">На пример, можете додати засебни елемент одобрења за сваки од следећих корака:</span><span class="sxs-lookup"><span data-stu-id="e602a-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="e602a-118">Менаџер запосленог одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="e602a-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="e602a-119">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="e602a-119">The budget owner approves the expense report.</span></span>
