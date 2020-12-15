---
title: Преглед препознавања прихода
description: Ова тема пружа информације о препознавању прихода у услузи Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6844f4c5d4cda8a6a901b0302448f70f4c597f5d
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531542"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="0e582-103">Преглед препознавања прихода</span><span class="sxs-lookup"><span data-stu-id="0e582-103">Revenue recognition overview</span></span>

<span data-ttu-id="0e582-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="0e582-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="0e582-105">У услузи Dynamics 365 Project Operations, принципи препознавања прихода варирају у зависности од изабраног начина обрачуна за пројекат или део пројекта.</span><span class="sxs-lookup"><span data-stu-id="0e582-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="0e582-106">Ова тема пружа информације о препознавању прихода у услузи Project Operations.</span><span class="sxs-lookup"><span data-stu-id="0e582-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="0e582-107">Преузете трансакције користећи начин наплате за време и материјал</span><span class="sxs-lookup"><span data-stu-id="0e582-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="0e582-108">Повезани су препознавање трошкова и прихода.</span><span class="sxs-lookup"><span data-stu-id="0e582-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="0e582-109">Трошкови трансакције и нефактурисане продаје књиже се помоћу [Project Operations дневника интеграције](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="0e582-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="0e582-110">Профил трошкова и прихода пројекта одређује да ли се нефактурисане продајне трансакције књиже у главну књигу.</span><span class="sxs-lookup"><span data-stu-id="0e582-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="0e582-111">Ако је изабран **Припадајући приход**, систем користи конта за **WIP продајну вредност** и **Вредност продаје оствареног прихода** током књижења.</span><span class="sxs-lookup"><span data-stu-id="0e582-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="0e582-112">Следеће је пример овог начина.</span><span class="sxs-lookup"><span data-stu-id="0e582-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="0e582-113">Тип трансакције</span><span class="sxs-lookup"><span data-stu-id="0e582-113">Transaction type</span></span> | <span data-ttu-id="0e582-114">Задужење/Одобрење</span><span class="sxs-lookup"><span data-stu-id="0e582-114">Debit/Credit</span></span> | <span data-ttu-id="0e582-115">Износ</span><span class="sxs-lookup"><span data-stu-id="0e582-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="0e582-116">Продајна вредност за рад на пројекту</span><span class="sxs-lookup"><span data-stu-id="0e582-116">WIP Sales value</span></span> | <span data-ttu-id="0e582-117">Задужење</span><span class="sxs-lookup"><span data-stu-id="0e582-117">Debit</span></span> | <span data-ttu-id="0e582-118">100</span><span class="sxs-lookup"><span data-stu-id="0e582-118">100</span></span> |
  | <span data-ttu-id="0e582-119">Вредност продаје за обрачунати приход</span><span class="sxs-lookup"><span data-stu-id="0e582-119">Accrued revenue sales value</span></span> | <span data-ttu-id="0e582-120">Одобрење</span><span class="sxs-lookup"><span data-stu-id="0e582-120">Credit</span></span> | <span data-ttu-id="0e582-121">100</span><span class="sxs-lookup"><span data-stu-id="0e582-121">100</span></span> |

- <span data-ttu-id="0e582-122">Приход се препознаје при фактурисању.</span><span class="sxs-lookup"><span data-stu-id="0e582-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="0e582-123">Систем користи конто **Фактурисани приход** током књижења.</span><span class="sxs-lookup"><span data-stu-id="0e582-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="0e582-124">Следеће је пример овог начина.</span><span class="sxs-lookup"><span data-stu-id="0e582-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="0e582-125">Тип трансакције</span><span class="sxs-lookup"><span data-stu-id="0e582-125">Transaction type</span></span> | <span data-ttu-id="0e582-126">Задужење/Одобрење</span><span class="sxs-lookup"><span data-stu-id="0e582-126">Debit/Credit</span></span> | <span data-ttu-id="0e582-127">Износ</span><span class="sxs-lookup"><span data-stu-id="0e582-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="0e582-128">Биланс клијента</span><span class="sxs-lookup"><span data-stu-id="0e582-128">Customer balance</span></span> | <span data-ttu-id="0e582-129">Задужење</span><span class="sxs-lookup"><span data-stu-id="0e582-129">Debit</span></span> | <span data-ttu-id="0e582-130">120</span><span class="sxs-lookup"><span data-stu-id="0e582-130">120</span></span> |
  | <span data-ttu-id="0e582-131">Дуговани порез на промет</span><span class="sxs-lookup"><span data-stu-id="0e582-131">Sales tax payable</span></span> | <span data-ttu-id="0e582-132">Одобрење</span><span class="sxs-lookup"><span data-stu-id="0e582-132">Credit</span></span> | <span data-ttu-id="0e582-133">20</span><span class="sxs-lookup"><span data-stu-id="0e582-133">20</span></span> |
  | <span data-ttu-id="0e582-134">Фактурисани приход</span><span class="sxs-lookup"><span data-stu-id="0e582-134">Invoiced Revenue</span></span> | <span data-ttu-id="0e582-135">Одобрење</span><span class="sxs-lookup"><span data-stu-id="0e582-135">Credit</span></span> | <span data-ttu-id="0e582-136">100</span><span class="sxs-lookup"><span data-stu-id="0e582-136">100</span></span> |

- <span data-ttu-id="0e582-137">Ако је приход настао приликом књижења нефактурисане продаје, систем ће сторнирани остварени приход приликом фактурисања.</span><span class="sxs-lookup"><span data-stu-id="0e582-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="0e582-138">Тип трансакције</span><span class="sxs-lookup"><span data-stu-id="0e582-138">Transaction type</span></span> | <span data-ttu-id="0e582-139">Задужење/Одобрење</span><span class="sxs-lookup"><span data-stu-id="0e582-139">Debit/Credit</span></span> | <span data-ttu-id="0e582-140">Износ</span><span class="sxs-lookup"><span data-stu-id="0e582-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="0e582-141">Продајна вредност за рад на пројекту</span><span class="sxs-lookup"><span data-stu-id="0e582-141">WIP Sales value</span></span> | <span data-ttu-id="0e582-142">Одобрење</span><span class="sxs-lookup"><span data-stu-id="0e582-142">Credit</span></span> | <span data-ttu-id="0e582-143">100</span><span class="sxs-lookup"><span data-stu-id="0e582-143">100</span></span> |
  | <span data-ttu-id="0e582-144">Вредност продаје за обрачунати приход</span><span class="sxs-lookup"><span data-stu-id="0e582-144">Accrued revenue sales value</span></span> | <span data-ttu-id="0e582-145">Задужење</span><span class="sxs-lookup"><span data-stu-id="0e582-145">Debit</span></span> | <span data-ttu-id="0e582-146">100</span><span class="sxs-lookup"><span data-stu-id="0e582-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="0e582-147">Преузете трансакције користећи начин наплате фиксне цене</span><span class="sxs-lookup"><span data-stu-id="0e582-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="0e582-148">Препознавање трошкова и прихода су засебни.</span><span class="sxs-lookup"><span data-stu-id="0e582-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="0e582-149">Трошак трансакције се књижи помоћу [Project Operations дневника интеграције](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="0e582-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="0e582-150">Нефактурисане продајне трансакције се не креирају.</span><span class="sxs-lookup"><span data-stu-id="0e582-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="0e582-151">Приход може бити препознат током фактурисања ако трошак производа и профил прихода имају **Принцип коришћен за израчунавања довршетка пројекта** подешен на **Није рад на пројекту**.</span><span class="sxs-lookup"><span data-stu-id="0e582-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="0e582-152">Овај начин користите само за краткорочне, једноставне пројекте.</span><span class="sxs-lookup"><span data-stu-id="0e582-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="0e582-153">Приход можете признати помоћу процене прихода са фиксном ценом, било са начином **Завршен уговор** или **Признавање прихода по проценту довршења**.</span><span class="sxs-lookup"><span data-stu-id="0e582-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="0e582-154">Додатни ресурси</span><span class="sxs-lookup"><span data-stu-id="0e582-154">Additional resources</span></span>
[<span data-ttu-id="0e582-155">Чланак о конфигурисању рачуноводства за наплативе пројекте</span><span class="sxs-lookup"><span data-stu-id="0e582-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="0e582-156">Процена прихода пројеката са фиксном ценом</span><span class="sxs-lookup"><span data-stu-id="0e582-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="0e582-157">Управљање проценама прихода</span><span class="sxs-lookup"><span data-stu-id="0e582-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="0e582-158">Методи од трошка до довршетка</span><span class="sxs-lookup"><span data-stu-id="0e582-158">Cost to complete methods</span></span>](cost-complete-methods.md)