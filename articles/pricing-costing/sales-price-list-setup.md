---
title: Подешавање продајног ценовника
description: Ова тема пружа информације о раду са продајним ценовницима за одређивање цена производа у пројекту.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: eb8dfa61a2d17ba644daf1552889cbcde0f1e47a
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176269"
---
# <a name="set-up-a-sales-price-list"></a><span data-ttu-id="e5669-103">Подешавање продајног ценовника</span><span class="sxs-lookup"><span data-stu-id="e5669-103">Set up a sales price list</span></span>

<span data-ttu-id="e5669-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="e5669-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e5669-105">За пројектне понуде и уговоре, ценовник пројекта има различит образац за замену цена у односу на ценовник производа.</span><span class="sxs-lookup"><span data-stu-id="e5669-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="e5669-106">У ставци понуде заснованој на каталогу производа можете да замените цену за улоге и категорије директно у ставци понуде, јер свака ставка понуде указује на тачно једну ставку каталога.</span><span class="sxs-lookup"><span data-stu-id="e5669-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="e5669-107">Међутим, у ставци понуде заснованој на пројекту не можете да замените цену за улоге и категорије директно у ставци понуде.</span><span class="sxs-lookup"><span data-stu-id="e5669-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="e5669-108">Ценовник пројеката можете користити за рад са два различита обрасца замене.</span><span class="sxs-lookup"><span data-stu-id="e5669-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="e5669-109">Препоручујемо да имате посебан ценовник за ресурсе пројекта и ставке каталога, због разлика у понашању између њих када замените цене.</span><span class="sxs-lookup"><span data-stu-id="e5669-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="e5669-110">Сваки од следећих ентитета може имати једну или више придружених ценовника продаје за цену пројеката:</span><span class="sxs-lookup"><span data-stu-id="e5669-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="e5669-111">Клијент (пословни контакт)</span><span class="sxs-lookup"><span data-stu-id="e5669-111">Customer (account)</span></span> 
- <span data-ttu-id="e5669-112">Могућност за пословање</span><span class="sxs-lookup"><span data-stu-id="e5669-112">Opportunity</span></span> 
- <span data-ttu-id="e5669-113">Понуда</span><span class="sxs-lookup"><span data-stu-id="e5669-113">Quote</span></span> 
- <span data-ttu-id="e5669-114">Уговор за пројекат</span><span class="sxs-lookup"><span data-stu-id="e5669-114">Project Contract</span></span>

<span data-ttu-id="e5669-115">Повезивање ових ентитета са ценовником је назначено ценовником пројекта.</span><span class="sxs-lookup"><span data-stu-id="e5669-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="e5669-116">Можете да повежете неке ценовнике са ентитетима продаје Клијент, Могућност за пословање, Понуда и Уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="e5669-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="e5669-117">Подразумевани ценовник пројекта се не уноси аутоматски у запис клијента.</span><span class="sxs-lookup"><span data-stu-id="e5669-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="e5669-118">Међутим, ценовник пројекта можете ручно приложити запису клијента.</span><span class="sxs-lookup"><span data-stu-id="e5669-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="e5669-119">Ипак, требало би ручно да приложите ценовник пројекта само када имате прилагођени уговор о одређивању цена са клијентом.</span><span class="sxs-lookup"><span data-stu-id="e5669-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="e5669-120">Када је ценовник пројекта приложен ентитету продаје, проверавају се следеће информације:</span><span class="sxs-lookup"><span data-stu-id="e5669-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="e5669-121">Да ли ценовник има контекст **продаје**.</span><span class="sxs-lookup"><span data-stu-id="e5669-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="e5669-122">Да ли се валута ценовника подудара са валутом клијента.</span><span class="sxs-lookup"><span data-stu-id="e5669-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="e5669-123">У уговору о пројекту се користи следећи редослед приоритета да би се аутоматски подесили повезани ценовници пројекта:</span><span class="sxs-lookup"><span data-stu-id="e5669-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="e5669-124">Понуда</span><span class="sxs-lookup"><span data-stu-id="e5669-124">Quote</span></span>
2. <span data-ttu-id="e5669-125">Могућност за пословање</span><span class="sxs-lookup"><span data-stu-id="e5669-125">Opportunity</span></span>
3. <span data-ttu-id="e5669-126">Клијент</span><span class="sxs-lookup"><span data-stu-id="e5669-126">Customer</span></span> 
4. <span data-ttu-id="e5669-127">Глобална подешавања</span><span class="sxs-lookup"><span data-stu-id="e5669-127">Global settings</span></span> 

<span data-ttu-id="e5669-128">Када се ценовник пројекта унесе подразумевано, систем проверава да ли се валута подудара са валутом клијента и да ли подразумевани ценовници који су унети имају контекст **продаје**.</span><span class="sxs-lookup"><span data-stu-id="e5669-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="e5669-129">Можете да повежете више ценовника пројекта са ентитетима Клијент, Могућност за пословање, Понуда и Уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="e5669-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="e5669-130">Ова могућност подржава подразумеване цене за одређени датум за дугорочни уговор о пројекту, где можете да захтевате више од једног ценовника како бисте у обзир узели измене цена до којих долази због инфлације.</span><span class="sxs-lookup"><span data-stu-id="e5669-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="e5669-131">Међутим, ако се за ценовнике које повежете са ентитетом Клијент, Могућност за пословање, Понуда или Уговор о пројекту преклапају датуми ступања на снагу, подразумеване цене могу бити нетачне.</span><span class="sxs-lookup"><span data-stu-id="e5669-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="e5669-132">Због тога би требало да проверите да ценовници пројеката са датумима ступања на снагу који се преклапају нису повезани са тим ентитетима.</span><span class="sxs-lookup"><span data-stu-id="e5669-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
