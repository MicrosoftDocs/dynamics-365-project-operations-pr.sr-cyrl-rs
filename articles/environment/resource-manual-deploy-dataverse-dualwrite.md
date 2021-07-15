---
title: Ручно распоређивање Project Operations Dataverse апликације са подршком за двоструко уписивање
description: Ова тема објашњава како да ручно примените Project Operations Dataverse апликацију тако да подржава двоструко уписивање.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/18/2021
ms.locfileid: "6274026"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a><span data-ttu-id="e6e93-103">Ручно распоређивање Project Operations Dataverse апликације са подршком за двоструко уписивање</span><span class="sxs-lookup"><span data-stu-id="e6e93-103">Manually deploy the Project Operations Dataverse app with dual-write support</span></span>

<span data-ttu-id="e6e93-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="e6e93-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e6e93-105">Ова тема објашњава како да ручно примените апликацију Microsoft Dynamics 365 Project Operations на платформи Microsoft Dataverse тако да подржава двоструко уписивање.</span><span class="sxs-lookup"><span data-stu-id="e6e93-105">This topic explains how to manually deploy Microsoft Dynamics 365 Project Operations in Microsoft Dataverse so that it supports dual-write.</span></span> <span data-ttu-id="e6e93-106">Project Operations открива конфигурацију окружења и додаје додатну подршку за двоструко уписивање ако су испуњени предуслови.</span><span class="sxs-lookup"><span data-stu-id="e6e93-106">Project Operations detects the environment's configuration and adds additional support for dual-write if the prerequisites are met.</span></span>

<span data-ttu-id="e6e93-107">Током примене преко услуге Microsoft Dynamics Lifecycle Services (LCS), ако сте следили упутства у овој теми, можете прескочити примену Microsoft Power Platform интеграције (раније познате као Common Data Service окружење).</span><span class="sxs-lookup"><span data-stu-id="e6e93-107">During deployment through Microsoft Dynamics Lifecycle Services (LCS), if you've followed the instructions in this topic, you can skip the deployment of the Microsoft Power Platform integration (previously known as the Common Data Service environment).</span></span>

<span data-ttu-id="e6e93-108">Процес примене услуге Project Operations на платформи Dataverse тако да подржава двоструко уписивање има четири главна корака:</span><span class="sxs-lookup"><span data-stu-id="e6e93-108">The process of deploying Project Operations in Dataverse so that it supports dual-write has four main steps:</span></span>

