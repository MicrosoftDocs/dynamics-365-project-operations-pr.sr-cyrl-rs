---
title: Преглед ставки понуде за пројекат
description: Ова тема пружа информације о коришћењу ставки понуде за пројекат за рад на пројекту.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: c585bbc55119e678a4f75f5dfe8966a436db1a34
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368089"
---
# <a name="project-quote-lines-overview"></a><span data-ttu-id="a3c1a-103">Преглед ставки понуде за пројекат</span><span class="sxs-lookup"><span data-stu-id="a3c1a-103">Project quote lines overview</span></span>

<span data-ttu-id="a3c1a-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="a3c1a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a3c1a-105">Ставке понуде засноване на пројекту осмишљене су да помогну у процени рада на пројекту при ангажовању.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="a3c1a-106">Структура ставке понуде на основу пројекта проширена је за процене пројеката следећим концептима:</span><span class="sxs-lookup"><span data-stu-id="a3c1a-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="a3c1a-107">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="a3c1a-107">Billing Method</span></span>
- <span data-ttu-id="a3c1a-108">Мапирање пројеката</span><span class="sxs-lookup"><span data-stu-id="a3c1a-108">Project Mapping</span></span>
- <span data-ttu-id="a3c1a-109">Укључене класе трансакција</span><span class="sxs-lookup"><span data-stu-id="a3c1a-109">Included Transaction classes</span></span>
- <span data-ttu-id="a3c1a-110">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="a3c1a-111">Подешавање наплативости</span><span class="sxs-lookup"><span data-stu-id="a3c1a-111">Chargeability setup</span></span>
- <span data-ttu-id="a3c1a-112">Процена помоћу детаља ставки понуде</span><span class="sxs-lookup"><span data-stu-id="a3c1a-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="a3c1a-113">Клијенти ставки понуде</span><span class="sxs-lookup"><span data-stu-id="a3c1a-113">Quote line Customers</span></span>

