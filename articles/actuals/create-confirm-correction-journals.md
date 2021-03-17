---
title: Креирање и потврда дневника са исправкама
description: Ова тема пружа информације о томе како да креирате и потврдите дневник са исправкама.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 8ca35d1e66cbacaf65b7cd43493e3588f213788e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276951"
---
# <a name="create-and-confirm-correction-journals"></a><span data-ttu-id="78c78-103">Креирање и потврда дневника са исправкама</span><span class="sxs-lookup"><span data-stu-id="78c78-103">Create and confirm Correction journals</span></span>

<span data-ttu-id="78c78-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="78c78-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="78c78-105">Повремено се може погрешно унети ставка времена или трошка.</span><span class="sxs-lookup"><span data-stu-id="78c78-105">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="78c78-106">На пример, консултант може да одабере погрешан датум приликом креирања ставке времена или може да пренесе бројеве приликом уноса трошка.</span><span class="sxs-lookup"><span data-stu-id="78c78-106">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="78c78-107">Ако консултант не може да обави ажурирања прослеђених ставки, администратор може директно да исправи ставку за пројекат.</span><span class="sxs-lookup"><span data-stu-id="78c78-107">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="78c78-108">Да бисте довршили процедуре у овој теми, требаће вам дозволе администратора.</span><span class="sxs-lookup"><span data-stu-id="78c78-108">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="78c78-109">Исправне одобрене ставке времена</span><span class="sxs-lookup"><span data-stu-id="78c78-109">Correct approved time entries</span></span>     

<span data-ttu-id="78c78-110">Обавите следеће кораке да бисте исправили појединачне или вишеструке ставке за пројекат.</span><span class="sxs-lookup"><span data-stu-id="78c78-110">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="78c78-111">У области **Продаја** изаберите **Трансакције**, а затим изаберите **Одобрено време**.</span><span class="sxs-lookup"><span data-stu-id="78c78-111">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="78c78-112">На листи **Одобрено време** пронађите и изаберите једну одобрену ставку времена или више њих да бисте их исправили.</span><span class="sxs-lookup"><span data-stu-id="78c78-112">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="78c78-113">Можете користити филтер да бисте пронашли повезане ставке.</span><span class="sxs-lookup"><span data-stu-id="78c78-113">You can use the filter to locate related entries.</span></span> <span data-ttu-id="78c78-114">На пример, можете да филтрирате ID пројекта и да изаберете све одобрене ставке времена са тим ID-ом пројекта.</span><span class="sxs-lookup"><span data-stu-id="78c78-114">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="78c78-115">Изаберите **Исправи ставке**.</span><span class="sxs-lookup"><span data-stu-id="78c78-115">Select **Correct entries**.</span></span> <span data-ttu-id="78c78-116">Нови дневник исправки се аутоматски креира, са додељеном врстом **Исправка времена**.</span><span class="sxs-lookup"><span data-stu-id="78c78-116">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="78c78-117">Стаке које сте изабрали се додају у главну књигу.</span><span class="sxs-lookup"><span data-stu-id="78c78-117">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="78c78-118">На страници **Нова главна књига** унесите **Опис** за ваш дневник исправки, а затим изаберите картицу **Исправке ставки времена**.</span><span class="sxs-lookup"><span data-stu-id="78c78-118">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  

5. <span data-ttu-id="78c78-119">У одељку **Нове вредности за ставке времена** по потреби ажурирајте поља исправним информацијама.</span><span class="sxs-lookup"><span data-stu-id="78c78-119">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="78c78-120">На пример, можете да промените додељени пројекат или ресурс који је могуће резервисати.</span><span class="sxs-lookup"><span data-stu-id="78c78-120">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="78c78-121">Изаберите **Преглед**.</span><span class="sxs-lookup"><span data-stu-id="78c78-121">Select **Preview**.</span></span> <span data-ttu-id="78c78-122">У дијалогу изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="78c78-122">In the dialog box, select **OK**.</span></span> <span data-ttu-id="78c78-123">На картици **Ставке у главној књизи** можете видети листу оригиналног тренутног стања које је повезано са изабраним ставкама времена које су опозване и са исправљеним одговарајућим ставкама које су креиране.</span><span class="sxs-lookup"><span data-stu-id="78c78-123">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="78c78-124">Ако је потребно да се изврше додатне исправке, поновите кораке 5 и 6.</span><span class="sxs-lookup"><span data-stu-id="78c78-124">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="78c78-125">Све исправљене стварне вредности имаће исте вредности које сте изабрали у одељку **Нове вредности за ставке времена**.</span><span class="sxs-lookup"><span data-stu-id="78c78-125">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="78c78-126">Ако се исправке појаве како се очекује, изаберите **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="78c78-126">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="78c78-127">У дијалогу изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="78c78-127">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="78c78-128">Вратите се на област **Продаја**, изаберите **Пројекти**, а затим отворите пројекат за који сте управо ажурирали ставке времена.</span><span class="sxs-lookup"><span data-stu-id="78c78-128">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="78c78-129">На страници **Пројекти**, на картици **Стварне вредности**, погледајте промене које сте извршили.</span><span class="sxs-lookup"><span data-stu-id="78c78-129">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="78c78-130">Ако картица **Актуелно** није видљива, изаберите **Повезано** > **Стварне вредности**.</span><span class="sxs-lookup"><span data-stu-id="78c78-130">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="78c78-131">На листи **Везани приказ стварних вредности** можете видети да су оригиналне ставке времена које су опозване и даље наведене, као што су наведене и одговарајуће исправљене ставке времена.</span><span class="sxs-lookup"><span data-stu-id="78c78-131">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="78c78-132">На пример, на следећој слици постоје две ставке чија је количина 8,00 а које имају задужења наведена у колони Износ.</span><span class="sxs-lookup"><span data-stu-id="78c78-132">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="78c78-133">Уз то, постоје две ставке чија је количина -8,00 које приказују задужене износе у колони Износ.</span><span class="sxs-lookup"><span data-stu-id="78c78-133">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="78c78-134">Ове исправке своде количину на нулу.</span><span class="sxs-lookup"><span data-stu-id="78c78-134">These corrections bring the quantity to zero.</span></span>

 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="78c78-135">Исправне одобрене ставке трошкова</span><span class="sxs-lookup"><span data-stu-id="78c78-135">Correct approved expense entries</span></span>

