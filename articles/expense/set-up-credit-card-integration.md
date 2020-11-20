---
title: Подешавање интеграције кредитне картице
description: Ова тема објашњава како да уведете и одржавате трансакције кредитне картице повезане са трошковима.
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
ms.openlocfilehash: e0004f9096ea8a03745dbfce35fe0d32d3d707f6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120876"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="b13f2-103">Подешавање интеграције кредитне картице</span><span class="sxs-lookup"><span data-stu-id="b13f2-103">Set up credit card integration</span></span>

<span data-ttu-id="b13f2-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="b13f2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b13f2-105">Трансакције повезане са трошковима кредитне картице могу се подесити тако да се аутоматски увозе по редовном распореду.</span><span class="sxs-lookup"><span data-stu-id="b13f2-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="b13f2-106">Осим тога, трансакције се могу ручно увести по потреби.</span><span class="sxs-lookup"><span data-stu-id="b13f2-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="b13f2-107">Трансакције кредитном картицом се увозе преко ентитета података трансакција кредитном картицом.</span><span class="sxs-lookup"><span data-stu-id="b13f2-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="b13f2-108">Увоз трансакција кредитном картицом</span><span class="sxs-lookup"><span data-stu-id="b13f2-108">Import credit card transactions</span></span>

1. <span data-ttu-id="b13f2-109">На страници **Трансакције кредитним картицама** изаберите **Увези трансакције**.</span><span class="sxs-lookup"><span data-stu-id="b13f2-109">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="b13f2-110">Ако први пут отварате управљање подацима, систем мора да ажурира листу ентитета података пре него што можете да наставите.</span><span class="sxs-lookup"><span data-stu-id="b13f2-110">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="b13f2-111">У пољу **Назив** унесите јединствени опис посла увоза.</span><span class="sxs-lookup"><span data-stu-id="b13f2-111">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="b13f2-112">У пољу **Формат изворних података** изаберите формат датотеке која садржи трансакције кредитном картицом за увоз.</span><span class="sxs-lookup"><span data-stu-id="b13f2-112">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="b13f2-113">Изаберите **Отпреми**, а затим пронађите и изаберите датотеку за увоз.</span><span class="sxs-lookup"><span data-stu-id="b13f2-113">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="b13f2-114">Након што је датотека отпремљена, потврдите мапирање датотеке трансакције кредитне картице и колона ентитета података трансакција кредитном картицом избором везе **Прикажи мапу** на плочици.</span><span class="sxs-lookup"><span data-stu-id="b13f2-114">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="b13f2-115">Ако постоје грешке у мапирању или ако морате да промените мапирање, направите промене у мапирању са картице **Визуелизација мапирања** или **Детаљи мапирања**.</span><span class="sxs-lookup"><span data-stu-id="b13f2-115">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="b13f2-116">Да бисте аутоматизовали трансакције кредитном картицом, изаберите **Креирај периодичан посао са подацима**.</span><span class="sxs-lookup"><span data-stu-id="b13f2-116">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="b13f2-117">Затим можете подесити понављање које дефинише колико често треба увозити трансакције кредитним картицама.</span><span class="sxs-lookup"><span data-stu-id="b13f2-117">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="b13f2-118">Када завршите, изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="b13f2-118">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="b13f2-119">Да бисте сада увезли изабрану датотеку, изаберите **Увези**.</span><span class="sxs-lookup"><span data-stu-id="b13f2-119">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="b13f2-120">Ако се током увоза појаве грешке, можете прегледати евиденцију извршења или податке о припреми да бисте видели грешке које морате исправити да бисте гарантовали успешан увоз.</span><span class="sxs-lookup"><span data-stu-id="b13f2-120">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="b13f2-121">Ако морате увести више од једног формата датотеке, морате створити засебне послове увоза за сваки тип формата.</span><span class="sxs-lookup"><span data-stu-id="b13f2-121">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="b13f2-122">Поново доделите трансакције кредитном картицом отказаним запосленима</span><span class="sxs-lookup"><span data-stu-id="b13f2-122">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="b13f2-123">Након укидања евиденције запосленог, онемогућен је његов Active Directory Domain Services (AD DS) налог.</span><span class="sxs-lookup"><span data-stu-id="b13f2-123">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="b13f2-124">Међутим, можда постоје активне трансакције кредитним картицама које се и даље морају трошити и надокнадити.</span><span class="sxs-lookup"><span data-stu-id="b13f2-124">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="b13f2-125">На страници **Трансакције кредитним картицама** можете доделити запосленог било којој трансакцији кредитном картицом за коју је повезани запослени укинут.</span><span class="sxs-lookup"><span data-stu-id="b13f2-125">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="b13f2-126">Изаберите једну или више трансакција кредитном картицом, а затим изаберите **Поново доделите трансакције**.</span><span class="sxs-lookup"><span data-stu-id="b13f2-126">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="b13f2-127">Затим можете да изаберете другог запосленог коме ћете доделити трансакције кредитном картицом.</span><span class="sxs-lookup"><span data-stu-id="b13f2-127">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="b13f2-128">Након што се трансакције са кредитном картицом прераспореде, могу се одабрати за извештај о трошковима и платити кроз уобичајени поступак за накнаду трошкова.</span><span class="sxs-lookup"><span data-stu-id="b13f2-128">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>
