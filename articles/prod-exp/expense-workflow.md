---
title: Ток посла за управљање трошковима
description: Ова тема објашњава како можете да користите систем токова посла у услузи Microsoft Dynamics 365 Finance, да бисте успоставили поступак прегледа извештаја о трошковима у управљању трошковима.
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
ms.openlocfilehash: 51ac2712f62d5c5d85b21c0ea929517ccb893bca
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005224"
---
# <a name="expense-management-workflow"></a><span data-ttu-id="180e5-103">Ток посла за управљање трошковима</span><span class="sxs-lookup"><span data-stu-id="180e5-103">Expense management workflow</span></span>

<span data-ttu-id="180e5-104">Можете да користите систем токова посла да бисте успоставили поступак прегледа извештаја о трошковима у управљању трошковима.</span><span class="sxs-lookup"><span data-stu-id="180e5-104">You can use the workflow system to set up a review process for expense reports in Expense management.</span></span> <span data-ttu-id="180e5-105">Можете да подесите ток посла који користи следеће критеријуме да бисте одредили ко одобрава извештаје о трошковима:</span><span class="sxs-lookup"><span data-stu-id="180e5-105">You can set up a workflow that uses the following criteria to determine who approves expense reports:</span></span>

- <span data-ttu-id="180e5-106">Хијерархија извештавања запослених и унапред дефинисана ограничења одобрења</span><span class="sxs-lookup"><span data-stu-id="180e5-106">The employee reporting hierarchy and predefined approval limits</span></span>
- <span data-ttu-id="180e5-107">Одобравање на више нивоа које подржава привремене и коначне даваоце одобрења</span><span class="sxs-lookup"><span data-stu-id="180e5-107">Multi-level approval that supports interim approvers and a final approver</span></span>
- <span data-ttu-id="180e5-108">Финансијске димензије и пројектна одговорност</span><span class="sxs-lookup"><span data-stu-id="180e5-108">Financial dimensions and project responsibility</span></span>
- <span data-ttu-id="180e5-109">Додељивање одређеним корисницима или групама корисника</span><span class="sxs-lookup"><span data-stu-id="180e5-109">Assignment to specific users or user groups</span></span>

<span data-ttu-id="180e5-110">Одобравања токова посла могу се креирати за извештаје о трошковима, захтева за путовање, аконтације и повраћај пореза на додату вредност (ПДВ).</span><span class="sxs-lookup"><span data-stu-id="180e5-110">Workflow approvals can be created for expense reports, travel requisitions, cash advances, and value-added tax (VAT) recovery.</span></span>

<span data-ttu-id="180e5-111">**Пример**</span><span class="sxs-lookup"><span data-stu-id="180e5-111">**Example**</span></span>

<span data-ttu-id="180e5-112">Следећи поступак је пример тока посла за управљање трошковима за извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="180e5-112">The following process is an example of the expense management workflow for an expense report.</span></span>

1. <span data-ttu-id="180e5-113">Запослени креира и чува извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="180e5-113">An employee creates and saves an expense report.</span></span>
2. <span data-ttu-id="180e5-114">Запослени прослеђује извештај о трошковима на одобрење.</span><span class="sxs-lookup"><span data-stu-id="180e5-114">The employee submits the expense report for approval.</span></span> <span data-ttu-id="180e5-115">Давалац одобрења се идентификује на основу правила која су дефинисана приликом подешавања тока посла.</span><span class="sxs-lookup"><span data-stu-id="180e5-115">The approver is identified based on the rules that were defined when the workflow was set up.</span></span>
3. <span data-ttu-id="180e5-116">Давалац одобрења добија обавештење да је извештај о трошковима спреман за одобрење.</span><span class="sxs-lookup"><span data-stu-id="180e5-116">The approver receives a notification that an expense report is ready for approval.</span></span> <span data-ttu-id="180e5-117">Давалац одобрења прегледа извештај о трошковима и потврђује да су испуњени следећи услови:</span><span class="sxs-lookup"><span data-stu-id="180e5-117">The approver reviews the expense report and verifies that the following conditions are met:</span></span>

    - <span data-ttu-id="180e5-118">Трошкови не крше ниједну смерницу трошкова.</span><span class="sxs-lookup"><span data-stu-id="180e5-118">The expenses don't violate any expense policies.</span></span> <span data-ttu-id="180e5-119">Ако трошак крши смернице, давалац одобрења потврђује да извештај о трошковима садржи ваљано пословно оправдање.</span><span class="sxs-lookup"><span data-stu-id="180e5-119">If an expense violates a policy, the approver verifies that the expense report includes a valid business justification.</span></span>
    - <span data-ttu-id="180e5-120">Електронски рачуни су приложени извештају о трошковима.</span><span class="sxs-lookup"><span data-stu-id="180e5-120">Electronic receipts are attached to the expense report.</span></span>

4. <span data-ttu-id="180e5-121">Давалац одобрења одобрава извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="180e5-121">The approver approves the expense report.</span></span>
5. <span data-ttu-id="180e5-122">Извештај о трошковима додељује се координатору за дуговања на књижење.</span><span class="sxs-lookup"><span data-stu-id="180e5-122">The expense report is assigned to the Accounts payable coordinator for posting.</span></span>
6. <span data-ttu-id="180e5-123">Долази до једног од следећих корака, у зависности од тога да ли је конфигурисано аутоматско књижење:</span><span class="sxs-lookup"><span data-stu-id="180e5-123">One of the following steps occurs, depending on whether automatic posting is configured:</span></span>

    - <span data-ttu-id="180e5-124">Ако је конфигурисано аутоматско књижење, извештај о трошковима се обрађује за плаћање и ажурира се статус извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="180e5-124">If automatic posting is configured, the expense report is processed for payment, and the status of the expense report is updated.</span></span>
    - <span data-ttu-id="180e5-125">Ако аутоматско књижење није конфигурисано, координатор дуговања верификује да су предати сви оригинални рачуни и да су рачуни усклађени са трошковима у извештају о трошковима.</span><span class="sxs-lookup"><span data-stu-id="180e5-125">If automatic posting isn't configured, the Accounts payable coordinator verifies that all original receipts have been submitted, and that the receipts are aligned with the expenses on the expense report.</span></span> <span data-ttu-id="180e5-126">Све шифре пореза које су унете у извештај о трошковима такође морају бити верификоване као тачне.</span><span class="sxs-lookup"><span data-stu-id="180e5-126">All tax codes that are entered on the expense report must also be verified as correct.</span></span>

<span data-ttu-id="180e5-127">Након што се ови захтеви провере, извештај о трошковима се књижи.</span><span class="sxs-lookup"><span data-stu-id="180e5-127">After these requirements are verified, the expense report is posted.</span></span>

<span data-ttu-id="180e5-128">Након што се прокњижи извештај о трошковима, одобрава се плаћање за извештај о трошковима, а запосленом се надокнађује.</span><span class="sxs-lookup"><span data-stu-id="180e5-128">After the expense report is posted, payment is authorized for the expense report, and the employee is reimbursed.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]