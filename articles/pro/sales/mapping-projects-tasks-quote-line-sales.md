---
title: Мапирање пројеката и задатака на ставку понуде засноване на пројекту
description: Ова тема пружа информације о томе како да мапирате пројекте и задатке у предмет задатка заснованог на пројекту.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d726ab09da0e502da99191f7e7469c47f79b6e7c
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083864"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="ec0db-103">Мапирање пројеката и задатака на ставку понуде засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="ec0db-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="ec0db-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="ec0db-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ec0db-105">У ставкама понуде засноване на пројекту можете мапирати одређене задатке пројекта који је већ повезан са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="ec0db-106">Када мапирате задатке у ставку понуде, следеће ставке које сте дефинисали у ставци понуде примењиваће се само на те задатке:</span><span class="sxs-lookup"><span data-stu-id="ec0db-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="ec0db-107">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="ec0db-107">Billing method</span></span>
- <span data-ttu-id="ec0db-108">Опције наплативости</span><span class="sxs-lookup"><span data-stu-id="ec0db-108">Chargeability options</span></span>
- <span data-ttu-id="ec0db-109">Ограничења која не смеју да се прекораче</span><span class="sxs-lookup"><span data-stu-id="ec0db-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="ec0db-110">Клијенти</span><span class="sxs-lookup"><span data-stu-id="ec0db-110">Customers</span></span>

<span data-ttu-id="ec0db-111">На пример, можда имате пројекат где је једна фаза фиксна цена, а све остале фазе су време и материјали.</span><span class="sxs-lookup"><span data-stu-id="ec0db-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="ec0db-112">У том случају, прву фазу и све њене подређене задатке можете повезати са ставком понуде за ту фазу методом обрачуна са фиксном ценом.</span><span class="sxs-lookup"><span data-stu-id="ec0db-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="ec0db-113">Затим можете повезати све остале фазе са ставком понуде заснованом на времену и материјалима.</span><span class="sxs-lookup"><span data-stu-id="ec0db-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="ec0db-114">Повезивање задатака са ставкама понуде заснованим на пројекту</span><span class="sxs-lookup"><span data-stu-id="ec0db-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="ec0db-115">Задатке можете повезати са ставкама понуде са следећих локација:</span><span class="sxs-lookup"><span data-stu-id="ec0db-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="ec0db-116">Страница **Пројекат** > картица **Обрачун задатака** (оптимално)</span><span class="sxs-lookup"><span data-stu-id="ec0db-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="ec0db-117">Страница **Ставка понуде** > картица **Задаци који се наплаћују**</span><span class="sxs-lookup"><span data-stu-id="ec0db-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="ec0db-118">Са странице Пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0db-118">From the Project page</span></span>

<span data-ttu-id="ec0db-119">Страница **Пројекат** пружа оптимално искуство за повезивање задатака са ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="ec0db-120">Ову страницу можете користити за избор више задатака и повезивање свих њих, као и њихових подређених задатака, у изабрану ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="ec0db-121">На картици **Општи подаци** ставке понуде засноване на пројекту, проверите да ли је поље **Пројекат** попуњено.</span><span class="sxs-lookup"><span data-stu-id="ec0db-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="ec0db-122">У пољу **Укључени задаци** изаберите **Само изабрани задаци**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="ec0db-123">Сачувајте ставку понуде засновану на пројекту.</span><span class="sxs-lookup"><span data-stu-id="ec0db-123">Save the project-based quote line.</span></span> <span data-ttu-id="ec0db-124">Када се образац освежи, приказаће се картица **Задаци који се наплаћују**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="ec0db-125">На картици **Општи подаци** изаберите везу за поље **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="ec0db-126">На страници **Пројекат** изаберите картицу **Обрачун задатака**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="ec0db-127">У другој мрежи, која се односи на подешавање обрачуна за одређени задатак, изаберите један или више задатака, а затим изаберите **Повезивање ставки понуде**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="ec0db-128">На страници дијалога која се појави, изаберите ставку понуде која приказује ставке понуде засноване на пројекту у понуди.</span><span class="sxs-lookup"><span data-stu-id="ec0db-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="ec0db-129">У пољу **Тип обрачуна** , назначите да ли су ови задаци наплативи или ненаплативи.</span><span class="sxs-lookup"><span data-stu-id="ec0db-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="ec0db-130">Означите поље за потврду да бисте назначили да ли повезивање треба да садржи подређене задатке изабраних задатака.</span><span class="sxs-lookup"><span data-stu-id="ec0db-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="ec0db-131">Ако означите то поље, повезаћете подређене задатке изабраних задатака са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="ec0db-132">Изаберите **У реду** да бисте затворили дијалог.</span><span class="sxs-lookup"><span data-stu-id="ec0db-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="ec0db-133">Са странице Ставка понуде</span><span class="sxs-lookup"><span data-stu-id="ec0db-133">From the Quote line page</span></span>

