---
title: Конфигурисање управљања трошковима
description: Овај чланак описује разматрања и одлуке које морате донети током процеса планирања пре него што конфигуришете управљање трошковима у услузи Microsoft Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: db3529597c662a326730cf6a0b855ae865f0dce5
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960355"
---
# <a name="configure-expense-management"></a><span data-ttu-id="326dd-103">Конфигурисање управљања трошковима</span><span class="sxs-lookup"><span data-stu-id="326dd-103">Configure expense management</span></span>

<span data-ttu-id="326dd-104">Ова тема описује разматрања и одлуке које морате донети током процеса планирања пре него што конфигуришете управљање трошковима.</span><span class="sxs-lookup"><span data-stu-id="326dd-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="326dd-105">У управљању трошковима можете да чувате информације о начинима плаћања, путним захтевима, извештајима о трошковима, смерницама итд.</span><span class="sxs-lookup"><span data-stu-id="326dd-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="326dd-106">Будући да се многе одлуке које доносите када планирате конфигурацију за управљање трошковима заснивају на хијерархији и финансијској структури ваше организације, морате погледати документе за планирање за та подручја.</span><span class="sxs-lookup"><span data-stu-id="326dd-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="326dd-107">Међукомпанијски трошкови</span><span class="sxs-lookup"><span data-stu-id="326dd-107">Intercompany expenses</span></span>

<span data-ttu-id="326dd-108">Када омогућите међукомпанијске трошкове, дозвољавате правним лицима и запосленима да праве трошкове у име другог правног лица и прикупљају уплате од правног лица запосленог у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="326dd-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="326dd-109">На пример, запослени у правном лицу А завршава пројекат за правно лице Б, а пројекат обухвата путне трошкове.</span><span class="sxs-lookup"><span data-stu-id="326dd-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="326dd-110">Ако су омогућени међукомпанијски трошкови, запослени тада може поднети извештај о трошковима који ће трошак књижити правном лицу Б, а трошак тада мора платити правно лице А. Ако ваша организација нема више правних лица, не морате да омогућите међукомпанијске трошкове.</span><span class="sxs-lookup"><span data-stu-id="326dd-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="326dd-111">**Одлука:** Да ли желите да омогућите међукомпанијске трошкове?</span><span class="sxs-lookup"><span data-stu-id="326dd-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="326dd-112">Финансијски менаџмент</span><span class="sxs-lookup"><span data-stu-id="326dd-112">Financial management</span></span>

<span data-ttu-id="326dd-113">Управљање трошковима је уско интегрисано са финансијским управљањем ваше организације.</span><span class="sxs-lookup"><span data-stu-id="326dd-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="326dd-114">Велики део ваше конфигурације за управљање трошковима засниваће се на одлукама које сте донели о финансијама организације.</span><span class="sxs-lookup"><span data-stu-id="326dd-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="326dd-115">Следећи одељци описују различита подручја која захтевају планирање и доношење одлука, на основу финансијских одлука ваше организације и смерница вашег руководећег тима.</span><span class="sxs-lookup"><span data-stu-id="326dd-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="326dd-116">Дневнице</span><span class="sxs-lookup"><span data-stu-id="326dd-116">Per diems</span></span>

<span data-ttu-id="326dd-117">Морате дефинисати дневнице за запослене које пружа ваша организација.</span><span class="sxs-lookup"><span data-stu-id="326dd-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="326dd-118">Будући да се дневнице обично користе за покривање трошкова као што су оброци, смештај и други случајни трошкови, можете креирати правила за дневнице које ваша организација нуди.</span><span class="sxs-lookup"><span data-stu-id="326dd-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="326dd-119">Износи дневница могу се заснивати на добу године, локацији путовања или обоје.</span><span class="sxs-lookup"><span data-stu-id="326dd-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="326dd-120">Када дефинишете правило за дневницу, можете да одредите да се проценат дневнице задржава ако радник добије бесплатне оброке или услуге.</span><span class="sxs-lookup"><span data-stu-id="326dd-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="326dd-121">Такође можете да дефинишете нивое дневница да бисте одредили минимални и максимални број сати за који дневница може да се примењује на путовање радника.</span><span class="sxs-lookup"><span data-stu-id="326dd-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="326dd-122">**Одлуке:**</span><span class="sxs-lookup"><span data-stu-id="326dd-122">**Decisions:**</span></span>

