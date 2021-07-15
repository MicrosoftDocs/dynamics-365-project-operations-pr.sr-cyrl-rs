---
title: Преглед ставки понуде засноване на пројекту
description: Ова тема пружа информације о коришћењу ставки понуде заснованим на пројекту за рад на пројекту.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: b7076a4b9280472f8c30d0b58c3aa9b9bc86d651
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369889"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="c1f3b-103">Преглед ставки понуде засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="c1f3b-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="c1f3b-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре, Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="c1f3b-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c1f3b-105">Ставке понуде засноване на пројекту осмишљене су да помогну у процени рада на пројекту при ангажовању.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="c1f3b-106">Структура ставке понуде на основу пројекта проширена је за процене пројеката следећим концептима:</span><span class="sxs-lookup"><span data-stu-id="c1f3b-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="c1f3b-107">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="c1f3b-107">Billing Method</span></span>
- <span data-ttu-id="c1f3b-108">Мапирање пројеката и задатака</span><span class="sxs-lookup"><span data-stu-id="c1f3b-108">Project and Task Mapping</span></span>
- <span data-ttu-id="c1f3b-109">Укључене класе трансакција</span><span class="sxs-lookup"><span data-stu-id="c1f3b-109">Included Transaction classes</span></span>
- <span data-ttu-id="c1f3b-110">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="c1f3b-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="c1f3b-111">Подешавање наплативости</span><span class="sxs-lookup"><span data-stu-id="c1f3b-111">Chargeability setup</span></span>
- <span data-ttu-id="c1f3b-112">Процена помоћу детаља ставки понуде</span><span class="sxs-lookup"><span data-stu-id="c1f3b-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="c1f3b-113">Клијенти ставки понуде</span><span class="sxs-lookup"><span data-stu-id="c1f3b-113">Quote line Customers</span></span>

