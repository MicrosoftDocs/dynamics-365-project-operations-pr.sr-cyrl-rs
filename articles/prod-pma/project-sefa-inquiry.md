---
title: Распоред трошкова истраге савезне помоћи
description: Ова тема пружа информације о Распореду трошкова истраге савезне помоћи.
author: velofog
manager: Ann Beebe
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: 70dff12c106723dda801668412cfd084c462db4b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288982"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="c3780-103">Распоред трошкова истраге савезне помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-103">Schedule of Expenditures of Federal Awards inquiry</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="c3780-104">Према циркуларном обавештењу А-133 Канцеларије за управљање и буџет, агенције које примају савезна средства подлежу захтевима ревизије, које су познате и као појединачне ревизије.</span><span class="sxs-lookup"><span data-stu-id="c3780-104">According to Office of Management and Budget Circular A-133, agencies that receive federal funds are subject to audit requirements, which are also known as single audits.</span></span> <span data-ttu-id="c3780-105">Процес ревизије се користи за редовно извештавање о приходима и расходима савезних бесповратних средстава.</span><span class="sxs-lookup"><span data-stu-id="c3780-105">The audit process is used to report on the revenues and expenditures of federal grants on a recurring basis.</span></span> <span data-ttu-id="c3780-106">Део извештаја појединачне ревизије укључује Распоред трошкова истраге савезне помоћи (SEFA).</span><span class="sxs-lookup"><span data-stu-id="c3780-106">Part of the single audit report includes the Schedule of Expenditures of Federal Awards (SEFA).</span></span>

<span data-ttu-id="c3780-107">Распоред трошкова истраге савезне помоћи укључује назив и број Каталога савезне домаће помоћи (CFDA), број бесповратне помоћи, годину доделе, назив савезне агенције која обезбеђује средства и назив ентитета који даје одобрење.</span><span class="sxs-lookup"><span data-stu-id="c3780-107">The Schedule of Expenditures of Federal Awards inquiry includes the Catalog of Federal Domestic Assistance (CFDA) title and number, the grant number, the year of the grant, the name of the federal agency that provides the funds, and the name of the pass-through entity.</span></span> <span data-ttu-id="c3780-108">Упит се односи на одређени период.</span><span class="sxs-lookup"><span data-stu-id="c3780-108">The inquiry is for a specific period.</span></span> <span data-ttu-id="c3780-109">Типично је тај период исти као и период финансијских извештаја, који је фискална година.</span><span class="sxs-lookup"><span data-stu-id="c3780-109">Typically, that period is the same as the financial statement period, which is a fiscal year.</span></span>

<span data-ttu-id="c3780-110">Упит укључује грантове који имају датуме пројекције у одабраном временском распону.</span><span class="sxs-lookup"><span data-stu-id="c3780-110">The inquiry includes grants that have projection dates in the selected date range.</span></span> <span data-ttu-id="c3780-111">Колона **Агенција која даје помоћ** у упиту приказује клијента помоћи или, за пролазну помоћ, агенцију која даје помоћ.</span><span class="sxs-lookup"><span data-stu-id="c3780-111">The **Grantor agency** column of the inquiry shows the grant customer or, for a pass-through grant, the grantor agency.</span></span> <span data-ttu-id="c3780-112">За пролазну помоћ, колона **Пролазна агенција** приказује клијента који је добио помоћ.</span><span class="sxs-lookup"><span data-stu-id="c3780-112">For a pass-through grant, the **Pass-through agency** column shows the grant customer.</span></span> <span data-ttu-id="c3780-113">Ако помоћ није пролазна, колона **Пролазна агенција** је празна.</span><span class="sxs-lookup"><span data-stu-id="c3780-113">If the grant isn't a pass-through grant, the **Pass-through agency** column is blank.</span></span>

## <a name="set-up-the-cfda-clusters"></a><span data-ttu-id="c3780-114">Подешавање CFDA група</span><span class="sxs-lookup"><span data-stu-id="c3780-114">Set up the CFDA clusters</span></span>

