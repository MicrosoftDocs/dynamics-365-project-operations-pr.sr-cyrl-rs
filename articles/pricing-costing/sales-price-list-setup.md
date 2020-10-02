---
title: Подешавање продајног ценовника
description: Ова тема пружа информације о раду са продајним ценовницима за одређивање цена производа у пројекту.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2a66802adfcadab7b4d34149b146ca3cb27c903e
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896479"
---
# <a name="sales-price-list-setup"></a><span data-ttu-id="ba6b7-103">Подешавање продајног ценовника</span><span class="sxs-lookup"><span data-stu-id="ba6b7-103">Sales price list setup</span></span>

<span data-ttu-id="ba6b7-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="ba6b7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ba6b7-105">За пројектне понуде и уговоре, ценовник пројекта има различит образац за замену цена у односу на ценовник производа.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="ba6b7-106">У ставци понуде заснованој на каталогу производа можете да замените цену за улоге и категорије директно у ставци понуде, јер свака ставка понуде указује на тачно једну ставку каталога.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="ba6b7-107">Међутим, у ставци понуде заснованој на пројекту не можете да замените цену за улоге и категорије директно у ставци понуде.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="ba6b7-108">Ценовник пројеката можете користити за рад са два различита обрасца замене.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="ba6b7-109">Препоручујемо да имате посебан ценовник за ресурсе пројекта и ставке каталога, због разлика у понашању између њих када замените цене.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="ba6b7-110">Сваки од следећих ентитета може имати једну или више придружених ценовника продаје за цену пројеката:</span><span class="sxs-lookup"><span data-stu-id="ba6b7-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="ba6b7-111">Клијент (пословни контакт)</span><span class="sxs-lookup"><span data-stu-id="ba6b7-111">Customer (account)</span></span> 
- <span data-ttu-id="ba6b7-112">Могућност за пословање</span><span class="sxs-lookup"><span data-stu-id="ba6b7-112">Opportunity</span></span> 
- <span data-ttu-id="ba6b7-113">Понуда</span><span class="sxs-lookup"><span data-stu-id="ba6b7-113">Quote</span></span> 
- <span data-ttu-id="ba6b7-114">Уговор за пројекат</span><span class="sxs-lookup"><span data-stu-id="ba6b7-114">Project Contract</span></span>

<span data-ttu-id="ba6b7-115">Повезивање ових ентитета са ценовником је назначено ценовником пројекта.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="ba6b7-116">Можете да повежете неке ценовнике са ентитетима продаје Клијент, Могућност за пословање, Понуда и Уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="ba6b7-117">Подразумевани ценовник пројекта се не уноси аутоматски у запис клијента.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="ba6b7-118">Међутим, ценовник пројекта можете ручно приложити запису клијента.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="ba6b7-119">Ипак, требало би ручно да приложите ценовник пројекта само када имате прилагођени уговор о одређивању цена са клијентом.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="ba6b7-120">Када је ценовник пројекта приложен ентитету продаје, проверавају се следеће информације:</span><span class="sxs-lookup"><span data-stu-id="ba6b7-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="ba6b7-121">Да ли ценовник има контекст **продаје**.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="ba6b7-122">Да ли се валута ценовника подудара са валутом клијента.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="ba6b7-123">У уговору о пројекту се користи следећи редослед приоритета да би се аутоматски подесили повезани ценовници пројекта:</span><span class="sxs-lookup"><span data-stu-id="ba6b7-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="ba6b7-124">Понуда</span><span class="sxs-lookup"><span data-stu-id="ba6b7-124">Quote</span></span>
2. <span data-ttu-id="ba6b7-125">Могућност за пословање</span><span class="sxs-lookup"><span data-stu-id="ba6b7-125">Opportunity</span></span>
3. <span data-ttu-id="ba6b7-126">Клијент</span><span class="sxs-lookup"><span data-stu-id="ba6b7-126">Customer</span></span> 
4. <span data-ttu-id="ba6b7-127">Глобална подешавања</span><span class="sxs-lookup"><span data-stu-id="ba6b7-127">Global settings</span></span> 

<span data-ttu-id="ba6b7-128">Када се ценовник пројекта унесе подразумевано, систем проверава да ли се валута подудара са валутом клијента и да ли подразумевани ценовници који су унети имају контекст **продаје**.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="ba6b7-129">Можете да повежете више ценовника пројекта са ентитетима Клијент, Могућност за пословање, Понуда и Уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="ba6b7-130">Ова могућност подржава подразумеване цене за одређени датум за дугорочни уговор о пројекту, где можете да захтевате више од једног ценовника како бисте у обзир узели измене цена до којих долази због инфлације.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="ba6b7-131">Међутим, ако се за ценовнике које повежете са ентитетом Клијент, Могућност за пословање, Понуда или Уговор о пројекту преклапају датуми ступања на снагу, подразумеване цене могу бити нетачне.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="ba6b7-132">Због тога би требало да проверите да ценовници пројеката са датумима ступања на снагу који се преклапају нису повезани са тим ентитетима.</span><span class="sxs-lookup"><span data-stu-id="ba6b7-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
