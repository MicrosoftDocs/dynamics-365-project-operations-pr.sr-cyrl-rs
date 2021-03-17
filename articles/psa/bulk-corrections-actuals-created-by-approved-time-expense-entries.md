---
title: Масовне исправке тренутног стања креираног одобреним ставкама времена и трошка
description: Ова тема објашњава како администратор може да изврши појединачне или масовне исправке претходно одобрених ставки времена или трошка уколико наплата није потпуна.
author: rumant
manager: AnnBe
ms.date: 04/02/2020
ms.topic: article
ms.service: dynamics-ax-applications
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
search.app:
- ProjectOperations
ms.openlocfilehash: 17d6648840e27a4e573985af2cdd74c4adf878e1
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290917"
---
# <a name="bulk-corrections-of-actuals-created-by-approved-time-and-expense-entries"></a><span data-ttu-id="e9b1e-103">Масовне исправке тренутног стања креираног одобреним ставкама времена и трошка</span><span class="sxs-lookup"><span data-stu-id="e9b1e-103">Bulk corrections of actuals created by approved time and expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="e9b1e-104">Повремено се може погрешно унети ставка времена или трошка.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-104">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="e9b1e-105">На пример, консултант може да одабере погрешан датум приликом креирања ставке времена или може да пренесе бројеве приликом уноса трошка.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-105">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="e9b1e-106">Ако консултант не може да обави ажурирања прослеђених ставки, администратор може директно да исправи ставку за пројекат.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-106">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="e9b1e-107">Да бисте довршили процедуре у овој теми, требаће вам дозволе администратора.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-107">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="e9b1e-108">Исправне одобрене ставке времена</span><span class="sxs-lookup"><span data-stu-id="e9b1e-108">Correct approved time entries</span></span>     

<span data-ttu-id="e9b1e-109">Обавите следеће кораке да бисте исправили појединачне или вишеструке ставке за пројекат.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-109">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="e9b1e-110">У области **Продаја** изаберите **Трансакције**, а затим изаберите **Одобрено време**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-110">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="e9b1e-111">На листи **Одобрено време** пронађите и изаберите једну одобрену ставку времена или више њих да бисте их исправили.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-111">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="e9b1e-112">Можете користити филтер да бисте пронашли повезане ставке.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-112">You can use the filter to locate related entries.</span></span> <span data-ttu-id="e9b1e-113">На пример, можете да филтрирате ID пројекта и да изаберете све одобрене ставке времена са тим ID-ом пројекта.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-113">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="e9b1e-114">Изаберите **Исправи ставке**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-114">Select **Correct entries**.</span></span> <span data-ttu-id="e9b1e-115">Нови дневник исправки се аутоматски креира, са додељеном врстом **Исправка времена**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-115">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="e9b1e-116">Стаке које сте изабрали се додају у главну књигу.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-116">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="e9b1e-117">На страници **Нова главна књига** унесите **Опис** за ваш дневник исправки, а затим изаберите картицу **Исправке ставки времена**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-117">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  
5. <span data-ttu-id="e9b1e-118">У одељку **Нове вредности за ставке времена** по потреби ажурирајте поља исправним информацијама.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-118">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="e9b1e-119">На пример, можете да промените додељени пројекат или ресурс који је могуће резервисати.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-119">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="e9b1e-120">Изаберите **Преглед**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-120">Select **Preview**.</span></span> <span data-ttu-id="e9b1e-121">У дијалогу изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-121">In the dialog box, select **OK**.</span></span> <span data-ttu-id="e9b1e-122">На картици **Ставке у главној књизи** можете видети листу оригиналног тренутног стања које је повезано са изабраним ставкама времена које су опозване и са исправљеним одговарајућим ставкама које су креиране.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-122">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="e9b1e-123">Ако је потребно да се изврше додатне исправке, поновите кораке 5 и 6.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-123">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="e9b1e-124">Све исправљене стварне вредности имаће исте вредности које сте изабрали у одељку **Нове вредности за ставке времена**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-124">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="e9b1e-125">Ако се исправке појаве како се очекује, изаберите **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-125">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="e9b1e-126">У дијалогу изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-126">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="e9b1e-127">Вратите се на област **Продаја**, изаберите **Пројекти**, а затим отворите пројекат за који сте управо ажурирали ставке времена.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-127">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="e9b1e-128">На страници **Пројекти**, на картици **Стварне вредности**, погледајте промене које сте извршили.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-128">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="e9b1e-129">Ако картица **Актуелно** није видљива, изаберите **Повезано** > **Стварне вредности**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-129">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="e9b1e-130">На листи **Везани приказ стварних вредности** можете видети да су оригиналне ставке времена које су опозване и даље наведене, као што су наведене и одговарајуће исправљене ставке времена.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-130">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="e9b1e-131">На пример, на следећој слици постоје две ставке чија је количина 8,00 а које имају задужења наведена у колони Износ.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-131">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="e9b1e-132">Уз то, постоје две ставке чија је количина -8,00 које приказују задужене износе у колони Износ.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-132">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="e9b1e-133">Ове исправке своде количину на нулу.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-133">These corrections bring the quantity to zero.</span></span>

