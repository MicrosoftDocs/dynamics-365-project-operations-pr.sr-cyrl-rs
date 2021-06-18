---
title: Обрада признаница за трошкове
description: Ова тема пружа информације о обради признаница помоћу оптичког препознавања знакова (OCR). Ова функција је дизајнирана да побољша корисничко искуство приликом креирања извештаја о трошковима у услузи Microsoft Dynamics 365 Finance.
author: stsporen
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: ed9c97ba9cc505106599c2896dc2112358d0c408
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993524"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="2c2c5-104">Обрада признаница за трошкове</span><span class="sxs-lookup"><span data-stu-id="2c2c5-104">Expense receipt processing</span></span>

<span data-ttu-id="2c2c5-105">Унос трошкова је побољшан увођењем обраду признаница путем оптичког препознавања знакова (OCR).</span><span class="sxs-lookup"><span data-stu-id="2c2c5-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="2c2c5-106">Ова функција је дизајнирана да побољша корисничко искуство приликом креирања извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="2c2c5-107">Кључне функције</span><span class="sxs-lookup"><span data-stu-id="2c2c5-107">Key features</span></span>

- <span data-ttu-id="2c2c5-108">Са признанице се издвајају име трговца, датум и укупан износ.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="2c2c5-109">Функција покушава да усклади невезане признанице са невезаним трансакцијама трошкова.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="2c2c5-110">Корисници из признаница могу да креирају ручно унете трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="2c2c5-111">Примери употребе</span><span class="sxs-lookup"><span data-stu-id="2c2c5-111">Usage examples</span></span>

<span data-ttu-id="2c2c5-112">Да бисте аутоматски приложили признанице које укључују трансакције кредитном картицом када се креира извештај о трошковима, извршите следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="2c2c5-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="2c2c5-113">Отворите радни простор **Управљање трошковима**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="2c2c5-114">На картици **Признанице** проверите да ли постоје неприложене признанице.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="2c2c5-115">Такође можете да отпремите признанице на картицу **Признанице**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="2c2c5-116">На картици **Трошкови** проверите да ли постоје неприложени трошкови.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="2c2c5-117">Обично их администратор трошкова увози од добављача кредитне картице.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="2c2c5-118">Изаберите **Нови извештај о трошковима**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-118">Select **New expense report**.</span></span> <span data-ttu-id="2c2c5-119">Обратите пажњу да и сада можете да укључите трошкове и признанице када креирате извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="2c2c5-120">Ако додате и трошкове и рачуне, активираће се аутоматско упоређивање признанице и трошкова.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="2c2c5-121">Да бисте створили трошак или упоредили трошак са признанице, извршите следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="2c2c5-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="2c2c5-122">На извештају о трошковима, на картици **Признанице**, приложите признаницу избором ставке **Додај признанице**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="2c2c5-123">Испод отпремљене слике признанице видећете опције **Креирај** и **Упореди**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="2c2c5-124">Изаберите **Креирај** да бисте креирали ручно унете трансакције трошкова и попунили вредности које су издвојене из признанице.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="2c2c5-125">Ако изаберете **Упореди**, систем покушава да постојећи трошак усклади са признаницом.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-125">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="2c2c5-126">Инсталација</span><span class="sxs-lookup"><span data-stu-id="2c2c5-126">Installation</span></span>