<span data-ttu-id="c3780-115">Морате да поставите CFDA групе који се могу повезати са CFDA бројевима у Распореду трошкова истраге савезне помоћи.</span><span class="sxs-lookup"><span data-stu-id="c3780-115">You must set up the CFDA clusters that can be associated with CFDA numbers in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="c3780-116">Идите на **Управљање пројектима и рачуноводство \> Подешавање \> Помоћ \> Каталог група савезне домаће помоћи**.</span><span class="sxs-lookup"><span data-stu-id="c3780-116">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance clusters**.</span></span>
2. <span data-ttu-id="c3780-117">Да бисте креирали CFDA групу, изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="c3780-117">Select **New** to create a CFDA cluster.</span></span>
3. <span data-ttu-id="c3780-118">Унесите назив групе.</span><span class="sxs-lookup"><span data-stu-id="c3780-118">Enter the cluster name.</span></span>
4. <span data-ttu-id="c3780-119">Изаберите **Сачувај** да бисте сачували промене.</span><span class="sxs-lookup"><span data-stu-id="c3780-119">Select **Save** to save your changes.</span></span>

## <a name="set-up-cfda-numbers"></a><span data-ttu-id="c3780-120">Подесите CFDA бројеве</span><span class="sxs-lookup"><span data-stu-id="c3780-120">Set up CFDA numbers</span></span>

<span data-ttu-id="c3780-121">Морате да поставите CFDA бројеве који се могу додати у помоћ и укључити у Распоред трошкова истраге савезне помоћи.</span><span class="sxs-lookup"><span data-stu-id="c3780-121">You must set up CFDA numbers that can be added to grants and included in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="c3780-122">Идите на **Управљање пројектима и рачуноводство \> Подешавање \> Помоћ \> Каталог бројева савезне домаће помоћи**.</span><span class="sxs-lookup"><span data-stu-id="c3780-122">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance numbers**.</span></span>
2. <span data-ttu-id="c3780-123">Да бисте креирали CFDA број, изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="c3780-123">Select **New** to create a CFDA number.</span></span>
3. <span data-ttu-id="c3780-124">У колону **Број** унесите CFDA број.</span><span class="sxs-lookup"><span data-stu-id="c3780-124">In the **Number** column, enter the CFDA number.</span></span>
4. <span data-ttu-id="c3780-125">Притисните тастер **Tab**.</span><span class="sxs-lookup"><span data-stu-id="c3780-125">Press the **Tab** key.</span></span>
5. <span data-ttu-id="c3780-126">У колону **Опис** унесите CFDA назив.</span><span class="sxs-lookup"><span data-stu-id="c3780-126">In the **Description** column, enter the CFDA title.</span></span>
6. <span data-ttu-id="c3780-127">Притисните тастер **Tab**.</span><span class="sxs-lookup"><span data-stu-id="c3780-127">Press the **Tab** key.</span></span>
7. <span data-ttu-id="c3780-128">Опционално: У поље **Група програма** додајте одговарајућу CFDA групу.</span><span class="sxs-lookup"><span data-stu-id="c3780-128">Optional: In the **Program cluster** field, add the appropriate CFDA cluster.</span></span>
8. <span data-ttu-id="c3780-129">Изаберите **Сачувај** да бисте сачували промене.</span><span class="sxs-lookup"><span data-stu-id="c3780-129">Select **Save** to save your changes.</span></span>

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="c3780-130">Поставите помоћ ради извештавања о Распореду трошкова истраге савезне помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-130">Set up grants to report for the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="c3780-131">Идите на **Управљање пројектима и рачуноводство \> Помоћ \> Помоћ**, и изаберите постојећу помоћ.</span><span class="sxs-lookup"><span data-stu-id="c3780-131">Go to **Project management and accounting \> Grants \> Grants**, and select an existing grant.</span></span>
2. <span data-ttu-id="c3780-132">На брзој картици **Подешавање**, у пољу **Каталог савезне домаће помоћи** доделите CFDA број.</span><span class="sxs-lookup"><span data-stu-id="c3780-132">On the **Setup** FastTab, in the **Catalog of Federal Domestic Assistance** field, assign the CFDA number.</span></span> <span data-ttu-id="c3780-133">CFDA број на помоћи одређује CFDA групу за извештавање.</span><span class="sxs-lookup"><span data-stu-id="c3780-133">The CFDA number on the grant determines the CFDA cluster for reporting.</span></span>
3. <span data-ttu-id="c3780-134">На брзој картици **Контакт информације** унесите информације о даваоцу помоћи пратећи ове кораке:</span><span class="sxs-lookup"><span data-stu-id="c3780-134">On **Contact information** FastTab, enter the grantor information by following these steps:</span></span>

    1. <span data-ttu-id="c3780-135">У пољу **Одобри клијента** унесите клијента који је одговоран за помоћ.</span><span class="sxs-lookup"><span data-stu-id="c3780-135">In the **Grant customer** field, enter the customer who is responsible for the grant.</span></span> <span data-ttu-id="c3780-136">За постојећу помоћ ове информације су можда већ унете.</span><span class="sxs-lookup"><span data-stu-id="c3780-136">For an existing grant, this information might already be entered.</span></span>
    2. <span data-ttu-id="c3780-137">Наведите да ли је корисник помоћи донатор.</span><span class="sxs-lookup"><span data-stu-id="c3780-137">Indicate whether the grant customer is the funder.</span></span> <span data-ttu-id="c3780-138">Ако је корисник помоћи донатор, оставите поље за потврду **Пролазно** празно.</span><span class="sxs-lookup"><span data-stu-id="c3780-138">If the grant customer is the funder, leave the **Pass-through** check box cleared.</span></span> <span data-ttu-id="c3780-139">Ако је други клијент донатор, а корисник бесповратне помоћи је одговоран за трошење и праћење новца, потврдите избор у пољу за потврду **Пролазно**.</span><span class="sxs-lookup"><span data-stu-id="c3780-139">If another customer is the funder, and the grant customer is responsible for spending and tracking the money, select the **Pass-through** check box.</span></span>

