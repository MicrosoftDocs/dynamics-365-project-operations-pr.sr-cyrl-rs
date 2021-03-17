---
title: Преглед ставки понуде засноване на пројекту – једноставно
description: Ова тема пружа информације о коришћењу ставки понуде заснованим на пројекту за рад на пројекту. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4865c06691fba09eacf5fe6449adfaf542444520
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272991"
---
# <a name="project-based-quote-lines-overview---lite"></a><span data-ttu-id="bba96-104">Преглед ставки понуде засноване на пројекту – једноставно</span><span class="sxs-lookup"><span data-stu-id="bba96-104">Project-based quote lines overview - lite</span></span>

<span data-ttu-id="bba96-105">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="bba96-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bba96-106">Ставке понуде засноване на пројекту осмишљене су да помогну у процени рада на пројекту при ангажовању.</span><span class="sxs-lookup"><span data-stu-id="bba96-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="bba96-107">Структура ставке понуде на основу пројекта проширена је за процене пројеката следећим концептима:</span><span class="sxs-lookup"><span data-stu-id="bba96-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="bba96-108">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="bba96-108">Billing Method</span></span>
- <span data-ttu-id="bba96-109">Мапирање пројеката и задатака</span><span class="sxs-lookup"><span data-stu-id="bba96-109">Project and Task Mapping</span></span>
- <span data-ttu-id="bba96-110">Укључене класе трансакција</span><span class="sxs-lookup"><span data-stu-id="bba96-110">Included Transaction classes</span></span>
- <span data-ttu-id="bba96-111">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="bba96-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="bba96-112">Подешавање наплативости</span><span class="sxs-lookup"><span data-stu-id="bba96-112">Chargeability setup</span></span>
- <span data-ttu-id="bba96-113">Процена помоћу детаља ставки понуде</span><span class="sxs-lookup"><span data-stu-id="bba96-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="bba96-114">Клијенти ставки понуде</span><span class="sxs-lookup"><span data-stu-id="bba96-114">Quote line Customers</span></span>

