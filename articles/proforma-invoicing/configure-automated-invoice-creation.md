---
title: Конфигурисање аутоматског креирања фактуре
description: Ова тема пружа информације о најновијим начинима конфигурисања система за аутоматско генерисање фактура.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898144"
---
# <a name="configure-automated-invoice-creation"></a><span data-ttu-id="6d245-103">Конфигурисање аутоматског креирања фактуре</span><span class="sxs-lookup"><span data-stu-id="6d245-103">Configure automated invoice creation</span></span>

<span data-ttu-id="6d245-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="6d245-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6d245-105">Довршите следеће кораке да бисте конфигурисали аутоматско покретање фактура услузи Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6d245-105">Complete the following steps to configure an automated invoice run in Project operations.</span></span>

1. <span data-ttu-id="6d245-106">Идите до ставке **Подешавања** \> **Групни послови**.</span><span class="sxs-lookup"><span data-stu-id="6d245-106">Go to **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="6d245-107">Креирајте групни посао и именујте га **Креирање фактура у услузи Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="6d245-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="6d245-108">Назив групног посла мора да садржи термин „креирање фактура“.</span><span class="sxs-lookup"><span data-stu-id="6d245-108">The name of the batch job must include the term "create invoices."</span></span>
3. <span data-ttu-id="6d245-109">У пољу **Врста посла** изаберите **Ниједна**.</span><span class="sxs-lookup"><span data-stu-id="6d245-109">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="6d245-110">Подразумевано се опције **Дневна учесталост** и **Је активна** подешавају на **Да**.</span><span class="sxs-lookup"><span data-stu-id="6d245-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="6d245-111">Изаберите **Покрени ток посла**.</span><span class="sxs-lookup"><span data-stu-id="6d245-111">Select **Run Workflow**.</span></span> <span data-ttu-id="6d245-112">У дијалогу **Проналажење записа** ћете видети три тока посла:</span><span class="sxs-lookup"><span data-stu-id="6d245-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="6d245-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="6d245-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="6d245-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="6d245-114">ProcessRunner</span></span>
    - <span data-ttu-id="6d245-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="6d245-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="6d245-116">Изаберите **ProcessRunCaller**, а затим **Додај**.</span><span class="sxs-lookup"><span data-stu-id="6d245-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="6d245-117">У следећем дијалогу изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="6d245-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="6d245-118">Ток посла **Хибернација** прати ток посла **Процес**.</span><span class="sxs-lookup"><span data-stu-id="6d245-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="6d245-119">Можете изабрати и **ProcessRunner** у кораку 5.</span><span class="sxs-lookup"><span data-stu-id="6d245-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="6d245-120">Након тога, када изаберете **У реду**, ток посла **Процес** ће бити праћен током посла **Хибернација**.</span><span class="sxs-lookup"><span data-stu-id="6d245-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="6d245-121">Токови посла **ProcessRunCaller** и **ProcessRunner** креирају фактуре.</span><span class="sxs-lookup"><span data-stu-id="6d245-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="6d245-122">**ProcessRunCaller** позива **ProcessRunner**.</span><span class="sxs-lookup"><span data-stu-id="6d245-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="6d245-123">**ProcessRunner** је ток посла који заправо креира фактуре.</span><span class="sxs-lookup"><span data-stu-id="6d245-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="6d245-124">Он пролази кроз све предмете уговора за које се морају креирати фактуре и креира фактуре за те предмете.</span><span class="sxs-lookup"><span data-stu-id="6d245-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="6d245-125">Да би одредио предмете уговора за које фактуре морају бити креиране, посао тражи датуме покретања фактуре за предмете уговора.</span><span class="sxs-lookup"><span data-stu-id="6d245-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="6d245-126">Ако предмети уговора који припадају једном уговору имају исти датум покретања фактуре, трансакције се комбинују у једну фактуру која има две ставке фактуре.</span><span class="sxs-lookup"><span data-stu-id="6d245-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="6d245-127">Ако не постоје трансакције за које треба креирати фактуре, посао прескаче креирање фактуре.</span><span class="sxs-lookup"><span data-stu-id="6d245-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="6d245-128">Након што се **ProcessRunner** покрене, он позива **ProcessRunCaller**, обезбеђује време завршетка и затвара се.</span><span class="sxs-lookup"><span data-stu-id="6d245-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="6d245-129">**ProcessRunCaller** затим покреће тајмер који ће бити покренут током периода од 24 часа од одређеног времена завршетка.</span><span class="sxs-lookup"><span data-stu-id="6d245-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="6d245-130">На крају тајмера **ProcessRunCaller** се затвара.</span><span class="sxs-lookup"><span data-stu-id="6d245-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="6d245-131">Посао групне обраде за креирање фактура је периодични посао.</span><span class="sxs-lookup"><span data-stu-id="6d245-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="6d245-132">Ако се ова групна обрада покреће више пута, креира се више инстанци посла и изазивају грешке.</span><span class="sxs-lookup"><span data-stu-id="6d245-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="6d245-133">Због тога би требало само једном да покренете групну обраду и требало би да је поново покренете само ако престане да ради.</span><span class="sxs-lookup"><span data-stu-id="6d245-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="6d245-134">Групно фактурисање се изводи само за предмете уговора о пројекту који су конфигурисани према распоредима фактура.</span><span class="sxs-lookup"><span data-stu-id="6d245-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="6d245-135">Предмет уговора са начином наплате уз фиксну цену мора да има конфигурисане контролне тачке.</span><span class="sxs-lookup"><span data-stu-id="6d245-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="6d245-136">Предмет уговора за пројекат са начином наплате времена и материјала треба да успостави распоред фактура на основу датума.</span><span class="sxs-lookup"><span data-stu-id="6d245-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="6d245-137">Исто се односи и на предмет уговора заснован на пројекту.</span><span class="sxs-lookup"><span data-stu-id="6d245-137">The same applies to a project-based contract line.</span></span>     
