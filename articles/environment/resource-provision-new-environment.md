---
title: Обезбеђење новог окружења
description: Ова тема пружа информације о начину обезбеђења новог Project Operations окружења.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a43b947207b6d4276ef27ec996713bf3883e7906
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083859"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="32bc6-103">Обезбеђење новог окружења</span><span class="sxs-lookup"><span data-stu-id="32bc6-103">Provision a new environment</span></span>

<span data-ttu-id="32bc6-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="32bc6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="32bc6-105">Ова тема пружа информације о начину обезбеђења новог Dynamics 365 Project Operations окружења за сценарије засноване на ресурсима / без залиха.</span><span class="sxs-lookup"><span data-stu-id="32bc6-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="32bc6-106">Омогућавање Project Operations аутоматског обезбеђивања у LCS пројекту</span><span class="sxs-lookup"><span data-stu-id="32bc6-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="32bc6-107">Користите следеће кораке да омогућите Project Operations аутоматизовани ток обезбеђивања за ваш LCS пројекат.</span><span class="sxs-lookup"><span data-stu-id="32bc6-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="32bc6-108">Идите на [LCS](https://lcs.dynamics.com/v2) и изаберите плочицу **Преглед управљања функцијама**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="32bc6-109">На листи **Функција прегледа** изаберите **Project Operations Feature** и изаберите **Омогућена функција прегледа** како би се омогућила услуга Project Operations.</span><span class="sxs-lookup"><span data-stu-id="32bc6-109">In the **Preview feature** list, select **Project Operations Feature** , and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="32bc6-110">Овај корак се изводи само једном по LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="32bc6-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="32bc6-111">Обезбеђивање Project Operations окружења</span><span class="sxs-lookup"><span data-stu-id="32bc6-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="32bc6-112">Отвори нову примену Dynamics 365 Finance [демо окружења](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) или [sandbox/производног окружења](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="32bc6-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="32bc6-113">Прођите кроз чаробњак **Обезбеђивање окружења**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="32bc6-114">Уверите се да је изабрана верзија апликације 10.0.13 или новија.</span><span class="sxs-lookup"><span data-stu-id="32bc6-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="32bc6-115">Да бисте обезбедили Project Operations, у делу **Напредна подешавања** изаберите **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-115">To provision Project Operations, under **Advance settings** , select **Common Data Service**.</span></span> 
4. <span data-ttu-id="32bc6-116">Омогућите **Common Data Service подешавање** бирајући **Да** , а затим унесите податке у обавезна поља:</span><span class="sxs-lookup"><span data-stu-id="32bc6-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="32bc6-117">Име</span><span class="sxs-lookup"><span data-stu-id="32bc6-117">Name</span></span>
  - <span data-ttu-id="32bc6-118">Регион</span><span class="sxs-lookup"><span data-stu-id="32bc6-118">Region</span></span>
  - <span data-ttu-id="32bc6-119">Језик</span><span class="sxs-lookup"><span data-stu-id="32bc6-119">Language</span></span>
  - <span data-ttu-id="32bc6-120">Валута</span><span class="sxs-lookup"><span data-stu-id="32bc6-120">Currency</span></span>
 
5. <span data-ttu-id="32bc6-121">У пољу **Common Data Service предложак** , изаберите **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="32bc6-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="32bc6-122">Изаберите врсту окружења за вашу примену.</span><span class="sxs-lookup"><span data-stu-id="32bc6-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="32bc6-123">Пробно време засновано на претплати омогућиће вам да примените CDS окружење на 30 дана.</span><span class="sxs-lookup"><span data-stu-id="32bc6-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Подешавања примене](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="32bc6-125">Изаберите **Слажем се** да бисте прихватили услове услуге, а затим изаберите **Готово** да се вратите на подешавања примене.</span><span class="sxs-lookup"><span data-stu-id="32bc6-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Сагласност за примену](./media/2DeploymentConsent.png)

7. <span data-ttu-id="32bc6-127">Попуните преостала обавезна поља у чаробњаку и потврдите примену.</span><span class="sxs-lookup"><span data-stu-id="32bc6-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="32bc6-128">Време обезбеђивања окружења варира у зависности од врсте окружења.</span><span class="sxs-lookup"><span data-stu-id="32bc6-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="32bc6-129">Обезбеђење може потрајати до шест сати.</span><span class="sxs-lookup"><span data-stu-id="32bc6-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="32bc6-130">Када се примена успешно заврши, окружење ће се приказати као **Примењено**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="32bc6-131">Да бисте потврдили да је окружење успешно постављено, изаберите **Пријављивање** и пријавите се у окружење да бисте потврдили.</span><span class="sxs-lookup"><span data-stu-id="32bc6-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Детаљи  окружења](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="32bc6-133">Примена Project Operations Finance демо података (опционални корак)</span><span class="sxs-lookup"><span data-stu-id="32bc6-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="32bc6-134">Примените Project Operations Finance демо податке на 10.0.13 издање услуге у окружењу које се хостује у облаку, као што је описано у [овом чланку](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="32bc6-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="32bc6-135">Примените исправке на Finance окружење</span><span class="sxs-lookup"><span data-stu-id="32bc6-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="32bc6-136">Project Operations захтева Finance окружење са верзијом апликације **10.0.13 (10.0.569.20009)** или новијом.</span><span class="sxs-lookup"><span data-stu-id="32bc6-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="32bc6-137">Можда ћете морати да примените исправке квалитета у свом Finance окружењу да бисте добили ову верзију.</span><span class="sxs-lookup"><span data-stu-id="32bc6-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="32bc6-138">У LCS-у, на страници **Детаљи окружења** , у одељку **Доступне исправке** изаберите **Прикажи исправку**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Приказ исправки](./media/5ViewUpdates.png)

2. <span data-ttu-id="32bc6-140">На страници **Бинарна ажурирања** изаберите **Сачувај пакет.**</span><span class="sxs-lookup"><span data-stu-id="32bc6-140">On the **Binary updates** page, select **Save package.**</span></span>

![Сачувај пакет](./media/6SavePackage.png)

3. <span data-ttu-id="32bc6-142">Кликните на **Изабери све** , а затим изаберите **Сачувај пакет**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-142">Click **Select all** and then select **Save package**.</span></span>

![Прегледајте и сачувајте исправке](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="32bc6-144">Унесите назив и опис пакета, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="32bc6-145">У зависности од интернет везе, овај поступак може потрајати.</span><span class="sxs-lookup"><span data-stu-id="32bc6-145">Depending on the internet connection, this process might take some time.</span></span>

![Отпремите пакет у библиотеку средстава](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="32bc6-147">Када се пакет сачува, изаберите **Готово** и сачувајте овај пакет у библиотеци средстава у вашем LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="32bc6-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="32bc6-148">Чување и потврђивање пакета може потрајати око 15 минута.</span><span class="sxs-lookup"><span data-stu-id="32bc6-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="32bc6-149">Да бисте применили исправку, идите на страницу **Детаљи окружења** у LCS-у и изаберите **Одржавање** > **Примени исправке**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Одржавање окружења](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="32bc6-151">На листи исправки изаберите пакет који сте креирали и изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Примена исправки](./media/10ApplyUpdates.png)

<span data-ttu-id="32bc6-153">Сервисирање окружења ће потрајати неко време.</span><span class="sxs-lookup"><span data-stu-id="32bc6-153">Environment servicing will take some time.</span></span> <span data-ttu-id="32bc6-154">По завршетку, окружење ће се вратити у примењено стање.</span><span class="sxs-lookup"><span data-stu-id="32bc6-154">After it is complete, the environment will return to a deployed state.</span></span>

![Примењено окружење](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="32bc6-156">Успоставите везу са двоструким уписивањем</span><span class="sxs-lookup"><span data-stu-id="32bc6-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="32bc6-157">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="32bc6-158">У одељку **Common Data Service информације о окружењу** , изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-158">Under **Common Data Service Environment Information** , select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="32bc6-159">Када се повезивање заврши, поново изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="32bc6-160">Бићете преусмерени на двоструко уписивање у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="32bc6-160">You will be redirected to Dual Write in Finance.</span></span>

![Повезивање са услугом CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="32bc6-162">Изаберите **Примени решење** за приступ ентитетима који ће бити мапирани у интеграцији.</span><span class="sxs-lookup"><span data-stu-id="32bc6-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Примена решења](./media/13ApplySolutions.png)

5. <span data-ttu-id="32bc6-164">Изаберите оба решења, **Dynamics 365 Finance and Operations мапа ентитета за двоструко уписивање** и **Dynamics 365 Project Operations мапе ентитета двоструког уписивања** , а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps** , and then select **Apply**.</span></span>

![Потврда решења](./media/14ConfirmSolutions.png)

<span data-ttu-id="32bc6-166">Када примените решења, ентитети двоструког уписивања се примењују на окружење.</span><span class="sxs-lookup"><span data-stu-id="32bc6-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Примена решења](./media/15ApplyingSolutions.png)

<span data-ttu-id="32bc6-168">Када се ентитети примене, сва расположива мапирања се наводе у окружењу.</span><span class="sxs-lookup"><span data-stu-id="32bc6-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Мапе за двоструко уписивање](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="32bc6-170">Освежите ентитете података након исправке</span><span class="sxs-lookup"><span data-stu-id="32bc6-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="32bc6-171">У услузи Finance идите на радни простор **Управљање подацима**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-171">In Finance, go to the **Data management** workspace.</span></span>

![Радни простор за управљање подацима](./media/16DataManagement.png)

2. <span data-ttu-id="32bc6-173">Изаберите плочицу **Параметри радног оквира**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-173">Select the **Framework parameters** tile.</span></span>

![Параметри радног оквира](./media/17FrameworkParameters.png)

3. <span data-ttu-id="32bc6-175">На страници **Подешавања ентитета** , изаберите **Освежи листу ентитета**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Освежи листу ентитета](./media/18RefreshEntityList.png)

<span data-ttu-id="32bc6-177">Освежавање ће трајати приближно 20 минута.</span><span class="sxs-lookup"><span data-stu-id="32bc6-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="32bc6-178">Добићете упозорење када се заврши.</span><span class="sxs-lookup"><span data-stu-id="32bc6-178">You will receive an alert when it is complete.</span></span>

![Потврда освежавања](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="32bc6-180">Покрените Project Operations мапе двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="32bc6-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="32bc6-181">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="32bc6-182">У одељку **Common Data Service информације о окружењу** , изаберите **Повежи са услугом CDS за апликације.**</span><span class="sxs-lookup"><span data-stu-id="32bc6-182">Under **Common Data Service Environment Information** , select **Link to CDS for Apps.**</span></span> <span data-ttu-id="32bc6-183">Када изаберете везу, бићете преусмерени на листу ентитета у мапирањима.</span><span class="sxs-lookup"><span data-stu-id="32bc6-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="32bc6-184">Покрените мапе као што је описано у следећој табели.</span><span class="sxs-lookup"><span data-stu-id="32bc6-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="32bc6-185">Уверите се да следите наведени редослед.</span><span class="sxs-lookup"><span data-stu-id="32bc6-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="32bc6-186">**Мапа ентитета**</span><span class="sxs-lookup"><span data-stu-id="32bc6-186">**Entity Map**</span></span> | <span data-ttu-id="32bc6-187">**Освежавање ентитета**</span><span class="sxs-lookup"><span data-stu-id="32bc6-187">**Refresh entity**</span></span> | <span data-ttu-id="32bc6-188">**Почетна синхронизација**</span><span class="sxs-lookup"><span data-stu-id="32bc6-188">**Initial sync**</span></span> | <span data-ttu-id="32bc6-189">**Мастер за почетну синхронизацију**</span><span class="sxs-lookup"><span data-stu-id="32bc6-189">**Master for initial sync**</span></span> | <span data-ttu-id="32bc6-190">**Предуслови за покретање**</span><span class="sxs-lookup"><span data-stu-id="32bc6-190">**Run prerequisites**</span></span> | <span data-ttu-id="32bc6-191">**Почетна синхронизација предуслова**</span><span class="sxs-lookup"><span data-stu-id="32bc6-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="32bc6-192">**Улоге пројектних ресурса за сва предузећа (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="32bc6-193">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-193">No</span></span> | <span data-ttu-id="32bc6-194">Да</span><span class="sxs-lookup"><span data-stu-id="32bc6-194">Yes</span></span> | <span data-ttu-id="32bc6-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="32bc6-195">Common Data Service</span></span> | <span data-ttu-id="32bc6-196">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-196">No</span></span> | <span data-ttu-id="32bc6-197">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-197">N\A</span></span> |
| <span data-ttu-id="32bc6-198">**Правна лица (cdm\_предузећа)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="32bc6-199">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-199">No</span></span> | <span data-ttu-id="32bc6-200">Да</span><span class="sxs-lookup"><span data-stu-id="32bc6-200">Yes</span></span> | <span data-ttu-id="32bc6-201">Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="32bc6-201">Finance and Operations apps</span></span> | <span data-ttu-id="32bc6-202">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-202">No</span></span> | <span data-ttu-id="32bc6-203">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-203">N\A</span></span> |
| <span data-ttu-id="32bc6-204">**Project Operations стварне вредности интеграције (msdyn\_стварне вредности)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="32bc6-205">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-205">No</span></span> | <span data-ttu-id="32bc6-206">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-206">No</span></span> | <span data-ttu-id="32bc6-207">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-207">N\A</span></span> | <span data-ttu-id="32bc6-208">Да</span><span class="sxs-lookup"><span data-stu-id="32bc6-208">Yes</span></span> | <span data-ttu-id="32bc6-209">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-209">No</span></span> |
| <span data-ttu-id="32bc6-210">**Предмети уговора пројекта (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="32bc6-211">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-211">No</span></span> | <span data-ttu-id="32bc6-212">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-212">No</span></span> | <span data-ttu-id="32bc6-213">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-213">N\A</span></span> | <span data-ttu-id="32bc6-214">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-214">No</span></span> | <span data-ttu-id="32bc6-215">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-215">No</span></span> |
| <span data-ttu-id="32bc6-216">**Ентитет интеграције за односе трансакција пројекта (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="32bc6-217">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-217">No</span></span> | <span data-ttu-id="32bc6-218">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-218">No</span></span> | <span data-ttu-id="32bc6-219">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-219">N\A</span></span> | <span data-ttu-id="32bc6-220">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-220">No</span></span> | <span data-ttu-id="32bc6-221">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-221">N\A</span></span> |
| <span data-ttu-id="32bc6-222">**Project Operations контролне тачке предмета уговора о интеграцији (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="32bc6-223">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-223">No</span></span> | <span data-ttu-id="32bc6-224">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-224">No</span></span> | <span data-ttu-id="32bc6-225">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-225">N\A</span></span> | <span data-ttu-id="32bc6-226">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-226">No</span></span> | <span data-ttu-id="32bc6-227">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-227">N\A</span></span> |
| <span data-ttu-id="32bc6-228">**Project Operations ентитет интеграције за процене трошкова (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="32bc6-229">Ne</span><span class="sxs-lookup"><span data-stu-id="32bc6-229">No</span></span> | <span data-ttu-id="32bc6-230">Ne</span><span class="sxs-lookup"><span data-stu-id="32bc6-230">No</span></span> | <span data-ttu-id="32bc6-231">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-231">N\A</span></span> | <span data-ttu-id="32bc6-232">Ne</span><span class="sxs-lookup"><span data-stu-id="32bc6-232">No</span></span> | <span data-ttu-id="32bc6-233">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-233">N\A</span></span> |
| <span data-ttu-id="32bc6-234">**Project Operations ентитет извоза категорија трошкова пројекта (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-234">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="32bc6-235">Ne</span><span class="sxs-lookup"><span data-stu-id="32bc6-235">No</span></span> | <span data-ttu-id="32bc6-236">Ne</span><span class="sxs-lookup"><span data-stu-id="32bc6-236">No</span></span> | <span data-ttu-id="32bc6-237">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-237">N\A</span></span> | <span data-ttu-id="32bc6-238">Ne</span><span class="sxs-lookup"><span data-stu-id="32bc6-238">No</span></span> | <span data-ttu-id="32bc6-239">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-239">N\A</span></span> |
| <span data-ttu-id="32bc6-240">**Project Operations ентитет извоза трошкова интеграције пројекта (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="32bc6-241">Да</span><span class="sxs-lookup"><span data-stu-id="32bc6-241">Yes</span></span> | <span data-ttu-id="32bc6-242">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-242">No</span></span> | <span data-ttu-id="32bc6-243">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-243">N\A</span></span> | <span data-ttu-id="32bc6-244">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-244">No</span></span> | <span data-ttu-id="32bc6-245">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-245">N\A</span></span> |
| <span data-ttu-id="32bc6-246">**Project Operations ентитет интеграције за процене сати (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="32bc6-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="32bc6-247">Да</span><span class="sxs-lookup"><span data-stu-id="32bc6-247">Yes</span></span> | <span data-ttu-id="32bc6-248">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-248">No</span></span> | <span data-ttu-id="32bc6-249">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-249">N\A</span></span> | <span data-ttu-id="32bc6-250">Не</span><span class="sxs-lookup"><span data-stu-id="32bc6-250">No</span></span> | <span data-ttu-id="32bc6-251">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="32bc6-251">N\A</span></span> |


4. <span data-ttu-id="32bc6-252">Да бисте освежили ентитет, изаберите назив мапе, а затим изаберите **Освежи ентитете**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Освежавање мапе](./media/20RefreshMapping.png)

5. <span data-ttu-id="32bc6-254">Када се освежавање заврши, покренита мапу .</span><span class="sxs-lookup"><span data-stu-id="32bc6-254">After the refresh is complete, run the map.</span></span> <span data-ttu-id="32bc6-255">Пре него што омогућите следећу мапу, проверите да ли је мапа у табели у стању **Покренута**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="32bc6-256">Покретање мапа са већим бројем предуслова може потрајати.</span><span class="sxs-lookup"><span data-stu-id="32bc6-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="32bc6-257">Да бисте покренули мапу са предусловима, омогућите преклопно дугме **Прикажи повезане мапе ентитета**.</span><span class="sxs-lookup"><span data-stu-id="32bc6-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="32bc6-258">Ако табела показује да **Почетна синхронизација предуслова** има вредност **Не** , проверите да ли је заставица **Почетна синхронизација** **искључена** у свим мапама предуслова пре него што је покренете.</span><span class="sxs-lookup"><span data-stu-id="32bc6-258">If the table indicates **Prerequisite initial sync** is **No** , verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Покретање мапе](./media/21RunMap.png)

6. <span data-ttu-id="32bc6-260">Потврдите да су све мапе повезане са пројектом у активном стању.</span><span class="sxs-lookup"><span data-stu-id="32bc6-260">Validate all project related maps are in the running state.</span></span>

![Све мапе су покренуте](./media/22AllMapsRunning.png)

<span data-ttu-id="32bc6-262">Ваше Project Operations окружење је сада обезбеђено и конфигурисано.</span><span class="sxs-lookup"><span data-stu-id="32bc6-262">Your Project Operations environment is now provisioned and configured.</span></span>