<span data-ttu-id="bba96-115">Следећа табела пружа информације о пољима на картици **Општи подаци** ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="bba96-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="bba96-116">Ова поља помажу у постављању основе за детаљну, основну процену рада на пројекту.</span><span class="sxs-lookup"><span data-stu-id="bba96-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="bba96-117">**Поље**</span><span class="sxs-lookup"><span data-stu-id="bba96-117">**Field**</span></span> | <span data-ttu-id="bba96-118">**Опис**</span><span class="sxs-lookup"><span data-stu-id="bba96-118">**Description**</span></span> | <span data-ttu-id="bba96-119">**Последични утицај**</span><span class="sxs-lookup"><span data-stu-id="bba96-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="bba96-120">Именуј</span><span class="sxs-lookup"><span data-stu-id="bba96-120">Name</span></span> | <span data-ttu-id="bba96-121">Назив ставке понуде која би требало да вам помогне да идентификујете дискретну компоненту понуде која се процењује.</span><span class="sxs-lookup"><span data-stu-id="bba96-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="bba96-122">Копира се у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-123">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="bba96-123">Billing Method</span></span> | <span data-ttu-id="bba96-124">У понуди креираној из могућности за пословање, ова вредност се копира из одговарајућег поља у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="bba96-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="bba96-125">Ово поље укључује два главна модела уговарања које Dynamics 365 Project Operations подржава:</span><span class="sxs-lookup"><span data-stu-id="bba96-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="bba96-126">- Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="bba96-126">- Fixed price</span></span></br><span data-ttu-id="bba96-127">- Време и материјал.</span><span class="sxs-lookup"><span data-stu-id="bba96-127">- Time and material.</span></span>| <span data-ttu-id="bba96-128">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-129">Project</span><span class="sxs-lookup"><span data-stu-id="bba96-129">Project</span></span> | <span data-ttu-id="bba96-130">Користите ово опционално поље за идентификовање пројекта који ће се користити за извођење радова при овом ангажовању.</span><span class="sxs-lookup"><span data-stu-id="bba96-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="bba96-131">Када се пројекат мапира у ставку понуде, то помаже у постављању наплативих задатака, као и у доношењу процене засноване на пројекту у ставци понуде као детаље ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="bba96-132">Када пројекат није мапиран у ставку понуде засновану на пројекту, процену треба креирати ручно креирањем сваког детаља ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="bba96-133">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="bba96-134">Обухваћени задаци</span><span class="sxs-lookup"><span data-stu-id="bba96-134">Included Tasks</span></span> | <span data-ttu-id="bba96-135">Означава да ли се ова ставка понуде користи за све или неке пројектне задатке за изабрани пројекат.</span><span class="sxs-lookup"><span data-stu-id="bba96-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="bba96-136">Ово поље подложно уређивању има следеће могуће вредности:</span><span class="sxs-lookup"><span data-stu-id="bba96-136">This field has the following possible values:</span></span></br><span data-ttu-id="bba96-137">- Сви пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="bba96-137">- All project tasks</span></span></br><span data-ttu-id="bba96-138">- Само изабрани пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="bba96-138">- Selected project tasks only</span></span></br><span data-ttu-id="bba96-139">Празна вредност у овом пољу је еквивалентна опцији **Сви пројектни задаци**.</span><span class="sxs-lookup"><span data-stu-id="bba96-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="bba96-140">Када је на страници пројекта изабрана опција **Само изабрани пројектни задаци**, картица **Постављање задатка за обрачун** омогућава вам да изаберете одређене задатке да бисте их повезали са овом ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="bba96-141">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-142">Садржи време</span><span class="sxs-lookup"><span data-stu-id="bba96-142">Include Time</span></span> | <span data-ttu-id="bba96-143">Заставица **Да**/**Не** означава да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="bba96-144">Вредност **Не** означава да временске трансакције или трошкови рада неће бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="bba96-145">Вредност **Да** означава да ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="bba96-146">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-147">Садржи трошак</span><span class="sxs-lookup"><span data-stu-id="bba96-147">Include Expense</span></span> | <span data-ttu-id="bba96-148">Заставица **Да**/**Не** означава да ли ће цене трошкова на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="bba96-149">Вредност **Не** означава да цена трошка неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="bba96-150">Вредност **Да** означава да ће цена трошка бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="bba96-151">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-152">Садржи накнаду</span><span class="sxs-lookup"><span data-stu-id="bba96-152">Include Fee</span></span> | <span data-ttu-id="bba96-153">Заставица **Да**/**Не** означава да ли ће накнаде на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="bba96-154">Вредност **Не** означава да накнаде неће бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="bba96-155">Вредност **Да** означава да ће накнаде бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="bba96-156">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-157">Понуђени износ</span><span class="sxs-lookup"><span data-stu-id="bba96-157">Quoted Amount</span></span> | <span data-ttu-id="bba96-158">Ово је износ који ће бити наведен клијенту за све радове предвиђене у овој ставци понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="bba96-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="bba96-159">У понуди креираној из могућности за пословање, ова вредност се копира из поља **Буџет клијента** у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="bba96-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="bba96-160">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="bba96-161">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-162">Процењени порез</span><span class="sxs-lookup"><span data-stu-id="bba96-162">Estimated Tax</span></span> | <span data-ttu-id="bba96-163">То поље може да уређује корисник да би додао процењени износ пореза у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="bba96-164">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа пореза на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="bba96-165">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-166">Понуђени опорезовани износ</span><span class="sxs-lookup"><span data-stu-id="bba96-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="bba96-167">Ово поље је опорезовани износ ставке понуде и само је за читање.</span><span class="sxs-lookup"><span data-stu-id="bba96-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="bba96-168">Износ у овом пољу се израчунава као *Понуђени износ + порез*.</span><span class="sxs-lookup"><span data-stu-id="bba96-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="bba96-169">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-170">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="bba96-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="bba96-171">Ово поље је могуће уређивати и доступно је само у ставкама понуде заснованим на пројекту чији начин обрачуна је **Време и материјал**.</span><span class="sxs-lookup"><span data-stu-id="bba96-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="bba96-172">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bba96-173">Буџет клијента</span><span class="sxs-lookup"><span data-stu-id="bba96-173">Customer Budget</span></span> | <span data-ttu-id="bba96-174">Ово поље може да се уређује и копира се из одговарајућег поља ставке могућности за пословање ако је понуда креирана из могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="bba96-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="bba96-175">Ово поље се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="bba96-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="bba96-176">Правила за валидацију за поља на картици Општи подаци ставки понуде заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="bba96-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="bba96-177">**1. правило**: Ако је поље **Укључени задаци** празно или ако је подешено на **Сви пројектни задаци**, пројекат је укључен у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="bba96-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="bba96-178">**2. правило**: Ако је поље **Укључени задаци** празно или ако је постављено на **Сви пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени само у једну ставку понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="bba96-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="bba96-179">**3. правило**: Ако је поље **Укључени задаци** постављено на **Само изабрани пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени у више ставки понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="bba96-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="bba96-180">**4. правило**: Ако могућност за пословање има више понуда, могу постојати ставке понуде из различитих понуда које се односе на исти пројекат и укључују исту класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="bba96-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="bba96-181">**5. правило**: Ако понуде не припадају истој могућности за пословање, не могу да укључују исти пројекат и класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="bba96-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="bba96-182">
                    <strong>Могућност за пословање</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="bba96-183">
                    <strong>Понуда</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="bba96-184">
                    <strong>Ставка понуде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="bba96-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="bba96-186">
                    <strong>Обухваћени задаци</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="bba96-187">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="bba96-188">
                    <strong>Садржи трошак</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="bba96-189">
                    <strong>Уврсти</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="bba96-190">
                    <strong>Накнада</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="bba96-191">
                    <strong>Важи / Не важи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="bba96-192">
                    <strong>Разлог</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bba96-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-193">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-194">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-195">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-196">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-197">Празно</span><span class="sxs-lookup"><span data-stu-id="bba96-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-198">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-199">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-200">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-201">Не важи</span><span class="sxs-lookup"><span data-stu-id="bba96-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-202">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="bba96-202">Violation of Rule #2.</span></span> <span data-ttu-id="bba96-203">Време, трошкови и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="bba96-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-204">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-205">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-206">QL2</span><span class="sxs-lookup"><span data-stu-id="bba96-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-207">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-208">Празно</span><span class="sxs-lookup"><span data-stu-id="bba96-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-209">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-210">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-211">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-211">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="bba96-212">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-213">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-214">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-215">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-216">Празно</span><span class="sxs-lookup"><span data-stu-id="bba96-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-217">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-218">Не</span><span class="sxs-lookup"><span data-stu-id="bba96-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-219">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-220">Не важи</span><span class="sxs-lookup"><span data-stu-id="bba96-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-221">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="bba96-221">Violation of Rule #2.</span></span> <span data-ttu-id="bba96-222">Време и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="bba96-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-223">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-224">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-225">QL2</span><span class="sxs-lookup"><span data-stu-id="bba96-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-226">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-227">Празно</span><span class="sxs-lookup"><span data-stu-id="bba96-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-228">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-229">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-230">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-230">Yes</span></span> </p>
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
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-231">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-232">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-233">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-234">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-235">Празно</span><span class="sxs-lookup"><span data-stu-id="bba96-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-236">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-237">Не</span><span class="sxs-lookup"><span data-stu-id="bba96-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-238">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-239">Важећи</span><span class="sxs-lookup"><span data-stu-id="bba96-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="bba96-240">Време и накнаде за пројекат P1 су укључени у QL1.</span><span class="sxs-lookup"><span data-stu-id="bba96-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="bba96-241">Трошкови за пројекат P1 укључени су у QL2.</span><span class="sxs-lookup"><span data-stu-id="bba96-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="bba96-242">Нема преклапања у ономе што је укључено у сваку ставку понуде и што је важеће.</span><span class="sxs-lookup"><span data-stu-id="bba96-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-243">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-244">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-245">QL2</span><span class="sxs-lookup"><span data-stu-id="bba96-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-246">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-247">Празно</span><span class="sxs-lookup"><span data-stu-id="bba96-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-248">Не</span><span class="sxs-lookup"><span data-stu-id="bba96-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-249">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-250">Не</span><span class="sxs-lookup"><span data-stu-id="bba96-250">No</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="bba96-251">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-252">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-253">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-254">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-255">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="bba96-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-256">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-257">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-258">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-259">Не важи</span><span class="sxs-lookup"><span data-stu-id="bba96-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-260">Кршење горенаведеног правила бр. 2</span><span class="sxs-lookup"><span data-stu-id="bba96-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="bba96-261">Q1 укључује време, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="bba96-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="bba96-262">QL2 укључује време, трошкове и накнаде за цео пројекат P1 и преклапа се са оним што је укључено у Q1.</span><span class="sxs-lookup"><span data-stu-id="bba96-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-263">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-264">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-265">QL2</span><span class="sxs-lookup"><span data-stu-id="bba96-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-266">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-267">Празно</span><span class="sxs-lookup"><span data-stu-id="bba96-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-268">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-269">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-270">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-270">Yes</span></span> </p>
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
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-271">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-272">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-273">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-274">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-275">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="bba96-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-276">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-277">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-278">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-279">Важећи</span><span class="sxs-lookup"><span data-stu-id="bba96-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-280">По горенаведеном правилу бр. 3,</span><span class="sxs-lookup"><span data-stu-id="bba96-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="bba96-281">Q1 укључује време, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="bba96-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="bba96-282">QL2 укључује време, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="bba96-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="bba96-283">Једина додатна провера ваљаности односи се на подскуп задатака на QL1 који се разликују од подскупа задатака на QL2.</span><span class="sxs-lookup"><span data-stu-id="bba96-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="bba96-284">Ово осигурава да нема преклапања.</span><span class="sxs-lookup"><span data-stu-id="bba96-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="bba96-285">То систем ради када су задаци повезани.</span><span class="sxs-lookup"><span data-stu-id="bba96-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-286">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-287">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-288">QL2</span><span class="sxs-lookup"><span data-stu-id="bba96-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-289">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-290">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="bba96-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-291">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-292">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-293">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-293">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="bba96-294">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-295">Q1</span><span class="sxs-lookup"><span data-stu-id="bba96-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-296">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-297">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-298">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="bba96-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-299">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-300">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-301">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="bba96-302">Важећи</span><span class="sxs-lookup"><span data-stu-id="bba96-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-303">На основу правила бр. 5, Q1 и Q2 су две понуде у истој могућности за пословање, тако да обе могу проценити исте компоненте пројекта.</span><span class="sxs-lookup"><span data-stu-id="bba96-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-304">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-305">Q2</span><span class="sxs-lookup"><span data-stu-id="bba96-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-306">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-307">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-308">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="bba96-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-309">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-310">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-311">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-311">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="bba96-312">O1</span><span class="sxs-lookup"><span data-stu-id="bba96-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-313">К1</span><span class="sxs-lookup"><span data-stu-id="bba96-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-314">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-315">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-316">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="bba96-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-317">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-318">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-319">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="bba96-320">Важећи</span><span class="sxs-lookup"><span data-stu-id="bba96-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bba96-321">На основу правила бр. 4, Q1 и Q2 су две понуде у различитим могућностима за пословање, тако да оне не могу проценити компоненте истог пројекта.</span><span class="sxs-lookup"><span data-stu-id="bba96-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bba96-322">O2</span><span class="sxs-lookup"><span data-stu-id="bba96-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bba96-323">К1</span><span class="sxs-lookup"><span data-stu-id="bba96-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-324">QL1</span><span class="sxs-lookup"><span data-stu-id="bba96-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-325">P1</span><span class="sxs-lookup"><span data-stu-id="bba96-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="bba96-326">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="bba96-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-327">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bba96-328">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bba96-329">Да</span><span class="sxs-lookup"><span data-stu-id="bba96-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="bba96-330">Не важи</span><span class="sxs-lookup"><span data-stu-id="bba96-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]