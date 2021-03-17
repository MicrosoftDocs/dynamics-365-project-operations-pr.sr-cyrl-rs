---
title: Интеграција услуге Microsoft Project Client
description: Планирање и одржавање распореда пројекта може бити сложено, па менаџери пројеката морају да користе алате који им помажу у управљању овим задатком. Интеграција са услугом Microsoft Project Client пружа подршку за отварање и управљање структурне анализе посла на пројекту.
author: Yowelle
manager: AnnBe
ms.date: 12/11/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: e93d23559d1f3aca9022cd97dae3b0726bb5ca05
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289342"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="7826d-104">Интеграција услуге Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="7826d-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="7826d-105">Планирање и одржавање распореда пројекта може бити сложено, па менаџери пројеката морају да користе алате који им помажу у управљању овим задатком.</span><span class="sxs-lookup"><span data-stu-id="7826d-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="7826d-106">Интеграција са услугом Microsoft Project Client пружа подршку за отварање и управљање структурне анализе посла на пројекту.</span><span class="sxs-lookup"><span data-stu-id="7826d-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="7826d-107">Менаџер пројекта може објавити све промене на структурној анализи посла Dynamics 365 Finance пројекта.</span><span class="sxs-lookup"><span data-stu-id="7826d-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="7826d-108">Ако користите исправку из јула (верзија 10.0.4), морате инсталирати KB 4054797 и 4055884.</span><span class="sxs-lookup"><span data-stu-id="7826d-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="7826d-109">Конфигурисање програмског додатка за Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="7826d-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="7826d-110">Да бисте омогућили интеграцију са услугом Microsoft Project Client, потребно је да инсталирате Microsoft Dynamics 365 програмски додатак у корисниковој клијентској апликацији Microsoft Project.</span><span class="sxs-lookup"><span data-stu-id="7826d-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="7826d-111">То се постиже отварањем **Радног простора за управљање пројектима**.</span><span class="sxs-lookup"><span data-stu-id="7826d-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="7826d-112">•   Кликните на **Конфигуриши програмски додатак за клијента** из одељка **Везе** > **Подешавањ** радног простора.</span><span class="sxs-lookup"><span data-stu-id="7826d-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="7826d-113">•   Кликните на **Отвори**, а затим кликните на **Покрени** када то буде затражено.</span><span class="sxs-lookup"><span data-stu-id="7826d-113">•   Click **Open**, then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="7826d-114">Отворите и уредите постојећу пробну верзију структурне анализе посла у програму Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="7826d-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="7826d-115">Ако пројекат у услузи Dynamics 365 Finance већ има креирану структурну анализу посла, структурна анализа посла може се отворити у апликацији Microsoft Project Client ако је структурна анализа посла у статусу радне верзије.</span><span class="sxs-lookup"><span data-stu-id="7826d-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="7826d-116">Да бисте отворили страницу **Пројекат**, кликните на везу **Отвори у програму Microsoft Project** на картици **План**. Ова страница се такође може отворити из апликације Microsoft Project Client кликом на **Отвори** на картици **Microsoft Dynamics 365**. Изаберите **Правно лице** и **Пројекат** са листе.</span><span class="sxs-lookup"><span data-stu-id="7826d-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="7826d-117">Ако користите Internet Explorer као прегледач, мораћете да кликнете на **Сачувај** да бисте је ручно отворили са локације на коју се датотека преузима.</span><span class="sxs-lookup"><span data-stu-id="7826d-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="7826d-118">Или кликните на **Сачувај и отвори** да бисте отворили датотеку у програму Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="7826d-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="7826d-119">Немојте да преименујете назив датотеке приликом чувања.</span><span class="sxs-lookup"><span data-stu-id="7826d-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="7826d-120">Пре него што извршите било какву измену датотеке користећи Microsoft Project Client, треба да је проверите. Кликните на **Провери** на картици **Microsoft Dynamics 365**. Ово ће спречити друге кориснике да истовремено уређују структурну анализу посла из услуге Finance.</span><span class="sxs-lookup"><span data-stu-id="7826d-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="7826d-121">Да бисте објавили структурну анализу посла након довршавања било каквих измена, кликните на **Пријави** на картици **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="7826d-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="7826d-122">Ако је пројектни тим већ додат пројекту у услузи Finance, листа ресурса ће се попунити члановима тима.</span><span class="sxs-lookup"><span data-stu-id="7826d-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="7826d-123">Ако пројектни тим још није додат у пројекат, можете одабрати ресурсе и изградити тим унутар апликације Microsoft Project Client кликом на дугме **Ресурси** на картици **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="7826d-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="7826d-124">Следећи подаци ће се синхронизовати натраг у Finance као део процеса пријаве:</span><span class="sxs-lookup"><span data-stu-id="7826d-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="7826d-125">•   Назив задатка</span><span class="sxs-lookup"><span data-stu-id="7826d-125">•   Task name</span></span>