<span data-ttu-id="78c78-136">Обавите следеће кораке да бисте исправили једну ставку трошкова или више њих.</span><span class="sxs-lookup"><span data-stu-id="78c78-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="78c78-137">У области **Продаја** у левом окну за навигацију, у оквиру **Трансакције**, изаберите **Одобрени трошкови**.</span><span class="sxs-lookup"><span data-stu-id="78c78-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="78c78-138">На листи **Одобрени трошкови** изаберите пројекат који желите да исправите, а затим изаберите **Исправи ставке**.</span><span class="sxs-lookup"><span data-stu-id="78c78-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="78c78-139">Креира се нови дневник исправки са додељеном врстом **Исправка трошка**.</span><span class="sxs-lookup"><span data-stu-id="78c78-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="78c78-140">На страници **Нови дневник** унесите **Опис** за исправку а на картици **Исправка трошка**, у одељку **Нове вредности за трошкове**, изаберите поља података која желите да исправите за одабране ставке трошка.</span><span class="sxs-lookup"><span data-stu-id="78c78-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="78c78-141">На пример, можете да доделите трошак другом **Пројекту** или да исправите ставку **Категорија трошка**, **Датум трошка** или **Ресурс који може да се резервише**.</span><span class="sxs-lookup"><span data-stu-id="78c78-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="78c78-142">Изаберите **Преглед**.</span><span class="sxs-lookup"><span data-stu-id="78c78-142">Select **Preview**.</span></span> <span data-ttu-id="78c78-143">У дијалогу изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="78c78-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="78c78-144">Проверите исправке на картици **Ставке у главној књизи**. Можете видети листу оригиналног тренутног стања које је повезано са изабраним ставкама трошкова које су опозване и са исправљеним одговарајућим ставкама које су креиране.</span><span class="sxs-lookup"><span data-stu-id="78c78-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="78c78-145">Ако су исправљене вредности према очекивању, изаберите **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="78c78-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="78c78-146">У дијалогу изаберите **У реду.**</span><span class="sxs-lookup"><span data-stu-id="78c78-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="78c78-147">Ако се вредности не приказују како се очекује, изаберите **Откажи** да бисте се вратили на листу **Одобрени трошкови**.</span><span class="sxs-lookup"><span data-stu-id="78c78-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="78c78-148">Поновите кораке од 2 до 5.</span><span class="sxs-lookup"><span data-stu-id="78c78-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="78c78-149">Исправљене стварне вредности имаће исте вредности које сте изабрали у одељку **Нове вредности за трошкове**.</span><span class="sxs-lookup"><span data-stu-id="78c78-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="78c78-150">Након што потврдите дневник исправки, вратите се на пројекат или пројекте које сте ажурирали да бисте погледали своје измене.</span><span class="sxs-lookup"><span data-stu-id="78c78-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="78c78-151">На страници пројекта, на картици **Актуелно**, прегледајте **Везани приказ стварних вредности**.</span><span class="sxs-lookup"><span data-stu-id="78c78-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="78c78-152">Наведене су изворне ставке и исправљене ставке.</span><span class="sxs-lookup"><span data-stu-id="78c78-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="78c78-153">Следећа слика приказује изворне износе ставке трошка и одговарајуће исправљене износе ставке трошка.</span><span class="sxs-lookup"><span data-stu-id="78c78-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 




[!INCLUDE[footer-include](../includes/footer-banner.md)]