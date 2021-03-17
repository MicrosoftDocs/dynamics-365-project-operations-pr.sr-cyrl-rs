---
title: Креирање ад-хок авансне уплате за уговор
description: Ова тема пружа информације о креирању аванса за уговор по потреби.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2f0a6391a3bf6dd39d21504a6f286e4ff1954183
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273615"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract"></a><span data-ttu-id="618d2-103">Креирање ад-хок авансне уплате за уговор</span><span class="sxs-lookup"><span data-stu-id="618d2-103">Creating an ad hoc advance on a contract</span></span>

<span data-ttu-id="618d2-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="618d2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="618d2-105">Microsoft Dynamics 365 Project Operations подржава сценарије фактурисања који укључују претплату и авансе.</span><span class="sxs-lookup"><span data-stu-id="618d2-105">Microsoft Dynamics 365 Project Operations supports invoicing scenarios that involve pre-payments and advances.</span></span> <span data-ttu-id="618d2-106">Процес коришћења **Аванса** у услузи **Project Operations** је сличан **авансним** уговорима.</span><span class="sxs-lookup"><span data-stu-id="618d2-106">The process for using **Advances** in **Project Operations** is similar to **Retainer** contracts.</span></span> 

<span data-ttu-id="618d2-107">Довршите следеће кораке да бисте клијенту фактурисали аванс.</span><span class="sxs-lookup"><span data-stu-id="618d2-107">Complete the following steps to invoice the customer for an advance.</span></span>

1. <span data-ttu-id="618d2-108">Идите на страницу **Уговор за пројекат**, а затим изаберите картицу **Аконтације и аванси**.</span><span class="sxs-lookup"><span data-stu-id="618d2-108">Go to the **Project Contract** page, and then select the **Advances and Retainers** tab.</span></span>
2. <span data-ttu-id="618d2-109">У подформи која садржи списак свих претходно забележених аванса и авансних плаћања, изаберите **+ Аванс на уговор за нови пројекат**.</span><span class="sxs-lookup"><span data-stu-id="618d2-109">In the subgrid that lists all the previously recorded advances and prepayments, select **+ New Project contract retainer**.</span></span> 

    <span data-ttu-id="618d2-110">Отвориће се образац **Брзо креирање** за евидентирање претплате или аванса.</span><span class="sxs-lookup"><span data-stu-id="618d2-110">The **Quick Create** form opens for recording a prepayment or advance.</span></span>
    
