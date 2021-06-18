---
title: Мапирање пројеката и задатака на ставку понуде засноване на пројекту
description: Ова тема пружа информације о томе како да мапирате пројекте и задатке у предмет задатка заснованог на пројекту.
author: rumant
ms.date: 10/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d1c98d6a903393a0afc0e94d7f9859d55b9dc1f7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994604"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="be60b-103">Мапирање пројеката и задатака на ставку понуде засноване на пројекту</span><span class="sxs-lookup"><span data-stu-id="be60b-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="be60b-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="be60b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="be60b-105">У ставкама понуде засноване на пројекту можете мапирати одређене задатке пројекта који је већ повезан са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="be60b-106">Када мапирате задатке у ставку понуде, следеће ставке које сте дефинисали у ставци понуде примењиваће се само на те задатке:</span><span class="sxs-lookup"><span data-stu-id="be60b-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="be60b-107">Начин наплате</span><span class="sxs-lookup"><span data-stu-id="be60b-107">Billing method</span></span>
- <span data-ttu-id="be60b-108">Опције наплативости</span><span class="sxs-lookup"><span data-stu-id="be60b-108">Chargeability options</span></span>
- <span data-ttu-id="be60b-109">Ограничења која не смеју да се прекораче</span><span class="sxs-lookup"><span data-stu-id="be60b-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="be60b-110">Клијенти</span><span class="sxs-lookup"><span data-stu-id="be60b-110">Customers</span></span>

<span data-ttu-id="be60b-111">На пример, можда имате пројекат где је једна фаза фиксна цена, а све остале фазе су време и материјали.</span><span class="sxs-lookup"><span data-stu-id="be60b-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="be60b-112">У том случају, прву фазу и све њене подређене задатке можете повезати са ставком понуде за ту фазу методом обрачуна са фиксном ценом.</span><span class="sxs-lookup"><span data-stu-id="be60b-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="be60b-113">Затим можете повезати све остале фазе са ставком понуде заснованом на времену и материјалима.</span><span class="sxs-lookup"><span data-stu-id="be60b-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="be60b-114">Повезивање задатака са ставкама понуде заснованим на пројекту</span><span class="sxs-lookup"><span data-stu-id="be60b-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="be60b-115">Задатке можете повезати са ставкама понуде са следећих локација:</span><span class="sxs-lookup"><span data-stu-id="be60b-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="be60b-116">Страница **Пројекат** > картица **Обрачун задатака** (оптимално)</span><span class="sxs-lookup"><span data-stu-id="be60b-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="be60b-117">Страница **Ставка понуде** > картица **Задаци који се наплаћују**</span><span class="sxs-lookup"><span data-stu-id="be60b-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="be60b-118">Са странице Пројекат</span><span class="sxs-lookup"><span data-stu-id="be60b-118">From the Project page</span></span>

<span data-ttu-id="be60b-119">Страница **Пројекат** пружа оптимално искуство за повезивање задатака са ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="be60b-120">Ову страницу можете користити за избор више задатака и повезивање свих њих, као и њихових подређених задатака, у изабрану ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="be60b-121">На картици **Општи подаци** ставке понуде засноване на пројекту, проверите да ли је поље **Пројекат** попуњено.</span><span class="sxs-lookup"><span data-stu-id="be60b-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="be60b-122">У пољу **Укључени задаци** изаберите **Само изабрани задаци**.</span><span class="sxs-lookup"><span data-stu-id="be60b-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="be60b-123">Сачувајте ставку понуде засновану на пројекту.</span><span class="sxs-lookup"><span data-stu-id="be60b-123">Save the project-based quote line.</span></span> <span data-ttu-id="be60b-124">Када се образац освежи, приказаће се картица **Задаци који се наплаћују**.</span><span class="sxs-lookup"><span data-stu-id="be60b-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="be60b-125">На картици **Општи подаци** изаберите везу за поље **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="be60b-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="be60b-126">На страници **Пројекат** изаберите картицу **Обрачун задатака**.</span><span class="sxs-lookup"><span data-stu-id="be60b-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="be60b-127">У другој мрежи, која се односи на подешавање обрачуна за одређени задатак, изаберите један или више задатака, а затим изаберите **Повезивање ставки понуде**.</span><span class="sxs-lookup"><span data-stu-id="be60b-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="be60b-128">На страници дијалога која се појави, изаберите ставку понуде која приказује ставке понуде засноване на пројекту у понуди.</span><span class="sxs-lookup"><span data-stu-id="be60b-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="be60b-129">У пољу **Тип обрачуна**, назначите да ли су ови задаци наплативи или ненаплативи.</span><span class="sxs-lookup"><span data-stu-id="be60b-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="be60b-130">Означите поље за потврду да бисте назначили да ли повезивање треба да садржи подређене задатке изабраних задатака.</span><span class="sxs-lookup"><span data-stu-id="be60b-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="be60b-131">Ако означите то поље, повезаћете подређене задатке изабраних задатака са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="be60b-132">Изаберите **У реду** да бисте затворили дијалог.</span><span class="sxs-lookup"><span data-stu-id="be60b-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="be60b-133">Са странице Ставка понуде</span><span class="sxs-lookup"><span data-stu-id="be60b-133">From the Quote line page</span></span>

