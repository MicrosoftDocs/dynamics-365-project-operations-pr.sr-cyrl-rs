---
title: Обезбеђење новог окружења
description: Ова тема пружа информације о начину обезбеђења новог Project Operations окружења.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 9ed502a1312b702e029d8910d62f72b8e0e4df06
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643007"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="f3446-103">Обезбеђење новог окружења</span><span class="sxs-lookup"><span data-stu-id="f3446-103">Provision a new environment</span></span>

<span data-ttu-id="f3446-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="f3446-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="f3446-105">Ова тема пружа информације о начину да обезбедите ново Dynamics 365 Project Operations окружење за сценарије засноване на ресурсима/без залиха.</span><span class="sxs-lookup"><span data-stu-id="f3446-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="f3446-106">Омогућавање Project Operations аутоматског обезбеђивања у LCS пројекту</span><span class="sxs-lookup"><span data-stu-id="f3446-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="f3446-107">Користите следеће кораке да омогућите Project Operations аутоматизовани ток обезбеђивања за ваш LCS пројекат.</span><span class="sxs-lookup"><span data-stu-id="f3446-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="f3446-108">Идите на [LCS](https://lcs.dynamics.com/v2) и изаберите плочицу **Преглед управљања функцијама**.</span><span class="sxs-lookup"><span data-stu-id="f3446-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="f3446-109">На листи **Функција прегледа** изаберите **Project Operations Feature** и изаберите **Омогућена функција прегледа** како би се омогућила услуга Project Operations.</span><span class="sxs-lookup"><span data-stu-id="f3446-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="f3446-110">Овај корак се изводи само једном по LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="f3446-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="f3446-111">Обезбеђивање Project Operations окружења</span><span class="sxs-lookup"><span data-stu-id="f3446-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="f3446-112">Отвори нову примену Dynamics 365 Finance [демо окружења](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) или [sandbox/производног окружења](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="f3446-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="f3446-113">Прођите кроз чаробњак **Обезбеђивање окружења**.</span><span class="sxs-lookup"><span data-stu-id="f3446-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="f3446-114">Уверите се да је изабрана верзија апликације 10.0.13 или новија.</span><span class="sxs-lookup"><span data-stu-id="f3446-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="f3446-115">Да бисте обезбедили Project Operations, у делу **Напредна подешавања** изаберите **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="f3446-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="f3446-116">Омогућите **Common Data Service подешавање** бирајући **Да**, а затим унесите податке у обавезна поља:</span><span class="sxs-lookup"><span data-stu-id="f3446-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="f3446-117">Име</span><span class="sxs-lookup"><span data-stu-id="f3446-117">Name</span></span>
  - <span data-ttu-id="f3446-118">Регион</span><span class="sxs-lookup"><span data-stu-id="f3446-118">Region</span></span>
  - <span data-ttu-id="f3446-119">Језик</span><span class="sxs-lookup"><span data-stu-id="f3446-119">Language</span></span>
  - <span data-ttu-id="f3446-120">Валута</span><span class="sxs-lookup"><span data-stu-id="f3446-120">Currency</span></span>
 
5. <span data-ttu-id="f3446-121">У пољу **Common Data Service предложак**, изаберите **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="f3446-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="f3446-122">Изаберите врсту окружења за вашу примену.</span><span class="sxs-lookup"><span data-stu-id="f3446-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="f3446-123">Пробно време засновано на претплати омогућиће вам да примените CDS окружење на 30 дана.</span><span class="sxs-lookup"><span data-stu-id="f3446-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Подешавања примене](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="f3446-125">Изаберите **Слажем се** да бисте прихватили услове услуге, а затим изаберите **Готово** да се вратите на подешавања примене.</span><span class="sxs-lookup"><span data-stu-id="f3446-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Сагласност за примену](./media/2DeploymentConsent.png)

