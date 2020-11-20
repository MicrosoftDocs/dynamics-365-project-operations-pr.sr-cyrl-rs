---
title: Затварање понуде – једноставно
description: Ова тема пружа информације о затварању понуде у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ad206232d616cdbdc83e2a17b9177cfb98ffda9
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175729"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="d6bae-103">Затварање понуде – једноставно</span><span class="sxs-lookup"><span data-stu-id="d6bae-103">Close a quote - lite</span></span>

<span data-ttu-id="d6bae-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="d6bae-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d6bae-105">Понуда за пројекат може да се затвори као остварена или неостварена.</span><span class="sxs-lookup"><span data-stu-id="d6bae-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="d6bae-106">Будући да операције Активирање и Ревизија нису подржане у понудама у услузи Microsoft Dynamics 365 Project Operations, можете затворити радну верзију понуде.</span><span class="sxs-lookup"><span data-stu-id="d6bae-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="d6bae-107">Затварање понуде као остварене</span><span class="sxs-lookup"><span data-stu-id="d6bae-107">Close a quote as Won</span></span>

<span data-ttu-id="d6bae-108">Затварање понуде за пројекат као остварене затвориће понуду са статусом постављеним на Затворено и разлогом статуса постављеним на Остварено.</span><span class="sxs-lookup"><span data-stu-id="d6bae-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="d6bae-109">Затварање понуде је поставља понуду за пројекат у статус само за читање и креира радну верзију уговора за пројекат која садржи све информације из понуде.</span><span class="sxs-lookup"><span data-stu-id="d6bae-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="d6bae-110">Постоји дијалог за потврду пре него што се промене изврше, јер се затворена понуда не може поново отворити и промене су неповратне.</span><span class="sxs-lookup"><span data-stu-id="d6bae-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="d6bae-111">Ако приложите понуду уз могућност за пословање, све остале понуде за пројекат у могућности за пословање аутоматски се затварају као неостварене.</span><span class="sxs-lookup"><span data-stu-id="d6bae-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="d6bae-112">Финансијски утицај затварања понуде као остварене</span><span class="sxs-lookup"><span data-stu-id="d6bae-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="d6bae-113">Ако постоје стварни подаци за време забележено на пројекту док је још увек приложен уз радну верзију понуде, бележе се само трошкови времена или расхода.</span><span class="sxs-lookup"><span data-stu-id="d6bae-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="d6bae-114">Након што се понуда затвори као остварена, апликација ће рефакторисати трошкове сторнирањем старијих стварних трошкова и поновним креирањем нових стварних трошкова.</span><span class="sxs-lookup"><span data-stu-id="d6bae-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="d6bae-115">Апликација ће обрадити ове стварне трошкове на основу методе наплате повезаног предмета уговора о пројекту.</span><span class="sxs-lookup"><span data-stu-id="d6bae-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="d6bae-116">Ако се стварни износи трошкова односе на предмет уговора о времену и материјалу, систем ће аутоматски креирати одговарајуће ненаплаћене стварне податке о продаји када се понуда затвори и креира пројектни уговор.</span><span class="sxs-lookup"><span data-stu-id="d6bae-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="d6bae-117">Ако се стварни подаци о трошковима позивају на предмет уговора са фиксном ценом, апликација ће зауставити поновну обраду стварних трошкова на основу правила подељеног обрачуна за клијенте по уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="d6bae-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="d6bae-118">Затварање понуде као неостварене:</span><span class="sxs-lookup"><span data-stu-id="d6bae-118">Closing a quote as lost:</span></span>

<span data-ttu-id="d6bae-119">Затварање понуде за пројекат као неостварене поставиће статус понуде на Затворено а разлог статуса на Неостварено.</span><span class="sxs-lookup"><span data-stu-id="d6bae-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="d6bae-120">Затварање понуде поставља понуду за пројекат у режим само за читање.</span><span class="sxs-lookup"><span data-stu-id="d6bae-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="d6bae-121">Будући да затворену понуду не можете поново отворити, пре него што затворите понуду, дијалог за потврду ће потврдити ваше промене.</span><span class="sxs-lookup"><span data-stu-id="d6bae-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="d6bae-122">Ако понуда за пројекат која је затворена као неостварена има пројекат на који се позива било који од њених предмета, тај пројекат се такође означава као затворен и све резервације за ресурсе од тог дана надаље се отказују.</span><span class="sxs-lookup"><span data-stu-id="d6bae-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="d6bae-123">У услузи Project Operations, затварање понуде као остварене или неостварене неће утицати на статус могућности за пословање, која ће остати отворена све док се ручно не затвори.</span><span class="sxs-lookup"><span data-stu-id="d6bae-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
