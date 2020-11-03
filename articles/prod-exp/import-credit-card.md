---
title: Увоз и одржавање трансакција кредитним картицама
description: Ова тема објашњава како да уведете и одржавате трансакције кредитне картице повезане са трошковима. Ове трансакције се могу подесити тако да се аутоматски увозе по редовном распореду или се могу ручно увести по потреби.
author: KimANelson
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: 6cec15e436bc699e361577c970dd5845c6c68908
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084125"
---
# <a name="import-and-maintain-credit-card-transactions"></a><span data-ttu-id="8e231-104">Увоз и одржавање трансакција кредитним картицама</span><span class="sxs-lookup"><span data-stu-id="8e231-104">Import and maintain credit card transactions</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="8e231-105">Трансакције повезане са трошковима кредитне картице могу се подесити тако да се аутоматски увозе по редовном распореду.</span><span class="sxs-lookup"><span data-stu-id="8e231-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="8e231-106">Осим тога, трансакције се могу ручно увести по потреби.</span><span class="sxs-lookup"><span data-stu-id="8e231-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="8e231-107">Трансакције кредитном картицом се увозе преко ентитета података трансакција кредитном картицом.</span><span class="sxs-lookup"><span data-stu-id="8e231-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

<span data-ttu-id="8e231-108">За више информација о ентитетима података погледајте [Ентитети података](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span><span class="sxs-lookup"><span data-stu-id="8e231-108">For more information about data entities, see [Data entities](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="8e231-109">Увоз трансакција кредитном картицом</span><span class="sxs-lookup"><span data-stu-id="8e231-109">Import credit card transactions</span></span>

1. <span data-ttu-id="8e231-110">На страници **Трансакције кредитним картицама** изаберите **Увези трансакције**.</span><span class="sxs-lookup"><span data-stu-id="8e231-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="8e231-111">Ако први пут отварате управљање подацима, систем мора да ажурира листу ентитета података пре него што можете да наставите.</span><span class="sxs-lookup"><span data-stu-id="8e231-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="8e231-112">У пољу **Назив** унесите јединствени опис посла увоза.</span><span class="sxs-lookup"><span data-stu-id="8e231-112">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="8e231-113">У пољу **Формат изворних података** изаберите формат датотеке која садржи трансакције кредитном картицом за увоз.</span><span class="sxs-lookup"><span data-stu-id="8e231-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="8e231-114">Изаберите **Отпреми** , а затим пронађите и изаберите датотеку за увоз.</span><span class="sxs-lookup"><span data-stu-id="8e231-114">Select **Upload** , and then find and select the file to import.</span></span>
5. <span data-ttu-id="8e231-115">Након што је датотека отпремљена, потврдите мапирање датотеке трансакције кредитне картице и колона ентитета података трансакција кредитном картицом избором везе **Прикажи мапу** на плочици.</span><span class="sxs-lookup"><span data-stu-id="8e231-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="8e231-116">Ако постоје грешке у мапирању или ако морате да промените мапирање, направите промене у мапирању са картице **Визуелизација мапирања** или **Детаљи мапирања**.</span><span class="sxs-lookup"><span data-stu-id="8e231-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="8e231-117">Да бисте аутоматизовали трансакције кредитном картицом, изаберите **Креирај периодичан посао са подацима**.</span><span class="sxs-lookup"><span data-stu-id="8e231-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="8e231-118">Затим можете подесити понављање које дефинише колико често треба увозити трансакције кредитним картицама.</span><span class="sxs-lookup"><span data-stu-id="8e231-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="8e231-119">Када завршите, изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="8e231-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="8e231-120">Да бисте сада увезли изабрану датотеку, изаберите **Увези**.</span><span class="sxs-lookup"><span data-stu-id="8e231-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="8e231-121">Ако се током увоза појаве грешке, можете прегледати евиденцију извршења или податке о припреми да бисте видели грешке које морате исправити да бисте гарантовали успешан увоз.</span><span class="sxs-lookup"><span data-stu-id="8e231-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="8e231-122">Ако морате увести више од једног формата датотеке, морате створити засебне послове увоза за сваки тип формата.</span><span class="sxs-lookup"><span data-stu-id="8e231-122">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="8e231-123">Поново доделите трансакције кредитном картицом отказаним запосленима</span><span class="sxs-lookup"><span data-stu-id="8e231-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="8e231-124">Након укидања евиденције запосленог, онемогућен је његов Active Directory Domain Services (AD DS) налог.</span><span class="sxs-lookup"><span data-stu-id="8e231-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="8e231-125">Међутим, можда постоје активне трансакције кредитним картицама које се и даље морају трошити и надокнадити.</span><span class="sxs-lookup"><span data-stu-id="8e231-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="8e231-126">На страници **Трансакције кредитним картицама** можете доделити запосленог било којој трансакцији кредитном картицом за коју је повезани запослени укинут.</span><span class="sxs-lookup"><span data-stu-id="8e231-126">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="8e231-127">Изаберите једну или више трансакција кредитном картицом, а затим изаберите **Поново доделите трансакције**.</span><span class="sxs-lookup"><span data-stu-id="8e231-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="8e231-128">Затим можете да изаберете другог запосленог коме ћете доделити трансакције кредитном картицом.</span><span class="sxs-lookup"><span data-stu-id="8e231-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="8e231-129">Након што се трансакције са кредитном картицом прераспореде, могу се одабрати за извештај о трошковима и платити кроз уобичајени поступак за надокнаду трошкова.</span><span class="sxs-lookup"><span data-stu-id="8e231-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>
