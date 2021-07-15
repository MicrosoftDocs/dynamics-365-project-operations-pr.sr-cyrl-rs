---
title: Преглед предмета уговора заснованих на пројекту
description: Ова тема пружа информације о раду са предметима уговора заснованим на пројекту.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 22e8ff927c5ff6c3748a35031e7703e3fcfe0dab
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369934"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="db6e2-103">Преглед предмета уговора заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="db6e2-103">Project-based contract lines overview</span></span>

<span data-ttu-id="db6e2-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="db6e2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="db6e2-105">Предмети уговора засновани на пројекту у услузи Dynamics 365 Project Operations дизајнирани су тако да држе уговоре о процени и обрачуну за одређене компоненте пројектног рада на ангажману.</span><span class="sxs-lookup"><span data-stu-id="db6e2-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="db6e2-106">Структура ставке уговора засноване на пројекту проширена је за процене пројеката и сценарије наплате са следећим концептима:</span><span class="sxs-lookup"><span data-stu-id="db6e2-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="db6e2-107">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="db6e2-107">Billing method</span></span>
- <span data-ttu-id="db6e2-108">Мапирање пројеката и задатака</span><span class="sxs-lookup"><span data-stu-id="db6e2-108">Project and task mapping</span></span>
- <span data-ttu-id="db6e2-109">Укључене класе трансакција</span><span class="sxs-lookup"><span data-stu-id="db6e2-109">Included transaction classes</span></span>
- <span data-ttu-id="db6e2-110">Ограничење које не сме да се прекорачи</span><span class="sxs-lookup"><span data-stu-id="db6e2-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="db6e2-111">Подешавање наплативости</span><span class="sxs-lookup"><span data-stu-id="db6e2-111">Chargeability setup</span></span>
- <span data-ttu-id="db6e2-112">Процене коришћењем детаља о предмета уговора</span><span class="sxs-lookup"><span data-stu-id="db6e2-112">Estimates using contract line details</span></span>
- <span data-ttu-id="db6e2-113">Клијенти предмета уговора</span><span class="sxs-lookup"><span data-stu-id="db6e2-113">Contract line customers</span></span>