3. <span data-ttu-id="618d2-111">У табели у наставку наведена су поља за бележење аванса и разматрања која треба имати на уму приликом креирања нових:</span><span class="sxs-lookup"><span data-stu-id="618d2-111">The table below lists the fields for recording an advance and the considerations to keep in mind as you create new ones:</span></span>

    | <span data-ttu-id="618d2-112">Поље</span><span class="sxs-lookup"><span data-stu-id="618d2-112">Field</span></span> | <span data-ttu-id="618d2-113">Опис</span><span class="sxs-lookup"><span data-stu-id="618d2-113">Description</span></span> | <span data-ttu-id="618d2-114">Последични утицај</span><span class="sxs-lookup"><span data-stu-id="618d2-114">Downstream impact</span></span> |
    | --- | --- | --- |
    | <span data-ttu-id="618d2-115">**Клијент уговора за пројекат**</span><span class="sxs-lookup"><span data-stu-id="618d2-115">**Project Contract Customer**</span></span> | <span data-ttu-id="618d2-116">Ово поље означава којем клијенту на уговору ће се фактурисати за ову аконтацију.</span><span class="sxs-lookup"><span data-stu-id="618d2-116">This field indicates which customer on the contract will be invoiced for this advance.</span></span> | <span data-ttu-id="618d2-117">Ако имате више клијената на уговору и желите да фактуришете сваком од њих за одређену аконтацију или авансни износ, ручно креирајте аванс за сваког клијента понаособ.</span><span class="sxs-lookup"><span data-stu-id="618d2-117">If you have multiple customers on the contract and want to invoice each of them for a specific retainer or advance amount, create an advance for each customer individually.</span></span> |
    | <span data-ttu-id="618d2-118">**Опис**</span><span class="sxs-lookup"><span data-stu-id="618d2-118">**Description**</span></span> | <span data-ttu-id="618d2-119">Опис сврхе или времена аванса који ће вам помоћи да га идентификујете.</span><span class="sxs-lookup"><span data-stu-id="618d2-119">The description of the purpose or timing of the advance to help identify this advance.</span></span> | <span data-ttu-id="618d2-120">Овај опис се приказује у ставки фактуре за овај аванс.</span><span class="sxs-lookup"><span data-stu-id="618d2-120">This description is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="618d2-121">**Износ**</span><span class="sxs-lookup"><span data-stu-id="618d2-121">**Amount**</span></span> | <span data-ttu-id="618d2-122">Износ претплате или аванса.</span><span class="sxs-lookup"><span data-stu-id="618d2-122">The amount for the pre-payment or advance.</span></span> | <span data-ttu-id="618d2-123">Овај износ се приказује у ставки фактуре за овај аванс.</span><span class="sxs-lookup"><span data-stu-id="618d2-123">This amount is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="618d2-124">**Датум фактуре**</span><span class="sxs-lookup"><span data-stu-id="618d2-124">**Invoice Date**</span></span> | <span data-ttu-id="618d2-125">Датум на који се клијенту фактурише овај аванс.</span><span class="sxs-lookup"><span data-stu-id="618d2-125">The date on which this advance is invoiced to the customer.</span></span> | <span data-ttu-id="618d2-126">Ово је датум за поступак аутоматског креирања фактуре за креирање ставке фактуре за овај аванс.</span><span class="sxs-lookup"><span data-stu-id="618d2-126">This is the date for the automated invoice creation process to create an invoice line for this advance.</span></span> |
    | <span data-ttu-id="618d2-127">**Статус фактуре**</span><span class="sxs-lookup"><span data-stu-id="618d2-127">**Invoice Status**</span></span> | <span data-ttu-id="618d2-128">Ово је подешавање опције које показује да ли је овај аванс додат радној верзији фактуре за овог клијента.</span><span class="sxs-lookup"><span data-stu-id="618d2-128">This is an option setting that indicates whether this advance is added to a draft invoice for this customer.</span></span> <span data-ttu-id="618d2-129">Могуће вредности су следеће:</span><span class="sxs-lookup"><span data-stu-id="618d2-129">The possible values are:</span></span></br><span data-ttu-id="618d2-130">- **Није спремно за фактурисање**</span><span class="sxs-lookup"><span data-stu-id="618d2-130">- **Not ready to invoice**</span></span></br><span data-ttu-id="618d2-131">- **Спремно за фактурисање**</span><span class="sxs-lookup"><span data-stu-id="618d2-131">- **Ready to invoice**</span></span> | <span data-ttu-id="618d2-132">Када се аванс или претплата означи као **Спремно за фактурисање**, додаје се као време ставке на радној верзији фактуре.</span><span class="sxs-lookup"><span data-stu-id="618d2-132">When an advance or pre-payment is marked as **Ready to invoice**, it is added as a line time on a draft invoice.</span></span> <span data-ttu-id="618d2-133">Само потпуно фактурисани аванс се може користити за усаглашавање са пројектним трошковима за следећи период фактурисања.</span><span class="sxs-lookup"><span data-stu-id="618d2-133">Only a fully invoiced advance can be used to reconcile against project costs for the next invoice period.</span></span> |

4. <span data-ttu-id="618d2-134">Изаберите **Сачувај и затвори** у дијалогу за брзо креирање за бележење аванса или претплате.</span><span class="sxs-lookup"><span data-stu-id="618d2-134">Select **Save and close** on the quick create dialog to record the advance or the pre-payment.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]