<span data-ttu-id="a3c1a-114">Следећа табела пружа информације о пољима на картици **Општи подаци** ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="a3c1a-115">Ова поља помажу у постављању основе за детаљну, основну процену рада на пројекту.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="a3c1a-116">**Поље**</span><span class="sxs-lookup"><span data-stu-id="a3c1a-116">**Field**</span></span> | <span data-ttu-id="a3c1a-117">**Опис**</span><span class="sxs-lookup"><span data-stu-id="a3c1a-117">**Description**</span></span> | <span data-ttu-id="a3c1a-118">**Последични утицај**</span><span class="sxs-lookup"><span data-stu-id="a3c1a-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a3c1a-119">Именуј</span><span class="sxs-lookup"><span data-stu-id="a3c1a-119">Name</span></span> | <span data-ttu-id="a3c1a-120">Назив ставке понуде која би требало да вам помогне да идентификујете дискретну компоненту понуде која се процењује.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="a3c1a-121">Копира се у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-122">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="a3c1a-122">Billing Method</span></span> | <span data-ttu-id="a3c1a-123">У понуди креираној из могућности за пословање, ова вредност се копира из одговарајућег поља у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="a3c1a-124">Ово поље укључује два главна модела уговарања које Dynamics 365 Project Operations подржава:</span><span class="sxs-lookup"><span data-stu-id="a3c1a-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="a3c1a-125">- Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="a3c1a-125">- Fixed price</span></span></br><span data-ttu-id="a3c1a-126">- Време и материјал.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-126">- Time and material.</span></span>| <span data-ttu-id="a3c1a-127">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-128">Project</span><span class="sxs-lookup"><span data-stu-id="a3c1a-128">Project</span></span> | <span data-ttu-id="a3c1a-129">Користите ово опционално поље за идентификовање пројекта који ће се користити за извођење радова при овом ангажовању.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="a3c1a-130">Када се пројекат мапира у ставку понуде, то помаже у постављању наплативих задатака, као и у доношењу процене засноване на пројекту у ставци понуде као детаље ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="a3c1a-131">Када пројекат није мапиран у ставку понуде засновану на пројекту, процену треба креирати ручно креирањем сваког детаља ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="a3c1a-132">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-133">Садржи време</span><span class="sxs-lookup"><span data-stu-id="a3c1a-133">Include Time</span></span> | <span data-ttu-id="a3c1a-134">Заставица **Да**/**Не** означава да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="a3c1a-135">Вредност **Не** означава да временске трансакције или трошкови рада неће бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="a3c1a-136">Вредност **Да** означава да ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="a3c1a-137">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-138">Садржи трошак</span><span class="sxs-lookup"><span data-stu-id="a3c1a-138">Include Expense</span></span> | <span data-ttu-id="a3c1a-139">Заставица **Да**/**Не** означава да ли ће цене трошкова на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="a3c1a-140">Вредност **Не** означава да цена трошка неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="a3c1a-141">Вредност **Да** означава да ће цена трошка бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="a3c1a-142">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-143">Садржи накнаду</span><span class="sxs-lookup"><span data-stu-id="a3c1a-143">Include Fee</span></span> | <span data-ttu-id="a3c1a-144">Заставица **Да**/**Не** означава да ли ће накнаде на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="a3c1a-145">Вредност **Не** означава да накнаде неће бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="a3c1a-146">Вредност **Да** означава да ће накнаде бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="a3c1a-147">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-148">Понуђени износ</span><span class="sxs-lookup"><span data-stu-id="a3c1a-148">Quoted Amount</span></span> | <span data-ttu-id="a3c1a-149">Ово је износ који ће бити наведен клијенту за све радове предвиђене у овој ставци понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="a3c1a-150">У понуди креираној из могућности за пословање, ова вредност се копира из поља **Буџет клијента** у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="a3c1a-151">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="a3c1a-152">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-153">Процењени порез</span><span class="sxs-lookup"><span data-stu-id="a3c1a-153">Estimated Tax</span></span> | <span data-ttu-id="a3c1a-154">То поље може да уређује корисник да би додао процењени износ пореза у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="a3c1a-155">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа пореза на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="a3c1a-156">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-157">Понуђени опорезовани износ</span><span class="sxs-lookup"><span data-stu-id="a3c1a-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="a3c1a-158">Ово поље је опорезовани износ ставке понуде и само је за читање.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="a3c1a-159">Износ у овом пољу се израчунава као *Понуђени износ + порез*.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="a3c1a-160">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-161">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="a3c1a-162">Ово поље је могуће уређивати и доступно је само у ставкама понуде заснованим на пројекту чији начин обрачуна је **Време и материјал**.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="a3c1a-163">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="a3c1a-164">Буџет клијента</span><span class="sxs-lookup"><span data-stu-id="a3c1a-164">Customer Budget</span></span> | <span data-ttu-id="a3c1a-165">Ово поље може да се уређује и копира се из одговарајућег поља ставке могућности за пословање ако је понуда креирана из могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="a3c1a-166">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="a3c1a-167">Правила за валидацију за поља на картици Општи подаци ставки понуде заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="a3c1a-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="a3c1a-168">**1. правило**: Одређена класа трансакција на изабраном пројекту може се укључити само у једну ставку понуде на основу пројекта.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="a3c1a-169">**2. правило**: Ако могућност за пословање има више понуда, могу постојати ставке понуде из различитих понуда које се односе на исти пројекат и укључују исту класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="a3c1a-170">**3. правило**: Ако понуде не припадају истој могућности за пословање, не могу да укључују исти пројекат и класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="a3c1a-171">
                    <strong>Могућност за пословање</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="a3c1a-172">
                    <strong>Понуда</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="a3c1a-173">
                    <strong>Ставка понуде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="a3c1a-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="a3c1a-175">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="a3c1a-176">
                    <strong>Садржи трошак</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="a3c1a-177">
                    <strong>Уврсти</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="a3c1a-178">
                    <strong>накнада</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="a3c1a-179">
                    <strong>Важи / Не важи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="a3c1a-180">
                    <strong>Разлог</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a3c1a-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-181">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-182">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-183">QL1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-184">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-185">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-186">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-187">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-188">Не важи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-189">Кршење правила бр. 1.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-189">Violation of Rule #1.</span></span> <span data-ttu-id="a3c1a-190">Време, трошкови и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-191">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-192">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-193">QL2</span><span class="sxs-lookup"><span data-stu-id="a3c1a-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-194">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-195">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-196">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-197">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-197">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-198">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-199">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-200">QL1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-201">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-202">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-203">Не</span><span class="sxs-lookup"><span data-stu-id="a3c1a-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-204">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-205">Не важи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-206">Кршење правила бр. 1.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-206">Violation of Rule #1.</span></span> <span data-ttu-id="a3c1a-207">Време и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-208">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-209">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-210">QL2</span><span class="sxs-lookup"><span data-stu-id="a3c1a-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-211">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-212">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-213">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-214">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-214">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-215">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-216">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-217">QL1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-218">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-219">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-220">Не</span><span class="sxs-lookup"><span data-stu-id="a3c1a-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-221">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-222">Важећи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="a3c1a-223">Време и накнаде за пројекат P1 су укључени у QL1.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="a3c1a-224">Трошкови за пројекат P1 укључени су у QL2.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="a3c1a-225">Нема преклапања у ономе што је укључено у сваку ставку понуде, тако да је то важеће.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-226">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-227">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-228">QL2</span><span class="sxs-lookup"><span data-stu-id="a3c1a-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-229">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-230">Не</span><span class="sxs-lookup"><span data-stu-id="a3c1a-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-231">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-232">Не</span><span class="sxs-lookup"><span data-stu-id="a3c1a-232">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-233">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-234">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-235">QL1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-236">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-237">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-238">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-239">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-240">Не важи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-241">Кршење горенаведеног правила бр. 1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="a3c1a-242">Q1 укључује време, трошкове и накнаде за цео пројекат P1.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="a3c1a-243">QL2 укључује време, трошкове и накнаде за цео пројекат P1 и преклапа се са оним што је укључено у Q1.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-244">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-245">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-246">QL2</span><span class="sxs-lookup"><span data-stu-id="a3c1a-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-247">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-248">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-249">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-250">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-250">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-251">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-252">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-253">QL1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-254">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-255">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-256">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-257">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="a3c1a-258">Важећи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-259">На основу правила бр. 2, Q1 и Q2 су две понуде у истој могућности за пословање, тако да обе могу проценити исте компоненте пројекта.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-260">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-261">К2</span><span class="sxs-lookup"><span data-stu-id="a3c1a-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-262">QL1 на Q2</span><span class="sxs-lookup"><span data-stu-id="a3c1a-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-263">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-264">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-265">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-266">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-266">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-267">O1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-268">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-269">QL1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-270">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-271">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-272">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-273">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="a3c1a-274">Важећи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a3c1a-275">На основу правила бр. 3, Q1 и Q2 су две понуде у различитим могућностима за пословање, тако да оне не могу проценити компоненте истог пројекта.</span><span class="sxs-lookup"><span data-stu-id="a3c1a-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="a3c1a-276">O2</span><span class="sxs-lookup"><span data-stu-id="a3c1a-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="a3c1a-277">К1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-278">QL1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-279">П1</span><span class="sxs-lookup"><span data-stu-id="a3c1a-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-280">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="a3c1a-281">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="a3c1a-282">Да</span><span class="sxs-lookup"><span data-stu-id="a3c1a-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="a3c1a-283">Не важи</span><span class="sxs-lookup"><span data-stu-id="a3c1a-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
