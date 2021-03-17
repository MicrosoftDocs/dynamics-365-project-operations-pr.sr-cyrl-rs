---
title: Преглед интерног фактурисања у оквиру предузећа
description: Ова тема пружа информације и примере о интерном фактурисању између предузећа за пројекте.
author: sigitac
manager: tfehr
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 3ad75089de1a2f99646f7aba213e199a2bec347d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287346"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="38cfe-103">Преглед интерног фактурисања у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="38cfe-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="38cfe-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="38cfe-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="38cfe-105">Ваша организација може имати више одељења, подружница и других правних лица која међусобно преносе производе и услуге за пројекте.</span><span class="sxs-lookup"><span data-stu-id="38cfe-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="38cfe-106">Правно лице које пружа услугу или даје производ назива се *правно лице које позајмљује*.</span><span class="sxs-lookup"><span data-stu-id="38cfe-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="38cfe-107">Правно лице које прима услугу или производ назива се *правно лице које се задужује*.</span><span class="sxs-lookup"><span data-stu-id="38cfe-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="38cfe-108">Следећа илустрација приказује типични сценарио када два правна лица, Contoso Robotics USA (правно лице које се задужује) и Contoso Robotics UK (правно лице које позајмљује) деле ресурсе како би испоручили пројекат клијенту, Adventure works.</span><span class="sxs-lookup"><span data-stu-id="38cfe-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="38cfe-109">За овај сценарио, Contoso Robotics USA по уговору треба да испоручи посао предузећу Adventure Works.</span><span class="sxs-lookup"><span data-stu-id="38cfe-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![Интерно фактурисање у оквиру предузећа](./media/IntercompanyScenario.png) 

<span data-ttu-id="38cfe-111">Dynamics 365 Project Operations користи следећи ток за обраду трансакција између предузећа:</span><span class="sxs-lookup"><span data-stu-id="38cfe-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="38cfe-112">Ресурси правног лица које даје позајмице евидентирају трансакције времена или трошкова између предузећа према времену и трошку резервације у основу на пројекте правног лица које се задужује.</span><span class="sxs-lookup"><span data-stu-id="38cfe-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="38cfe-113">Трошкови времена и трошкова евидентирају се у предузећу које позајмљује коришћењем јединичног ценовника трошкова предузећа које се задужује.</span><span class="sxs-lookup"><span data-stu-id="38cfe-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="38cfe-114">Ненаплаћене продајне трансакције између предузећа евидентирају се у компанији која позајмљује коришћењем јединичног ценовника трошкова предузећа које се задужује.</span><span class="sxs-lookup"><span data-stu-id="38cfe-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="38cfe-115">Нефактурисани приход се евидентира у предузећу које се задужује користећи ценовник продајних цена по уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="38cfe-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="38cfe-116">Клијенту можете наплатити када се евидентира нефактурисани приход.</span><span class="sxs-lookup"><span data-stu-id="38cfe-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="38cfe-117">Клијент не мора да чека док се обрада фактура између предузећа не заврши.</span><span class="sxs-lookup"><span data-stu-id="38cfe-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="38cfe-118">Фактуре клијената између предузећа се креирају периодично у предузећу које позајмљује.</span><span class="sxs-lookup"><span data-stu-id="38cfe-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="38cfe-119">Фактуре се креирају ручно или коришћењем периодичног аутоматизованог процеса.</span><span class="sxs-lookup"><span data-stu-id="38cfe-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="38cfe-120">За свако правно лице које се задужује можете креирати појединачну фактуру или засебне фактуре могу бити креиране пројектом.</span><span class="sxs-lookup"><span data-stu-id="38cfe-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="38cfe-121">Када се фактура клијента између предузећа књижи у правном лицу које позајмљује, у правном лицу које се задужује креира се одговарајућа фактура добављача на чекању.</span><span class="sxs-lookup"><span data-stu-id="38cfe-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="38cfe-122">Трошкови на фактури добављача на чекању евидентираће се у поткњизи пројекта када се фактура прокњижи.</span><span class="sxs-lookup"><span data-stu-id="38cfe-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="38cfe-123">Следећи дијаграм илуструје фактурисање између предузећа које се односи на рачуноводствене догађаје и очекивана књижења у главну књигу.</span><span class="sxs-lookup"><span data-stu-id="38cfe-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![Ток између предузећа](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="38cfe-125">Додатни ресурси</span><span class="sxs-lookup"><span data-stu-id="38cfe-125">Additional resources</span></span>

- [<span data-ttu-id="38cfe-126">Конфигурисање интерног фактурисања у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="38cfe-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="38cfe-127">Евидентирање трансакција у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="38cfe-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="38cfe-128">Креирање интерних фактура клијента и добављача у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="38cfe-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]