<span data-ttu-id="db6e2-114">Следећа табела укључује поља на картици **Општи подаци** предмета уговора заснованих на пројекту који помажу у постављању основе за детаљну, основну процену и аранжмане за обрачун за пројектни рад.</span><span class="sxs-lookup"><span data-stu-id="db6e2-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="db6e2-115">Поље</span><span class="sxs-lookup"><span data-stu-id="db6e2-115">Field</span></span> | <span data-ttu-id="db6e2-116">Опис</span><span class="sxs-lookup"><span data-stu-id="db6e2-116">Description</span></span> | <span data-ttu-id="db6e2-117">Последични утицај</span><span class="sxs-lookup"><span data-stu-id="db6e2-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="db6e2-118">**Именуј**</span><span class="sxs-lookup"><span data-stu-id="db6e2-118">**Name**</span></span> | <span data-ttu-id="db6e2-119">Назив предмета уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-119">Name of the contract line.</span></span> <span data-ttu-id="db6e2-120">Ово идентификује дискретну компоненту уговора која се процењује.</span><span class="sxs-lookup"><span data-stu-id="db6e2-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="db6e2-121">За пројектни уговор креиран из понуде, ова вредност се копира из одговарајуће вредности ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="db6e2-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="db6e2-122">Име копирано у ставку фактуре за пројекат која се креира из овог предмета уговора када се креира фактура.</span><span class="sxs-lookup"><span data-stu-id="db6e2-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="db6e2-123">**Начин наплате**</span><span class="sxs-lookup"><span data-stu-id="db6e2-123">**Billing Method**</span></span> | <span data-ttu-id="db6e2-124">За пројектни уговор креиран из понуде, ова вредност се копира из одговарајућег поља на ставки понуде.</span><span class="sxs-lookup"><span data-stu-id="db6e2-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="db6e2-125">Ово је скуп опција који представља два главна модела уговарања која подржава услуга Project Operations:</span><span class="sxs-lookup"><span data-stu-id="db6e2-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="db6e2-126">- **Фиксна цена**</span><span class="sxs-lookup"><span data-stu-id="db6e2-126">- **Fixed Price**</span></span></br><span data-ttu-id="db6e2-127">- **Време и материјал**</span><span class="sxs-lookup"><span data-stu-id="db6e2-127">- **Time and Material**</span></span> | <span data-ttu-id="db6e2-128">На основу начина наплате наведеног предмета уговора, стварна трансакција ће бити обрађена.</span><span class="sxs-lookup"><span data-stu-id="db6e2-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="db6e2-129">Ако предмет уговора на који се позива стварна вредност има начин наплате времена и материјала, креирају се записи стварних вредности трошкова и ненаплаћене продаје.</span><span class="sxs-lookup"><span data-stu-id="db6e2-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="db6e2-130">Ако предмет уговора на који се позива стварна вредност има начин обрачуна са фиксном ценом, креираће се само стварни трошак.</span><span class="sxs-lookup"><span data-stu-id="db6e2-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="db6e2-131">**Project**</span><span class="sxs-lookup"><span data-stu-id="db6e2-131">**Project**</span></span> | <span data-ttu-id="db6e2-132">Користите ово поље за идентификовање пројекта који ће се користити за извођење радова на овом ангажману.</span><span class="sxs-lookup"><span data-stu-id="db6e2-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="db6e2-133">Ова вредност ће се користити заједно са **Обухваћени задаци** и **Обухваћене класе трансакција** да се реши референца на предмет уговора на стварном или процењеном запису ставке.</span><span class="sxs-lookup"><span data-stu-id="db6e2-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="db6e2-134">**Обухваћени задаци**</span><span class="sxs-lookup"><span data-stu-id="db6e2-134">**Included Tasks**</span></span> | <span data-ttu-id="db6e2-135">Означава да ли ова линија уговора укључује све пројектне задатке за изабрани пројекат или само подскуп задатака.</span><span class="sxs-lookup"><span data-stu-id="db6e2-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="db6e2-136">Ово је скуп опција који има следеће могуће вредности:</span><span class="sxs-lookup"><span data-stu-id="db6e2-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="db6e2-137">- **Сви пројектни задаци**</span><span class="sxs-lookup"><span data-stu-id="db6e2-137">- **All Project Tasks**</span></span></br><span data-ttu-id="db6e2-138">- **Само изабрани пројектни задаци**.</span><span class="sxs-lookup"><span data-stu-id="db6e2-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="db6e2-139">Празна вредност у овом пољу једнака је одабиру **Сви пројектни задаци**.</span><span class="sxs-lookup"><span data-stu-id="db6e2-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="db6e2-140">Ако је изабрана опција **Само изабрани задаци**, можете изабрати одређене задатке и повезати их са овим предметом уговора на картици **Подешавање задатка за обрачун** на страници **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="db6e2-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="db6e2-141">Вредност ће се користити заједно са класама **Пројекат** и **Укључене класе трансакција** да се разреши референца на предмет уговора на стварној вредности или запису предмета процене.</span><span class="sxs-lookup"><span data-stu-id="db6e2-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="db6e2-142">**Садржи време**</span><span class="sxs-lookup"><span data-stu-id="db6e2-142">**Include Time**</span></span> | <span data-ttu-id="db6e2-143">Вредност **Да**/**Не** показује да ли ће временске трансакције или трошкови рада на изабраном пројекту бити укључени у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="db6e2-144">Вредност **Не** означава да временске трансакције или трошкови рада неће бити укључени у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="db6e2-145">Вредност **Да** указује на то да хоће.</span><span class="sxs-lookup"><span data-stu-id="db6e2-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="db6e2-146">Ова вредност се користи заједно са пројектом за решавање референце на предмет уговора на стварном или процењеном запису ставке.</span><span class="sxs-lookup"><span data-stu-id="db6e2-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="db6e2-147">**Садржи трошак**</span><span class="sxs-lookup"><span data-stu-id="db6e2-147">**Include Expense**</span></span> | <span data-ttu-id="db6e2-148">Вредност **Да**/**Не** показује да ли ће цена трошкова на изабраном пројекту бити укључена у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="db6e2-149">Вредност **Не** означава да цена трошкова на изабраном пројекту неће бити укључена у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="db6e2-150">Вредност **Да** указује на то да хоће.</span><span class="sxs-lookup"><span data-stu-id="db6e2-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="db6e2-151">Ова вредност се користи заједно са пројектом за решавање референце на предмет уговора на стварном или процењеном запису ставке.</span><span class="sxs-lookup"><span data-stu-id="db6e2-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="db6e2-152">**Садржи материјале**</span><span class="sxs-lookup"><span data-stu-id="db6e2-152">**Include Materials**</span></span> | <span data-ttu-id="db6e2-153">Вредност **Да**/**Не** показује да ли ће цена материјала на изабраном пројекту бити укључена у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="db6e2-154">Вредност **Не** показује да цена материјала неће бити укључена у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="db6e2-155">Вредност **Да** указује на то да хоће.</span><span class="sxs-lookup"><span data-stu-id="db6e2-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="db6e2-156">Ова вредност се користи заједно са пројектом за решавање референце на предмет уговора на стварном или процењеном запису ставке.</span><span class="sxs-lookup"><span data-stu-id="db6e2-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="db6e2-157">**Садржи надокнаду**</span><span class="sxs-lookup"><span data-stu-id="db6e2-157">**Include Fee**</span></span> | <span data-ttu-id="db6e2-158">Вредност **Да**/**Не** показује да ли ће накнаде на изабраном пројекту бити укључене у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="db6e2-159">Вредност **Не** означава да накнаде неће бити укључене у овај предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="db6e2-160">Вредност **Да** указује на то да хоће.</span><span class="sxs-lookup"><span data-stu-id="db6e2-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="db6e2-161">Ова вредност се користи заједно са пројектом за решавање референце на предмет уговора на стварном или процењеном запису ставке.</span><span class="sxs-lookup"><span data-stu-id="db6e2-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="db6e2-162">**Уговорени износ**</span><span class="sxs-lookup"><span data-stu-id="db6e2-162">**Contracted Amount**</span></span> | <span data-ttu-id="db6e2-163">На предмету уговора са фиксном ценом, овај износ је уговорена вредност која ће се фактурисати клијенту за све радне компоненте повезане са овим предметом уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="db6e2-164">На предмету уговора за време и материјал, овај износ је процењена вредност онога што ће се фактурисати клијенту за све радне компоненте повезане са овим предметом уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="db6e2-165">За пројектни уговор који је креиран из понуде, ова вредност се копира из одговарајућег поља на ставки понуде.</span><span class="sxs-lookup"><span data-stu-id="db6e2-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="db6e2-166">Када предмет уговора заснован на пројекту садржи детаље ставки, ово поље се закључава за уређивање и сажима из износа у детаљима линије уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="db6e2-167">Када предмет уговора садржи детаље ставки, ова вредност се може изменити променом износа на детаљима ставки.</span><span class="sxs-lookup"><span data-stu-id="db6e2-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="db6e2-168">У предмету уговора са фиксном ценом, ова вредност се користи за генерисање износа пре опорезивања на периодичним контролним тачкама обрачуна.</span><span class="sxs-lookup"><span data-stu-id="db6e2-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="db6e2-169">**Процењени порез**</span><span class="sxs-lookup"><span data-stu-id="db6e2-169">**Estimated Tax**</span></span> | <span data-ttu-id="db6e2-170">Корисник може да уређује ово поље како би унео процењени износ пореза у предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="db6e2-171">Када предмет уговора заснован на пројекту садржи детаље ставки, ово поље се закључава за уређивање и сажима из износа пореза у детаљима предмета уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="db6e2-172">Када предмет уговора садржи детаље ставки, ова вредност се може изменити променом износа пореза на детаљима ставки.</span><span class="sxs-lookup"><span data-stu-id="db6e2-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="db6e2-173">У предмету уговора са фиксном ценом, ова вредност се користи за генерисање пореза на периодичним контролним тачкама обрачуна.</span><span class="sxs-lookup"><span data-stu-id="db6e2-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="db6e2-174">**Уговорени износ са порезом**</span><span class="sxs-lookup"><span data-stu-id="db6e2-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="db6e2-175">Износ предмета уговора са порезом.</span><span class="sxs-lookup"><span data-stu-id="db6e2-175">The contract line amount after tax.</span></span> <span data-ttu-id="db6e2-176">Ово поље је само за читање и израчунава се као **Уговорени износ + порез**.</span><span class="sxs-lookup"><span data-stu-id="db6e2-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="db6e2-177">У предмету уговора са фиксном ценом, ова вредност се користи за генерисање периодичних контролних тачака обрачуна.</span><span class="sxs-lookup"><span data-stu-id="db6e2-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="db6e2-178">**Ограничење које не сме да се прекорачи**</span><span class="sxs-lookup"><span data-stu-id="db6e2-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="db6e2-179">Корисник може да уређује ово поље и оно је доступно само на предметима уговора заснованим на пројекту чији начин обрачуна је постављен на време и материјал.</span><span class="sxs-lookup"><span data-stu-id="db6e2-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="db6e2-180">Корисник може да уређује ово поље.</span><span class="sxs-lookup"><span data-stu-id="db6e2-180">The user can edit this field.</span></span> <span data-ttu-id="db6e2-181">Када се стварна вредност за време и материјал односи на овај предмет уговора за време и материјал, износ на стварној вредности се процењује према ограничењу које не сме да се премаши на предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="db6e2-182">Ова процена се завршава након што се обрачунају већ потрошени и преузети износи.</span><span class="sxs-lookup"><span data-stu-id="db6e2-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="db6e2-183">**Буџет клијента**</span><span class="sxs-lookup"><span data-stu-id="db6e2-183">**Customer Budget**</span></span> | <span data-ttu-id="db6e2-184">Ово поље може да се уређује и копира се из одговарајућег поља на ставки понуде ако је уговор креиран из понуде.</span><span class="sxs-lookup"><span data-stu-id="db6e2-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="db6e2-185">Ово поље се користи само за информације и нема никакав даљи значај.</span><span class="sxs-lookup"><span data-stu-id="db6e2-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="db6e2-186">Правила за валидацију за опције на картици Општи подаци за предмете уговора засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="db6e2-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="db6e2-187">Правило 1: Ако је поље **Укључени задаци** празно или подешено на **Сви пројектни задаци**, сви задаци пројекта су укључени у предмет уговора.</span><span class="sxs-lookup"><span data-stu-id="db6e2-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="db6e2-188">Правило 2: Када је поље **Укључени задаци** празно или је изричито постављено на **Сви пројектни задаци**, пројекат и одређена класа трансакција могу бити укључени само у један предмет уговора заснован на пројекту.</span><span class="sxs-lookup"><span data-stu-id="db6e2-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="db6e2-189">Правило 3: Када је поље **Укључени задаци** постављено на **Само изабрани пројектни задаци**, пројекат и одређена класа трансакција могу да се укључе у више предмета уговора заснованих на пројекту.</span><span class="sxs-lookup"><span data-stu-id="db6e2-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="db6e2-190">
                    <strong>Уговор</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="db6e2-191">
                    <strong>Предмет уговора</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="db6e2-192">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="db6e2-193">
                    <strong>Обухваћени задаци</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="db6e2-194">
                    <strong>Садржи време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="db6e2-195">
                    <strong>Садржи трошак</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="db6e2-196">
                    <strong>Садржи материјале</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="db6e2-197">
                    <strong>Уврсти</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="db6e2-198">
                    <strong>Накнада</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="db6e2-199">
                    <strong>Важи / Не важи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="db6e2-200">
                    <strong>Разлог</strong>
                </span><span class="sxs-lookup"><span data-stu-id="db6e2-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-201">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-202">CL1</span><span class="sxs-lookup"><span data-stu-id="db6e2-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-203">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-204">Празно</span><span class="sxs-lookup"><span data-stu-id="db6e2-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-205">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-206">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-207">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-208">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-209">Не важи</span><span class="sxs-lookup"><span data-stu-id="db6e2-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-210">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="db6e2-210">Violation of Rule #2.</span></span> <span data-ttu-id="db6e2-211">Време, трошкови, материјали и накнаде на пројекту П1 укључени су у оба предмета уговора CL1 и CL2.</span><span class="sxs-lookup"><span data-stu-id="db6e2-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-212">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-213">CL2</span><span class="sxs-lookup"><span data-stu-id="db6e2-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-214">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-215">Празно</span><span class="sxs-lookup"><span data-stu-id="db6e2-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-216">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-217">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-218">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-219">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-220">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-221">CL1</span><span class="sxs-lookup"><span data-stu-id="db6e2-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-222">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-223">Празно</span><span class="sxs-lookup"><span data-stu-id="db6e2-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-224">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-225">No</span><span class="sxs-lookup"><span data-stu-id="db6e2-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-226">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-227">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-228">Не важи</span><span class="sxs-lookup"><span data-stu-id="db6e2-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-229">Кршење правила бр. 2.</span><span class="sxs-lookup"><span data-stu-id="db6e2-229">Violation of Rule #2.</span></span> <span data-ttu-id="db6e2-230">Време, трошкови, материјали и накнаде на пројекту P1 укључени су у оба предмета уговора CL1 и CL2.</span><span class="sxs-lookup"><span data-stu-id="db6e2-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-231">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-232">CL2</span><span class="sxs-lookup"><span data-stu-id="db6e2-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-233">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-234">Празно</span><span class="sxs-lookup"><span data-stu-id="db6e2-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-235">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-236">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-237">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-238">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-239">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-240">CL1</span><span class="sxs-lookup"><span data-stu-id="db6e2-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-241">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-242">Празно</span><span class="sxs-lookup"><span data-stu-id="db6e2-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-243">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-244">No</span><span class="sxs-lookup"><span data-stu-id="db6e2-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-245">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-246">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-247">Важеће</span><span class="sxs-lookup"><span data-stu-id="db6e2-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-248">Време, материјали и накнаде за пројекат P1 укључени су у CL1.</span><span class="sxs-lookup"><span data-stu-id="db6e2-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="db6e2-249">Трошкови за пројекат P1 укључени су у CL2.</span><span class="sxs-lookup"><span data-stu-id="db6e2-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="db6e2-250">Нема преклапања у ономе што је укључено у сваки предмет уговора и стога је важеће.</span><span class="sxs-lookup"><span data-stu-id="db6e2-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-251">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-252">CL2</span><span class="sxs-lookup"><span data-stu-id="db6e2-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-253">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-254">Празно</span><span class="sxs-lookup"><span data-stu-id="db6e2-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-255">No</span><span class="sxs-lookup"><span data-stu-id="db6e2-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-256">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-257">No</span><span class="sxs-lookup"><span data-stu-id="db6e2-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-258">No</span><span class="sxs-lookup"><span data-stu-id="db6e2-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-259">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-260">CL1</span><span class="sxs-lookup"><span data-stu-id="db6e2-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-261">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-262">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="db6e2-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-263">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-264">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-265">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-266">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-267">Не важи</span><span class="sxs-lookup"><span data-stu-id="db6e2-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-268">Кршење правила бр. 2</span><span class="sxs-lookup"><span data-stu-id="db6e2-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="db6e2-269">C1 укључује време, материјале, трошкове и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="db6e2-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="db6e2-270">CL2 укључује време, материјале, трошкове и накнаде за цео пројекат P1 и стога се преклапа са оним што је укључено у C1.</span><span class="sxs-lookup"><span data-stu-id="db6e2-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-271">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-272">CL2</span><span class="sxs-lookup"><span data-stu-id="db6e2-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-273">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-274">Празно</span><span class="sxs-lookup"><span data-stu-id="db6e2-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-275">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-276">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-277">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-278">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-279">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-280">CL1</span><span class="sxs-lookup"><span data-stu-id="db6e2-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-281">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-282">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="db6e2-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-283">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-284">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-285">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-286">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-287">Важеће</span><span class="sxs-lookup"><span data-stu-id="db6e2-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="db6e2-288">По правилу бр. 3</span><span class="sxs-lookup"><span data-stu-id="db6e2-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="db6e2-289">C1 укључује време, трошкове, материјале и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="db6e2-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="db6e2-290">CL2 укључује време, трошкове, материјале и накнаде за подскуп задатака на пројекту P1.</span><span class="sxs-lookup"><span data-stu-id="db6e2-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="db6e2-291">Једина додатна провера ваљаности око подскупа задатака на CL1 разликује се од подскупа задатака на CL2 како би се осигурало да тамо нема преклапања.</span><span class="sxs-lookup"><span data-stu-id="db6e2-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="db6e2-292">То систем ради када су задаци повезани.</span><span class="sxs-lookup"><span data-stu-id="db6e2-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="db6e2-293">C1</span><span class="sxs-lookup"><span data-stu-id="db6e2-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="db6e2-294">CL2</span><span class="sxs-lookup"><span data-stu-id="db6e2-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-295">П1</span><span class="sxs-lookup"><span data-stu-id="db6e2-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="db6e2-296">Само изабрани задаци</span><span class="sxs-lookup"><span data-stu-id="db6e2-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-297">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="db6e2-298">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-299">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="db6e2-300">Да</span><span class="sxs-lookup"><span data-stu-id="db6e2-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