- <span data-ttu-id="326dd-123">Подразумевана правила за дневнице за први и последњи дан:</span><span class="sxs-lookup"><span data-stu-id="326dd-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="326dd-124">Који је минималан број сати које запослени може тражити један дан, а да и даље добије дневницу?</span><span class="sxs-lookup"><span data-stu-id="326dd-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="326dd-125">Да ли постоји смањење количине која се нуди за оброке првог и последњег дана?</span><span class="sxs-lookup"><span data-stu-id="326dd-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="326dd-126">Ако постоји смањење, колики је проценат смањења?</span><span class="sxs-lookup"><span data-stu-id="326dd-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="326dd-127">Да ли постоји смањење количине која се нуди за хотел првог и последњег дана?</span><span class="sxs-lookup"><span data-stu-id="326dd-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="326dd-128">Ако постоји смањење, колики је проценат смањења?</span><span class="sxs-lookup"><span data-stu-id="326dd-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="326dd-129">Да ли постоји смањење количине која се нуди за друге трошкове до којих дође првог и последњег дана?</span><span class="sxs-lookup"><span data-stu-id="326dd-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="326dd-130">Ако постоји смањење, колики је проценат смањења?</span><span class="sxs-lookup"><span data-stu-id="326dd-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="326dd-131">Подразумевана правила за дневнице:</span><span class="sxs-lookup"><span data-stu-id="326dd-131">Default per diem rules:</span></span>

    - <span data-ttu-id="326dd-132">Да ли постоји процентуално смањење дневнице за сваки оброк ако је, на пример, оброк бесплатан?</span><span class="sxs-lookup"><span data-stu-id="326dd-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="326dd-133">Ако постоји смањење, колики је проценат смањења за сваки оброк?</span><span class="sxs-lookup"><span data-stu-id="326dd-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="326dd-134">Да ли се смањење оброка израчунава дневно, по путовању или по броју оброка дневно?</span><span class="sxs-lookup"><span data-stu-id="326dd-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="326dd-135">Да ли износе дневница треба редовно заокруживати или заокруживати нагоре?</span><span class="sxs-lookup"><span data-stu-id="326dd-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="326dd-136">Да ли се дневнице обрачунавају на 24-часовни период или на календарски дан?</span><span class="sxs-lookup"><span data-stu-id="326dd-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="326dd-137">Правила за дневнице заснована на локацији:</span><span class="sxs-lookup"><span data-stu-id="326dd-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="326dd-138">Да ли се дневнице разликују у зависности од локације?</span><span class="sxs-lookup"><span data-stu-id="326dd-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="326dd-139">Које су локације укључене?</span><span class="sxs-lookup"><span data-stu-id="326dd-139">What locations are included?</span></span>
    - <span data-ttu-id="326dd-140">Ако се дневнице разликују у зависности од локације, за сваку локацију, колики проценат се предвиђа за следеће врсте трошкова:</span><span class="sxs-lookup"><span data-stu-id="326dd-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="326dd-141">Оброци</span><span class="sxs-lookup"><span data-stu-id="326dd-141">Meals</span></span>
        - <span data-ttu-id="326dd-142">Хотел</span><span class="sxs-lookup"><span data-stu-id="326dd-142">Hotel</span></span>
        - <span data-ttu-id="326dd-143">Остали трошкови</span><span class="sxs-lookup"><span data-stu-id="326dd-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="326dd-144">Дневници и рачуни за управљање трошковима</span><span class="sxs-lookup"><span data-stu-id="326dd-144">Expense management journals and accounts</span></span>

<span data-ttu-id="326dd-145">Управљање трошковима захтева употребу више дневника и рачуна.</span><span class="sxs-lookup"><span data-stu-id="326dd-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="326dd-146">Морате да одлучите, на пример, да ли се исти рачун користи за аконтације и спорове о кредитним картицама.</span><span class="sxs-lookup"><span data-stu-id="326dd-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="326dd-147">**Одлуке:**</span><span class="sxs-lookup"><span data-stu-id="326dd-147">**Decisions:**</span></span>

