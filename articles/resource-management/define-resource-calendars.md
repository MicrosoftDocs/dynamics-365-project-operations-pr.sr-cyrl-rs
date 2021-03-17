---
title: Дефинисање календара ресурса
description: Ова тема пружа информације о томе како се дефинишу календари радног времена за ресурсе у услузи Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a7b7c45ad2116519b0369bfd3d7cf6743704f4e1
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279831"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="d9c77-103">Дефинисање календара ресурса</span><span class="sxs-lookup"><span data-stu-id="d9c77-103">Define resource calendars</span></span>

<span data-ttu-id="d9c77-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="d9c77-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d9c77-105">Сваки ресурс који може да се резервише који ради на пројекту мора имати календар радног времена да би се дефинисала његова доступност.</span><span class="sxs-lookup"><span data-stu-id="d9c77-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="d9c77-106">Радно време ресурса може се дефинисати на два начина:</span><span class="sxs-lookup"><span data-stu-id="d9c77-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="d9c77-107">Дефинишите појединачна правила календара за ресурс</span><span class="sxs-lookup"><span data-stu-id="d9c77-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="d9c77-108">Примените постојећи предложак календара за ресурс</span><span class="sxs-lookup"><span data-stu-id="d9c77-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="d9c77-109">Дефинишите радно време ресурса</span><span class="sxs-lookup"><span data-stu-id="d9c77-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="d9c77-110">У менију **Ресурси** изаберите **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="d9c77-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="d9c77-111">Из приказа мреже одаберите примењив **Ресурс који може да се резервише**.</span><span class="sxs-lookup"><span data-stu-id="d9c77-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="d9c77-112">На страници **Детаљи ресурса** изаберите картицу **Радно време**. Подразумевано је да календар ресурса могу да се резервишу подразумева радно време подразумеваног обрасца радног времена који је дефинисан за организацију.</span><span class="sxs-lookup"><span data-stu-id="d9c77-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="d9c77-113">Да бисте ажурирали радно време, кликните десним тастером миша на датум почетка предложеног календарског правила које треба дефинисати.</span><span class="sxs-lookup"><span data-stu-id="d9c77-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="d9c77-114">Помоћу менија календара дефинишите правило календара за одређени дан, остатак серије или цео календар.</span><span class="sxs-lookup"><span data-stu-id="d9c77-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="d9c77-115">Када изаберете опцију, можете дефинисати:</span><span class="sxs-lookup"><span data-stu-id="d9c77-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="d9c77-116">Дан у недељи у коме ће се примењивати радно време.</span><span class="sxs-lookup"><span data-stu-id="d9c77-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="d9c77-117">Радно време сваког дана.</span><span class="sxs-lookup"><span data-stu-id="d9c77-117">The working times within each day.</span></span>
    - <span data-ttu-id="d9c77-118">Временска зона за правило календара.</span><span class="sxs-lookup"><span data-stu-id="d9c77-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="d9c77-119">Ако је применљиво, за рад се такође може навести нерадно време.</span><span class="sxs-lookup"><span data-stu-id="d9c77-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="d9c77-120">Примена предлошка календара на ресурс</span><span class="sxs-lookup"><span data-stu-id="d9c77-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="d9c77-121">У менију **Ресурси** изаберите **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="d9c77-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="d9c77-122">Из приказа мреже изаберите до 25 **ресурса који могу дасе резервишу** да бисте их ажурирали.</span><span class="sxs-lookup"><span data-stu-id="d9c77-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="d9c77-123">Изаберите **Подеси календар** и појавиће се дијалог са листом доступних предложака радног времена.</span><span class="sxs-lookup"><span data-stu-id="d9c77-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="d9c77-124">Изаберите предложак који желите да користите, а затим изаберите дугме **Примени**.</span><span class="sxs-lookup"><span data-stu-id="d9c77-124">Select the template you want to use, and then select **Apply**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]