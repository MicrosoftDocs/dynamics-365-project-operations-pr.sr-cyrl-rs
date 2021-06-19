---
title: Преглед интерног фактурисања у оквиру предузећа
description: Ова тема пружа информације и примере о интерном фактурисању између предузећа за пројекте.
author: sigitac
ms.date: 11/19/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42af89105f8325f1c94df6d2133d2c329facf2b3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002659"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="dbbe8-103">Преглед интерног фактурисања у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="dbbe8-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="dbbe8-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="dbbe8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="dbbe8-105">Ваша организација може имати више одељења, подружница и других правних лица која међусобно преносе производе и услуге за пројекте.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="dbbe8-106">Правно лице које пружа услугу или даје производ назива се *правно лице које позајмљује*.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="dbbe8-107">Правно лице које прима услугу или производ назива се *правно лице које се задужује*.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="dbbe8-108">Следећа илустрација приказује типичан сценарио када два правна лица, Contoso Robotics USA (правно лице које се задужује) и Contoso Robotics UK (правно лице које позајмљује) дели ресурсе за испоруку пројекта за клијента, Adventure works.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="dbbe8-109">За овај сценарио, Contoso Robotics USA је уговорио испоруку дела за Adventure Works.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![Интерно фактурисање у оквиру предузећа](./media/IntercompanyScenario.png) 

<span data-ttu-id="dbbe8-111">Dynamics 365 Project Operations користи следећи ток за обраду трансакција између предузећа:</span><span class="sxs-lookup"><span data-stu-id="dbbe8-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="dbbe8-112">Ресурси правног лица које даје позајмице евидентирају трансакције времена или трошкова између предузећа према времену и трошку резервације у основу на пројекте правног лица које се задужује.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="dbbe8-113">Трошкови времена и трошкова евидентирају се у предузећу које позајмљује коришћењем јединичног ценовника трошкова предузећа које се задужује.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="dbbe8-114">Ненаплаћене продајне трансакције између предузећа евидентирају се у компанији која позајмљује коришћењем јединичног ценовника трошкова предузећа које се задужује.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="dbbe8-115">Нефактурисани приход се евидентира у предузећу које се задужује користећи ценовник продајних цена по уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="dbbe8-116">Клијенту можете наплатити када се евидентира нефактурисани приход.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="dbbe8-117">Клијент не мора да чека док се обрада фактура између предузећа не заврши.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="dbbe8-118">Фактуре клијената између предузећа се креирају периодично у предузећу које позајмљује.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="dbbe8-119">Фактуре се креирају ручно или коришћењем периодичног аутоматизованог процеса.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="dbbe8-120">За свако правно лице које се задужује можете креирати појединачну фактуру или засебне фактуре могу бити креиране пројектом.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="dbbe8-121">Када се фактура клијента између предузећа књижи у правном лицу које позајмљује, у правном лицу које се задужује креира се одговарајућа фактура добављача на чекању.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="dbbe8-122">Трошкови на фактури добављача на чекању евидентираће се у поткњизи пројекта када се фактура прокњижи.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="dbbe8-123">Следећи дијаграм илуструје фактурисање између предузећа које се односи на рачуноводствене догађаје и очекивана књижења у главну књигу.</span><span class="sxs-lookup"><span data-stu-id="dbbe8-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![Ток између предузећа](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="dbbe8-125">Додатни ресурси</span><span class="sxs-lookup"><span data-stu-id="dbbe8-125">Additional resources</span></span>

- [<span data-ttu-id="dbbe8-126">Конфигурисање интерног фактурисања у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="dbbe8-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="dbbe8-127">Евидентирање трансакција у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="dbbe8-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="dbbe8-128">Креирање интерних фактура клијента и добављача у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="dbbe8-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]