7. <span data-ttu-id="f3446-127">Попуните преостала обавезна поља у чаробњаку и потврдите примену.</span><span class="sxs-lookup"><span data-stu-id="f3446-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="f3446-128">Време обезбеђивања окружења варира у зависности од врсте окружења.</span><span class="sxs-lookup"><span data-stu-id="f3446-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="f3446-129">Обезбеђење може потрајати до шест сати.</span><span class="sxs-lookup"><span data-stu-id="f3446-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="f3446-130">Када се примена успешно заврши, окружење ће се приказати као **Примењено**.</span><span class="sxs-lookup"><span data-stu-id="f3446-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="f3446-131">Да бисте потврдили да је окружење успешно постављено, изаберите **Пријављивање** и пријавите се у окружење да бисте потврдили.</span><span class="sxs-lookup"><span data-stu-id="f3446-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Детаљи  окружења](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="f3446-133">Примена Project Operations Finance демо података (опционални корак)</span><span class="sxs-lookup"><span data-stu-id="f3446-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="f3446-134">Примените Project Operations Finance демо податке на 10.0.13 издање услуге у окружењу које се хостује у облаку, као што је описано у [овом чланку](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="f3446-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="f3446-135">Примените исправке на Finance окружење</span><span class="sxs-lookup"><span data-stu-id="f3446-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="f3446-136">Project Operations захтева Finance окружење са верзијом апликације **10.0.13 (10.0.569.20009)** или новијом.</span><span class="sxs-lookup"><span data-stu-id="f3446-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="f3446-137">Можда ћете морати да примените исправке квалитета у свом Finance окружењу да бисте добили ову верзију.</span><span class="sxs-lookup"><span data-stu-id="f3446-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="f3446-138">У LCS-у, на страници **Детаљи окружења**, у одељку **Доступне исправке** изаберите **Прикажи исправку**.</span><span class="sxs-lookup"><span data-stu-id="f3446-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Приказ исправки](./media/5ViewUpdates.png)

2. <span data-ttu-id="f3446-140">На страници **Бинарна ажурирања** изаберите **Сачувај пакет.**</span><span class="sxs-lookup"><span data-stu-id="f3446-140">On the **Binary updates** page, select **Save package.**</span></span>

![Сачувај пакет](./media/6SavePackage.png)

3. <span data-ttu-id="f3446-142">Кликните на **Изабери све**, а затим изаберите **Сачувај пакет**.</span><span class="sxs-lookup"><span data-stu-id="f3446-142">Click **Select all** and then select **Save package**.</span></span>

![Прегледајте и сачувајте исправке](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="f3446-144">Унесите назив и опис пакета, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="f3446-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="f3446-145">У зависности од интернет везе, овај поступак може потрајати.</span><span class="sxs-lookup"><span data-stu-id="f3446-145">Depending on the internet connection, this process might take some time.</span></span>

![Отпремите пакет у библиотеку средстава](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="f3446-147">Када се пакет сачува, изаберите **Готово** и сачувајте овај пакет у библиотеци средстава у вашем LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="f3446-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="f3446-148">Чување и потврђивање пакета може потрајати око 15 минута.</span><span class="sxs-lookup"><span data-stu-id="f3446-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="f3446-149">Да бисте применили исправку, идите на страницу **Детаљи окружења** у LCS-у и изаберите **Одржавање** > **Примени исправке**.</span><span class="sxs-lookup"><span data-stu-id="f3446-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Одржавање окружења](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="f3446-151">На листи исправки изаберите пакет који сте креирали и изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="f3446-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Примена исправки](./media/10ApplyUpdates.png)

<span data-ttu-id="f3446-153">Сервисирање окружења ће потрајати неко време.</span><span class="sxs-lookup"><span data-stu-id="f3446-153">Environment servicing will take some time.</span></span> <span data-ttu-id="f3446-154">По завршетку, окружење ће се вратити у примењено стање.</span><span class="sxs-lookup"><span data-stu-id="f3446-154">After it is complete, the environment will return to a deployed state.</span></span>

![Примењено окружење](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="f3446-156">Успоставите везу са двоструким уписивањем</span><span class="sxs-lookup"><span data-stu-id="f3446-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="f3446-157">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="f3446-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="f3446-158">У одељку **Common Data Service информације о окружењу**, изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="f3446-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="f3446-159">Када се повезивање заврши, поново изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="f3446-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="f3446-160">Бићете преусмерени на двоструко уписивање у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="f3446-160">You will be redirected to Dual Write in Finance.</span></span>

![Повезивање са услугом CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="f3446-162">Изаберите **Примени решење** за приступ ентитетима који ће бити мапирани у интеграцији.</span><span class="sxs-lookup"><span data-stu-id="f3446-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Примена решења](./media/13ApplySolutions.png)

5. <span data-ttu-id="f3446-164">Изаберите оба решења, **Dynamics 365 Finance and Operations мапа ентитета за двоструко писање** и **Dynamics 365 Project Operations мапе ентитета за двоструко писање**, а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="f3446-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Потврда решења](./media/14ConfirmSolutions.png)

<span data-ttu-id="f3446-166">Када примените решења, ентитети двоструког уписивања се примењују на окружење.</span><span class="sxs-lookup"><span data-stu-id="f3446-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Примена решења](./media/15ApplyingSolutions.png)

<span data-ttu-id="f3446-168">Када се ентитети примене, сва расположива мапирања се наводе у окружењу.</span><span class="sxs-lookup"><span data-stu-id="f3446-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Мапе за двоструко уписивање](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="f3446-170">Освежите ентитете података након исправке</span><span class="sxs-lookup"><span data-stu-id="f3446-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="f3446-171">У услузи Finance идите на радни простор **Управљање подацима**.</span><span class="sxs-lookup"><span data-stu-id="f3446-171">In Finance, go to the **Data management** workspace.</span></span>

![Радни простор за управљање подацима](./media/16DataManagement.png)

2. <span data-ttu-id="f3446-173">Изаберите плочицу **Параметри радног оквира**.</span><span class="sxs-lookup"><span data-stu-id="f3446-173">Select the **Framework parameters** tile.</span></span>

![Параметри радног оквира](./media/17FrameworkParameters.png)

3. <span data-ttu-id="f3446-175">На страници **Подешавања ентитета**, изаберите **Освежи листу ентитета**.</span><span class="sxs-lookup"><span data-stu-id="f3446-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Освежи листу ентитета](./media/18RefreshEntityList.png)

<span data-ttu-id="f3446-177">Освежавање ће трајати приближно 20 минута.</span><span class="sxs-lookup"><span data-stu-id="f3446-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="f3446-178">Добићете упозорење када се заврши.</span><span class="sxs-lookup"><span data-stu-id="f3446-178">You will receive an alert when it is complete.</span></span>

![Потврда освежавања](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="f3446-180">Покрените Project Operations мапе двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="f3446-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="f3446-181">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="f3446-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="f3446-182">У одељку **Common Data Service информације о окружењу**, изаберите **Повежи са услугом CDS за апликације.**</span><span class="sxs-lookup"><span data-stu-id="f3446-182">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="f3446-183">Када изаберете везу, бићете преусмерени на листу ентитета у мапирањима.</span><span class="sxs-lookup"><span data-stu-id="f3446-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="f3446-184">Покрените мапе као што је описано у следећој табели.</span><span class="sxs-lookup"><span data-stu-id="f3446-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="f3446-185">Уверите се да следите наведени редослед.</span><span class="sxs-lookup"><span data-stu-id="f3446-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="f3446-186">**Мапа ентитета**</span><span class="sxs-lookup"><span data-stu-id="f3446-186">**Entity Map**</span></span> | <span data-ttu-id="f3446-187">**Освежавање ентитета**</span><span class="sxs-lookup"><span data-stu-id="f3446-187">**Refresh entity**</span></span> | <span data-ttu-id="f3446-188">**Почетна синхронизација**</span><span class="sxs-lookup"><span data-stu-id="f3446-188">**Initial sync**</span></span> | <span data-ttu-id="f3446-189">**Мастер за почетну синхронизацију**</span><span class="sxs-lookup"><span data-stu-id="f3446-189">**Master for initial sync**</span></span> | <span data-ttu-id="f3446-190">**Предуслови за покретање**</span><span class="sxs-lookup"><span data-stu-id="f3446-190">**Run prerequisites**</span></span> | <span data-ttu-id="f3446-191">**Почетна синхронизација предуслова**</span><span class="sxs-lookup"><span data-stu-id="f3446-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="f3446-192">**Улоге пројектних ресурса за сва предузећа (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="f3446-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="f3446-193">No</span><span class="sxs-lookup"><span data-stu-id="f3446-193">No</span></span> | <span data-ttu-id="f3446-194">Да</span><span class="sxs-lookup"><span data-stu-id="f3446-194">Yes</span></span> | <span data-ttu-id="f3446-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="f3446-195">Common Data Service</span></span> | <span data-ttu-id="f3446-196">No</span><span class="sxs-lookup"><span data-stu-id="f3446-196">No</span></span> | <span data-ttu-id="f3446-197">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-197">N\A</span></span> |
| <span data-ttu-id="f3446-198">**Правна лица (cdm\_предузећа)**</span><span class="sxs-lookup"><span data-stu-id="f3446-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="f3446-199">No</span><span class="sxs-lookup"><span data-stu-id="f3446-199">No</span></span> | <span data-ttu-id="f3446-200">Да</span><span class="sxs-lookup"><span data-stu-id="f3446-200">Yes</span></span> | <span data-ttu-id="f3446-201">Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="f3446-201">Finance and Operations apps</span></span> | <span data-ttu-id="f3446-202">No</span><span class="sxs-lookup"><span data-stu-id="f3446-202">No</span></span> | <span data-ttu-id="f3446-203">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-203">N\A</span></span> |
| <span data-ttu-id="f3446-204">**Књига (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="f3446-204">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="f3446-205">No</span><span class="sxs-lookup"><span data-stu-id="f3446-205">No</span></span> | <span data-ttu-id="f3446-206">Да</span><span class="sxs-lookup"><span data-stu-id="f3446-206">Yes</span></span> | <span data-ttu-id="f3446-207">Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="f3446-207">Finance and Operations apps</span></span> | <span data-ttu-id="f3446-208">Да</span><span class="sxs-lookup"><span data-stu-id="f3446-208">Yes</span></span> | <span data-ttu-id="f3446-209">Да, Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="f3446-209">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="f3446-210">**Project Operations стварне вредности интеграције (msdyn\_стварне вредности)**</span><span class="sxs-lookup"><span data-stu-id="f3446-210">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="f3446-211">No</span><span class="sxs-lookup"><span data-stu-id="f3446-211">No</span></span> | <span data-ttu-id="f3446-212">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-212">No</span></span> | <span data-ttu-id="f3446-213">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-213">N\A</span></span> | <span data-ttu-id="f3446-214">Да</span><span class="sxs-lookup"><span data-stu-id="f3446-214">Yes</span></span> | <span data-ttu-id="f3446-215">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-215">No</span></span> |
| <span data-ttu-id="f3446-216">**Предмети уговора пројекта (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="f3446-216">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="f3446-217">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-217">No</span></span> | <span data-ttu-id="f3446-218">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-218">No</span></span> | <span data-ttu-id="f3446-219">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-219">N\A</span></span> | <span data-ttu-id="f3446-220">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-220">No</span></span> | <span data-ttu-id="f3446-221">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-221">No</span></span> |
| <span data-ttu-id="f3446-222">**Ентитет интеграције за односе трансакција пројекта (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="f3446-222">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="f3446-223">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-223">No</span></span> | <span data-ttu-id="f3446-224">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-224">No</span></span> | <span data-ttu-id="f3446-225">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-225">N\A</span></span> | <span data-ttu-id="f3446-226">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-226">No</span></span> | <span data-ttu-id="f3446-227">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-227">N\A</span></span> |
| <span data-ttu-id="f3446-228">**Project Operations контролне тачке предмета уговора о интеграцији (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="f3446-228">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="f3446-229">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-229">No</span></span> | <span data-ttu-id="f3446-230">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-230">No</span></span> | <span data-ttu-id="f3446-231">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-231">N\A</span></span> | <span data-ttu-id="f3446-232">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-232">No</span></span> | <span data-ttu-id="f3446-233">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-233">N\A</span></span> |
| <span data-ttu-id="f3446-234">**Project Operations ентитет интеграције за процене трошкова (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="f3446-234">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="f3446-235">Ne</span><span class="sxs-lookup"><span data-stu-id="f3446-235">No</span></span> | <span data-ttu-id="f3446-236">Ne</span><span class="sxs-lookup"><span data-stu-id="f3446-236">No</span></span> | <span data-ttu-id="f3446-237">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-237">N\A</span></span> | <span data-ttu-id="f3446-238">Ne</span><span class="sxs-lookup"><span data-stu-id="f3446-238">No</span></span> | <span data-ttu-id="f3446-239">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-239">N\A</span></span> |
| <span data-ttu-id="f3446-240">**Project Operations ентитет извоза категорија трошкова пројекта (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="f3446-240">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="f3446-241">Ne</span><span class="sxs-lookup"><span data-stu-id="f3446-241">No</span></span> | <span data-ttu-id="f3446-242">Ne</span><span class="sxs-lookup"><span data-stu-id="f3446-242">No</span></span> | <span data-ttu-id="f3446-243">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-243">N\A</span></span> | <span data-ttu-id="f3446-244">Ne</span><span class="sxs-lookup"><span data-stu-id="f3446-244">No</span></span> | <span data-ttu-id="f3446-245">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-245">N\A</span></span> |
| <span data-ttu-id="f3446-246">**Project Operations ентитет извоза трошкова интеграције пројекта (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="f3446-246">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="f3446-247">Да</span><span class="sxs-lookup"><span data-stu-id="f3446-247">Yes</span></span> | <span data-ttu-id="f3446-248">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-248">No</span></span> | <span data-ttu-id="f3446-249">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-249">N\A</span></span> | <span data-ttu-id="f3446-250">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-250">No</span></span> | <span data-ttu-id="f3446-251">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-251">N\A</span></span> |
| <span data-ttu-id="f3446-252">**Project Operations ентитет интеграције за процене сати (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="f3446-252">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="f3446-253">Да</span><span class="sxs-lookup"><span data-stu-id="f3446-253">Yes</span></span> | <span data-ttu-id="f3446-254">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-254">No</span></span> | <span data-ttu-id="f3446-255">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-255">N\A</span></span> | <span data-ttu-id="f3446-256">Не</span><span class="sxs-lookup"><span data-stu-id="f3446-256">No</span></span> | <span data-ttu-id="f3446-257">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="f3446-257">N\A</span></span> |


4. <span data-ttu-id="f3446-258">Да бисте освежили ентитет, изаберите назив мапе, а затим изаберите **Освежи ентитете**.</span><span class="sxs-lookup"><span data-stu-id="f3446-258">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Освежавање мапе](./media/20RefreshMapping.png)

5. <span data-ttu-id="f3446-260">Када се освежавање заврши, покренита мапу .</span><span class="sxs-lookup"><span data-stu-id="f3446-260">After the refresh is complete, run the map.</span></span> <span data-ttu-id="f3446-261">Пре него што омогућите следећу мапу, проверите да ли је мапа у табели у стању **Покренута**.</span><span class="sxs-lookup"><span data-stu-id="f3446-261">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="f3446-262">Покретање мапа са већим бројем предуслова може потрајати.</span><span class="sxs-lookup"><span data-stu-id="f3446-262">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="f3446-263">Да бисте покренули мапу са предусловима, омогућите преклопно дугме **Прикажи повезане мапе ентитета**.</span><span class="sxs-lookup"><span data-stu-id="f3446-263">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="f3446-264">Ако табела показује да **Почетна синхронизација предуслова** има вредност **Не**, проверите да ли је заставица **Почетна синхронизација** **искључена** у свим мапама предуслова пре него што је покренете.</span><span class="sxs-lookup"><span data-stu-id="f3446-264">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Покретање мапе](./media/21RunMap.png)

6. <span data-ttu-id="f3446-266">Потврдите да су све мапе повезане са пројектом у активном стању.</span><span class="sxs-lookup"><span data-stu-id="f3446-266">Validate all project related maps are in the running state.</span></span>

![Све мапе су покренуте](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="f3446-268">Примена података о конфигурацији у услузи CDS за Project Operations (опционално)</span><span class="sxs-lookup"><span data-stu-id="f3446-268">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="f3446-269">Ако сте применили демо податке на Finance окружење, погледајте чланак [Подешавање и примена података о конфигурацији у услузи Common Data Service за Project Operations](resource-apply-pro-setup-config-data.md) за примену демо података на CDS окружење.</span><span class="sxs-lookup"><span data-stu-id="f3446-269">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="f3446-270">Ваше Project Operations окружење је сада обезбеђено и конфигурисано.</span><span class="sxs-lookup"><span data-stu-id="f3446-270">Your Project Operations environment is now provisioned and configured.</span></span> 
