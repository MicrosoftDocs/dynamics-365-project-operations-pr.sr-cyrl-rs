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
ms.openlocfilehash: 9b9826c89e9deb870adb053f82bd049906f56052
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276546"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="c708e-103">Извештаји о трошковима и више одобравалаца</span><span class="sxs-lookup"><span data-stu-id="c708e-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="c708e-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="c708e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c708e-105">У зависности од смерница одобравања трошкова у вашој организацији, поднети извештај о трошковима ће можда морати да одобри више особа.</span><span class="sxs-lookup"><span data-stu-id="c708e-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="c708e-106">Када успостављате процес тока посла за одобравање извештаја о трошковима, можете да додате елементе тока посла који укључују задатке или кораке за једног даваоца одобрења за извештај о трошковима или више њих.</span><span class="sxs-lookup"><span data-stu-id="c708e-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="c708e-107">На пример, можда ћете захтевати да све извештаје о трошковима одобре две засебне особе, менаџер запосленог који је поднео извештај и координатор за дуговања.</span><span class="sxs-lookup"><span data-stu-id="c708e-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="c708e-108">Ако одлучите да захтевате више давалаца одобрења за извештај о трошковима, можете да додате елементе тока посла на било који од следећих начина:</span><span class="sxs-lookup"><span data-stu-id="c708e-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="c708e-109">Додајте један елемент одобрења који има један корак.</span><span class="sxs-lookup"><span data-stu-id="c708e-109">Add one approval element that has one step.</span></span> <span data-ttu-id="c708e-110">На пример, корак може захтевати да се извештај о трошковима додели групи корисника и да га одобри 50% чланова групе корисника.</span><span class="sxs-lookup"><span data-stu-id="c708e-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="c708e-111">Додајте један елемент одобрења који има више корака.</span><span class="sxs-lookup"><span data-stu-id="c708e-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="c708e-112">На пример, елемент одобрења може имати следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="c708e-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="c708e-113">Директор запосленог који је поднео извештај о трошковима га одобрава.</span><span class="sxs-lookup"><span data-stu-id="c708e-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="c708e-114">Службеник за дуговања верификује признанице и ставке извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="c708e-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="c708e-115">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="c708e-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="c708e-116">Додајте више елемената одобрења, од којих сваки има један корак.</span><span class="sxs-lookup"><span data-stu-id="c708e-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="c708e-117">На пример, можете додати засебни елемент одобрења за сваки од следећих корака:</span><span class="sxs-lookup"><span data-stu-id="c708e-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="c708e-118">Менаџер запосленог одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="c708e-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="c708e-119">Власник буџета одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="c708e-119">The budget owner approves the expense report.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]