---
title: Обезбеђење новог окружења
description: Ова тема пружа информације о начину обезбеђења новог Project Operations окружења.
author: sigitac
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 45700371c50e3b5a840df45fc24fa8a5b4584b61
ms.sourcegitcommit: 87b7a8d793c19c50f3765b8d788cde24a6a0ca24
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949380"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="0d2c2-103">Обезбеђење новог окружења</span><span class="sxs-lookup"><span data-stu-id="0d2c2-103">Provision a new environment</span></span>

<span data-ttu-id="0d2c2-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="0d2c2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="0d2c2-105">Ова тема пружа информације о начину обезбеђења новог Dynamics 365 Project Operations окружења за сценарије засноване на ресурсима / без залиха.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="0d2c2-106">Омогућавање Project Operations аутоматског обезбеђивања у LCS пројекту</span><span class="sxs-lookup"><span data-stu-id="0d2c2-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="0d2c2-107">Користите следеће кораке да омогућите Project Operations аутоматизовани ток обезбеђивања за ваш LCS пројекат.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="0d2c2-108">Идите на [LCS](https://lcs.dynamics.com/v2) и изаберите плочицу **Преглед управљања функцијама**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="0d2c2-109">У листи **Функција прегледа** изаберите **Пројектне операције** и изаберите **Омогућена функција прегледа** како би се омогућила услуга Project Operations.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-109">In the **Preview feature** list, select **Project Operations** and the select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="0d2c2-110">Овај корак се изводи само једном по LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="0d2c2-111">Обезбеђивање Project Operations окружења</span><span class="sxs-lookup"><span data-stu-id="0d2c2-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="0d2c2-112">Отвори нову примену Dynamics 365 Finance [демо окружења](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) или [sandbox/производног окружења](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="0d2c2-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="0d2c2-113">Прођите кроз чаробњак **Обезбеђивање окружења**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="0d2c2-114">Уверите се да је изабрана верзија апликације 10.0.13 или новија.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="0d2c2-115">Да бисте обезбедили Project Operations, у делу **Напредна подешавања** изаберите **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="0d2c2-116">Омогућите **Common Data Service подешавање** бирајући **Да**, а затим унесите податке у обавезна поља:</span><span class="sxs-lookup"><span data-stu-id="0d2c2-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="0d2c2-117">Име</span><span class="sxs-lookup"><span data-stu-id="0d2c2-117">Name</span></span>
  - <span data-ttu-id="0d2c2-118">Регион</span><span class="sxs-lookup"><span data-stu-id="0d2c2-118">Region</span></span>
  - <span data-ttu-id="0d2c2-119">Језик</span><span class="sxs-lookup"><span data-stu-id="0d2c2-119">Language</span></span>
  - <span data-ttu-id="0d2c2-120">Валута</span><span class="sxs-lookup"><span data-stu-id="0d2c2-120">Currency</span></span>
 
5. <span data-ttu-id="0d2c2-121">У пољу **Common Data Service предложак**, изаберите **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="0d2c2-122">Изаберите врсту окружења за вашу примену.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="0d2c2-123">Пробно време засновано на претплати омогућиће вам да примените CDS окружење на 30 дана.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Подешавања примене](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="0d2c2-125">Изаберите **Слажем се** да бисте прихватили услове услуге, а затим изаберите **Готово** да се вратите на подешавања примене.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Сагласност за примену](./media/2DeploymentConsent.png)