<span data-ttu-id="be60b-134">Пројектне задатке можете повезати са ставкама понуде са картице **Задаци који се наплаћују** на страници **Понуда**.</span><span class="sxs-lookup"><span data-stu-id="be60b-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="be60b-135">Оптимално место за повезивање пројектних задатака са ставкама понуде је на картици **Обрачун задатака** на страници **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="be60b-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="be60b-136">Ако повежете задатке са картице **Задаци који се наплаћују** на страници **Ставка понуде**, сваки пројекат морате ручно повезати.</span><span class="sxs-lookup"><span data-stu-id="be60b-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="be60b-137">На картици **Општи подаци** ставке понуде засноване на пројекту, проверите да ли је изабран пројекат у пољу **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="be60b-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="be60b-138">У пољу **Укључени задаци** изаберите **Само изабрани задаци**.</span><span class="sxs-lookup"><span data-stu-id="be60b-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="be60b-139">Сачувајте ставку понуде засновану на пројекту.</span><span class="sxs-lookup"><span data-stu-id="be60b-139">Save the project-based quote line.</span></span> <span data-ttu-id="be60b-140">Када се образац освежи, приказаће се картица **Задаци који се наплаћују**.</span><span class="sxs-lookup"><span data-stu-id="be60b-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="be60b-141">На картици **Задаци који се наплаћују**, изаберите **Додај задатак ставке понуде**.</span><span class="sxs-lookup"><span data-stu-id="be60b-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="be60b-142">На страници **Задатак ставке понуде**, у пољу **Задаци** изаберите задатак и у пољу **Тип обрачуна** изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="be60b-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="be60b-143">Затворите страницу.</span><span class="sxs-lookup"><span data-stu-id="be60b-143">Close the page.</span></span> <span data-ttu-id="be60b-144">Изабрани задатак је сада повезан са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="be60b-145">Прекидање везе задатака са ставкама понуде заснованим на пројекту</span><span class="sxs-lookup"><span data-stu-id="be60b-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="be60b-146">Са странице Пројекат</span><span class="sxs-lookup"><span data-stu-id="be60b-146">From the Project page</span></span>

<span data-ttu-id="be60b-147">Овај метод пружа оптимално искуство за прекидање везе задатака са ставкама понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="be60b-148">Можете изабрати више задатака и прекинути везу свих њих, као и њихових подређених задатака, са изабраном ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="be60b-149">На картици **Општи подаци** ставке понуде засноване на пројекту, у пољу **Пројекат** изаберите везу ка пројекту.</span><span class="sxs-lookup"><span data-stu-id="be60b-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="be60b-150">На страници **Пројекат** изаберите картицу **Обрачун задатака**.</span><span class="sxs-lookup"><span data-stu-id="be60b-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="be60b-151">У другој мрежи, која се односи на подешавање обрачуна за одређени задатак, изаберите један или више задатака, а затим изаберите **Прекидање везе са ставкама понуде**.</span><span class="sxs-lookup"><span data-stu-id="be60b-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="be60b-152">На страници дијалога која се појави, изаберите ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="be60b-153">Означите поље за потврду да бисте назначили да ли повезивање треба такође да се уклони из подређених задатака изабраних задатака.</span><span class="sxs-lookup"><span data-stu-id="be60b-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="be60b-154">Ако означите то поље, прекинућете везу подређених задатака изабраних задатака са ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="be60b-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="be60b-155">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="be60b-155">Select **OK**.</span></span> <span data-ttu-id="be60b-156">Порука упозорења вас обавештава да ако уклоните ово повезивање, све стварне вредности претходно евидентиране у задатку могу да се опозову.</span><span class="sxs-lookup"><span data-stu-id="be60b-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="be60b-157">Изаберите **У реду** да би се наставило и уклањало повезивање између задатка и ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="be60b-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="be60b-158">Са странице Ставка понуде</span><span class="sxs-lookup"><span data-stu-id="be60b-158">From the Quote line page</span></span>

<span data-ttu-id="be60b-159">Везу пројектних задатака са ставкама понуде такође можете прекинути са картице **Задаци који се наплаћују** на страници **Понуда**.</span><span class="sxs-lookup"><span data-stu-id="be60b-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="be60b-160">На картици **Задаци који се наплаћују**, изаберите **Избриши задатак ставке понуде**.</span><span class="sxs-lookup"><span data-stu-id="be60b-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="be60b-161">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="be60b-161">Select **OK**.</span></span> <span data-ttu-id="be60b-162">Порука упозорења вас обавештава да ако уклоните ово повезивање, све стварне вредности претходно евидентиране у задатку могу да се опозову.</span><span class="sxs-lookup"><span data-stu-id="be60b-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="be60b-163">Изаберите **У реду** да би се наставило и уклањало повезивање између задатка и ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="be60b-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="be60b-164">Овај поступак не брише задатак из пројекта.</span><span class="sxs-lookup"><span data-stu-id="be60b-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="be60b-165">Само уклања повезивање задатка са ставке понуде засноване на пројекту.</span><span class="sxs-lookup"><span data-stu-id="be60b-165">It only removes the task association from the project-based quote line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]