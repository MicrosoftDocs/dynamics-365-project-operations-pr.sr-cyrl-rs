---
title: Преглед ставки понуде засноване на пројекту
description: Ова тема пружа информације о коришћењу ставки понуде заснованим на пројекту за рад на пројекту.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cfe98fc89130c93dd0a36af8583881fdcb4550c0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858716"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="1f5b0-103">Преглед ставки понуде засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="1f5b0-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="1f5b0-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре, Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="1f5b0-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1f5b0-105">Ставке понуде засноване на пројекту осмишљене су да помогну у процени рада на пројекту при ангажовању.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="1f5b0-106">Структура ставке понуде на основу пројекта проширена је за процене пројеката следећим концептима:</span><span class="sxs-lookup"><span data-stu-id="1f5b0-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="1f5b0-107">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="1f5b0-107">Billing Method</span></span>
- <span data-ttu-id="1f5b0-108">Мапирање пројеката и задатака</span><span class="sxs-lookup"><span data-stu-id="1f5b0-108">Project and Task Mapping</span></span>
- <span data-ttu-id="1f5b0-109">Укључене класе трансакција</span><span class="sxs-lookup"><span data-stu-id="1f5b0-109">Included Transaction classes</span></span>
- <span data-ttu-id="1f5b0-110">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="1f5b0-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="1f5b0-111">Подешавање наплативости</span><span class="sxs-lookup"><span data-stu-id="1f5b0-111">Chargeability setup</span></span>
- <span data-ttu-id="1f5b0-112">Процена помоћу детаља ставки понуде</span><span class="sxs-lookup"><span data-stu-id="1f5b0-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="1f5b0-113">Клијенти ставки понуде</span><span class="sxs-lookup"><span data-stu-id="1f5b0-113">Quote line Customers</span></span>