4. <span data-ttu-id="c3780-140">Ако сте изабрали поље за потврду **Пролазно** у претходном кораку, у поље **Агенција која даје помоћ** поље, унесите клијента који је обезбедио помоћ.</span><span class="sxs-lookup"><span data-stu-id="c3780-140">If you selected the **Pass-through** check box in the previous step, in the **Grantor agency** field, enter the customer who provided the grant.</span></span> <span data-ttu-id="c3780-141">Агенција која даје помоћ и корисник помоћи не може бити исти клијент.</span><span class="sxs-lookup"><span data-stu-id="c3780-141">The grantor agency and the grant customer can't be the same customer.</span></span>

<span data-ttu-id="c3780-142">Ево примера пролазне помоћи:</span><span class="sxs-lookup"><span data-stu-id="c3780-142">Here is an example of a pass-through grant:</span></span>

<span data-ttu-id="c3780-143">Савезна влада финансирала је инфраструктурни пројекат за државу.</span><span class="sxs-lookup"><span data-stu-id="c3780-143">The federal government funded an infrastructure project for a state.</span></span> <span data-ttu-id="c3780-144">Савезна влада дала је новац држави да га потроши.</span><span class="sxs-lookup"><span data-stu-id="c3780-144">The federal government gave the money to the state to spend.</span></span> <span data-ttu-id="c3780-145">У овом случају, савезна влада је агенција која даје помоћ, а држава је корисник помоћи.</span><span class="sxs-lookup"><span data-stu-id="c3780-145">In this case, the federal government is the grantor agency, and the state is the grant customer.</span></span>

> [!NOTE] 
> <span data-ttu-id="c3780-146">Када први пут укључите функцију, почетни CFDA бројеви ће се унети помоћу постојећих бројева у помоћи.</span><span class="sxs-lookup"><span data-stu-id="c3780-146">When you first turn on the feature, initial CFDA numbers will be entered by using the existing numbers on grants.</span></span>

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a><span data-ttu-id="c3780-147">Искључите помоћи из SEFA извештавања на основу врсте помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-147">Exclude grants from SEFA reporting based on the grant type</span></span>

