---
title: Зашто се цена подразумевано враћа на нулу у стварним подацима о цени за утрошено време?
description: Решавање проблема због чега се цена подразумевано враћа на 0 у стварним подацима о цени за утрошено време.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: ffe915a48f088bde457121a323325ba490c24e45
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993074"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a><span data-ttu-id="6456f-103">Зашто се цена подразумевано враћа на нулу у стварним подацима о цени за утрошено време?</span><span class="sxs-lookup"><span data-stu-id="6456f-103">Why is the price defaulting to zero on time cost actuals?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="6456f-104">Ова најчешћа питања се односе на стварне податке где је класа трансакције подешена на Време, а где је врста трансакције Трошак.</span><span class="sxs-lookup"><span data-stu-id="6456f-104">This FAQ applies to actuals where the transaction class is set to Time and transaction type is Cost.</span></span> <span data-ttu-id="6456f-105">Следе три провере које ће вам олакшати да решите због чега се цена подразумевано враћа на вредност 0 у стварним подацима о цени за утрошено време.</span><span class="sxs-lookup"><span data-stu-id="6456f-105">The following three checks will help you troubleshoot why the price is defaulting to 0 on time cost actuals.</span></span>
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a><span data-ttu-id="6456f-106">Провера 1: Идентификујте ценовник коштања за пројекат</span><span class="sxs-lookup"><span data-stu-id="6456f-106">Check 1: Identify the cost price list for the project</span></span>

<span data-ttu-id="6456f-107">Пронађите пројекат из поља Пројекат за стварни податак, а затим идите на страницу пројекта.</span><span class="sxs-lookup"><span data-stu-id="6456f-107">Find the project from the project field of the actual and then go to the project page.</span></span> <span data-ttu-id="6456f-108">Кликните на везу јединице уговарања у пољу.</span><span class="sxs-lookup"><span data-stu-id="6456f-108">Click on the contracting unit link in the field.</span></span> <span data-ttu-id="6456f-109">На страници Јединица уговарања проверите да ли јединица уговарања има ценовник у мрежи Ценовници коштања.</span><span class="sxs-lookup"><span data-stu-id="6456f-109">On the Contracting Unit page, check if the contracting unit has a price list in the Cost Price Lists grid.</span></span>

<span data-ttu-id="6456f-110">Ако постоји више од једног ценовника, изоловали сте проблем.</span><span class="sxs-lookup"><span data-stu-id="6456f-110">If there is more than one price list, you have isolated the problem.</span></span> <span data-ttu-id="6456f-111">Project Service подржава само један ценовник по организационој јединици.</span><span class="sxs-lookup"><span data-stu-id="6456f-111">Project Service only supports one price list per organizational unit.</span></span> <span data-ttu-id="6456f-112">Уклоните све ценовнике из овог ентитета све док не остане само један приложен ценовник у мрежи Ценовници коштања за организациону јединицу.</span><span class="sxs-lookup"><span data-stu-id="6456f-112">Remove all prices lists from this entity until there is only one price list attached in the Cost Price Lists grid of the Organizational Unit.</span></span>

<span data-ttu-id="6456f-113">Ако организационој јединици није приложен ниједан ценовник, забележите валуту организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="6456f-113">If there are no price lists attached to the Organizational Unit, make a note of the currency of the Organizational unit.</span></span> <span data-ttu-id="6456f-114">Идите у Project Service, а затим на ставку Параметри и отворите картицу Ценовници. Проверите да ли постоје ценовници чији је контекст подешен на Цена, а да се валута подудара са валутом организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="6456f-114">Go to the Project Service and then Parameters and open the Price Lists tab. Check if there are any price lists with context set to Cost and currency that matches the currency of the Organizational Unit.</span></span>
 
<span data-ttu-id="6456f-115">Ако не постоје ценовници који испуњавају критеријуме, изоловали сте проблем.</span><span class="sxs-lookup"><span data-stu-id="6456f-115">If there are no price lists that match that criteria, you have isolated the problem.</span></span> <span data-ttu-id="6456f-116">Уверите се да имате бар један ценовник чији је контекст подешен на Цена и чија се валута подудара са валутом организационе јединице.</span><span class="sxs-lookup"><span data-stu-id="6456f-116">Make sure to have at least one price list whose context is set to Cost and whose currency matches the currency of the Organizational Unit.</span></span>

<span data-ttu-id="6456f-117">Ако постоји више ценовника који испуњавају критеријуме, наставите са читањем овог документа како бисте обавили додатне провере.</span><span class="sxs-lookup"><span data-stu-id="6456f-117">If there is more than one price list that match that criteria, continue reading this document to make more checks.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a><span data-ttu-id="6456f-118">Провера 2: Да ли је било који од ценовника идентификованих изнад важећи за одређени датум стварног податка о цени за утрошено време?</span><span class="sxs-lookup"><span data-stu-id="6456f-118">Check 2: Are any of the price lists identified above valid for the specific date of the time cost actual?</span></span>

