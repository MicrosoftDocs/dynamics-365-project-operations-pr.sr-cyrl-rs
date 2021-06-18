---
title: Измена продајних ценовника за пројекат
description: Ова тема пружа информације о креирању прилагођених продајних ценовника.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: db2ff6acaad6ab4cbcc98d3d5b06b36ed23b758f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995099"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="92980-103">Измена продајних ценовника за пројекат</span><span class="sxs-lookup"><span data-stu-id="92980-103">Override project sales price lists</span></span>

<span data-ttu-id="92980-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="92980-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="92980-105">Ценовници пројеката специфични за клијента</span><span class="sxs-lookup"><span data-stu-id="92980-105">Customer-specific project price lists</span></span>

<span data-ttu-id="92980-106">Уговори о ценама специфични за клијента могу се поставити као ценовници пројеката у запису пословног контакта у услузи Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="92980-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="92980-107">Да бисте поставили ценовник пројеката специфичан за клијента, у области **Продаја**, дођите до записа о пословном контакту.</span><span class="sxs-lookup"><span data-stu-id="92980-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="92980-108">Отворите страницу листе **Пословни контакти**.</span><span class="sxs-lookup"><span data-stu-id="92980-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="92980-109">Пронађите и двапут кликните на запис клијента да бисте отворили страницу са детаљима о **пословном контакту**.</span><span class="sxs-lookup"><span data-stu-id="92980-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="92980-110">На картици **Ценовници пројекта** изаберите **+ Нови ценовник пројекта**.</span><span class="sxs-lookup"><span data-stu-id="92980-110">On the **Project Price lists** tab, select **+ New Project Price List**.</span></span>
4. <span data-ttu-id="92980-111">На страници **Нови ценовник пројекта**, из падајуће листе изаберите ценовник.</span><span class="sxs-lookup"><span data-stu-id="92980-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="92980-112">Укључени су само ценовници којима је контекст постављен на **Продаја** и чија валута се подудара са валутом пословног контакта.</span><span class="sxs-lookup"><span data-stu-id="92980-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="92980-113">Именујте повезивање, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="92980-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="92980-114">Креираће се ценовник пројекта специфичан за клијента.</span><span class="sxs-lookup"><span data-stu-id="92980-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="92980-115">Овај ценовник ће се користити за подразумеване цене за пројекат у понудама или уговорима за пројекат креираним за овог клијента када датум креирања понуде или уговора за пројекат спада у датум ефективности ценовника.</span><span class="sxs-lookup"><span data-stu-id="92980-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="92980-116">Прилагођено одређивање цена у понудама за пројекат</span><span class="sxs-lookup"><span data-stu-id="92980-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="92980-117">У понудама за пројекат, можете имати цене пројеката које почињу са подразумеваним стандардним ценовником који добија подразумеване вредности од клијента или из параметара пројекта.</span><span class="sxs-lookup"><span data-stu-id="92980-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="92980-118">Када вам је потребно прилагођено одређивање цена за посао у вези са пројектом за одређену понуду, то можете добити из ентитета повезаног са ценовницима пројеката.</span><span class="sxs-lookup"><span data-stu-id="92980-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="92980-119">Довршите следеће кораке да бисте поставили цене пројеката специфичне за понуду.</span><span class="sxs-lookup"><span data-stu-id="92980-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="92980-120">Отворите понуду за пројекат и изаберите картицу **Ценовници пројекта**.</span><span class="sxs-lookup"><span data-stu-id="92980-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="92980-121">У подформи изаберите **Креирај прилагођене цене**.</span><span class="sxs-lookup"><span data-stu-id="92980-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="92980-122">Сви ценовници пројекта који су приложени уз понуду копирају се у нове ценовнике.</span><span class="sxs-lookup"><span data-stu-id="92980-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="92980-123">Називи нових ценовника одражавају назив понуде са обележјем датума и времена када су ови ценовници креирани.</span><span class="sxs-lookup"><span data-stu-id="92980-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="92980-124">Можете да користите сваки од тих ценовника и ажурирате цене рада (цена улоге) и цене трошкова (цена категорије).</span><span class="sxs-lookup"><span data-stu-id="92980-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="92980-125">Ове цене ће се примењивати само на ову понуду за пројекат.</span><span class="sxs-lookup"><span data-stu-id="92980-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="92980-126">Ценовници у уговору за пројекат</span><span class="sxs-lookup"><span data-stu-id="92980-126">Price lists on a project contract</span></span>

<span data-ttu-id="92980-127">У уговору за пројекат, одређивање цена за пројекат се увек подразумева из прилагођеног ценовника са називом уговора и обележјем датума и времена креирања који се додаје називу.</span><span class="sxs-lookup"><span data-stu-id="92980-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="92980-128">То је тачно да ли је уговор креиран када је понуда добијена или је уговор креиран испочетка.</span><span class="sxs-lookup"><span data-stu-id="92980-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="92980-129">Ако је потребно, можете уклонити ово повезивање са прилагођеним ценовником и уместо тога придружити стандардни ценовник уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="92980-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="92980-130">Када стандардни ценовник придружите ценовницима пројекта у понуди или уговору, све промене цена у ценовнику утицаће на све понуде и уговоре који користе тај ценовник.</span><span class="sxs-lookup"><span data-stu-id="92980-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]