1. <span data-ttu-id="e6e93-109">[Креирање новог окружења на платформи Dataverse које подржава двоструко уписивање](#create).</span><span class="sxs-lookup"><span data-stu-id="e6e93-109">[Create a new environment in Dataverse that supports dual-write](#create).</span></span>
2. <span data-ttu-id="e6e93-110">[Додавање предуслова за двоструко уписивање у окружење](#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="e6e93-110">[Add dual-write prerequisites to the environment](#prerequisites).</span></span>
3. <span data-ttu-id="e6e93-111">[Додавање апликације Project Operations Dataverse](#dataverse).</span><span class="sxs-lookup"><span data-stu-id="e6e93-111">[Add the Project Operations Dataverse app](#dataverse).</span></span>
4. <span data-ttu-id="e6e93-112">[Повезивање окружења](#link).</span><span class="sxs-lookup"><span data-stu-id="e6e93-112">[Link your environments](#link).</span></span>

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a><span data-ttu-id="e6e93-113">Креирање новог окружења на платформи Dataverse које подржава двоструко уписивање</span><span class="sxs-lookup"><span data-stu-id="e6e93-113">Create a new environment in Dataverse that supports dual-write</span></span>

<span data-ttu-id="e6e93-114">Да бисте довршили ову процедуру, морате се пријавити као администратор.</span><span class="sxs-lookup"><span data-stu-id="e6e93-114">To complete this procedure, you must sign in as an administrator.</span></span>

1. <span data-ttu-id="e6e93-115">Отворите [Power Platform центар администрације](https://admin.powerplatform.com) и пријавите се као администратор.</span><span class="sxs-lookup"><span data-stu-id="e6e93-115">Open the [Power Platform admin center](https://admin.powerplatform.com), and sign in as an administrator.</span></span>
2. <span data-ttu-id="e6e93-116">Креирајте ново окружење и именујте га.</span><span class="sxs-lookup"><span data-stu-id="e6e93-116">Create a new environment, and name it.</span></span>
3. <span data-ttu-id="e6e93-117">Изаберите тип окружења.</span><span class="sxs-lookup"><span data-stu-id="e6e93-117">Select the environment type.</span></span> <span data-ttu-id="e6e93-118">Ако сте се пријавили за понуду пробне верзије, изаберите **Пробна верзија (заснована на претплати)**.</span><span class="sxs-lookup"><span data-stu-id="e6e93-118">If you signed up for the trial offer, select **Trial (subscription-based)**.</span></span>
4. <span data-ttu-id="e6e93-119">Потврдите регион примене.</span><span class="sxs-lookup"><span data-stu-id="e6e93-119">Confirm the deployment region.</span></span>
5. <span data-ttu-id="e6e93-120">Омогућите опцију **Креирање базе података за ово окружење**.</span><span class="sxs-lookup"><span data-stu-id="e6e93-120">Enable the **Create a database for this environment** option.</span></span> 
6. <span data-ttu-id="e6e93-121">Потврдите језик, а затим потврдите да се валута подудара са валутом за ваше Finance and Operations апликације.</span><span class="sxs-lookup"><span data-stu-id="e6e93-121">Confirm the language, and then confirm that the currency matches the currency for your Finance and Operations apps.</span></span>
7. <span data-ttu-id="e6e93-122">Омогућите **Dynamics 365 апликације** и потврдите да је поље **Аутоматски примени ове апликације** подешено на **Ниједна**.</span><span class="sxs-lookup"><span data-stu-id="e6e93-122">Enable the **Dynamics 365 apps** option, and confirm that the **Automatically deploy these apps** field is set to **None**.</span></span>
8. <span data-ttu-id="e6e93-123">Додајте безбедносну групу ако је потребна безбедносна група.</span><span class="sxs-lookup"><span data-stu-id="e6e93-123">Add a security group, if a security group is required.</span></span>
9. <span data-ttu-id="e6e93-124">Изаберите **Сачувај** да бисте креирали окружење.</span><span class="sxs-lookup"><span data-stu-id="e6e93-124">Select **Save** to create the environment.</span></span>
10. <span data-ttu-id="e6e93-125">Сачекајте док се примена не заврши и окружење не достигне статус **Спремно**.</span><span class="sxs-lookup"><span data-stu-id="e6e93-125">Wait until the deployment is completed and the environment reaches the **Ready** state.</span></span>

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a><span data-ttu-id="e6e93-126">Додавање предуслова за двоструко уписивање у окружење</span><span class="sxs-lookup"><span data-stu-id="e6e93-126">Add dual-write prerequisites to the environment</span></span>

<span data-ttu-id="e6e93-127">Подршка за двоструко уписивање укључује додатна поља која се додају кључним ентитетима, као што је ентитет **Предузеће**.</span><span class="sxs-lookup"><span data-stu-id="e6e93-127">Dual-write support includes additional fields that are added to key entities, such as the **Company** entity.</span></span> <span data-ttu-id="e6e93-128">Ако додајете подршку за двоструко уписивање у постојеће окружење, можда ћете морати да ажурирате податке да бисте га омогућили.</span><span class="sxs-lookup"><span data-stu-id="e6e93-128">If you're adding dual-write support to an existing environment, you might have to update the data to enable the support.</span></span> <span data-ttu-id="e6e93-129">За информације о начину покретања података, погледајте чланак [Подаци за покретање предузећа](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span><span class="sxs-lookup"><span data-stu-id="e6e93-129">For information about how to bootstrap the data, see [Bootstrap company data](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span></span> <span data-ttu-id="e6e93-130">За више информација о двоструком уписивању, погледајте чланак [Системски захтеви за двоструко уписивање](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span><span class="sxs-lookup"><span data-stu-id="e6e93-130">For more information about dual-write, see [Dual-write system requirements](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span></span>

<span data-ttu-id="e6e93-131">Довршите овај поступак да бисте додали предуслове за двоструко уписивање у своје окружење.</span><span class="sxs-lookup"><span data-stu-id="e6e93-131">Complete this procedure to add the dual-write prerequisites to your environment.</span></span>

1. <span data-ttu-id="e6e93-132">Отворите окружење које сте управо креирали, а затим идите у **Ресурс** \> **Dynamics 365 апликације**.</span><span class="sxs-lookup"><span data-stu-id="e6e93-132">Open the environment that you just created, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="e6e93-133">Изаберите **Основно решење са двоструким уписивањем** на листи апликација и инсталирајте га.</span><span class="sxs-lookup"><span data-stu-id="e6e93-133">Select **Dual-write core solution** in the app list, and install it.</span></span>
3. <span data-ttu-id="e6e93-134">Сачекајте док се инсталација не заврши.</span><span class="sxs-lookup"><span data-stu-id="e6e93-134">Wait until the installation is completed.</span></span> <span data-ttu-id="e6e93-135">Затим изаберите **Решење оркестрације апликације са двоструким уписивањем** на листи апликација и инсталирајте га.</span><span class="sxs-lookup"><span data-stu-id="e6e93-135">Then select **Dual-write application orchestration solution** in the app list, and install it.</span></span>

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a><span data-ttu-id="e6e93-136">Додавање Project Operations Dataverse апликације</span><span class="sxs-lookup"><span data-stu-id="e6e93-136">Add the Project Operations Dataverse app</span></span>

<span data-ttu-id="e6e93-137">Ову процедуру можете довршити само ако сте завршили претходне процедуре пре него што сте инсталирали Project Operations.</span><span class="sxs-lookup"><span data-stu-id="e6e93-137">You can complete this procedure only if you completed the previous procedures before you installed Project Operations.</span></span> <span data-ttu-id="e6e93-138">Током инсталације, систем анализира конфигурацију окружења и додаје подршку за двоструко уписивање ако је потребно.</span><span class="sxs-lookup"><span data-stu-id="e6e93-138">During installation, the system analyzes the environment configuration and adds support for dual-write if it's required.</span></span>

1. <span data-ttu-id="e6e93-139">Отворите окружење које сте раније креирали, а затим идите у **Ресурс** \> **Dynamics 365 апликације**.</span><span class="sxs-lookup"><span data-stu-id="e6e93-139">Open the environment that you created earlier, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="e6e93-140">Изаберите **Microsoft Dynamics 365 Project Operations** на листи апликација и инсталирајте је.</span><span class="sxs-lookup"><span data-stu-id="e6e93-140">Select **Microsoft Dynamics 365 Project Operations** in the app list, and install it.</span></span>

## <a name="link-your-environments"></a><a name="link"></a><span data-ttu-id="e6e93-141">Повезивање окружења</span><span class="sxs-lookup"><span data-stu-id="e6e93-141">Link your environments</span></span>

<span data-ttu-id="e6e93-142">Када се Dataverse окружење примени, можете подесити везу у својим Finance and Operations апликацијама.</span><span class="sxs-lookup"><span data-stu-id="e6e93-142">After the Dataverse environment is deployed, you can set up the link in your Finance and Operations apps.</span></span> <span data-ttu-id="e6e93-143">Следите кораке у чланку [Коришћење чаробњака за двоструко уписивање ради повезивања окружења](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span><span class="sxs-lookup"><span data-stu-id="e6e93-143">Follow the steps in [Use the dual-write wizard to link your environments](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span></span>
