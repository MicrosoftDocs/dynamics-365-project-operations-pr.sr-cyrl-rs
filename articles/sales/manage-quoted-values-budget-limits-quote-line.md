---
title: Преглед ставки понуде за пројекат
description: Ова тема пружа информације о коришћењу ставки понуде за пројекат за рад на пројекту.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fa48a90c275eae1b0c0dbce685ae718dd9674c88
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858050"
---
# <a name="project-quote-lines-overview"></a><span data-ttu-id="f3c3e-103">Преглед ставки понуде за пројекат</span><span class="sxs-lookup"><span data-stu-id="f3c3e-103">Project quote lines overview</span></span>

<span data-ttu-id="f3c3e-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="f3c3e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f3c3e-105">Ставке понуде засноване на пројекту осмишљене су да помогну у процени рада на пројекту при ангажовању.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="f3c3e-106">Структура ставке понуде на основу пројекта проширена је за процене пројеката следећим концептима:</span><span class="sxs-lookup"><span data-stu-id="f3c3e-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="f3c3e-107">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="f3c3e-107">Billing Method</span></span>
- <span data-ttu-id="f3c3e-108">Мапирање пројеката</span><span class="sxs-lookup"><span data-stu-id="f3c3e-108">Project Mapping</span></span>
- <span data-ttu-id="f3c3e-109">Укључене класе трансакција</span><span class="sxs-lookup"><span data-stu-id="f3c3e-109">Included Transaction classes</span></span>
- <span data-ttu-id="f3c3e-110">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="f3c3e-111">Подешавање наплативости</span><span class="sxs-lookup"><span data-stu-id="f3c3e-111">Chargeability setup</span></span>
- <span data-ttu-id="f3c3e-112">Процена помоћу детаља ставки понуде</span><span class="sxs-lookup"><span data-stu-id="f3c3e-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="f3c3e-113">Клијенти ставки понуде</span><span class="sxs-lookup"><span data-stu-id="f3c3e-113">Quote line Customers</span></span>

