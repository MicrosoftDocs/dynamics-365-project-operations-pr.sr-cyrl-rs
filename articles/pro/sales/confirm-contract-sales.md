---
title: Потврдите уговор за пројекат
description: Ова тема пружа информације о начину потврђивања уговора у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: babce9c64098a9c87072786d914d2340251a8986
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084092"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="0e465-103">Потврдите уговор за пројекат</span><span class="sxs-lookup"><span data-stu-id="0e465-103">Confirm a project contract</span></span>

<span data-ttu-id="0e465-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="0e465-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0e465-105">Уговор за пројекат у програму Dynamics 365 Project Operations може бити активан са разлогом **Потврђено** или затворен са разлогом **Изгубљено**.</span><span class="sxs-lookup"><span data-stu-id="0e465-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed** , or closed with a reason of **Lost**.</span></span> <span data-ttu-id="0e465-106">Када потврдите уговор о пројекту, статус се ажурира са **Радна верзија** на **Активно** , а разлог статуса је **Потврђено**.</span><span class="sxs-lookup"><span data-stu-id="0e465-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="0e465-107">Активни или затворени уговор не може се уређивати или поново отварати.</span><span class="sxs-lookup"><span data-stu-id="0e465-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="0e465-108">Финансијски утицај потврђивања уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="0e465-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="0e465-109">Након што се уговор за пројекат потврди, апликација ће поново израчунати трошкове сторнирањем старијих стварних трошкова и креирањем нових стварних трошкова.</span><span class="sxs-lookup"><span data-stu-id="0e465-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="0e465-110">Нови стварни трошкови се затим обрађују на основу методе наплате повезаног предмета уговора о пројекту.</span><span class="sxs-lookup"><span data-stu-id="0e465-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="0e465-111">Ако се стварни трошкови односе на предмет уговора о времену и материјалу, апликација аутоматски поново креира одговарајуће ненаплаћене стварне трошкове продаје.</span><span class="sxs-lookup"><span data-stu-id="0e465-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="0e465-112">Ако се стварни подаци о трошковима односе на предмет уговора са фиксном ценом, апликација зауставља поновну обраду стварних трошкова.</span><span class="sxs-lookup"><span data-stu-id="0e465-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="0e465-113">Ограничења која се не смеју премашити, подешавање наплативости и утврђивање цена и трошкова на стварним подацима процењују се, а затим ажурирају као део процеса потврде.</span><span class="sxs-lookup"><span data-stu-id="0e465-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="0e465-114">Затворите уговор за пројекат као изгубљен</span><span class="sxs-lookup"><span data-stu-id="0e465-114">Close a project contract as lost</span></span>

<span data-ttu-id="0e465-115">Када уговор о пројекту затворите као изгубљен, статус уговора се ажурира на **Затворено** , а разлог статуса је **Изгубљено**.</span><span class="sxs-lookup"><span data-stu-id="0e465-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="0e465-116">Уговор о пројекту постаје само за читање.</span><span class="sxs-lookup"><span data-stu-id="0e465-116">The project contract becomes read-only.</span></span> <span data-ttu-id="0e465-117">Дијалог за потврду се наводи пре него што се промене доврше јер не можете поново отворити затворени уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="0e465-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="0e465-118">Ако уговор о пројекту који је затворен као изгубљен упућује на пројекат на својим ставкама, тај пројекат је такође означен као затворен.</span><span class="sxs-lookup"><span data-stu-id="0e465-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="0e465-119">Све резервације ресурса од тог дана надаље отказују се.</span><span class="sxs-lookup"><span data-stu-id="0e465-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="0e465-120">Сви ненаплаћени стварни трошкови продаје на уговору за пројект који већ нису на фактури биће сторнирани.</span><span class="sxs-lookup"><span data-stu-id="0e465-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="0e465-121">У услузи Dynamics 365 Project Operations, затварање уговора о пројекту као изгубљеног неће утицати на тај статус повезане могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="0e465-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="0e465-122">Могућност за пословање ће остати отворена и мора се ручно затворити.</span><span class="sxs-lookup"><span data-stu-id="0e465-122">The opportunity will remain open and must be manually closed.</span></span>