<span data-ttu-id="ec0db-134">Пројектне задатке можете повезати са ставкама понуде са картице **Задаци који се наплаћују** на страници **Понуда**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="ec0db-135">Оптимално место за повезивање пројектних задатака са ставкама понуде је на картици **Обрачун задатака** на страници **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="ec0db-136">Ако повежете задатке са картице **Задаци који се наплаћују** на страници **Ставка понуде** , сваки пројекат морате ручно повезати.</span><span class="sxs-lookup"><span data-stu-id="ec0db-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="ec0db-137">На картици **Општи подаци** ставке понуде засноване на пројекту, проверите да ли је изабран пројекат у пољу **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="ec0db-138">У пољу **Укључени задаци** изаберите **Само изабрани задаци**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="ec0db-139">Сачувајте ставку понуде засновану на пројекту.</span><span class="sxs-lookup"><span data-stu-id="ec0db-139">Save the project-based quote line.</span></span> <span data-ttu-id="ec0db-140">Када се образац освежи, приказаће се картица **Задаци који се наплаћују**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="ec0db-141">На картици **Задаци који се наплаћују** , изаберите **Додај задатак ставке понуде**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="ec0db-142">На страници **Задатак ставке понуде** , у пољу **Задаци** изаберите задатак и у пољу **Тип обрачуна** изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="ec0db-143">Затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="ec0db-143">Close the page.</span></span> <span data-ttu-id="ec0db-144">Изабрани задатак је сада повезан са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="ec0db-145">Прекидање везе задатака са ставкама понуде заснованим на пројекту</span><span class="sxs-lookup"><span data-stu-id="ec0db-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="ec0db-146">Са странице Пројекат</span><span class="sxs-lookup"><span data-stu-id="ec0db-146">From the Project page</span></span>

<span data-ttu-id="ec0db-147">Овај метод пружа оптимално искуство за прекидање везе задатака са ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="ec0db-148">Можете изабрати више задатака и прекинути везу свих њих, као и њихових подређених задатака, са изабраном ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="ec0db-149">На картици **Општи подаци** ставке понуде засноване на пројекту, у пољу **Пројекат** изаберите везу ка пројекту.</span><span class="sxs-lookup"><span data-stu-id="ec0db-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="ec0db-150">На страници **Пројекат** изаберите картицу **Обрачун задатака**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="ec0db-151">У другој мрежи, која се односи на подешавање обрачуна за одређени задатак, изаберите један или више задатака, а затим изаберите **Прекидање везе са ставкама понуде**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="ec0db-152">На страници дијалога која се појави, изаберите ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="ec0db-153">Означите поље за потврду да бисте назначили да ли повезивање треба такође да се уклони из подређених задатака изабраних задатака.</span><span class="sxs-lookup"><span data-stu-id="ec0db-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="ec0db-154">Ако означите то поље, прекинућете везу подређених задатака изабраних задатака са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="ec0db-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="ec0db-155">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-155">Select **OK**.</span></span> <span data-ttu-id="ec0db-156">Порука упозорења вас обавештава да ако уклоните ово повезивање, све стварне вредности претходно евидентиране у задатку могу да се опозову.</span><span class="sxs-lookup"><span data-stu-id="ec0db-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="ec0db-157">Изаберите **У реду** да би се наставило и уклањало повезивање између задатка и ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="ec0db-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="ec0db-158">Са странице Ставка понуде</span><span class="sxs-lookup"><span data-stu-id="ec0db-158">From the Quote line page</span></span>

<span data-ttu-id="ec0db-159">Везу пројектних задатака са ставкама понуде такође можете прекинути са картице **Задаци који се наплаћују** на страници **Понуда**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="ec0db-160">На картици **Задаци који се наплаћују** , изаберите **Избриши задатак ставке понуде**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="ec0db-161">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="ec0db-161">Select **OK**.</span></span> <span data-ttu-id="ec0db-162">Порука упозорења вас обавештава да ако уклоните ово повезивање, све стварне вредности претходно евидентиране у задатку могу да се опозову.</span><span class="sxs-lookup"><span data-stu-id="ec0db-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="ec0db-163">Изаберите **У реду** да би се наставило и уклањало повезивање између задатка и ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="ec0db-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="ec0db-164">Овај поступак не брише задатак из пројекта.</span><span class="sxs-lookup"><span data-stu-id="ec0db-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="ec0db-165">Само уклања повезивање задатка са ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="ec0db-165">It only removes the task association from the project-based quote line.</span></span>
