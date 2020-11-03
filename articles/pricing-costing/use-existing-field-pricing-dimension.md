---
title: Project Operations поља као димензија за одређивање цена
description: Ова тема пружа информације о коришћењу постојећих поља као димензија за одређивање цена у услузи Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 56ff45169058d96d7ef81a710de309eec698a75f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084035"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="34a65-103">Project Operations поља као димензија за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="34a65-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="34a65-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="34a65-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="34a65-105">Ентитет **Стварне вредности** има много поља која се могу користити као димензије за одређивања цена за цене засноване на ресурсима.</span><span class="sxs-lookup"><span data-stu-id="34a65-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="34a65-106">На пример, једно уобичајено поље је **Ресурс који се може резервисати**.</span><span class="sxs-lookup"><span data-stu-id="34a65-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="34a65-107">Мања предузећа са мање од 20-30 наплативих ресурса могу да открију да је једноставнији приступ ако имају стопе наплате и трошкова специфичне за сваки ресурс.</span><span class="sxs-lookup"><span data-stu-id="34a65-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="34a65-108">Међутим, како расте наплатива радна снага, одржавање стопа сецифичних ресурса може постати нереално.</span><span class="sxs-lookup"><span data-stu-id="34a65-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="34a65-109">Цена ресурса и стопе наплате почињу да се разликују како се ресурси унапређују, стичу више искуства или како усвајају другачији скуп вештина.</span><span class="sxs-lookup"><span data-stu-id="34a65-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="34a65-110">Други пример је категорија трансакције.</span><span class="sxs-lookup"><span data-stu-id="34a65-110">Another example is that of transaction category.</span></span> <span data-ttu-id="34a65-111">Клијенти и примењивачи су користили категорију трансакције да би класификовали посао и помоћу поља одређују цену и трошкове на основу категорије посла.</span><span class="sxs-lookup"><span data-stu-id="34a65-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>
