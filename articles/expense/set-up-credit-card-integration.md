---
title: Подешавање интеграције кредитне картице
description: Ова тема објашњава како се ради са трансакцијама кредитном картицом повезаним са трошковима.
author: suvaidya
manager: AnnBe
ms.date: 04/02/2021
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
ms.openlocfilehash: 72ff98f5985af4362cde3c9914e0d20247f1f09a
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/07/2021
ms.locfileid: "5866701"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="86c9c-103">Подешавање интеграције кредитне картице</span><span class="sxs-lookup"><span data-stu-id="86c9c-103">Set up credit card integration</span></span>

<span data-ttu-id="86c9c-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="86c9c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="86c9c-105">Трансакције повезане са трошковима кредитне картице могу се подесити тако да се аутоматски увозе по редовном распореду.</span><span class="sxs-lookup"><span data-stu-id="86c9c-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="86c9c-106">Осим тога, трансакције се могу ручно увести по потреби.</span><span class="sxs-lookup"><span data-stu-id="86c9c-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="86c9c-107">Трансакције кредитном картицом се увозе преко ентитета података трансакција кредитном картицом.</span><span class="sxs-lookup"><span data-stu-id="86c9c-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="86c9c-108">Увоз трансакција кредитном картицом</span><span class="sxs-lookup"><span data-stu-id="86c9c-108">Import credit card transactions</span></span>

<span data-ttu-id="86c9c-109">Да бисте увезли трансакције кредитном картицом, следите ове кораке:</span><span class="sxs-lookup"><span data-stu-id="86c9c-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="86c9c-110">На страници **Трансакције кредитним картицама** изаберите **Увези трансакције**.</span><span class="sxs-lookup"><span data-stu-id="86c9c-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="86c9c-111">Ако први пут отварате управљање подацима, систем мора да ажурира листу ентитета података пре него што можете да наставите.</span><span class="sxs-lookup"><span data-stu-id="86c9c-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="86c9c-112">У поље **Назив** унесите јединствени опис посла увоза.</span><span class="sxs-lookup"><span data-stu-id="86c9c-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="86c9c-113">У пољу **Формат изворних података** изаберите формат датотеке која садржи трансакције кредитном картицом за увоз.</span><span class="sxs-lookup"><span data-stu-id="86c9c-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="86c9c-114">Изаберите **Отпреми**, а затим пронађите и изаберите датотеку за увоз.</span><span class="sxs-lookup"><span data-stu-id="86c9c-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="86c9c-115">Када отпремите датотеку, потврдите мапирање датотеке трансакције кредитне картице и колоне ентитета података трансакција кредитном картицом избором везе **Прикажи мапу** на плочици.</span><span class="sxs-lookup"><span data-stu-id="86c9c-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="86c9c-116">Ако постоје грешке у мапирању или ако морате да промените мапирање, направите промене у мапирању са картице **Визуелизација мапирања** или **Детаљи мапирања**.</span><span class="sxs-lookup"><span data-stu-id="86c9c-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="86c9c-117">Да бисте аутоматизовали трансакције кредитном картицом, изаберите **Креирај периодичан посао са подацима**.</span><span class="sxs-lookup"><span data-stu-id="86c9c-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="86c9c-118">Затим можете подесити понављање које дефинише колико често треба увозити трансакције кредитним картицама.</span><span class="sxs-lookup"><span data-stu-id="86c9c-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="86c9c-119">Када завршите, изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="86c9c-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="86c9c-120">Да бисте сада увезли изабрану датотеку, изаберите **Увези**.</span><span class="sxs-lookup"><span data-stu-id="86c9c-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="86c9c-121">Ако се током увоза појаве грешке, можете прегледати евиденцију извршења или припремне податке да бисте видели грешке које морате исправити да бисте обезбедили успешан увоз.</span><span class="sxs-lookup"><span data-stu-id="86c9c-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="86c9c-122">Ако треба да увезете више од једног формата датотеке, морате креирати засебне послове увоза за сваки тип формата.</span><span class="sxs-lookup"><span data-stu-id="86c9c-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="86c9c-123">Поново доделите трансакције кредитном картицом отказаним запосленима</span><span class="sxs-lookup"><span data-stu-id="86c9c-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="86c9c-124">Након укидања евиденције запосленог, онемогућен је његов Active Directory Domain Services (AD DS) налог.</span><span class="sxs-lookup"><span data-stu-id="86c9c-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="86c9c-125">Међутим, можда постоје активне трансакције кредитним картицама које се и даље морају трошити и надокнадити.</span><span class="sxs-lookup"><span data-stu-id="86c9c-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="86c9c-126">На страници **Трансакције кредитним картицама** можете поново доделити запосленог за било коју трансакцију кредитном картицом у којој је повезани запослени прекинут.</span><span class="sxs-lookup"><span data-stu-id="86c9c-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="86c9c-127">Изаберите једну или више трансакција кредитном картицом, а затим изаберите **Поново доделите трансакције**.</span><span class="sxs-lookup"><span data-stu-id="86c9c-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="86c9c-128">Затим можете да изаберете другог запосленог коме ћете доделити трансакције кредитном картицом.</span><span class="sxs-lookup"><span data-stu-id="86c9c-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="86c9c-129">Након што се трансакције са кредитном картицом прераспореде, могу се одабрати за извештај о трошковима и платити кроз уобичајени поступак за накнаду трошкова.</span><span class="sxs-lookup"><span data-stu-id="86c9c-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="86c9c-130">Брисање трансакција кредитном картицом</span><span class="sxs-lookup"><span data-stu-id="86c9c-130">Delete credit card transactions</span></span> 

<span data-ttu-id="86c9c-131">Понекад, након увоза трансакција кредитном картицом, одређене трансакције можда треба избрисати.</span><span class="sxs-lookup"><span data-stu-id="86c9c-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="86c9c-132">То је можда зато што су трансакције дупликати или што подаци можда нису тачни.</span><span class="sxs-lookup"><span data-stu-id="86c9c-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="86c9c-133">Администратори могу да користе функцију **„Брисање трансакција кредитном картицом“** за одабир и брисање трансакција кредитном картицом које **нису приложене** на извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="86c9c-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="86c9c-134">Идите на страницу **Периодични задаци** > **Брисање трансакција кредитном картицом**.</span><span class="sxs-lookup"><span data-stu-id="86c9c-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="86c9c-135">Изаберите **Филтер** и наведите информације за идентификацију записа које треба укључити.</span><span class="sxs-lookup"><span data-stu-id="86c9c-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="86c9c-136">Изаберите **У реду** да бисте избрисали записе.</span><span class="sxs-lookup"><span data-stu-id="86c9c-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