<span data-ttu-id="6456f-119">Да би Project Service размотрио ценовник за подразумевану цену, тај ценовник треба да буде примењив за датум на стварном податку о цени за утрошено време.</span><span class="sxs-lookup"><span data-stu-id="6456f-119">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the time cost actual.</span></span> <span data-ttu-id="6456f-120">Проверите следеће да бисте проверили да ли су ценовници идентификовани изнад примењиви:</span><span class="sxs-lookup"><span data-stu-id="6456f-120">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="6456f-121">Проверите да ли су датуми почетка и завршетка на картици Општи подаци за приложене ценовнике празни.</span><span class="sxs-lookup"><span data-stu-id="6456f-121">Check if the start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="6456f-122">Ако су датуми почетка и завршетка на ценовницима идентификованим горе празни, изоловали сте проблем.</span><span class="sxs-lookup"><span data-stu-id="6456f-122">If the start and end dates on price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="6456f-123">Забележите поље датума почетка на стварном податку о цени за утрошено време и проверите да ли је неки од идентификованих ценовника примењив за тај датум.</span><span class="sxs-lookup"><span data-stu-id="6456f-123">Make a note of the start date field on your time cost actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="6456f-124">На пример, датум стварног податка о цени за утрошено време би требало да пада унутар датума почетка и завршетка у ценовнику.</span><span class="sxs-lookup"><span data-stu-id="6456f-124">For example, the date of the time cost actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="6456f-125">Ако не постоји ниједан ценовник који покрива тај датум на стварном податку о цени за утрошено време, изоловали сте проблем.</span><span class="sxs-lookup"><span data-stu-id="6456f-125">If there is no price list that covers that date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="6456f-126">Измените датуме почетка и завршетка за ценовник да бисте осигурали да ценовник покрива датум стварног податка о цени за утрошено време.</span><span class="sxs-lookup"><span data-stu-id="6456f-126">Modify the start and end dates of the price list to ensure that the price list covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="6456f-127">Ако постоји више ценовника који покривају тај датум на стварном податку о цени за утрошено време, изоловали сте проблем.</span><span class="sxs-lookup"><span data-stu-id="6456f-127">If there is more than one price list that covers the date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="6456f-128">Ово можете да исправите уређивањем датума почетка и завршетка ценовника, тако да постоји само један ценовник који покрива датум стварног податка о цени за утрошено време.</span><span class="sxs-lookup"><span data-stu-id="6456f-128">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="6456f-129">Ако постоји само један ценовник који покрива датум стварног податка о цени за утрошено време, пређите на следећу проверу у документу.</span><span class="sxs-lookup"><span data-stu-id="6456f-129">If there is only one price list that covers that date of the time cost actual, move to the next check in the document.</span></span>
<span data-ttu-id="6456f-130">Након што сте обавили потребне поправке, поново креирајте унос утрошеног времена, одобрите га и потврдите да стварни податак о цени за утрошено време приказује важећу цену.</span><span class="sxs-lookup"><span data-stu-id="6456f-130">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a><span data-ttu-id="6456f-131">Проверите 3: Да ли постоји цена у ценовнику за димензије формирања цене на стварној податку о цени за утрошено време?</span><span class="sxs-lookup"><span data-stu-id="6456f-131">Check 3: Is there a price in the price list for the pricing dimensions on the time cost actual?</span></span>

<span data-ttu-id="6456f-132">Ако сте успешно довршили проверу 1 и проверу 2, требало би сада да имате само један ценовник који је применљив за датум стварног податка о цени за утрошено време.</span><span class="sxs-lookup"><span data-stu-id="6456f-132">If you have successfully completed Check 1 and Check 2, you should now have only one price list that is applicable for the date of the time cost actual.</span></span> <span data-ttu-id="6456f-133">Отворите овај ценовник и идите до картице Цене улога. Уверите се да постоји ред у мрежи за димензије образовања цена у стварном податку о цени за утрошено време.</span><span class="sxs-lookup"><span data-stu-id="6456f-133">Open this Price List and go to the Role Prices tab. Make sure that there is a row in the grid for the pricing dimensions on the time cost actual.</span></span>

<span data-ttu-id="6456f-134">Ако у мрежи улоге цене не постоји ред за димензије образовања цене на стварном податку о цени за утрошено време, онда сте изоловали проблем.</span><span class="sxs-lookup"><span data-stu-id="6456f-134">If there is no row in the role price grid for the pricing dimensions on the time cost actual, then you have isolated the problem.</span></span> <span data-ttu-id="6456f-135">Креирајте ред у мрежи Цене улога за димензије одређивања цена на стварном податку о цени за утрошено време.</span><span class="sxs-lookup"><span data-stu-id="6456f-135">Create a row in the Role prices grid for the pricing dimensions on your time cost actual.</span></span> <span data-ttu-id="6456f-136">Након што то урадите, поново креирајте унос утрошеног времена, одобрите га и потврдите да стварни податак о цени за утрошено време приказује важећу цену.</span><span class="sxs-lookup"><span data-stu-id="6456f-136">Once this is done, recreate time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>
 
<span data-ttu-id="6456f-137">Ако и даље не видите важећу цену у стварном податку о цени за утрошено време након што обавите горенаведене три провере, пошаљите тикет подршци.</span><span class="sxs-lookup"><span data-stu-id="6456f-137">If you still don't see a valid price on your time cost actual after you’ve done the three checks above, please log a support ticket.</span></span>





[!INCLUDE[footer-include](../includes/footer-banner.md)]