<span data-ttu-id="2c2c5-127">Ова функција ради у комбинацији са функцијом **Редизајнирани извештаји о трошковима** која вам помаже да поједноставите искуство са трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="2c2c5-128">Ова функција је доступна само за окружења 2. нивоа и виших, а то су Sandbox и Производња.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="2c2c5-129">Да бисте користили ове напредне могућности трошкова, инсталирајте програмски додатак Услуга управљања трошковима за Microsoft Dynamics 365 Finance и уклјучите функције у вашој инстанци.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="2c2c5-130">Програмском додатку можете приступити из свог пројекта у услузи Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="2c2c5-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="2c2c5-131">Пријавите се на LCS и отворите жељено окружење.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="2c2c5-132">Иди на ставку **Сви детаљи**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="2c2c5-133">Изаберите **Одржавање** или се померите надоле до брзе картице **Програмски додаци за животну средину**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-133">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="2c2c5-134">Изаберите ставку **Инсталирајте нови програмски додатак**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="2c2c5-135">Изаберите ставку **Услуга управљања трошковима**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="2c2c5-136">Следите упутства за инсталацију и прихватите одредбе и услове.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="2c2c5-137">Изаберите **Инсталирај**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-137">Select **Install**.</span></span>

<span data-ttu-id="2c2c5-138">У радном простору **Управљање функцијама** укључите следеће функције:</span><span class="sxs-lookup"><span data-stu-id="2c2c5-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="2c2c5-139">Поновно осмишљени извештаји о трошковима</span><span class="sxs-lookup"><span data-stu-id="2c2c5-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="2c2c5-140">Аутоматско подударање и креирање трошкова из признанице</span><span class="sxs-lookup"><span data-stu-id="2c2c5-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="2c2c5-141">Када укључите ове функције, дешавају се следеће радње:</span><span class="sxs-lookup"><span data-stu-id="2c2c5-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="2c2c5-142">Постојећи радни простор **Управљање трошковима** се замењује новим радним простором.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="2c2c5-143">Додата је нова ставка менија за видљивост поља трошкова.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="2c2c5-144">Још увек можете отворити претходну страницу **Извештаји о трошковима** одласком на **Управљање трошковима > Моји трошкови > Извештаји о трошковима**.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="2c2c5-145">Токови посла и сва одобрења вас и даље воде на постојећу страницу са извештајима о трошковима.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="2c2c5-146">Признанице ће се обрађивати путем Microsoft Azure Cognitive Services, а метаподаци ће бити издвојени и додати.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="2c2c5-147">Додата је опција која вам омогућава да направите извештај о трошковима који укључује одговарајуће неприложене признанице.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="2c2c5-148">Опција која се додаје извештајима о трошковима омогућава вам да креирате линију трошкова из признаница или покушате да упоредите постојећу признаницу са постојећом линијом трошкова.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="2c2c5-149">За више информација о редизајнираној функцији извештаја о трошковима погледајте [Редизајнирани извештаји о трошковима](ExpenseWorkspaceNew.md).</span><span class="sxs-lookup"><span data-stu-id="2c2c5-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="2c2c5-150">Најчешћа питања</span><span class="sxs-lookup"><span data-stu-id="2c2c5-150">Frequently asked questions</span></span>

<span data-ttu-id="2c2c5-151">**Да ли Microsoft користи моје податке за своје моделе?**</span><span class="sxs-lookup"><span data-stu-id="2c2c5-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="2c2c5-152">Не, Microsoft је изградио општи модел машинског учења за услугу обраде признаница.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="2c2c5-153">Овај модел се не заснива на признаницама које отпремите.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="2c2c5-154">**Где је ова функција доступна и обрађена?**</span><span class="sxs-lookup"><span data-stu-id="2c2c5-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="2c2c5-155">Тренутно су подржане Сједињене Државе.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="2c2c5-156">**Где одлазе моје признанице?**</span><span class="sxs-lookup"><span data-stu-id="2c2c5-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="2c2c5-157">Финансије ће контактирати Cognitive Services да би извукли податке са терена.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="2c2c5-158">Cognitive Services ће задржати копију ваше признанице и до 24 сата док траје обрада.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="2c2c5-159">По завршетку обраде, Cognitive Services ће уклонити признаницу.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="2c2c5-160">Признанице се и даље чувају у Финансијама.</span><span class="sxs-lookup"><span data-stu-id="2c2c5-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="2c2c5-161">За више информација погледајте [Омогућите разумевање признанице са новом способношћу препознавања образаца](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="2c2c5-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]