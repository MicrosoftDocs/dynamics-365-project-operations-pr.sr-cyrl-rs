---
title: Подударање признанице са трошком користећи OCR
description: Ова тема пружа информације о обради признаница помоћу оптичког препознавања знакова (OCR).
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 55f63c8c092942b73a55c9d86d867bca600f42e5
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124341"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a><span data-ttu-id="ca283-103">Подударање признанице са трошком користећи OCR</span><span class="sxs-lookup"><span data-stu-id="ca283-103">Match a receipt to an expense using OCR</span></span>

<span data-ttu-id="ca283-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="ca283-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ca283-105">Унос трошкова је побољшан увођењем обраду признаница путем оптичког препознавања знакова (OCR).</span><span class="sxs-lookup"><span data-stu-id="ca283-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="ca283-106">Ова функционалност је дизајнирана да побољша корисничко искуство приликом креирања извештаја о трошковима.</span><span class="sxs-lookup"><span data-stu-id="ca283-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="ca283-107">Кључне функције</span><span class="sxs-lookup"><span data-stu-id="ca283-107">Key features</span></span>

- <span data-ttu-id="ca283-108">Систем издваја име трговца, датум и укупан износ са признанице.</span><span class="sxs-lookup"><span data-stu-id="ca283-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="ca283-109">Систем ће покушати да усклади невезане признанице са невезаним трансакцијама трошкова.</span><span class="sxs-lookup"><span data-stu-id="ca283-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="ca283-110">Из признаница можете да креирате ручно унете трансакције трошкова.</span><span class="sxs-lookup"><span data-stu-id="ca283-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="ca283-111">Приложите признанице уз извештај о трошковима</span><span class="sxs-lookup"><span data-stu-id="ca283-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="ca283-112">Да бисте аутоматски приложили признанице које укључују трансакције кредитном картицом када се креира извештај о трошковима, извршите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="ca283-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="ca283-113">Отворите радни простор **Управљање трошковима**.</span><span class="sxs-lookup"><span data-stu-id="ca283-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="ca283-114">На картици **Признанице** проверите да ли постоје неприложене признанице.</span><span class="sxs-lookup"><span data-stu-id="ca283-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="ca283-115">Такође можете да отпремите признанице на картицу **Признанице**.</span><span class="sxs-lookup"><span data-stu-id="ca283-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="ca283-116">На картици **Трошкови** проверите да ли постоје неприложени трошкови.</span><span class="sxs-lookup"><span data-stu-id="ca283-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="ca283-117">Обично их администратор трошкова увози од добављача кредитне картице.</span><span class="sxs-lookup"><span data-stu-id="ca283-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="ca283-118">Изаберите **Нови извештај о трошковима**.</span><span class="sxs-lookup"><span data-stu-id="ca283-118">Select **New expense report**.</span></span> <span data-ttu-id="ca283-119">Обратите пажњу да и сада можете да укључите трошкове и признанице када креирате извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="ca283-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="ca283-120">Ако додате и трошкове и рачуне, активираће се аутоматско упоређивање признанице и трошкова.</span><span class="sxs-lookup"><span data-stu-id="ca283-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="ca283-121">Креирајте или упоредите признанице са извештајем о трошковима</span><span class="sxs-lookup"><span data-stu-id="ca283-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="ca283-122">Да бисте створили трошак или упоредили трошак са признанице, извршите следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="ca283-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="ca283-123">На извештају о трошковима, на картици **Признанице**, приложите признаницу избором ставке **Додај признанице**.</span><span class="sxs-lookup"><span data-stu-id="ca283-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="ca283-124">Испод отпремљене слике признанице видећете опције **Креирај** и **Упореди**.</span><span class="sxs-lookup"><span data-stu-id="ca283-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="ca283-125">Изаберите **Креирај** да бисте креирали ручно унете трансакције трошкова и попунили вредности које су издвојене из признанице.</span><span class="sxs-lookup"><span data-stu-id="ca283-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="ca283-126">Ако изаберете **Упореди**, систем покушава да постојећи трошак усклади са признаницом.</span><span class="sxs-lookup"><span data-stu-id="ca283-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="ca283-127">Инсталација</span><span class="sxs-lookup"><span data-stu-id="ca283-127">Installation</span></span>

