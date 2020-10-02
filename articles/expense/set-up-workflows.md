---
title: Подесите токове посла за управљање трошковима
description: Можете да подесите процес тока посла који се користи за преглед и одобравање путних и трошковних докумената.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: dfc5945f32bb8d4073fc31499979ba279fef66a4
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896569"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="2c778-103">Подесите токове посла за управљање трошковима</span><span class="sxs-lookup"><span data-stu-id="2c778-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="2c778-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="2c778-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2c778-105">Можете да подесите процес тока посла за преглед и одобравање путних и трошковних докумената.</span><span class="sxs-lookup"><span data-stu-id="2c778-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="2c778-106">Можете да дефинишете токове посла за извештаје о трошковима, путне захтеве и захтеве за готовинским авансом.</span><span class="sxs-lookup"><span data-stu-id="2c778-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="2c778-107">Ток посла представља пословни процес и дефинише како документ пролази кроз систем.</span><span class="sxs-lookup"><span data-stu-id="2c778-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="2c778-108">Ток посла такође показује ко мора да изврши задатак или одобри документ.</span><span class="sxs-lookup"><span data-stu-id="2c778-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="2c778-109">Постоји неколико предности коришћења система тока посла у вашој организацији:</span><span class="sxs-lookup"><span data-stu-id="2c778-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="2c778-110">**Доследни процеси** : Можете да дефинишете поступак одобравања за одређене документе, као што су захтеви за куповину и извештаји о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c778-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="2c778-111">Коришћење система тока посла помаже у обезбеђивању обраде и одобравања докумената на доследан и ефикасан начин.</span><span class="sxs-lookup"><span data-stu-id="2c778-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="2c778-112">**Видљивост процеса** : Можете пратити статус, историју и показатеље учинка одређене инстанце тока посла.</span><span class="sxs-lookup"><span data-stu-id="2c778-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="2c778-113">Ово вам помаже да утврдите да ли треба извршити промене у току посла како бисте побољшали ефикасност.</span><span class="sxs-lookup"><span data-stu-id="2c778-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="2c778-114">**Централизована радна листа** : Корисници могу да виде централизовану листу послова да би видели задатке тока посла и одобрења која су им додељена.</span><span class="sxs-lookup"><span data-stu-id="2c778-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="2c778-115">Типови тока посла</span><span class="sxs-lookup"><span data-stu-id="2c778-115">Workflow types</span></span>

<span data-ttu-id="2c778-116">Следећа табела наводи типове токова посла у којима можете да креирате **Управљање трошковима**.</span><span class="sxs-lookup"><span data-stu-id="2c778-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="2c778-117"><strong>Тип</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="2c778-118"><strong>Користите овај тип за</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="2c778-119"><strong>Аутоматско одобравање извештаја о трошковима</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="2c778-120">Креирајте токове одобрења за извештаје о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c778-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="2c778-121"><strong>Аутоматско објављивање извештаја о трошковима</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="2c778-122">Креирајте токове аутоматског објављивања за извештаје о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c778-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="2c778-123"><strong>Ставка трошка</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="2c778-124">Креирајте токове одобрења за ставке у извештајима о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c778-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="2c778-125"><strong>Аутоматско објављивање ставке трошка</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="2c778-126">Креирајте токове аутоматског објављивања за ставке у извештајима о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c778-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="2c778-127"><strong>Захтев за путовањем</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="2c778-128">Креирајте токове посла одобрења за путне захтеве.</span><span class="sxs-lookup"><span data-stu-id="2c778-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="2c778-129"><strong>Захтев за готовински аванс</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="2c778-130">Креирајте токове одобрења за захтеве за готовинским авансом.</span><span class="sxs-lookup"><span data-stu-id="2c778-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="2c778-131"><strong>Повраћај ПДВ-а</strong></span><span class="sxs-lookup"><span data-stu-id="2c778-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="2c778-132">Креирајте токове одобрења за повраћај пореза на додату вредност (ПДВ).</span><span class="sxs-lookup"><span data-stu-id="2c778-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |
