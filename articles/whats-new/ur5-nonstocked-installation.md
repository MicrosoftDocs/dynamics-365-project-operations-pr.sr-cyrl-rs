---
title: Ажурирање услуге Project Operations у Finance окружењу
description: Ова тема пружа информације о томе како да ажурирате услугу Project Operations у Dynamics 365 Finance окружењу.
author: ruhercul
manager: tfehr
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d68296ec59f0bd58f848154c90e02c58f275ab12
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291997"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="3c21c-103">Ажурирање услуге Project Operations у Finance окружењу</span><span class="sxs-lookup"><span data-stu-id="3c21c-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="3c21c-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="3c21c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="3c21c-105">Ова тема пружа информације о томе како да ажурирате Dynamics 365 Project Operations у Dynamics 365 Finance окружењу.</span><span class="sxs-lookup"><span data-stu-id="3c21c-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="3c21c-106">Постоје три процедуре потребне за ажурирање услуге Project Operations на исправку 5 (Microsoft Dynamics CRM 2011 Update Rollup 5):</span><span class="sxs-lookup"><span data-stu-id="3c21c-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="3c21c-107">Увоз пакета у пројекат прегледа</span><span class="sxs-lookup"><span data-stu-id="3c21c-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="3c21c-108">Примена исправке</span><span class="sxs-lookup"><span data-stu-id="3c21c-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="3c21c-109">Ажурирање Dataverse окружења</span><span class="sxs-lookup"><span data-stu-id="3c21c-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="3c21c-110">Увоз пакета у LCS пројекат</span><span class="sxs-lookup"><span data-stu-id="3c21c-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="3c21c-111">Пријавите се на [Lifecycle Services (LCS)](https://lcs.dynamics.com/) као власник пројекта или менаџер окружења.</span><span class="sxs-lookup"><span data-stu-id="3c21c-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="3c21c-112">Са листе пројеката одаберите LCS пројекат.</span><span class="sxs-lookup"><span data-stu-id="3c21c-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="3c21c-113">На страници **Пројекат** у групи **Окружења** отворите окружење које желите да ажурирате.</span><span class="sxs-lookup"><span data-stu-id="3c21c-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="3c21c-114">Проверите да ли је окружење покренуто.</span><span class="sxs-lookup"><span data-stu-id="3c21c-114">Verify that the environment is running.</span></span> <span data-ttu-id="3c21c-115">Ако није покренуто, покрените окружење.</span><span class="sxs-lookup"><span data-stu-id="3c21c-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="3c21c-116">У одељку **Ново издање** под **Доступне исправке** изаберите **Прикажи исправку** за 10.0.15.</span><span class="sxs-lookup"><span data-stu-id="3c21c-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

![Дугме „Прикажи исправку“](media/view-update.png)

6. <span data-ttu-id="3c21c-118">На страници **Бинарна ажурирања** изаберите **Сачувај пакет**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="3c21c-119">На страници **Преглед и чување исправки** изаберите **Сачувај пакет**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="3c21c-120">У окну **Чување пакета у библиотеци средстава** које се отвори унесите назив пакета, а затим изаберите **Сачувај пакет**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="3c21c-121">Када LCS заврши чување пакета, дугме **Готово** ће бити омогућено.</span><span class="sxs-lookup"><span data-stu-id="3c21c-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="3c21c-122">Изаберите **Готово**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-122">Select **Done**.</span></span> <span data-ttu-id="3c21c-123">LCS ће верификовати пакет.</span><span class="sxs-lookup"><span data-stu-id="3c21c-123">LCS will verify the package.</span></span> <span data-ttu-id="3c21c-124">Верификација може трајати неколико минута, највише до сат времена.</span><span class="sxs-lookup"><span data-stu-id="3c21c-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="3c21c-125">Примена исправке пакета</span><span class="sxs-lookup"><span data-stu-id="3c21c-125">Apply the package update</span></span>

1. <span data-ttu-id="3c21c-126">У услузи LCS, на страници **Детаљи окружења** изаберите **Одржавај** > **Примени исправке**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="3c21c-127">На листи изаберите пакет који сте раније сачували, а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="3c21c-128">Изаберите **Да** да бисте потврдили да желите да примените пакет.</span><span class="sxs-lookup"><span data-stu-id="3c21c-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![Потврдите избор у дијалогу „Примена пакета“](media/confirm-package-deployment.png)

4. <span data-ttu-id="3c21c-130">Изаберите **Да** да бисте потврдили да желите да ажурирате апликацију.</span><span class="sxs-lookup"><span data-stu-id="3c21c-130">Select **Yes** to confirm that you want to update the application.</span></span>

![Потврдите избор у дијалогу „Ажурирање апликације“](media/confirm-application-update.png)

<span data-ttu-id="3c21c-132">Покренуће се примена и ажурирање апликације.</span><span class="sxs-lookup"><span data-stu-id="3c21c-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="3c21c-133">На страници **Детаљи окружења**, у горњем десном углу, статус окружења ће се ажурирати на **Сервисирање**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="3c21c-134">За отприлике два сата ажурирање ће бити готово.</span><span class="sxs-lookup"><span data-stu-id="3c21c-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="3c21c-135">Информације о издању апликације ће се ажурирати на **Microsoft Dynamics 365 for Finance and Operations 10.0.15** а статус окружења ће се ажурирати на **Примењено**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><a name="update"></a><span data-ttu-id="3c21c-136">Ажурирање Dataverse окружења</span><span class="sxs-lookup"><span data-stu-id="3c21c-136">Update your Dataverse environment</span></span>

1. <span data-ttu-id="3c21c-137">Пријавите се у [Power Platform центар администрације](https://admin.powerplatform.com/).</span><span class="sxs-lookup"><span data-stu-id="3c21c-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="3c21c-138">На листи пронађите и отворите окружење које сте користили за инсталирање услуге Project Operations.</span><span class="sxs-lookup"><span data-stu-id="3c21c-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="3c21c-139">На страници **Окружења** изаберите **Ресурс** > **Dynamics 365 апликације**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="3c21c-140">На листи пронађите **Microsoft Dynamics 365 Project Operations** и у колони **Статус** изаберите **Доступна исправка**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="3c21c-141">Означите поље за потврду **Слажем се са условима коришћења услуге**, а затим изаберите **Ажурирај**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="3c21c-142">Биће инсталирана најновија верзија решења.</span><span class="sxs-lookup"><span data-stu-id="3c21c-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="3c21c-143">По завршетку инсталације имаћете инсталирану верзију 4.5.0.134.</span><span class="sxs-lookup"><span data-stu-id="3c21c-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="3c21c-144">Конфигурисање нових функција</span><span class="sxs-lookup"><span data-stu-id="3c21c-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="3c21c-145">Омогућавање мапирања двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="3c21c-145">Enable dual-write mapping</span></span>

<span data-ttu-id="3c21c-146">Након што довршите ажурирање Finance и Dataverse окружења, можете омогућити потребна мапирања двоструког уписивања.</span><span class="sxs-lookup"><span data-stu-id="3c21c-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="3c21c-147">Обавите следеће процедуре да бисте омогућили мапирање двоструког уписивања.</span><span class="sxs-lookup"><span data-stu-id="3c21c-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="3c21c-148">Ажурирање безбедоносних подешавања у Customer Engagement окружењу</span><span class="sxs-lookup"><span data-stu-id="3c21c-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="3c21c-149">Освежавање ентитета података</span><span class="sxs-lookup"><span data-stu-id="3c21c-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="3c21c-150">Ажурирање и покретање мапирања двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="3c21c-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="3c21c-151">Ажурирање безбедоносних подешавања у Dataverse окружењу</span><span class="sxs-lookup"><span data-stu-id="3c21c-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="3c21c-152">Следеће исправке безбедносних привилегија за ентитете су потребне као део ажурирања на Microsoft Dynamics CRM 2011 Update Rollup 5.</span><span class="sxs-lookup"><span data-stu-id="3c21c-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="3c21c-153">У окружењу Dataverse идите на **Подешавања** и у групи **Систем** изаберите **Безбедност**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![Подешавања Dataverse окружења](media/Picture21.png)

2. <span data-ttu-id="3c21c-155">Изаберите **Безбедносне улоге**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="3c21c-156">Са листе улога изаберите **корисник апликације за двоструко уписивање** и изаберите картицу **Прилагођени ентитети**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="3c21c-157">Проверите да ли улога има дозволе **Читање** и **Приложи у** за:</span><span class="sxs-lookup"><span data-stu-id="3c21c-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="3c21c-158">**Тип девизног курса валуте**</span><span class="sxs-lookup"><span data-stu-id="3c21c-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="3c21c-159">**Графикон пословних контаката**</span><span class="sxs-lookup"><span data-stu-id="3c21c-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="3c21c-160">**Фискални календар**</span><span class="sxs-lookup"><span data-stu-id="3c21c-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="3c21c-161">**Главна књига**</span><span class="sxs-lookup"><span data-stu-id="3c21c-161">**Ledger**</span></span>

5. <span data-ttu-id="3c21c-162">Након ажурирања безбедносне улоге, идите на **Подешавања** > **Безбедност** > **Тимови**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="3c21c-163">Проверите да ли је улога **корисник апликације за двоструко уписивање** примењена на тим.</span><span class="sxs-lookup"><span data-stu-id="3c21c-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="3c21c-164">Освежавање ентитета података из исправке</span><span class="sxs-lookup"><span data-stu-id="3c21c-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="3c21c-165">У Finance окружењу отворите радни простор **Управљање подацима**, а затим отворите страницу **Параметри оквира**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="3c21c-166">На картици **Подешавања ентитета** изаберите **Освежи листу ентитета**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="3c21c-167">Изаберите **Затвори** да бисте потврдили освежавање ентитета.</span><span class="sxs-lookup"><span data-stu-id="3c21c-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="3c21c-168">Овај поступак ће се завршити за око 20 минута.</span><span class="sxs-lookup"><span data-stu-id="3c21c-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="3c21c-169">Бићете обавештени када се освежавање заврши.</span><span class="sxs-lookup"><span data-stu-id="3c21c-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="3c21c-170">Ажурирање мапирања двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="3c21c-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="3c21c-171">У радном простору **Управљање подацима** изаберите **Двоструко уписивање**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="3c21c-172">Изаберите **Примени решења**, изаберите оба решења са листе, а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="3c21c-173">На страници **Двоструко уписивање** изаберите следеће мапе табела, а затим изаберите **Заустави**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="3c21c-174">**Project Operations стварне вредности интеграције (msdyn_actuals)**</span><span class="sxs-lookup"><span data-stu-id="3c21c-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="3c21c-175">**Project Operations интеграција категорија трошкова пројеката (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="3c21c-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="3c21c-176">**Ентитет за извоз трошкова пројеката за Project Operations стварне вредности интеграције (msdyn_expenses)**</span><span class="sxs-lookup"><span data-stu-id="3c21c-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="3c21c-177">На страници **Верзија мапе табеле** примените нову верзију мапе на сваки од три ентитета.</span><span class="sxs-lookup"><span data-stu-id="3c21c-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="3c21c-178">На страници **Двоструко уписивање** изаберите „Покрени“ да бисте поново покренули мапе.</span><span class="sxs-lookup"><span data-stu-id="3c21c-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="3c21c-179">На листи мапа одаберите мапу **Главна књига (msdyn_ledgers)** са свим предусловима и означите поље за потврду **Почетна синхронизација**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="3c21c-180">У пољу **Мастер за почетну синхронизацију** изаберите **Finance and Operations апликације**, а затим изаберите **Покрени**.</span><span class="sxs-lookup"><span data-stu-id="3c21c-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![Синхронизација мапе главне књиге](media/DW6.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]