7. <span data-ttu-id="0d2c2-127">Попуните преостала обавезна поља у чаробњаку и потврдите примену.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="0d2c2-128">Време обезбеђивања окружења варира у зависности од врсте окружења.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="0d2c2-129">Обезбеђење може потрајати до шест сати.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="0d2c2-130">Када се примена успешно заврши, окружење ће се приказати као **Примењено**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="0d2c2-131">Да бисте потврдили да је окружење успешно постављено, изаберите **Пријављивање** и пријавите се у окружење да бисте потврдили.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Детаљи  окружења](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="0d2c2-133">Примена Project Operations Finance демо података (опционални корак)</span><span class="sxs-lookup"><span data-stu-id="0d2c2-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="0d2c2-134">Примените Project Operations Finance демо податке на 10.0.13 издање услуге у окружењу које се хостује у облаку, као што је описано у [овом чланку](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="0d2c2-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="0d2c2-135">Примените исправке на Finance окружење</span><span class="sxs-lookup"><span data-stu-id="0d2c2-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="0d2c2-136">Project Operations захтева Finance окружење са верзијом апликације **10.0.13 (10.0.569.20009)** или новијом.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="0d2c2-137">Можда ћете морати да примените исправке квалитета у свом Finance окружењу да бисте добили ову верзију.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="0d2c2-138">У LCS-у, на страници **Детаљи окружења**, у одељку **Доступне исправке** изаберите **Прикажи исправку**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Приказ исправки](./media/5ViewUpdates.png)

2. <span data-ttu-id="0d2c2-140">На страници **Бинарна ажурирања** изаберите **Сачувај пакет.**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-140">On the **Binary updates** page, select **Save package.**</span></span>

![Сачувај пакет](./media/6SavePackage.png)

3. <span data-ttu-id="0d2c2-142">Кликните на **Изабери све**, а затим изаберите **Сачувај пакет**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-142">Click **Select all** and then select **Save package**.</span></span>

![Прегледајте и сачувајте исправке](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="0d2c2-144">Унесите назив и опис пакета, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="0d2c2-145">У зависности од интернет везе, овај поступак може потрајати.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-145">Depending on the internet connection, this process might take some time.</span></span>

![Отпремите пакет у библиотеку средстава](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="0d2c2-147">Када се пакет сачува, изаберите **Готово** и сачувајте овај пакет у библиотеци средстава у вашем LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="0d2c2-148">Чување и потврђивање пакета може потрајати око 15 минута.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="0d2c2-149">Да бисте применили исправку, идите на страницу **Детаљи окружења** у LCS-у и изаберите **Одржавање** > **Примени исправке**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Одржавање окружења](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="0d2c2-151">На листи исправки изаберите пакет који сте креирали и изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Примена исправки](./media/10ApplyUpdates.png)

<span data-ttu-id="0d2c2-153">Сервисирање окружења ће потрајати неко време.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-153">Environment servicing will take some time.</span></span> <span data-ttu-id="0d2c2-154">По завршетку, окружење ће се вратити у примењено стање.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-154">After it is complete, the environment will return to a deployed state.</span></span>

![Примењено окружење](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="0d2c2-156">Успоставите везу са двоструким уписивањем</span><span class="sxs-lookup"><span data-stu-id="0d2c2-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="0d2c2-157">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="0d2c2-158">У одељку **Common Data Service информације о окружењу**, изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="0d2c2-159">Када се повезивање заврши, поново изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="0d2c2-160">Бићете преусмерени на двоструко уписивање у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-160">You will be redirected to Dual Write in Finance.</span></span>

![Повезивање са услугом CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="0d2c2-162">Изаберите **Примени решење** за приступ ентитетима који ће бити мапирани у интеграцији.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Примена решења](./media/13ApplySolutions.png)

5. <span data-ttu-id="0d2c2-164">Изаберите оба решења, **Dynamics 365 Finance and Operations мапа ентитета за двоструко уписивање** и **Dynamics 365 Project Operations мапе ентитета двоструког уписивања**, а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Потврда решења](./media/14ConfirmSolutions.png)

<span data-ttu-id="0d2c2-166">Када примените решења, ентитети двоструког уписивања се примењују на окружење.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Примена решења](./media/15ApplyingSolutions.png)

<span data-ttu-id="0d2c2-168">Када се ентитети примене, сва расположива мапирања се наводе у окружењу.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Мапе за двоструко уписивање](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="0d2c2-170">Освежите ентитете података након исправке</span><span class="sxs-lookup"><span data-stu-id="0d2c2-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="0d2c2-171">У услузи Finance идите на радни простор **Управљање подацима**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-171">In Finance, go to the **Data management** workspace.</span></span>

![Радни простор за управљање подацима](./media/16DataManagement.png)

2. <span data-ttu-id="0d2c2-173">Изаберите плочицу **Параметри радног оквира**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-173">Select the **Framework parameters** tile.</span></span>

![Параметри радног оквира](./media/17FrameworkParameters.png)

3. <span data-ttu-id="0d2c2-175">На страници **Подешавања ентитета**, изаберите **Освежи листу ентитета**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Освежи листу ентитета](./media/18RefreshEntityList.png)

