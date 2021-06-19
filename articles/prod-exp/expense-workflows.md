---
title: Подешавање токова посла за управљање трошковима
description: Можете да подесите процес тока посла за преглед и одобравање путних и трошковних докумената.
author: ShylaThompson
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 4070b4fb5109464abdabbce971688fb881dfcf2c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005134"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="acac4-103">Подешавање токова посла за управљање трошковима</span><span class="sxs-lookup"><span data-stu-id="acac4-103">Set up Expense management workflows</span></span>

<span data-ttu-id="acac4-104">Можете да подесите процес тока посла који се користи за преглед и одобравање путних и трошковних докумената.</span><span class="sxs-lookup"><span data-stu-id="acac4-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="acac4-105">Документи за које можете да дефинишете токове посла обухватају извештаје о трошковима, путне захтеве и захтеве за готовинским авансом.</span><span class="sxs-lookup"><span data-stu-id="acac4-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="acac4-106">Ток посла представља пословни процес.</span><span class="sxs-lookup"><span data-stu-id="acac4-106">A workflow represents a business process.</span></span> <span data-ttu-id="acac4-107">Дефинише како документ пролази кроз систем и указује на то ко мора да доврши задатак или одобри документ.</span><span class="sxs-lookup"><span data-stu-id="acac4-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="acac4-108">Постоји неколико предности коришћења система тока посла у вашој организацији:</span><span class="sxs-lookup"><span data-stu-id="acac4-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="acac4-109">**Доследни процеси** – Можете да дефинишете поступак одобравања за одређене документе, као што су захтеви за куповину и извештаји о трошковима.</span><span class="sxs-lookup"><span data-stu-id="acac4-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="acac4-110">Коришћење система тока посла помаже у обезбеђивању обраде и одобравања докумената на доследан и ефикасан начин.</span><span class="sxs-lookup"><span data-stu-id="acac4-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="acac4-111">Видљивост процеса – Можете пратити статус, историју и показатеље учинка одређене инстанце тока посла.</span><span class="sxs-lookup"><span data-stu-id="acac4-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="acac4-112">Ово вам помаже да утврдите да ли треба извршити промене у току посла како бисте побољшали ефикасност.</span><span class="sxs-lookup"><span data-stu-id="acac4-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="acac4-113">Централизована радна листа – Корисници могу да виде централизовану листу послова да би видели задатке тока посла и одобрења која су им додељена.</span><span class="sxs-lookup"><span data-stu-id="acac4-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="acac4-114">**Типови токова посла које можете креирати**</span><span class="sxs-lookup"><span data-stu-id="acac4-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="acac4-115">Следећа табела наводи типове токова посла у којима можете да креирате у одељку **Трошак**.</span><span class="sxs-lookup"><span data-stu-id="acac4-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="acac4-116"><strong>Тип</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="acac4-117"><strong>Користите овај тип за</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="acac4-118"><strong>Извештај о трошковима</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="acac4-119">Креирајте токове одобрења за извештаје о трошковима.</span><span class="sxs-lookup"><span data-stu-id="acac4-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="acac4-120"><strong>Аутоматско објављивање извештаја о трошковима</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="acac4-121">Креирајте токове аутоматског објављивања за извештаје о трошковима.</span><span class="sxs-lookup"><span data-stu-id="acac4-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="acac4-122"><strong>Ставка трошка</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="acac4-123">Креирајте токове одобрења за ставке у извештајима о трошковима.</span><span class="sxs-lookup"><span data-stu-id="acac4-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="acac4-124"><strong>Аутоматско објављивање ставке трошка</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="acac4-125">Креирајте токове аутоматског објављивања за ставке у извештајима о трошковима.</span><span class="sxs-lookup"><span data-stu-id="acac4-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="acac4-126"><strong>Захтев за путовањем</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="acac4-127">Креирајте токове посла одобрења за путне захтеве.</span><span class="sxs-lookup"><span data-stu-id="acac4-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="acac4-128"><strong>Захтев за готовински аванс</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="acac4-129">Креирајте токове одобрења за захтеве за готовинским авансом.</span><span class="sxs-lookup"><span data-stu-id="acac4-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="acac4-130"><strong>Повраћај ПДВ-а</strong></span><span class="sxs-lookup"><span data-stu-id="acac4-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="acac4-131">Креирајте токове одобрења за повраћај пореза на додату вредност (ПДВ).</span><span class="sxs-lookup"><span data-stu-id="acac4-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |



[!INCLUDE[footer-include](../includes/footer-banner.md)]