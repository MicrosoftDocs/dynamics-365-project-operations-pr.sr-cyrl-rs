---
title: Затварање понуде – једноставно
description: Ова тема пружа информације о затварању понуде у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8d387816f51f63ecd95df6534c7c012b323e6ddc
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764882"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="cda59-103">Затварање понуде – једноставно</span><span class="sxs-lookup"><span data-stu-id="cda59-103">Close a quote - lite</span></span>

<span data-ttu-id="cda59-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="cda59-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cda59-105">Понуда за пројекат може да се затвори као остварена или неостварена.</span><span class="sxs-lookup"><span data-stu-id="cda59-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="cda59-106">Радна верзија понуде може да се затвори јер Microsoft Dynamics 365 Project Operations не подржава операције Активирај и Ревидирај за понуде.</span><span class="sxs-lookup"><span data-stu-id="cda59-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="cda59-107">Затварање понуде као остварене</span><span class="sxs-lookup"><span data-stu-id="cda59-107">Close a quote as Won</span></span>

<span data-ttu-id="cda59-108">Када затворите понуду за пројекат као Добијену, статус се подешава на Затворено, а разлог статуса је Добијено.</span><span class="sxs-lookup"><span data-stu-id="cda59-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="cda59-109">Затварање понуде је поставља понуду за пројекат у статус само за читање и креира радну верзију уговора за пројекат која садржи све информације из понуде.</span><span class="sxs-lookup"><span data-stu-id="cda59-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="cda59-110">Будући да затворена понуда не може поново да се отвори, дијалог за потврду ће потврдити ваше промене.</span><span class="sxs-lookup"><span data-stu-id="cda59-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="cda59-111">Ако приложите понуду уз могућност за пословање, све остале понуде за пројекат у могућности за пословање аутоматски се затварају као неостварене.</span><span class="sxs-lookup"><span data-stu-id="cda59-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="cda59-112">Финансијски утицај затварања понуде као остварене</span><span class="sxs-lookup"><span data-stu-id="cda59-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="cda59-113">Ако постоје стварни подаци о времену на пројекту, док је он још увек приложен уз радну верзију понуде, евидентирају се само трошкови времена или трошкови.</span><span class="sxs-lookup"><span data-stu-id="cda59-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="cda59-114">Након што се понуда затвори као остварена, апликација ће рефакторисати трошкове сторнирањем старијих стварних трошкова и поновним креирањем нових стварних трошкова.</span><span class="sxs-lookup"><span data-stu-id="cda59-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="cda59-115">Апликација ће обрадити ове стварне трошкове на основу методе наплате повезаног предмета уговора о пројекту.</span><span class="sxs-lookup"><span data-stu-id="cda59-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="cda59-116">Ако се стварни подаци о трошковима односе на предмет уговора за време и материјал, одговарајуће ненаплаћене стварне продајне вредности креирају се када се понуда затвори и креира пројектни уговор.</span><span class="sxs-lookup"><span data-stu-id="cda59-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="cda59-117">Ако се стварни подаци о трошковима односе на предмет уговора са фиксном ценом, апликација ће зауставити поновну обраду стварних трошкова који се заснивају на правилима дељене наплате за клијенте уговора о пројекту.</span><span class="sxs-lookup"><span data-stu-id="cda59-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="cda59-118">Затварање понуде као неостварене:</span><span class="sxs-lookup"><span data-stu-id="cda59-118">Closing a quote as lost:</span></span>

<span data-ttu-id="cda59-119">Када затворите понуду за пројекат као Неостварену, статус се подешава на Затворено, а разлог статуса је Неостварено.</span><span class="sxs-lookup"><span data-stu-id="cda59-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="cda59-120">Затварање понуде поставља понуду за пројекат у режим само за читање.</span><span class="sxs-lookup"><span data-stu-id="cda59-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="cda59-121">Будући да затворену понуду не можете поново отворити, пре него што затворите понуду, дијалог за потврду ће потврдити ваше промене.</span><span class="sxs-lookup"><span data-stu-id="cda59-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="cda59-122">Ако се понуда пројекта која је затворена као Неостварена односи на пројекат у било ком реду, тај пројекат је такође означен као Затворен.</span><span class="sxs-lookup"><span data-stu-id="cda59-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="cda59-123">Све резервације ресурса од тог дана надаље отказују се.</span><span class="sxs-lookup"><span data-stu-id="cda59-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="cda59-124">У услузи Project Operations, затварање понуде као остварене или неостварене неће утицати на статус могућности за пословање, која ће остати отворена све док се ручно не затвори.</span><span class="sxs-lookup"><span data-stu-id="cda59-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