<span data-ttu-id="7826d-126">•   Датум почетка</span><span class="sxs-lookup"><span data-stu-id="7826d-126">•   Start date</span></span>

<span data-ttu-id="7826d-127">•   Датум завршетка</span><span class="sxs-lookup"><span data-stu-id="7826d-127">•   Finish date</span></span>

<span data-ttu-id="7826d-128">•   Претходни задаци</span><span class="sxs-lookup"><span data-stu-id="7826d-128">•   Predecessors</span></span>

<span data-ttu-id="7826d-129">•   Називи ресурса</span><span class="sxs-lookup"><span data-stu-id="7826d-129">•   Resource names</span></span>

<span data-ttu-id="7826d-130">•   Категорија</span><span class="sxs-lookup"><span data-stu-id="7826d-130">•   Category</span></span>

<span data-ttu-id="7826d-131">•   Категорија ресурса</span><span class="sxs-lookup"><span data-stu-id="7826d-131">•   Resource category</span></span>

<span data-ttu-id="7826d-132">•   Радно време</span><span class="sxs-lookup"><span data-stu-id="7826d-132">•   Work hours</span></span>

<span data-ttu-id="7826d-133">•   Напомене</span><span class="sxs-lookup"><span data-stu-id="7826d-133">•   Notes</span></span>

<span data-ttu-id="7826d-134">•   Приоритет</span><span class="sxs-lookup"><span data-stu-id="7826d-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="7826d-135">Ако додате било коју другу колону у Microsoft Project Client датотеку, она неће бити сачувана у датотеци и неће се приказати када се датотека поново отвори.</span><span class="sxs-lookup"><span data-stu-id="7826d-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="7826d-136">Направите структурну анализу посла за постојећи пројекат користећи Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="7826d-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="7826d-137">Да бисте креирали структурну анализу посла користећи Microsoft Project Client, следите ове кораке:</span><span class="sxs-lookup"><span data-stu-id="7826d-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="7826d-138">Отворите Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="7826d-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="7826d-139">На картици **Microsoft Dynamics 365**, кликните на **Отвори**.</span><span class="sxs-lookup"><span data-stu-id="7826d-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="7826d-140">Изаберите **Правно лице** за пројекат.</span><span class="sxs-lookup"><span data-stu-id="7826d-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="7826d-141">Изаберите **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="7826d-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="7826d-142">Кликните на **Провери** на картици **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="7826d-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="7826d-143">Када будете спремни за објављивање у Finance, кликните на **Пријави** на картици **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="7826d-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="7826d-144">Замените постојећу структурну анализу посла за постојећи пројекат користећи Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="7826d-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="7826d-145">Да бисте креирали нову структурну анализу посла помоћу апликације Microsoft Project Client и заменили постојећу структурну анализу посла за постојећи пројекат, следите ове кораке:</span><span class="sxs-lookup"><span data-stu-id="7826d-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="7826d-146">Отворите Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="7826d-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="7826d-147">Креирајте распоред у апликацији Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="7826d-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="7826d-148">На картици **Microsoft Dynamics 365**, кликните на **Сачувај промене** > **Замени постојећи пројекат**.</span><span class="sxs-lookup"><span data-stu-id="7826d-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="7826d-149">Изаберите **Правно лице** за пројекат.</span><span class="sxs-lookup"><span data-stu-id="7826d-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="7826d-150">Изаберите **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="7826d-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="7826d-151">Кликните на дугме **У реду**.</span><span class="sxs-lookup"><span data-stu-id="7826d-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="7826d-152">Креирајте нови пројекат из апликације Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="7826d-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="7826d-153">Отворите Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="7826d-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="7826d-154">Креирајте распоред у апликацији Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="7826d-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="7826d-155">На картици **Microsoft Dynamics 365**, кликните на **Сачувај промене** > **Сачувај у нови пројекат**.</span><span class="sxs-lookup"><span data-stu-id="7826d-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="7826d-156">Изаберите **Правно лице** за пројекат.</span><span class="sxs-lookup"><span data-stu-id="7826d-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="7826d-157">Унесите **ID пројекта**, ако је неопходно.</span><span class="sxs-lookup"><span data-stu-id="7826d-157">Enter the **Project ID**, if necessary.</span></span>

6.  <span data-ttu-id="7826d-158">Унесите **Назив пројекта**.</span><span class="sxs-lookup"><span data-stu-id="7826d-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="7826d-159">Изаберите **Тип пројекта**, **Групу пројекта** и **ID уговора о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="7826d-159">Select the **Project type**, **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="7826d-160">Алтернативно, можете да креирате нови уговор о пројекту кликом на **Ново**.</span><span class="sxs-lookup"><span data-stu-id="7826d-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="7826d-161">Изаберите **Календар** који ћете користити за обезбеђивање ресурса.</span><span class="sxs-lookup"><span data-stu-id="7826d-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="7826d-162">Кликните на дугме **У реду**.</span><span class="sxs-lookup"><span data-stu-id="7826d-162">Click **OK**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]