<span data-ttu-id="ca283-128">Да бисте користили ове напредне могућности трошкова, инсталирајте програмски додатак Услуга управљања трошковима за Microsoft Dynamics 365 Finance и уклјучите функције у вашој инстанци.</span><span class="sxs-lookup"><span data-stu-id="ca283-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="ca283-129">Програмском додатку можете приступити из свог пројекта у услузи Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="ca283-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="ca283-130">Пријавите се на LCS и отворите жељено окружење.</span><span class="sxs-lookup"><span data-stu-id="ca283-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="ca283-131">Иди на ставку **Сви детаљи**.</span><span class="sxs-lookup"><span data-stu-id="ca283-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="ca283-132">Изаберите **Одржавање** или се померите надоле до брзе картице **Програмски додаци за животну средину**.</span><span class="sxs-lookup"><span data-stu-id="ca283-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="ca283-133">Изаберите ставку **Инсталирајте нови програмски додатак**.</span><span class="sxs-lookup"><span data-stu-id="ca283-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="ca283-134">Изаберите ставку **Услуга управљања трошковима**.</span><span class="sxs-lookup"><span data-stu-id="ca283-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="ca283-135">Следите упутства за инсталацију и прихватите одредбе и услове.</span><span class="sxs-lookup"><span data-stu-id="ca283-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="ca283-136">Изаберите **Инсталирај**.</span><span class="sxs-lookup"><span data-stu-id="ca283-136">Select **Install**.</span></span>

<span data-ttu-id="ca283-137">У радном простору **Управљање функцијама** укључите следеће функције:</span><span class="sxs-lookup"><span data-stu-id="ca283-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="ca283-138">Поновно осмишљени извештаји о трошковима</span><span class="sxs-lookup"><span data-stu-id="ca283-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="ca283-139">Аутоматско подударање и креирање трошкова из признанице</span><span class="sxs-lookup"><span data-stu-id="ca283-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="ca283-140">Када укључите ове функције, дешавају се следеће радње:</span><span class="sxs-lookup"><span data-stu-id="ca283-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="ca283-141">Постојећи радни простор **Управљање трошковима** се замењује новим радним простором.</span><span class="sxs-lookup"><span data-stu-id="ca283-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="ca283-142">Додата је нова ставка менија за видљивост поља трошкова.</span><span class="sxs-lookup"><span data-stu-id="ca283-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="ca283-143">Још увек можете отворити претходну страницу **Извештаји о трошковима** одласком на **Управљање трошковима > Моји трошкови > Извештаји о трошковима**.</span><span class="sxs-lookup"><span data-stu-id="ca283-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="ca283-144">Токови посла и сва одобрења вас и даље воде на постојећу страницу са извештајима о трошковима.</span><span class="sxs-lookup"><span data-stu-id="ca283-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="ca283-145">Признанице ће се обрађивати путем Microsoft Azure Cognitive Services, а метаподаци ће бити издвојени и додати.</span><span class="sxs-lookup"><span data-stu-id="ca283-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="ca283-146">Додата је опција која вам омогућава да направите извештај о трошковима који укључује одговарајуће неприложене признанице.</span><span class="sxs-lookup"><span data-stu-id="ca283-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="ca283-147">Опција која се додаје извештајима о трошковима омогућава вам да креирате линију трошкова из признаница или покушате да упоредите постојећу признаницу са постојећом линијом трошкова.</span><span class="sxs-lookup"><span data-stu-id="ca283-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="ca283-148">Најчешћа питања</span><span class="sxs-lookup"><span data-stu-id="ca283-148">Frequently asked questions</span></span>

<span data-ttu-id="ca283-149">**Да ли Microsoft користи моје податке за своје моделе?**</span><span class="sxs-lookup"><span data-stu-id="ca283-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="ca283-150">Не, Microsoft је изградио општи модел машинског учења за услугу обраде признаница.</span><span class="sxs-lookup"><span data-stu-id="ca283-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="ca283-151">Овај модел се не заснива на признаницама које отпремите.</span><span class="sxs-lookup"><span data-stu-id="ca283-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="ca283-152">**Где је ова функција доступна и обрађена?**</span><span class="sxs-lookup"><span data-stu-id="ca283-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="ca283-153">Тренутно су подржане Сједињене Државе.</span><span class="sxs-lookup"><span data-stu-id="ca283-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="ca283-154">**Где одлазе моје признанице?**</span><span class="sxs-lookup"><span data-stu-id="ca283-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="ca283-155">Финансије ће контактирати Cognitive Services да би извукли податке са терена.</span><span class="sxs-lookup"><span data-stu-id="ca283-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="ca283-156">Cognitive Services ће задржати копију ваше признанице и до 24 сата док траје обрада.</span><span class="sxs-lookup"><span data-stu-id="ca283-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="ca283-157">По завршетку обраде, Cognitive Services ће уклонити признаницу.</span><span class="sxs-lookup"><span data-stu-id="ca283-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="ca283-158">Признанице се и даље чувају у Финансијама.</span><span class="sxs-lookup"><span data-stu-id="ca283-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="ca283-159">За више информација погледајте [Омогућите разумевање признанице са новом способношћу препознавања образаца](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="ca283-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