<span data-ttu-id="0d2c2-177">Освежавање ће трајати приближно 20 минута.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="0d2c2-178">Добићете упозорење када се заврши.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-178">You will receive an alert when it is complete.</span></span>

![Потврда освежавања](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="0d2c2-180">Покрените Project Operations мапе двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="0d2c2-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="0d2c2-181">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="0d2c2-182">У одељку **Common Data Service информације о окружењу**, изаберите **Повежи са услугом CDS за апликације.**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-182">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="0d2c2-183">Када изаберете везу, бићете преусмерени на листу ентитета у мапирањима.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="0d2c2-184">Покрените мапе као што је описано у следећој табели.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="0d2c2-185">Уверите се да следите наведени редослед.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="0d2c2-186">**Мапа ентитета**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-186">**Entity Map**</span></span> | <span data-ttu-id="0d2c2-187">**Освежавање ентитета**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-187">**Refresh entity**</span></span> | <span data-ttu-id="0d2c2-188">**Почетна синхронизација**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-188">**Initial sync**</span></span> | <span data-ttu-id="0d2c2-189">**Мастер за почетну синхронизацију**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-189">**Master for initial sync**</span></span> | <span data-ttu-id="0d2c2-190">**Предуслови за покретање**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-190">**Run prerequisites**</span></span> | <span data-ttu-id="0d2c2-191">**Почетна синхронизација предуслова**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="0d2c2-192">**Улоге пројектних ресурса за сва предузећа (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="0d2c2-193">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-193">No</span></span> | <span data-ttu-id="0d2c2-194">Да</span><span class="sxs-lookup"><span data-stu-id="0d2c2-194">Yes</span></span> | <span data-ttu-id="0d2c2-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="0d2c2-195">Common Data Service</span></span> | <span data-ttu-id="0d2c2-196">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-196">No</span></span> | <span data-ttu-id="0d2c2-197">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-197">N\A</span></span> |
| <span data-ttu-id="0d2c2-198">**Правна лица (cdm\_предузећа)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="0d2c2-199">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-199">No</span></span> | <span data-ttu-id="0d2c2-200">Да</span><span class="sxs-lookup"><span data-stu-id="0d2c2-200">Yes</span></span> | <span data-ttu-id="0d2c2-201">Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="0d2c2-201">Finance and Operations apps</span></span> | <span data-ttu-id="0d2c2-202">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-202">No</span></span> | <span data-ttu-id="0d2c2-203">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-203">N\A</span></span> |
| <span data-ttu-id="0d2c2-204">**Project Operations стварне вредности интеграције (msdyn\_стварне вредности)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="0d2c2-205">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-205">No</span></span> | <span data-ttu-id="0d2c2-206">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-206">No</span></span> | <span data-ttu-id="0d2c2-207">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-207">N\A</span></span> | <span data-ttu-id="0d2c2-208">Да</span><span class="sxs-lookup"><span data-stu-id="0d2c2-208">Yes</span></span> | <span data-ttu-id="0d2c2-209">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-209">No</span></span> |
| <span data-ttu-id="0d2c2-210">**Предмети уговора пројекта (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="0d2c2-211">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-211">No</span></span> | <span data-ttu-id="0d2c2-212">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-212">No</span></span> | <span data-ttu-id="0d2c2-213">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-213">N\A</span></span> | <span data-ttu-id="0d2c2-214">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-214">No</span></span> | <span data-ttu-id="0d2c2-215">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-215">No</span></span> |
| <span data-ttu-id="0d2c2-216">**Ентитет интеграције за односе трансакција пројекта (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="0d2c2-217">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-217">No</span></span> | <span data-ttu-id="0d2c2-218">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-218">No</span></span> | <span data-ttu-id="0d2c2-219">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-219">N\A</span></span> | <span data-ttu-id="0d2c2-220">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-220">No</span></span> | <span data-ttu-id="0d2c2-221">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-221">N\A</span></span> |
| <span data-ttu-id="0d2c2-222">**Project Operations контролне тачке предмета уговора о интеграцији (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="0d2c2-223">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-223">No</span></span> | <span data-ttu-id="0d2c2-224">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-224">No</span></span> | <span data-ttu-id="0d2c2-225">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-225">N\A</span></span> | <span data-ttu-id="0d2c2-226">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-226">No</span></span> | <span data-ttu-id="0d2c2-227">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-227">N\A</span></span> |
| <span data-ttu-id="0d2c2-228">**Project Operations ентитет интеграције за процене трошкова (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="0d2c2-229">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-229">No</span></span> | <span data-ttu-id="0d2c2-230">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-230">No</span></span> | <span data-ttu-id="0d2c2-231">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-231">N\A</span></span> | <span data-ttu-id="0d2c2-232">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-232">No</span></span> | <span data-ttu-id="0d2c2-233">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-233">N\A</span></span> |
| <span data-ttu-id="0d2c2-234">**Project Operations ентитет интеграције за процене сати (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-234">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="0d2c2-235">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-235">No</span></span> | <span data-ttu-id="0d2c2-236">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-236">No</span></span> | <span data-ttu-id="0d2c2-237">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-237">N\A</span></span> | <span data-ttu-id="0d2c2-238">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-238">No</span></span> | <span data-ttu-id="0d2c2-239">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-239">N\A</span></span> |
| <span data-ttu-id="0d2c2-240">**Project Operations ентитет извоза трошкова интеграције пројекта (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="0d2c2-241">Да</span><span class="sxs-lookup"><span data-stu-id="0d2c2-241">Yes</span></span> | <span data-ttu-id="0d2c2-242">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-242">No</span></span> | <span data-ttu-id="0d2c2-243">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-243">N\A</span></span> | <span data-ttu-id="0d2c2-244">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-244">No</span></span> | <span data-ttu-id="0d2c2-245">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-245">N\A</span></span> |
| <span data-ttu-id="0d2c2-246">**Project Operations ентитет интеграције за процене сати (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="0d2c2-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="0d2c2-247">Да</span><span class="sxs-lookup"><span data-stu-id="0d2c2-247">Yes</span></span> | <span data-ttu-id="0d2c2-248">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-248">No</span></span> | <span data-ttu-id="0d2c2-249">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-249">N\A</span></span> | <span data-ttu-id="0d2c2-250">Не</span><span class="sxs-lookup"><span data-stu-id="0d2c2-250">No</span></span> | <span data-ttu-id="0d2c2-251">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="0d2c2-251">N\A</span></span> |

4. <span data-ttu-id="0d2c2-252">Да бисте освежили ентитет, изаберите назив мапе, а затим изаберите **Освежи ентитете**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 
5. <span data-ttu-id="0d2c2-253">Наставите са извођењем мапе након завршетка освежавања.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-253">Proceed with running the map after the refresh is complete.</span></span>

![Освежавање мапе](./media/20RefreshMapping.png)

<span data-ttu-id="0d2c2-255">Пре него што омогућите следећу мапу, проверите да ли је мапа у табели у стању **Покренута**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="0d2c2-256">Покретање мапа са већим бројем предуслова може потрајати.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="0d2c2-257">Да бисте покренули мапу са предусловима, омогућите преклопно дугме **Прикажи повезане мапе ентитета**.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="0d2c2-258">Ако табела показује да **Почетна синхронизација предуслова** има вредност **Не**, проверите да ли је заставица **Почетна синхронизација** **искључена** у свим мапама предуслова пре него што је покренете.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-258">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Покретање мапе](./media/21RunMap.png)

6. <span data-ttu-id="0d2c2-260">Потврдите да су све мапе повезане са пројектом у активном стању.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-260">Validate all project related maps are in the running state.</span></span>

![Све мапе су покренуте](./media/22AllMapsRunning.png)

<span data-ttu-id="0d2c2-262">Ваше Project Operations окружење је сада обезбеђено и конфигурисано.</span><span class="sxs-lookup"><span data-stu-id="0d2c2-262">Your Project Operations environment is now provisioned and configured.</span></span>