- <span data-ttu-id="326dd-148">У којем се дневнику за књижење објављују одобрени извештаји о трошковима?</span><span class="sxs-lookup"><span data-stu-id="326dd-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="326dd-149">Који рачун се користи за аконтације?</span><span class="sxs-lookup"><span data-stu-id="326dd-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="326dd-150">Да ли треба одмах књижити аконтације?</span><span class="sxs-lookup"><span data-stu-id="326dd-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="326dd-151">Начини плаћања</span><span class="sxs-lookup"><span data-stu-id="326dd-151">Payment methods</span></span>

<span data-ttu-id="326dd-152">Када дозвољавате запосленима да праве трошкове у име вашег предузећа, морате да дефинишете начине плаћања које запослени смеју да користе.</span><span class="sxs-lookup"><span data-stu-id="326dd-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="326dd-153">На пример, запосленима можете дозволити да користе готовину или корпоративну кредитну картицу.</span><span class="sxs-lookup"><span data-stu-id="326dd-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="326dd-154">Такође можете дозволити запосленима да користе личне кредитне картице, а затим запосленима надокнадити новац.</span><span class="sxs-lookup"><span data-stu-id="326dd-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="326dd-155">Морате донети следеће одлуке за сваки начин плаћања који дозвољавате.</span><span class="sxs-lookup"><span data-stu-id="326dd-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="326dd-156">**Одлуке:**</span><span class="sxs-lookup"><span data-stu-id="326dd-156">**Decisions:**</span></span>

- <span data-ttu-id="326dd-157">Који су начини плаћања дозвољени?</span><span class="sxs-lookup"><span data-stu-id="326dd-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="326dd-158">Ко је власник трошкова плаћања?</span><span class="sxs-lookup"><span data-stu-id="326dd-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="326dd-159">Да ли постоји тип рачуна за пребијање дуговања?</span><span class="sxs-lookup"><span data-stu-id="326dd-159">Is there an offset account type?</span></span> <span data-ttu-id="326dd-160">Ако постоји тип рачуна за пребијање дуговања, шта је то?</span><span class="sxs-lookup"><span data-stu-id="326dd-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="326dd-161">Ако постоји тип рачуна за пребијање дуговања, који је то рачун?</span><span class="sxs-lookup"><span data-stu-id="326dd-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="326dd-162">Ако је начин плаћања кредитна картица, да ли би начин плаћања требало користити само код увезених трансакција?</span><span class="sxs-lookup"><span data-stu-id="326dd-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="326dd-163">Категорије трошкова и дељене категорије</span><span class="sxs-lookup"><span data-stu-id="326dd-163">Expense categories and shared categories</span></span>

<span data-ttu-id="326dd-164">Када запослени креирају извештај о трошковима, сваки трошак који евидентирају мора бити повезан са категоријом трошкова.</span><span class="sxs-lookup"><span data-stu-id="326dd-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="326dd-165">Категорије трошкова су изведене из дељених категорија које се могу делити између правних лица у вашој организацији.</span><span class="sxs-lookup"><span data-stu-id="326dd-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="326dd-166">Ове категорије се такође могу делити у управљању пројектима и рачуноводству, у зависности од начина на који је ваша организација дефинисана.</span><span class="sxs-lookup"><span data-stu-id="326dd-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="326dd-167">На основу дефиниције ваше организације и смерница тима за примену, морате да одредите да ли ће се категорије које се користе у управљању трошковима користити само у управљању трошковима или треба да се деле између управљања пројектима и рачуноводства и управљања трошковима.</span><span class="sxs-lookup"><span data-stu-id="326dd-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="326dd-168">Имајте на уму да се ове категорије се могу делити између управљања пројектима и трошкова или управљања пројектима и производње, али не између управљања трошковима и производње.</span><span class="sxs-lookup"><span data-stu-id="326dd-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="326dd-169">За сваку категорију трошкова морате донети следеће одлуке.</span><span class="sxs-lookup"><span data-stu-id="326dd-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="326dd-170">**Одлуке:**</span><span class="sxs-lookup"><span data-stu-id="326dd-170">**Decisions:**</span></span>