<span data-ttu-id="f3c3e-114">Следећа табела пружа информације о пољима на картици **Општи подаци** ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="f3c3e-115">Ова поља помажу у постављању основе за детаљну, основну процену рада на пројекту.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="f3c3e-116">**Поље**</span><span class="sxs-lookup"><span data-stu-id="f3c3e-116">**Field**</span></span> | <span data-ttu-id="f3c3e-117">**Опис**</span><span class="sxs-lookup"><span data-stu-id="f3c3e-117">**Description**</span></span> | <span data-ttu-id="f3c3e-118">**Последични утицај**</span><span class="sxs-lookup"><span data-stu-id="f3c3e-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f3c3e-119">Именуј</span><span class="sxs-lookup"><span data-stu-id="f3c3e-119">Name</span></span> | <span data-ttu-id="f3c3e-120">Назив ставке понуде која би требало да вам помогне да идентификујете дискретну компоненту понуде која се процењује.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="f3c3e-121">Копира се у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-122">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="f3c3e-122">Billing Method</span></span> | <span data-ttu-id="f3c3e-123">У понуди креираној из могућности за пословање, ова вредност се копира из одговарајућег поља у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="f3c3e-124">Ово поље укључује два главна модела уговарања које Dynamics 365 Project Operations подржава:</span><span class="sxs-lookup"><span data-stu-id="f3c3e-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="f3c3e-125">- Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="f3c3e-125">- Fixed price</span></span></br><span data-ttu-id="f3c3e-126">- Време и материјал.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-126">- Time and material.</span></span>| <span data-ttu-id="f3c3e-127">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-128">Project</span><span class="sxs-lookup"><span data-stu-id="f3c3e-128">Project</span></span> | <span data-ttu-id="f3c3e-129">Користите ово опционално поље за идентификовање пројекта који ће се користити за извођење радова при овом ангажовању.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="f3c3e-130">Када се пројекат мапира у ставку понуде, то помаже у постављању наплативих задатака, као и у доношењу процене засноване на пројекту у ставци понуде као детаље ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="f3c3e-131">Када пројекат није мапиран у ставку понуде засновану на пројекту, процену треба креирати ручно креирањем сваког детаља ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="f3c3e-132">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-133">Садржи време</span><span class="sxs-lookup"><span data-stu-id="f3c3e-133">Include Time</span></span> | <span data-ttu-id="f3c3e-134">Заставица **Да**/**Не** означава да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="f3c3e-135">Вредност **Не** означава да временске трансакције или трошкови рада неће бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="f3c3e-136">Вредност **Да** означава да ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="f3c3e-137">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-138">Садржи трошак</span><span class="sxs-lookup"><span data-stu-id="f3c3e-138">Include Expense</span></span> | <span data-ttu-id="f3c3e-139">Заставица **Да**/**Не** означава да ли ће цене трошкова на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="f3c3e-140">Вредност **Не** означава да цена трошка неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="f3c3e-141">Вредност **Да** означава да ће цена трошка бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="f3c3e-142">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-143">Садржи накнаду</span><span class="sxs-lookup"><span data-stu-id="f3c3e-143">Include Fee</span></span> | <span data-ttu-id="f3c3e-144">Заставица **Да**/**Не** означава да ли ће накнаде на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="f3c3e-145">Вредност **Не** означава да накнаде неће бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="f3c3e-146">Вредност **Да** означава да ће накнаде бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="f3c3e-147">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-148">Понуђени износ</span><span class="sxs-lookup"><span data-stu-id="f3c3e-148">Quoted Amount</span></span> | <span data-ttu-id="f3c3e-149">Ово је износ који ће бити наведен клијенту за све радове предвиђене у овој ставци понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="f3c3e-150">У понуди креираној из могућности за пословање, ова вредност се копира из поља **Буџет клијента** у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="f3c3e-151">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="f3c3e-152">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-153">Процењени порез</span><span class="sxs-lookup"><span data-stu-id="f3c3e-153">Estimated Tax</span></span> | <span data-ttu-id="f3c3e-154">То поље може да уређује корисник да би додао процењени износ пореза у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="f3c3e-155">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа пореза на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="f3c3e-156">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-157">Понуђени опорезовани износ</span><span class="sxs-lookup"><span data-stu-id="f3c3e-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="f3c3e-158">Ово поље је опорезовани износ ставке понуде и само је за читање.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="f3c3e-159">Износ у овом пољу се израчунава као *Понуђени износ + порез*.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="f3c3e-160">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-161">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="f3c3e-162">Ово поље је могуће уређивати и доступно је само у ставкама понуде заснованим на пројекту чији начин обрачуна је **Време и материјал**.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="f3c3e-163">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="f3c3e-164">Буџет клијента</span><span class="sxs-lookup"><span data-stu-id="f3c3e-164">Customer Budget</span></span> | <span data-ttu-id="f3c3e-165">Ово поље може да се уређује и копира се из одговарајућег поља ставке могућности за пословање ако је понуда креирана из могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="f3c3e-166">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="f3c3e-167">Правила за валидацију за поља на картици Општи подаци ставки понуде заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="f3c3e-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="f3c3e-168">**1. правило**: Одређена класа трансакција на изабраном пројекту може се укључити само у једну ставку понуде на основу пројекта.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="f3c3e-169">**2. правило**: Ако могућност за пословање има више понуда, могу постојати ставке понуде из различитих понуда које се односе на исти пројекат и укључују исту класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="f3c3e-170">**3. правило**: Ако понуде не припадају истој могућности за пословање, не могу да укључују исти пројекат и класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="f3c3e-171">
                    <strong>Могућност за пословање</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="f3c3e-172">
                    <strong>Понуда</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="f3c3e-173">
                    <strong>Ставка понуде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="f3c3e-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="f3c3e-175">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="f3c3e-176">
                    <strong>Садржи трошак</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="f3c3e-177">
                    <strong>Уврсти</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="f3c3e-178">
                    <strong>накнада</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="f3c3e-179">
                    <strong>Важи / Не важи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="f3c3e-180">
                    <strong>Разлог</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f3c3e-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="f3c3e-181">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-182">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-183">QL1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-184">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-185">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-186">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-187">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-188">Не важи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-189">Кршење правила бр. 1.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-189">Violation of Rule #1.</span></span> <span data-ttu-id="f3c3e-190">Време, трошкови и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="f3c3e-191">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-192">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-193">QL2</span><span class="sxs-lookup"><span data-stu-id="f3c3e-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-194">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-195">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-196">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-197">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-197">Yes</span></span> </p>
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
<span data-ttu-id="f3c3e-198">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-199">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-200">QL1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-201">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-202">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-203">Не</span><span class="sxs-lookup"><span data-stu-id="f3c3e-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-204">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-205">Не важи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-206">Кршење правила бр. 1.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-206">Violation of Rule #1.</span></span> <span data-ttu-id="f3c3e-207">Време и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="f3c3e-208">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-209">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-210">QL2</span><span class="sxs-lookup"><span data-stu-id="f3c3e-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-211">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-212">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-213">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-214">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-214">Yes</span></span> </p>
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
<span data-ttu-id="f3c3e-215">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-216">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-217">QL1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-218">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-219">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-220">Не</span><span class="sxs-lookup"><span data-stu-id="f3c3e-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-221">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-222">Важећи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="f3c3e-223">Време и накнаде за пројекат P1 су укључени у QL1.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="f3c3e-224">Трошкови за пројекат P1 укључени су у QL2.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="f3c3e-225">Нема преклапања у ономе што је укључено у сваку ставку понуде, тако да је то важеће.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="f3c3e-226">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-227">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-228">QL2</span><span class="sxs-lookup"><span data-stu-id="f3c3e-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-229">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-230">Не</span><span class="sxs-lookup"><span data-stu-id="f3c3e-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-231">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-232">Не</span><span class="sxs-lookup"><span data-stu-id="f3c3e-232">No</span></span> </p>
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
<span data-ttu-id="f3c3e-233">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-234">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-235">QL1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-236">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-237">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-238">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-239">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-240">Не важи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-241">Кршење горенаведеног правила бр. 1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="f3c3e-242">Q1 укључује време, трошкове и накнаде за цео пројекат P1.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="f3c3e-243">QL2 укључује време, трошкове и накнаде за цео пројекат P1 и преклапа се са оним што је укључено у Q1.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="f3c3e-244">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-245">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-246">QL2</span><span class="sxs-lookup"><span data-stu-id="f3c3e-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-247">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-248">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-249">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-250">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-250">Yes</span></span> </p>
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
<span data-ttu-id="f3c3e-251">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-252">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-253">QL1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-254">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-255">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-256">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-257">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="f3c3e-258">Важећи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-259">На основу правила бр. 2, Q1 и Q2 су две понуде у истој могућности за пословање, тако да обе могу проценити исте компоненте пројекта.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="f3c3e-260">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-261">К2</span><span class="sxs-lookup"><span data-stu-id="f3c3e-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-262">QL1 на Q2</span><span class="sxs-lookup"><span data-stu-id="f3c3e-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-263">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-264">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-265">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-266">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-266">Yes</span></span> </p>
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
<span data-ttu-id="f3c3e-267">O1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-268">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-269">QL1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-270">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-271">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-272">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-273">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="f3c3e-274">Важећи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f3c3e-275">На основу правила бр. 3, Q1 и Q2 су две понуде у различитим могућностима за пословање, тако да оне не могу проценити компоненте истог пројекта.</span><span class="sxs-lookup"><span data-stu-id="f3c3e-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="f3c3e-276">O2</span><span class="sxs-lookup"><span data-stu-id="f3c3e-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="f3c3e-277">К1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-278">QL1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-279">П1</span><span class="sxs-lookup"><span data-stu-id="f3c3e-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-280">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="f3c3e-281">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="f3c3e-282">Да</span><span class="sxs-lookup"><span data-stu-id="f3c3e-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="f3c3e-283">Не важи</span><span class="sxs-lookup"><span data-stu-id="f3c3e-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