![Листа везаног приказа стварних вредности](https://github.com/MicrosoftDocs/dynamics-365-customer-engagement-pr/blob/bulk-corrections-actuals-created-by-approved-time-expense-entries.md/time-actuals.png)
 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="e9b1e-135">Исправне одобрене ставке трошкова</span><span class="sxs-lookup"><span data-stu-id="e9b1e-135">Correct approved expense entries</span></span>

<span data-ttu-id="e9b1e-136">Обавите следеће кораке да бисте исправили једну ставку трошкова или више њих.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="e9b1e-137">У области **Продаја** у левом окну за навигацију, у оквиру **Трансакције**, изаберите **Одобрени трошкови**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="e9b1e-138">На листи **Одобрени трошкови** изаберите пројекат који желите да исправите, а затим изаберите **Исправи ставке**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="e9b1e-139">Креира се нови дневник исправки са додељеном врстом **Исправка трошка**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="e9b1e-140">На страници **Нови дневник** унесите **Опис** за исправку а на картици **Исправка трошка**, у одељку **Нове вредности за трошкове**, изаберите поља података која желите да исправите за одабране ставке трошка.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="e9b1e-141">На пример, можете да доделите трошак другом **Пројекту** или да исправите ставку **Категорија трошка**, **Датум трошка** или **Ресурс који може да се резервише**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="e9b1e-142">Изаберите **Преглед**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-142">Select **Preview**.</span></span> <span data-ttu-id="e9b1e-143">У дијалогу изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="e9b1e-144">Проверите исправке на картици **Ставке у главној књизи**. Можете видети листу оригиналног тренутног стања које је повезано са изабраним ставкама трошкова које су опозване и са исправљеним одговарајућим ставкама које су креиране.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="e9b1e-145">Ако су исправљене вредности према очекивању, изаберите **Потврди**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="e9b1e-146">У дијалогу изаберите **У реду.**</span><span class="sxs-lookup"><span data-stu-id="e9b1e-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="e9b1e-147">Ако се вредности не приказују како се очекује, изаберите **Откажи** да бисте се вратили на листу **Одобрени трошкови**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="e9b1e-148">Поновите кораке од 2 до 5.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="e9b1e-149">Исправљене стварне вредности имаће исте вредности које сте изабрали у одељку **Нове вредности за трошкове**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="e9b1e-150">Након што потврдите дневник исправки, вратите се на пројекат или пројекте које сте ажурирали да бисте погледали своје измене.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="e9b1e-151">На страници пројекта, на картици **Актуелно**, прегледајте **Везани приказ стварних вредности**.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="e9b1e-152">Наведене су изворне ставке и исправљене ставке.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="e9b1e-153">Следећа слика приказује изворне износе ставке трошка и одговарајуће исправљене износе ставке трошка.</span><span class="sxs-lookup"><span data-stu-id="e9b1e-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 

![Трошак_стварна вредност](https://user-images.githubusercontent.com/60806505/77122219-4cd52900-69fa-11ea-8349-ccd2ffebf640.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]