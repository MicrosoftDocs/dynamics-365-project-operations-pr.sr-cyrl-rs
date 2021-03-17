---
title: Кориговане фактуре
description: Ова тема пружа информације о коригованим фактурама.
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
ms.openlocfilehash: 734dc01e15339a31ac21f92bb3fb20d634a075ad
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287841"
---
# <a name="corrected-invoices"></a><span data-ttu-id="b2831-103">Кориговане фактуре</span><span class="sxs-lookup"><span data-stu-id="b2831-103">Corrected invoices</span></span>

<span data-ttu-id="b2831-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="b2831-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b2831-105">Потврђене фактуре се могу уређивати.</span><span class="sxs-lookup"><span data-stu-id="b2831-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="b2831-106">Када уредите потврђну фактуру, креира се радна верзија кориговане фактуре.</span><span class="sxs-lookup"><span data-stu-id="b2831-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="b2831-107">Пошто је претпоставка да желите да сторнирате све трансакције и количине из оригиналне фактуре, ова коригована фактура укључује све трансакције из оригиналне фактуре, а све количине на њој су нула (0).</span><span class="sxs-lookup"><span data-stu-id="b2831-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="b2831-108">Када неке трансакције не захтевају корекцију, можете их уклонити из радне верзије кориговане фактуре.</span><span class="sxs-lookup"><span data-stu-id="b2831-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="b2831-109">Да бисте сторнирали или опозвали само делимичну количину, можете уредити поље Количина у детаљима ставке.</span><span class="sxs-lookup"><span data-stu-id="b2831-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="b2831-110">Ако отворите детаљ ставке фактуре, можете видети количину оригиналне фактуре.</span><span class="sxs-lookup"><span data-stu-id="b2831-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="b2831-111">Затим можете да уредите количину тренутне фактуре тако да буде мања или већа од количине оригиналне фактуре.</span><span class="sxs-lookup"><span data-stu-id="b2831-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="b2831-112">Када потврдите кориговану фактуру, сторнира се оригинална стварна вредности наплаћене продаје и креира се нова стварна вредност наплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="b2831-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="b2831-113">Ако је количина смањена, разлика ће довести до тога да се креира и нова стварна вредност ненаплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="b2831-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="b2831-114">На пример, ако је оригинална наплаћена продаја била за осам сати, а детаљ ставке кориговане фактуре има мању количину од шест сати, сторнира се првобитна наплаћена ставка продаје и креирају се две нове стварне вредности:</span><span class="sxs-lookup"><span data-stu-id="b2831-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="b2831-115">Стварна вредности наплаћене продаје за шест сати.</span><span class="sxs-lookup"><span data-stu-id="b2831-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="b2831-116">Стварна вредности ненаплаћене продаје за преостала два сата.</span><span class="sxs-lookup"><span data-stu-id="b2831-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="b2831-117">Ова трансакција може бити наплаћена касније или означена као ненаплатива, у зависности од преговора са клијентом.</span><span class="sxs-lookup"><span data-stu-id="b2831-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]