1. <span data-ttu-id="c3780-148">Идите на **Управљање пројектима и рачуноводство \> Подешавање \> Помоћ \> Врсте помоћи**.</span><span class="sxs-lookup"><span data-stu-id="c3780-148">Go to **Project management and accounting \> Setup \> Grants \> Grant types**.</span></span>
2. <span data-ttu-id="c3780-149">На брзој картици **Подразумеване информације** изаберите поље за потврду **Изузми из распореда трошкова савезне помоћи**.</span><span class="sxs-lookup"><span data-stu-id="c3780-149">On the **Default information** FastTab, select the **Exclude from Schedule of Expenditures of Federal Awards** check box.</span></span>
3. <span data-ttu-id="c3780-150">Изаберите **Сачувај** да бисте сачували промене.</span><span class="sxs-lookup"><span data-stu-id="c3780-150">Select **Save** to save your changes.</span></span>

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="c3780-151">Покрените Распоред трошкова истраге савезне помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-151">Run the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="c3780-152">Идите на **Управљање пројектима и рачуноводство \> Упити и извештаји \> Упит за помоћ \> Распоред трошкова истраге савезне помоћи**.</span><span class="sxs-lookup"><span data-stu-id="c3780-152">Go to **Project management and accounting \> Inquiries and reports \> Grant inquiry \> Schedule of Expenditures of Federal Awards**.</span></span>
2. <span data-ttu-id="c3780-153">У одељку **Параметри** пратите следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="c3780-153">In the **Parameters** section, follow these steps:</span></span>

    1. <span data-ttu-id="c3780-154">У пољу **Интервал датума** изаберите кôд за интервал датума.</span><span class="sxs-lookup"><span data-stu-id="c3780-154">In the **Date interval** field, select the code for the date interval.</span></span> <span data-ttu-id="c3780-155">Алтернативно, у пољима **Од датума** и **До данас** дефинишите датумски интервал.</span><span class="sxs-lookup"><span data-stu-id="c3780-155">Alternatively, in the **From date** and **To date** fields, define the date interval.</span></span>
    2. <span data-ttu-id="c3780-156">Опционално: Да бисте у упит укључили само обрачунате трансакције као приход, поставите опцију **Укључите само обрачунате приходе** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="c3780-156">Optional: To include only billed transactions as revenue in the inquiry, set the **Include only billed revenues** option to **Yes**.</span></span>

## <a name="columns"></a><span data-ttu-id="c3780-157">Колоне</span><span class="sxs-lookup"><span data-stu-id="c3780-157">Columns</span></span>

<span data-ttu-id="c3780-158">Распоред трошкова истраге савезне помоћи укључује следеће колоне:</span><span class="sxs-lookup"><span data-stu-id="c3780-158">The Schedule of Expenditures of Federal Awards inquiry includes the following columns:</span></span>

- <span data-ttu-id="c3780-159">Каталог назива група Савезне домаће помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-159">Catalog of Federal Domestic Assistance cluster name</span></span>
- <span data-ttu-id="c3780-160">Агенција која даје помоћ</span><span class="sxs-lookup"><span data-stu-id="c3780-160">Grantor agency</span></span>
- <span data-ttu-id="c3780-161">Пролазна агенција</span><span class="sxs-lookup"><span data-stu-id="c3780-161">Pass-through agency</span></span>
- <span data-ttu-id="c3780-162">Назив помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-162">Grant name</span></span>
- <span data-ttu-id="c3780-163">ID помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-163">Grant ID</span></span>
- <span data-ttu-id="c3780-164">ID пријаве за помоћ</span><span class="sxs-lookup"><span data-stu-id="c3780-164">Grant application ID</span></span>
- <span data-ttu-id="c3780-165">Каталог Савезне домаће помоћи</span><span class="sxs-lookup"><span data-stu-id="c3780-165">Catalog of Federal Domestic Assistance</span></span>
- <span data-ttu-id="c3780-166">Признанице</span><span class="sxs-lookup"><span data-stu-id="c3780-166">Receipts</span></span>
- <span data-ttu-id="c3780-167">Расходи</span><span class="sxs-lookup"><span data-stu-id="c3780-167">Expenditures</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]