<span data-ttu-id="c1f3b-114">Следећа табела пружа информације о пољима на картици **Општи подаци** ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="c1f3b-115">Ова поља помажу у постављању основе за детаљну, основну процену рада на пројекту.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="c1f3b-116">**Поље**</span><span class="sxs-lookup"><span data-stu-id="c1f3b-116">**Field**</span></span> | <span data-ttu-id="c1f3b-117">**Опис**</span><span class="sxs-lookup"><span data-stu-id="c1f3b-117">**Description**</span></span> | <span data-ttu-id="c1f3b-118">**Последични утицај**</span><span class="sxs-lookup"><span data-stu-id="c1f3b-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c1f3b-119">Име</span><span class="sxs-lookup"><span data-stu-id="c1f3b-119">Name</span></span> | <span data-ttu-id="c1f3b-120">Назив понуде који вам помаже да препознате дискретну компоненту понуде која се процењује.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="c1f3b-121">Копира се у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-122">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="c1f3b-122">Billing Method</span></span> | <span data-ttu-id="c1f3b-123">У понуди креираној из могућности за пословање, ова вредност се копира из одговарајућег поља у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="c1f3b-124">Ово поље укључује два главна модела уговарања које Dynamics 365 Project Operations подржава:</span><span class="sxs-lookup"><span data-stu-id="c1f3b-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="c1f3b-125">- Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="c1f3b-125">- Fixed price</span></span></br><span data-ttu-id="c1f3b-126">- Време и материјал.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-126">- Time and material.</span></span>| <span data-ttu-id="c1f3b-127">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-128">Project</span><span class="sxs-lookup"><span data-stu-id="c1f3b-128">Project</span></span> | <span data-ttu-id="c1f3b-129">Користите ово опционално поље за идентификовање пројекта који ће се користити за извођење радова при овом ангажовању.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="c1f3b-130">Када се пројекат мапира у ставку понуде, то помаже у постављању наплативих задатака, као и у доношењу процене засноване на пројекту у ставци понуде као детаље ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="c1f3b-131">Када пројекат није мапиран у ставку понуде засновану на пројекту, процену треба креирати ручно креирањем сваког детаља ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="c1f3b-132">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="c1f3b-133">Обухваћени задаци</span><span class="sxs-lookup"><span data-stu-id="c1f3b-133">Included Tasks</span></span> | <span data-ttu-id="c1f3b-134">Означава да ли се ова ставка понуде користи за све или неке пројектне задатке за изабрани пројекат.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="c1f3b-135">Ово поље подложно уређивању има следеће могуће вредности:</span><span class="sxs-lookup"><span data-stu-id="c1f3b-135">This field has the following possible values:</span></span></br><span data-ttu-id="c1f3b-136">- Сви пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="c1f3b-136">- All project tasks</span></span></br><span data-ttu-id="c1f3b-137">- Само изабрани пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="c1f3b-137">- Selected project tasks only</span></span></br><span data-ttu-id="c1f3b-138">Празна вредност у овом пољу је еквивалентна опцији **Сви пројектни задаци**.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="c1f3b-139">Када се на страници пројекта изабере **Само изабрани пројектни задаци**, картица **Подешавање наплате за задатак** вам омогућава да изаберете одређене задатке да бисте их повезали са овом ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="c1f3b-140">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-141">Садржи време</span><span class="sxs-lookup"><span data-stu-id="c1f3b-141">Include Time</span></span> | <span data-ttu-id="c1f3b-142">Вредност **Да**/**Не** показује да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-143">Вредност **Не** означава да временске трансакције или трошкови рада неће бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-144">Вредност **Да** означава да ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c1f3b-145">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-146">Садржи трошак</span><span class="sxs-lookup"><span data-stu-id="c1f3b-146">Include Expense</span></span> | <span data-ttu-id="c1f3b-147">Вредност **Да**/**Не** показује да ли ће цена трошкова на изабраном пројекту бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-148">Вредност **Не** означава да цена трошка неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-149">Вредност **Да** означава да ће цена трошка бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c1f3b-150">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-151">Садржи материјал</span><span class="sxs-lookup"><span data-stu-id="c1f3b-151">Include Material</span></span> | <span data-ttu-id="c1f3b-152">Вредност **Да**/**Не** показује да ли ће цена материјала на изабраном пројекту бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-153">Вредност **Не** показује да цена материјала неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-154">Вредност **Да** показује да цена материјала неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c1f3b-155">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-156">Садржи надокнаду</span><span class="sxs-lookup"><span data-stu-id="c1f3b-156">Include Fee</span></span> | <span data-ttu-id="c1f3b-157">Вредност **Да**/**Не** показује да ли ће накнаде на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-158">Вредност **Не** означава да накнаде неће бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="c1f3b-159">Вредност **Да** означава да ће накнаде бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="c1f3b-160">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-161">Понуђени износ</span><span class="sxs-lookup"><span data-stu-id="c1f3b-161">Quoted Amount</span></span> | <span data-ttu-id="c1f3b-162">Ово је износ који ће бити наведен клијенту за све радове предвиђене на овој ставци понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="c1f3b-163">У понуди креираној из могућности за пословање, ова вредност се копира из поља **Буџет клијента** у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="c1f3b-164">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="c1f3b-165">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-166">Процењени порез</span><span class="sxs-lookup"><span data-stu-id="c1f3b-166">Estimated Tax</span></span> | <span data-ttu-id="c1f3b-167">То поље може да уређује корисник да би додао процењени износ пореза у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="c1f3b-168">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа пореза на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="c1f3b-169">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-170">Понуђени опорезовани износ</span><span class="sxs-lookup"><span data-stu-id="c1f3b-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="c1f3b-171">Ово поље је опорезовани износ ставке понуде и само је за читање.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="c1f3b-172">Износ у овом пољу се израчунава као *Понуђени износ + порез*.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="c1f3b-173">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-174">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="c1f3b-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="c1f3b-175">Ово поље је могуће уређивати и доступно је само у ставкама понуде заснованим на пројекту чији начин обрачуна је **Време и материјал**.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="c1f3b-176">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="c1f3b-177">Буџет клијента</span><span class="sxs-lookup"><span data-stu-id="c1f3b-177">Customer Budget</span></span> | <span data-ttu-id="c1f3b-178">Ово поље може да се уређује и копира се из одговарајућег поља ставке могућности за пословање ако је понуда креирана из могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="c1f3b-179">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="c1f3b-180">Правила за валидацију за поља на картици Општи подаци ставки понуде заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="c1f3b-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="c1f3b-181">**1. правило**: Ако је поље **Укључени задаци** празно или ако је подешено на **Сви пројектни задаци**, пројекат је укључен у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="c1f3b-182">**2. правило**: Ако је поље **Укључени задаци** празно или ако је постављено на **Сви пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени само у једну ставку понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="c1f3b-183">**3. правило**: Ако је поље **Укључени задаци** постављено на **Само изабрани пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени у више ставки понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="c1f3b-184">**4. правило**: Ако могућност за пословање има више понуда, могу постојати ставке понуде из различитих понуда које се односе на исти пројекат и укључују исту класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="c1f3b-185">**5. правило**: Ако понуде не припадају истој могућности за пословање, не могу да укључују исти пројекат и класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="c1f3b-186">
                    <strong>Могућност за пословање</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="c1f3b-187">
                    <strong>Понуда</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="c1f3b-188">
                    <strong>Ставка понуде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="c1f3b-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="c1f3b-190">
                    <strong>Обухваћени задаци</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="c1f3b-191">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="c1f3b-192">
                    <strong>Садржи трошак</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="c1f3b-193">
                    <strong>Садржи материјал</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="c1f3b-194">
                    <strong>Уврсти</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="c1f3b-195">
                    <strong>Накнада</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="c1f3b-196">
                    <strong>Важи / Не важи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="c1f3b-197">
                    <strong>Разлог</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1f3b-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-198">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-199">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-200">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-201">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-202">Празно</span><span class="sxs-lookup"><span data-stu-id="c1f3b-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-203">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-204">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-205">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-206">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-207">Не важи</span><span class="sxs-lookup"><span data-stu-id="c1f3b-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-208">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-208">Violation of Rule #2.</span></span> <span data-ttu-id="c1f3b-209">Време, трошкови и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-210">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-211">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-212">QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-213">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-214">Празно</span><span class="sxs-lookup"><span data-stu-id="c1f3b-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-215">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-216">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-217">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-218">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-219">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-220">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-221">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-222">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-223">Празно</span><span class="sxs-lookup"><span data-stu-id="c1f3b-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-224">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-225">No</span><span class="sxs-lookup"><span data-stu-id="c1f3b-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-226">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-227">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-228">Не важи</span><span class="sxs-lookup"><span data-stu-id="c1f3b-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-229">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-229">Violation of Rule #2.</span></span> <span data-ttu-id="c1f3b-230">Време, материјал и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-231">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-232">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-233">QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-234">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-235">Празно</span><span class="sxs-lookup"><span data-stu-id="c1f3b-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-236">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-237">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-238">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-239">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-240">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-241">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-242">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-243">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-244">Празно</span><span class="sxs-lookup"><span data-stu-id="c1f3b-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-245">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-246">No</span><span class="sxs-lookup"><span data-stu-id="c1f3b-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-247">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-248">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-249">Важеће</span><span class="sxs-lookup"><span data-stu-id="c1f3b-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-250">Време, материјал и накнаде за пројекат P1 укључени су у QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="c1f3b-251">Трошкови за пројекат P1 укључени су у QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="c1f3b-252">Нема преклапања у ономе што је укључено у сваку ставку понуде и стога је важеће.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-253">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-254">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-255">QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-256">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-257">Празно</span><span class="sxs-lookup"><span data-stu-id="c1f3b-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-258">No</span><span class="sxs-lookup"><span data-stu-id="c1f3b-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-259">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-260">No</span><span class="sxs-lookup"><span data-stu-id="c1f3b-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-261">No</span><span class="sxs-lookup"><span data-stu-id="c1f3b-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-262">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-263">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-264">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-265">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-266">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c1f3b-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-267">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-268">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-269">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-270">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-271">Не важи</span><span class="sxs-lookup"><span data-stu-id="c1f3b-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-272">Кршење правила бр. 2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="c1f3b-273">Q1 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="c1f3b-274">QL2 укључује време, трошкове и накнаде за цео пројекат P1 и стога се преклапа са оним што је укључено у Q1.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-275">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-276">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-277">QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-278">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-279">Празно</span><span class="sxs-lookup"><span data-stu-id="c1f3b-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-280">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-281">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-282">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-283">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-284">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-285">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-286">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-287">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-288">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c1f3b-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-289">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-290">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-291">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-292">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-293">Важеће</span><span class="sxs-lookup"><span data-stu-id="c1f3b-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-294">По правилу бр. 3,</span><span class="sxs-lookup"><span data-stu-id="c1f3b-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="c1f3b-295">Q1 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="c1f3b-296">QL2 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="c1f3b-297">Једина додатна провера ваљаности око подскупа задатака на QL1 која се разликује од подскупа задатака на QL2 како би се осигурало да тамо нема преклапања.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="c1f3b-298">То систем ради када су задаци повезани.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-299">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-300">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-301">QL2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-302">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-303">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="c1f3b-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-304">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-305">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-306">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-307">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-308">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-309">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-310">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-311">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-312">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="c1f3b-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-313">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-314">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-315">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-316">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-317">Важеће</span><span class="sxs-lookup"><span data-stu-id="c1f3b-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-318">По правилу бр. 5, Q1 и Q2 су две понуде у истој могућности за пословање, тако да се могу обе проценити за исте компоненте пројекта.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-319">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-320">К2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-321">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-322">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-323">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="c1f3b-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-324">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-325">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-326">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-327">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-328">O1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-329">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-330">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-331">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-332">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="c1f3b-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-333">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-334">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-335">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-336">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-337">Не важи</span><span class="sxs-lookup"><span data-stu-id="c1f3b-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c1f3b-338">По правилу бр. 4, Q1 и Q2 су две понуде у различитим могућностима за пословање, тако да се не могу проценити за исте компоненте истог пројекта.</span><span class="sxs-lookup"><span data-stu-id="c1f3b-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="c1f3b-339">O2</span><span class="sxs-lookup"><span data-stu-id="c1f3b-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="c1f3b-340">К1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="c1f3b-341">QL1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-342">П1</span><span class="sxs-lookup"><span data-stu-id="c1f3b-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="c1f3b-343">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="c1f3b-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="c1f3b-344">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="c1f3b-345">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="c1f3b-346">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="c1f3b-347">Да</span><span class="sxs-lookup"><span data-stu-id="c1f3b-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