- <span data-ttu-id="326dd-171">Шта је то категорија трошкова?</span><span class="sxs-lookup"><span data-stu-id="326dd-171">What is the expense category?</span></span> <span data-ttu-id="326dd-172">Примери укључују категорије за летове, хотеле или километражу.</span><span class="sxs-lookup"><span data-stu-id="326dd-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="326dd-173">Може ли се категорија трошкова такође користити у управљању пројектима и рачуноводству?</span><span class="sxs-lookup"><span data-stu-id="326dd-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="326dd-174">Шта је то тип трошка?</span><span class="sxs-lookup"><span data-stu-id="326dd-174">What is the expense type?</span></span>
- <span data-ttu-id="326dd-175">Који је подразумевани начин плаћања за категорију трошка?</span><span class="sxs-lookup"><span data-stu-id="326dd-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="326dd-176">Морају ли се детаљно делити трошкови у категорији трошкова?</span><span class="sxs-lookup"><span data-stu-id="326dd-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="326dd-177">Који је главни подразумевани рачун за категорију трошка?</span><span class="sxs-lookup"><span data-stu-id="326dd-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="326dd-178">Која је подразумевана група пореза на промет производа за категорију трошкова?</span><span class="sxs-lookup"><span data-stu-id="326dd-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="326dd-179">Да ли су дозвољени додатни начини плаћања за категорију трошкова?</span><span class="sxs-lookup"><span data-stu-id="326dd-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="326dd-180">Ако су дозвољени додатни начини плаћања, који су то?</span><span class="sxs-lookup"><span data-stu-id="326dd-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="326dd-181">Постоје ли поткатегорије у овој категорији трошкова?</span><span class="sxs-lookup"><span data-stu-id="326dd-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="326dd-182">Ако постоје поткатегорије, морате донети и следеће одлуке:</span><span class="sxs-lookup"><span data-stu-id="326dd-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="326dd-183">Да ли је нека од поткатегорија изузета од повраћаја пореза?</span><span class="sxs-lookup"><span data-stu-id="326dd-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="326dd-184">Која је група пореза на промет производа за поткатегорије?</span><span class="sxs-lookup"><span data-stu-id="326dd-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="326dd-185">Ако се категорија трошкова користи и у управљању пројектима и рачуноводству, одговорите на преостала питања.</span><span class="sxs-lookup"><span data-stu-id="326dd-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="326dd-186">У супротном, пређите на следећи одељак.</span><span class="sxs-lookup"><span data-stu-id="326dd-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="326dd-187">Који рачуни трошкова ће се користити за следеће трошкове?</span><span class="sxs-lookup"><span data-stu-id="326dd-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="326dd-188">Цена</span><span class="sxs-lookup"><span data-stu-id="326dd-188">Cost</span></span>
    - <span data-ttu-id="326dd-189">Расподела зарада</span><span class="sxs-lookup"><span data-stu-id="326dd-189">Payroll allocation</span></span>
    - <span data-ttu-id="326dd-190">Приходи у току – вредност трошкова</span><span class="sxs-lookup"><span data-stu-id="326dd-190">WIP-cost value</span></span>
    - <span data-ttu-id="326dd-191">Ставка трошкова</span><span class="sxs-lookup"><span data-stu-id="326dd-191">Cost-item</span></span>
    - <span data-ttu-id="326dd-192">Приходи у току – вредност трошкова – ставка</span><span class="sxs-lookup"><span data-stu-id="326dd-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="326dd-193">Обрачунати губитак</span><span class="sxs-lookup"><span data-stu-id="326dd-193">Accrued loss</span></span>
    - <span data-ttu-id="326dd-194">Приходи у току – обрачунати губитак</span><span class="sxs-lookup"><span data-stu-id="326dd-194">WIP-accrued loss</span></span>