<span data-ttu-id="1f5b0-114">Следећа табела пружа информације о пољима на картици **Општи подаци** ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="1f5b0-115">Ова поља помажу у постављању основе за детаљну, основну процену рада на пројекту.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="1f5b0-116">**Поље**</span><span class="sxs-lookup"><span data-stu-id="1f5b0-116">**Field**</span></span> | <span data-ttu-id="1f5b0-117">**Опис**</span><span class="sxs-lookup"><span data-stu-id="1f5b0-117">**Description**</span></span> | <span data-ttu-id="1f5b0-118">**Последични утицај**</span><span class="sxs-lookup"><span data-stu-id="1f5b0-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1f5b0-119">Име</span><span class="sxs-lookup"><span data-stu-id="1f5b0-119">Name</span></span> | <span data-ttu-id="1f5b0-120">Назив понуде који вам помаже да препознате дискретну компоненту понуде која се процењује.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="1f5b0-121">Копира се у предмет уговора о пројекту који се креира из ове ставке понуде када се понуда оствари.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-122">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="1f5b0-122">Billing Method</span></span> | <span data-ttu-id="1f5b0-123">У понуди креираној из могућности за пословање, ова вредност се копира из одговарајућег поља у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="1f5b0-124">Ово поље укључује два главна модела уговарања које Dynamics 365 Project Operations подржава:</span><span class="sxs-lookup"><span data-stu-id="1f5b0-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="1f5b0-125">- Фиксна цена</span><span class="sxs-lookup"><span data-stu-id="1f5b0-125">- Fixed price</span></span></br><span data-ttu-id="1f5b0-126">- Време и материјал.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-126">- Time and material.</span></span>| <span data-ttu-id="1f5b0-127">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-128">Project</span><span class="sxs-lookup"><span data-stu-id="1f5b0-128">Project</span></span> | <span data-ttu-id="1f5b0-129">Користите ово опционално поље за идентификовање пројекта који ће се користити за извођење радова при овом ангажовању.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="1f5b0-130">Када се пројекат мапира у ставку понуде, то помаже у постављању наплативих задатака, као и у доношењу процене засноване на пројекту у ставци понуде као детаље ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="1f5b0-131">Када пројекат није мапиран у ставку понуде засновану на пројекту, процену треба креирати ручно креирањем сваког детаља ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="1f5b0-132">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="1f5b0-133">Обухваћени задаци</span><span class="sxs-lookup"><span data-stu-id="1f5b0-133">Included Tasks</span></span> | <span data-ttu-id="1f5b0-134">Означава да ли се ова ставка понуде користи за све или неке пројектне задатке за изабрани пројекат.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="1f5b0-135">Ово поље подложно уређивању има следеће могуће вредности:</span><span class="sxs-lookup"><span data-stu-id="1f5b0-135">This field has the following possible values:</span></span></br><span data-ttu-id="1f5b0-136">- Сви пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="1f5b0-136">- All project tasks</span></span></br><span data-ttu-id="1f5b0-137">- Само изабрани пројектни задаци</span><span class="sxs-lookup"><span data-stu-id="1f5b0-137">- Selected project tasks only</span></span></br><span data-ttu-id="1f5b0-138">Празна вредност у овом пољу је еквивалентна опцији **Сви пројектни задаци**.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="1f5b0-139">Када се на страници пројекта изабере **Само изабрани пројектни задаци**, картица **Подешавање наплате за задатак** вам омогућава да изаберете одређене задатке да бисте их повезали са овом ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="1f5b0-140">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-141">Садржи време</span><span class="sxs-lookup"><span data-stu-id="1f5b0-141">Include Time</span></span> | <span data-ttu-id="1f5b0-142">Вредност **Да**/**Не** показује да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-143">Вредност **Не** означава да временске трансакције или трошкови рада неће бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-144">Вредност **Да** означава да ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="1f5b0-145">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-146">Садржи трошак</span><span class="sxs-lookup"><span data-stu-id="1f5b0-146">Include Expense</span></span> | <span data-ttu-id="1f5b0-147">Вредност **Да**/**Не** показује да ли ће цена трошкова на изабраном пројекту бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-148">Вредност **Не** означава да цена трошка неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-149">Вредност **Да** означава да ће цена трошка бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="1f5b0-150">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-151">Садржи материјал</span><span class="sxs-lookup"><span data-stu-id="1f5b0-151">Include Material</span></span> | <span data-ttu-id="1f5b0-152">Вредност **Да**/**Не** показује да ли ће цена материјала на изабраном пројекту бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-153">Вредност **Не** показује да цена материјала неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-154">Вредност **Да** показује да цена материјала неће бити укључена у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="1f5b0-155">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-156">Садржи надокнаду</span><span class="sxs-lookup"><span data-stu-id="1f5b0-156">Include Fee</span></span> | <span data-ttu-id="1f5b0-157">Вредност **Да**/**Не** показује да ли ће накнаде на изабраном пројекту бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-158">Вредност **Не** означава да накнаде неће бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="1f5b0-159">Вредност **Да** означава да ће накнаде бити укључене у процену ове ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="1f5b0-160">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-161">Понуђени износ</span><span class="sxs-lookup"><span data-stu-id="1f5b0-161">Quoted Amount</span></span> | <span data-ttu-id="1f5b0-162">Ово је износ који ће бити наведен клијенту за све радове предвиђене на овој ставци понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="1f5b0-163">У понуди креираној из могућности за пословање, ова вредност се копира из поља **Буџет клијента** у ставци могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="1f5b0-164">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="1f5b0-165">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-166">Процењени порез</span><span class="sxs-lookup"><span data-stu-id="1f5b0-166">Estimated Tax</span></span> | <span data-ttu-id="1f5b0-167">То поље може да уређује корисник да би додао процењени износ пореза у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="1f5b0-168">Када ставка понуде заснована на пројекту садржи детаље о ставци, ово поље је закључано за уређивање и резимирано је из износа пореза на детаљима ставке понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="1f5b0-169">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-170">Понуђени опорезовани износ</span><span class="sxs-lookup"><span data-stu-id="1f5b0-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="1f5b0-171">Ово поље је опорезовани износ ставке понуде и само је за читање.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="1f5b0-172">Износ у овом пољу се израчунава као *Понуђени износ + порез*.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="1f5b0-173">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-174">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="1f5b0-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="1f5b0-175">Ово поље је могуће уређивати и доступно је само у ставкама понуде заснованим на пројекту чији начин обрачуна је **Време и материјал**.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="1f5b0-176">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="1f5b0-177">Буџет клијента</span><span class="sxs-lookup"><span data-stu-id="1f5b0-177">Customer Budget</span></span> | <span data-ttu-id="1f5b0-178">Ово поље може да се уређује и копира се из одговарајућег поља ставке могућности за пословање ако је понуда креирана из могућности за пословање.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="1f5b0-179">Ова вредност се копира у предмет уговора о пројекту који се креира из ове ставке понуде када се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="1f5b0-180">Правила за валидацију за поља на картици Општи подаци ставки понуде заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="1f5b0-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="1f5b0-181">**1. правило**: Ако је поље **Укључени задаци** празно или ако је подешено на **Сви пројектни задаци**, пројекат је укључен у ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="1f5b0-182">**2. правило**: Ако је поље **Укључени задаци** празно или ако је постављено на **Сви пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени само у једну ставку понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="1f5b0-183">**3. правило**: Ако је поље **Укључени задаци** постављено на **Само изабрани пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени у више ставки понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="1f5b0-184">**4. правило**: Ако могућност за пословање има више понуда, могу постојати ставке понуде из различитих понуда које се односе на исти пројекат и укључују исту класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="1f5b0-185">**5. правило**: Ако понуде не припадају истој могућности за пословање, не могу да укључују исти пројекат и класу трансакције.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="1f5b0-186">
                    <strong>Могућност за пословање</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="1f5b0-187">
                    <strong>Понуда</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="1f5b0-188">
                    <strong>Ставка понуде</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="1f5b0-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="1f5b0-190">
                    <strong>Обухваћени задаци</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="1f5b0-191">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="1f5b0-192">
                    <strong>Садржи трошак</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="1f5b0-193">
                    <strong>Садржи материјал</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="1f5b0-194">
                    <strong>Уврсти</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="1f5b0-195">
                    <strong>Накнада</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="1f5b0-196">
                    <strong>Важи / Не важи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="1f5b0-197">
                    <strong>Разлог</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1f5b0-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-198">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-199">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-200">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-201">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-202">Празно</span><span class="sxs-lookup"><span data-stu-id="1f5b0-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-203">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-204">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-205">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-206">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-207">Не важи</span><span class="sxs-lookup"><span data-stu-id="1f5b0-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-208">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-208">Violation of Rule #2.</span></span> <span data-ttu-id="1f5b0-209">Време, трошкови и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-210">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-211">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-212">QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-213">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-214">Празно</span><span class="sxs-lookup"><span data-stu-id="1f5b0-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-215">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-216">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-217">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-218">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-218">Yes</span></span> </p>
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
<span data-ttu-id="1f5b0-219">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-220">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-221">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-222">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-223">Празно</span><span class="sxs-lookup"><span data-stu-id="1f5b0-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-224">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-225">No</span><span class="sxs-lookup"><span data-stu-id="1f5b0-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-226">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-227">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-228">Не важи</span><span class="sxs-lookup"><span data-stu-id="1f5b0-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-229">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-229">Violation of Rule #2.</span></span> <span data-ttu-id="1f5b0-230">Време, материјал и накнаде за пројекат P1 укључени су у ставке понуде QL1 и QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-231">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-232">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-233">QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-234">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-235">Празно</span><span class="sxs-lookup"><span data-stu-id="1f5b0-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-236">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-237">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-238">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-239">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-239">Yes</span></span> </p>
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
<span data-ttu-id="1f5b0-240">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-241">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-242">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-243">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-244">Празно</span><span class="sxs-lookup"><span data-stu-id="1f5b0-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-245">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-246">No</span><span class="sxs-lookup"><span data-stu-id="1f5b0-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-247">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-248">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-249">Важеће</span><span class="sxs-lookup"><span data-stu-id="1f5b0-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-250">Време, материјал и накнаде за пројекат P1 укључени су у QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="1f5b0-251">Трошкови за пројекат P1 укључени су у QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="1f5b0-252">Нема преклапања у ономе што је укључено у сваку ставку понуде и стога је важеће.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-253">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-254">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-255">QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-256">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-257">Празно</span><span class="sxs-lookup"><span data-stu-id="1f5b0-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-258">No</span><span class="sxs-lookup"><span data-stu-id="1f5b0-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-259">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-260">No</span><span class="sxs-lookup"><span data-stu-id="1f5b0-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-261">No</span><span class="sxs-lookup"><span data-stu-id="1f5b0-261">No</span></span> </p>
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
<span data-ttu-id="1f5b0-262">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-263">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-264">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-265">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-266">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="1f5b0-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-267">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-268">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-269">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-270">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-271">Не важи</span><span class="sxs-lookup"><span data-stu-id="1f5b0-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-272">Кршење правила бр. 2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="1f5b0-273">Q1 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="1f5b0-274">QL2 укључује време, трошкове и накнаде за цео пројекат P1 и стога се преклапа са оним што је укључено у Q1.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-275">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-276">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-277">QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-278">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-279">Празно</span><span class="sxs-lookup"><span data-stu-id="1f5b0-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-280">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-281">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-282">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-283">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-283">Yes</span></span> </p>
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
<span data-ttu-id="1f5b0-284">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-285">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-286">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-287">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-288">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="1f5b0-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-289">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-290">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-291">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-292">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-293">Важеће</span><span class="sxs-lookup"><span data-stu-id="1f5b0-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-294">По правилу бр. 3,</span><span class="sxs-lookup"><span data-stu-id="1f5b0-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="1f5b0-295">Q1 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="1f5b0-296">QL2 укључује време, материјал, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="1f5b0-297">Једина додатна провера ваљаности око подскупа задатака на QL1 која се разликује од подскупа задатака на QL2 како би се осигурало да тамо нема преклапања.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="1f5b0-298">То систем ради када су задаци повезани.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-299">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-300">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-301">QL2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-302">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-303">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="1f5b0-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-304">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-305">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-306">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-307">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-307">Yes</span></span> </p>
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
<span data-ttu-id="1f5b0-308">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-309">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-310">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-311">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-312">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="1f5b0-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-313">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-314">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-315">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-316">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-317">Важеће</span><span class="sxs-lookup"><span data-stu-id="1f5b0-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-318">По правилу бр. 5, Q1 и Q2 су две понуде у истој могућности за пословање, тако да се могу обе проценити за исте компоненте пројекта.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-319">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-320">К2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-321">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-322">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-323">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="1f5b0-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-324">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-325">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-326">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-327">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-327">Yes</span></span> </p>
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
<span data-ttu-id="1f5b0-328">O1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-329">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-330">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-331">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-332">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="1f5b0-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-333">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-334">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-335">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-336">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-337">Не важи</span><span class="sxs-lookup"><span data-stu-id="1f5b0-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1f5b0-338">По правилу бр. 4, Q1 и Q2 су две понуде у различитим могућностима за пословање, тако да се не могу проценити за исте компоненте истог пројекта.</span><span class="sxs-lookup"><span data-stu-id="1f5b0-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="1f5b0-339">O2</span><span class="sxs-lookup"><span data-stu-id="1f5b0-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="1f5b0-340">К1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="1f5b0-341">QL1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-342">П1</span><span class="sxs-lookup"><span data-stu-id="1f5b0-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="1f5b0-343">Сви пројектни задаци или празни</span><span class="sxs-lookup"><span data-stu-id="1f5b0-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="1f5b0-344">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="1f5b0-345">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="1f5b0-346">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="1f5b0-347">Да</span><span class="sxs-lookup"><span data-stu-id="1f5b0-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