- <span data-ttu-id="326dd-195">Који рачуни прихода ће се користити за следеће?</span><span class="sxs-lookup"><span data-stu-id="326dd-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="326dd-196">Фактурисани приход</span><span class="sxs-lookup"><span data-stu-id="326dd-196">Invoiced revenue</span></span>
    - <span data-ttu-id="326dd-197">Обрачунати приход – Вредност продаје</span><span class="sxs-lookup"><span data-stu-id="326dd-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="326dd-198">Приходи у току – вредност продаје</span><span class="sxs-lookup"><span data-stu-id="326dd-198">WIP-sales value</span></span>
    - <span data-ttu-id="326dd-199">Обрачунати приход – производња</span><span class="sxs-lookup"><span data-stu-id="326dd-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="326dd-200">Приходи у току – производња</span><span class="sxs-lookup"><span data-stu-id="326dd-200">WIP-production</span></span>
    - <span data-ttu-id="326dd-201">Обрачунати приход – профит</span><span class="sxs-lookup"><span data-stu-id="326dd-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="326dd-202">Приходи у току – профит</span><span class="sxs-lookup"><span data-stu-id="326dd-202">WIP-profit</span></span>
    - <span data-ttu-id="326dd-203">Обрачунати приход – претплата</span><span class="sxs-lookup"><span data-stu-id="326dd-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="326dd-204">Приходи у току – претплата</span><span class="sxs-lookup"><span data-stu-id="326dd-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="326dd-205">Порези</span><span class="sxs-lookup"><span data-stu-id="326dd-205">Taxes</span></span>

<span data-ttu-id="326dd-206">За порезе повезане са трошковима морате утврдити шта је укључено или омогућено у извештајима о трошковима.</span><span class="sxs-lookup"><span data-stu-id="326dd-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="326dd-207">**Одлуке:**</span><span class="sxs-lookup"><span data-stu-id="326dd-207">**Decisions:**</span></span>

- <span data-ttu-id="326dd-208">Да ли је порез на промет укључен у износе трошкова?</span><span class="sxs-lookup"><span data-stu-id="326dd-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="326dd-209">Да ли треба омогућити поврат пореза на трошкове?</span><span class="sxs-lookup"><span data-stu-id="326dd-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="326dd-210">Када сте планирали главну књигу, ако сте одлучили да примените амерички порез на промет и користите пореска правила, не можете да омогућите повраћај пореза на трошкове.</span><span class="sxs-lookup"><span data-stu-id="326dd-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="326dd-211">(Да бисте применили амерички порез на промет и користили пореска правила, поставите опцију **Примени правила опорезивања за порез на промет** на **Да**.)</span><span class="sxs-lookup"><span data-stu-id="326dd-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="326dd-212">Смернице</span><span class="sxs-lookup"><span data-stu-id="326dd-212">Policies</span></span>

<span data-ttu-id="326dd-213">Креирањем смерница за извештавање о трошковима можете да помогнете својој организацији да уштеди време и новац када запослени направе трошкове у њено име.</span><span class="sxs-lookup"><span data-stu-id="326dd-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="326dd-214">Правила помажу да запослени остану у оквиру буџета, пруже све потребне информације и троше новац само онако како им је потребно.</span><span class="sxs-lookup"><span data-stu-id="326dd-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="326dd-215">Морате донети следеће одлуке за сваке смернице за извештавање о трошковима и сваке смернице за одобравање извештаја о трошковима коју креирате.</span><span class="sxs-lookup"><span data-stu-id="326dd-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="326dd-216">**Одлуке:**</span><span class="sxs-lookup"><span data-stu-id="326dd-216">**Decisions:**</span></span>

- <span data-ttu-id="326dd-217">Како се зову смернице?</span><span class="sxs-lookup"><span data-stu-id="326dd-217">What is the name of the policy?</span></span>
- <span data-ttu-id="326dd-218">Чему служе смернице о трошковима?</span><span class="sxs-lookup"><span data-stu-id="326dd-218">What is the expense policy for?</span></span>
- <span data-ttu-id="326dd-219">Ако сте претходно одлучили да омогућите међукомпанијске трошкове, на које компаније у вашој организацији ће се примењивати ове смернице?</span><span class="sxs-lookup"><span data-stu-id="326dd-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="326dd-220">Када смернице ступају на снагу?</span><span class="sxs-lookup"><span data-stu-id="326dd-220">When does the policy become effective?</span></span>
- <span data-ttu-id="326dd-221">Када смернице истичу?</span><span class="sxs-lookup"><span data-stu-id="326dd-221">When does the policy expire?</span></span>
- <span data-ttu-id="326dd-222">Какво је правило смерница?</span><span class="sxs-lookup"><span data-stu-id="326dd-222">What is the policy rule?</span></span>
- <span data-ttu-id="326dd-223">Какав је исход правила смерница?</span><span class="sxs-lookup"><span data-stu-id="326dd-223">What is the outcome of the policy rule?</span></span>
