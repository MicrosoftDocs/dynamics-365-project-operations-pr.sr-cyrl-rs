---
title: Обезбеђење новог окружења
description: Ова тема пружа информације о начину обезбеђења новог Project Operations окружења.
author: sigitac
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d0712d9d5dfc6c35ccd07142ff5948f50e6a254c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995504"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="6e890-103">Обезбеђење новог окружења</span><span class="sxs-lookup"><span data-stu-id="6e890-103">Provision a new environment</span></span>

<span data-ttu-id="6e890-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="6e890-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="6e890-105">Ова тема пружа информације о начину да обезбедите ново Dynamics 365 Project Operations окружење за сценарије засноване на ресурсима/без залиха.</span><span class="sxs-lookup"><span data-stu-id="6e890-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="6e890-106">Омогућавање Project Operations аутоматског обезбеђивања у LCS пројекту</span><span class="sxs-lookup"><span data-stu-id="6e890-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="6e890-107">Користите следеће кораке да омогућите Project Operations аутоматизовани ток обезбеђивања за ваш LCS пројекат.</span><span class="sxs-lookup"><span data-stu-id="6e890-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="6e890-108">Идите на [LCS](https://lcs.dynamics.com/v2) и изаберите плочицу **Преглед управљања функцијама**.</span><span class="sxs-lookup"><span data-stu-id="6e890-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="6e890-109">На листи **Функција прегледа** изаберите **Project Operations Feature** и изаберите **Омогућена функција прегледа** како би се омогућила услуга Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6e890-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="6e890-110">Овај корак се изводи само једном по LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="6e890-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="6e890-111">Обезбеђивање Project Operations окружења</span><span class="sxs-lookup"><span data-stu-id="6e890-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="6e890-112">Отвори нову примену Dynamics 365 Finance [демо окружења](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) или [sandbox/производног окружења](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="6e890-112">Open a new Dynamics 365 Finance [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="6e890-113">Прођите кроз чаробњак **Обезбеђивање окружења**.</span><span class="sxs-lookup"><span data-stu-id="6e890-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="6e890-114">Уверите се да је изабрана верзија апликације 10.0.13 или новија.</span><span class="sxs-lookup"><span data-stu-id="6e890-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="6e890-115">Да бисте обезбедили Project Operations, у делу **Напредна подешавања** изаберите **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="6e890-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="6e890-116">Омогућите **Common Data Service подешавање** бирајући **Да**, а затим унесите податке у обавезна поља:</span><span class="sxs-lookup"><span data-stu-id="6e890-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="6e890-117">Име</span><span class="sxs-lookup"><span data-stu-id="6e890-117">Name</span></span>
  - <span data-ttu-id="6e890-118">Регион</span><span class="sxs-lookup"><span data-stu-id="6e890-118">Region</span></span>
  - <span data-ttu-id="6e890-119">Језик</span><span class="sxs-lookup"><span data-stu-id="6e890-119">Language</span></span>
  - <span data-ttu-id="6e890-120">Валута</span><span class="sxs-lookup"><span data-stu-id="6e890-120">Currency</span></span>
 
5. <span data-ttu-id="6e890-121">У пољу **Common Data Service предложак**, изаберите **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="6e890-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="6e890-122">Изаберите врсту окружења за вашу примену.</span><span class="sxs-lookup"><span data-stu-id="6e890-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="6e890-123">Пробно време засновано на претплати омогућиће вам да примените CDS окружење на 30 дана.</span><span class="sxs-lookup"><span data-stu-id="6e890-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Подешавања примене](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="6e890-125">Изаберите **Слажем се** да бисте прихватили услове услуге, а затим изаберите **Готово** да се вратите на подешавања примене.</span><span class="sxs-lookup"><span data-stu-id="6e890-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Сагласност за примену](./media/2DeploymentConsent.png)

7. <span data-ttu-id="6e890-127">Опционално – примените демо податке на окружење.</span><span class="sxs-lookup"><span data-stu-id="6e890-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="6e890-128">Идите на **Напредна подешавања**, изаберите **Прилагоди конфигурацију SQL базе података** и подесите **Наведите скуп података за базу података апликације** на **Демо**.</span><span class="sxs-lookup"><span data-stu-id="6e890-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="6e890-129">Попуните преостала обавезна поља у чаробњаку и потврдите примену.</span><span class="sxs-lookup"><span data-stu-id="6e890-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="6e890-130">Време за припрему окружења варира у зависности од врсте окружења.</span><span class="sxs-lookup"><span data-stu-id="6e890-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="6e890-131">Обезбеђење може потрајати до шест сати.</span><span class="sxs-lookup"><span data-stu-id="6e890-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="6e890-132">Када се примена успешно заврши, окружење ће се приказати као **Примењено**.</span><span class="sxs-lookup"><span data-stu-id="6e890-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="6e890-133">Да бисте потврдили да се окружење успешно применило, изаберите **Пријави се** и пријавите се у окружење да бисте потврдили.</span><span class="sxs-lookup"><span data-stu-id="6e890-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Детаљи окружења](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="6e890-135">Примените исправке на Finance окружење</span><span class="sxs-lookup"><span data-stu-id="6e890-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="6e890-136">Project Operations захтева Finance окружење са верзијом апликације **10.0.13 (10.0.569.20009)** или новијом.</span><span class="sxs-lookup"><span data-stu-id="6e890-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="6e890-137">Можда ћете морати да примените исправке квалитета у свом Finance окружењу да бисте добили ову верзију.</span><span class="sxs-lookup"><span data-stu-id="6e890-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="6e890-138">У LCS-у, на страници **Детаљи окружења**, у одељку **Доступне исправке** изаберите **Прикажи исправку**.</span><span class="sxs-lookup"><span data-stu-id="6e890-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Приказ исправки](./media/5ViewUpdates.png)

2. <span data-ttu-id="6e890-140">На страници **Бинарна ажурирања** изаберите **Сачувај пакет.**</span><span class="sxs-lookup"><span data-stu-id="6e890-140">On the **Binary updates** page, select **Save package.**</span></span>

![Сачувај пакет](./media/6SavePackage.png)

3. <span data-ttu-id="6e890-142">Кликните на **Изабери све**, а затим изаберите **Сачувај пакет**.</span><span class="sxs-lookup"><span data-stu-id="6e890-142">Click **Select all** and then select **Save package**.</span></span>

![Прегледајте и сачувајте исправке](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="6e890-144">Унесите назив и опис пакета, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="6e890-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="6e890-145">У зависности од интернет везе, овај поступак може потрајати.</span><span class="sxs-lookup"><span data-stu-id="6e890-145">Depending on the internet connection, this process might take some time.</span></span>

![Отпремите пакет у библиотеку средстава](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="6e890-147">Када се пакет сачува, изаберите **Готово** и сачувајте овај пакет у библиотеци средстава у вашем LCS пројекту.</span><span class="sxs-lookup"><span data-stu-id="6e890-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="6e890-148">Чување и потврђивање пакета може потрајати око 15 минута.</span><span class="sxs-lookup"><span data-stu-id="6e890-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="6e890-149">Да бисте применили исправку, идите на страницу **Детаљи окружења** у LCS-у и изаберите **Одржавање** > **Примени исправке**.</span><span class="sxs-lookup"><span data-stu-id="6e890-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Одржавање окружења](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="6e890-151">На листи исправки изаберите пакет који сте креирали и изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="6e890-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Примена исправки](./media/10ApplyUpdates.png)

<span data-ttu-id="6e890-153">Сервисирање окружења ће потрајати неко време.</span><span class="sxs-lookup"><span data-stu-id="6e890-153">Environment servicing will take some time.</span></span> <span data-ttu-id="6e890-154">По завршетку, окружење ће се вратити у примењено стање.</span><span class="sxs-lookup"><span data-stu-id="6e890-154">After it is complete, the environment will return to a deployed state.</span></span>

![Примењено окружење](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="6e890-156">Успоставите везу са двоструким уписивањем</span><span class="sxs-lookup"><span data-stu-id="6e890-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="6e890-157">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="6e890-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="6e890-158">У одељку **Common Data Service информације о окружењу**, изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="6e890-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="6e890-159">Када се повезивање заврши, поново изаберите **Повежи са услугом CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="6e890-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="6e890-160">Бићете преусмерени на двоструко уписивање у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="6e890-160">You will be redirected to Dual Write in Finance.</span></span>

![Повезивање са услугом CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="6e890-162">Изаберите **Примени решење** за приступ ентитетима који ће бити мапирани у интеграцији.</span><span class="sxs-lookup"><span data-stu-id="6e890-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Примена решења](./media/13ApplySolutions.png)

5. <span data-ttu-id="6e890-164">Изаберите оба решења, **Dynamics 365 Finance and Operations мапа ентитета за двоструко писање** и **Dynamics 365 Project Operations мапе ентитета за двоструко писање**, а затим изаберите **Примени**.</span><span class="sxs-lookup"><span data-stu-id="6e890-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Потврда решења](./media/14ConfirmSolutions.png)

<span data-ttu-id="6e890-166">Када примените решења, ентитети двоструког уписивања се примењују на окружење.</span><span class="sxs-lookup"><span data-stu-id="6e890-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Примена решења](./media/15ApplyingSolutions.png)

<span data-ttu-id="6e890-168">Када се ентитети примене, сва расположива мапирања се наводе у окружењу.</span><span class="sxs-lookup"><span data-stu-id="6e890-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Мапе за двоструко уписивање](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="6e890-170">Освежите ентитете података након исправке</span><span class="sxs-lookup"><span data-stu-id="6e890-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="6e890-171">У услузи Finance идите на радни простор **Управљање подацима**.</span><span class="sxs-lookup"><span data-stu-id="6e890-171">In Finance, go to the **Data management** workspace.</span></span>

![Радни простор за управљање подацима](./media/16DataManagement.png)

2. <span data-ttu-id="6e890-173">Изаберите плочицу **Параметри радног оквира**.</span><span class="sxs-lookup"><span data-stu-id="6e890-173">Select the **Framework parameters** tile.</span></span>

![Параметри радног оквира](./media/17FrameworkParameters.png)

3. <span data-ttu-id="6e890-175">На страници **Подешавања ентитета**, изаберите **Освежи листу ентитета**.</span><span class="sxs-lookup"><span data-stu-id="6e890-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Освежи листу ентитета](./media/18RefreshEntityList.png)

<span data-ttu-id="6e890-177">Освежавање ће трајати приближно 20 минута.</span><span class="sxs-lookup"><span data-stu-id="6e890-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="6e890-178">Добићете упозорење када се заврши.</span><span class="sxs-lookup"><span data-stu-id="6e890-178">You will receive an alert when it is complete.</span></span>

![Потврда освежавања](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="6e890-180">Ажурирање безбедоносних подешавања у услузи Project Operations за Dataverse</span><span class="sxs-lookup"><span data-stu-id="6e890-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="6e890-181">Идите на Project Operations з Dataverse окружењу.</span><span class="sxs-lookup"><span data-stu-id="6e890-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="6e890-182">Идите на **Подешавања** > **Безбедност** > **Безбедносне улоге**.</span><span class="sxs-lookup"><span data-stu-id="6e890-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="6e890-183">На страници **Безбедоносне улоге** са листе улога изаберите **корисник апликације за двоструко уписивање** и изаберите картицу **Прилагођени ентитети**.</span><span class="sxs-lookup"><span data-stu-id="6e890-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="6e890-184">Проверите да ли улога има дозволе **Читање** и **Приложи у** за:</span><span class="sxs-lookup"><span data-stu-id="6e890-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="6e890-185">**Тип девизног курса валуте**</span><span class="sxs-lookup"><span data-stu-id="6e890-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="6e890-186">**Графикон пословних контаката**</span><span class="sxs-lookup"><span data-stu-id="6e890-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="6e890-187">**Фискални календар**</span><span class="sxs-lookup"><span data-stu-id="6e890-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="6e890-188">**Главна књига**</span><span class="sxs-lookup"><span data-stu-id="6e890-188">**Ledger**</span></span>

5. <span data-ttu-id="6e890-189">Након ажурирања безбедносне улоге, идите на **Подешавања** > **Безбедност** > **Тимови** и изаберите подразумевани тим у приказу тимова **Власник локалног предузећа**.</span><span class="sxs-lookup"><span data-stu-id="6e890-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="6e890-190">Изаберите **Управљање улогама** и проверите да ли је безбедносна привилегија **корисник апликације за двоструко уписивање** примењена на овај тим.</span><span class="sxs-lookup"><span data-stu-id="6e890-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="6e890-191">Покрените Project Operations мапе двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="6e890-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="6e890-192">У свом LCS пројекту идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="6e890-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="6e890-193">У одељку **Common Data Service информације о окружењу**, изаберите **Повежи са услугом CDS за апликације.**</span><span class="sxs-lookup"><span data-stu-id="6e890-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="6e890-194">Када изаберете везу, бићете преусмерени на листу ентитета у мапирањима.</span><span class="sxs-lookup"><span data-stu-id="6e890-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="6e890-195">Покрените мапе као што је описано у следећој табели.</span><span class="sxs-lookup"><span data-stu-id="6e890-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="6e890-196">Уверите се да следите наведени редослед.</span><span class="sxs-lookup"><span data-stu-id="6e890-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="6e890-197">**Мапа ентитета**</span><span class="sxs-lookup"><span data-stu-id="6e890-197">**Entity Map**</span></span> | <span data-ttu-id="6e890-198">**Освежавање ентитета**</span><span class="sxs-lookup"><span data-stu-id="6e890-198">**Refresh entity**</span></span> | <span data-ttu-id="6e890-199">**Почетна синхронизација**</span><span class="sxs-lookup"><span data-stu-id="6e890-199">**Initial sync**</span></span> | <span data-ttu-id="6e890-200">**Мастер за почетну синхронизацију**</span><span class="sxs-lookup"><span data-stu-id="6e890-200">**Master for initial sync**</span></span> | <span data-ttu-id="6e890-201">**Предуслови за покретање**</span><span class="sxs-lookup"><span data-stu-id="6e890-201">**Run prerequisites**</span></span> | <span data-ttu-id="6e890-202">**Почетна синхронизација предуслова**</span><span class="sxs-lookup"><span data-stu-id="6e890-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="6e890-203">**Улоге пројектних ресурса за сва предузећа (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="6e890-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="6e890-204">No</span><span class="sxs-lookup"><span data-stu-id="6e890-204">No</span></span> | <span data-ttu-id="6e890-205">Да</span><span class="sxs-lookup"><span data-stu-id="6e890-205">Yes</span></span> | <span data-ttu-id="6e890-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="6e890-206">Common Data Service</span></span> | <span data-ttu-id="6e890-207">No</span><span class="sxs-lookup"><span data-stu-id="6e890-207">No</span></span> | <span data-ttu-id="6e890-208">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-208">N\A</span></span> |
| <span data-ttu-id="6e890-209">**Правна лица (cdm\_предузећа)**</span><span class="sxs-lookup"><span data-stu-id="6e890-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="6e890-210">No</span><span class="sxs-lookup"><span data-stu-id="6e890-210">No</span></span> | <span data-ttu-id="6e890-211">Да</span><span class="sxs-lookup"><span data-stu-id="6e890-211">Yes</span></span> | <span data-ttu-id="6e890-212">Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="6e890-212">Finance and Operations apps</span></span> | <span data-ttu-id="6e890-213">No</span><span class="sxs-lookup"><span data-stu-id="6e890-213">No</span></span> | <span data-ttu-id="6e890-214">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-214">N\A</span></span> |
| <span data-ttu-id="6e890-215">**Књига (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="6e890-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="6e890-216">No</span><span class="sxs-lookup"><span data-stu-id="6e890-216">No</span></span> | <span data-ttu-id="6e890-217">Да</span><span class="sxs-lookup"><span data-stu-id="6e890-217">Yes</span></span> | <span data-ttu-id="6e890-218">Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="6e890-218">Finance and Operations apps</span></span> | <span data-ttu-id="6e890-219">Да</span><span class="sxs-lookup"><span data-stu-id="6e890-219">Yes</span></span> | <span data-ttu-id="6e890-220">Да, Finance and Operations апликације</span><span class="sxs-lookup"><span data-stu-id="6e890-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="6e890-221">**Project Operations стварне вредности интеграције (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="6e890-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="6e890-222">No</span><span class="sxs-lookup"><span data-stu-id="6e890-222">No</span></span> | <span data-ttu-id="6e890-223">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-223">No</span></span> | <span data-ttu-id="6e890-224">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-224">N\A</span></span> | <span data-ttu-id="6e890-225">Да</span><span class="sxs-lookup"><span data-stu-id="6e890-225">Yes</span></span> | <span data-ttu-id="6e890-226">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-226">No</span></span> |
| <span data-ttu-id="6e890-227">**Предмети уговора пројекта (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="6e890-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="6e890-228">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-228">No</span></span> | <span data-ttu-id="6e890-229">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-229">No</span></span> | <span data-ttu-id="6e890-230">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-230">N\A</span></span> | <span data-ttu-id="6e890-231">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-231">No</span></span> | <span data-ttu-id="6e890-232">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-232">No</span></span> |
| <span data-ttu-id="6e890-233">**Ентитет интеграције за односе трансакција пројекта (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="6e890-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="6e890-234">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-234">No</span></span> | <span data-ttu-id="6e890-235">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-235">No</span></span> | <span data-ttu-id="6e890-236">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-236">N\A</span></span> | <span data-ttu-id="6e890-237">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-237">No</span></span> | <span data-ttu-id="6e890-238">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-238">N\A</span></span> |
| <span data-ttu-id="6e890-239">**Project Operations контролне тачке предмета уговора о интеграцији (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="6e890-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="6e890-240">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-240">No</span></span> | <span data-ttu-id="6e890-241">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-241">No</span></span> | <span data-ttu-id="6e890-242">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-242">N\A</span></span> | <span data-ttu-id="6e890-243">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-243">No</span></span> | <span data-ttu-id="6e890-244">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-244">N\A</span></span> |
| <span data-ttu-id="6e890-245">**Project Operations ентитет интеграције за процене трошкова (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="6e890-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="6e890-246">Ne</span><span class="sxs-lookup"><span data-stu-id="6e890-246">No</span></span> | <span data-ttu-id="6e890-247">Ne</span><span class="sxs-lookup"><span data-stu-id="6e890-247">No</span></span> | <span data-ttu-id="6e890-248">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-248">N\A</span></span> | <span data-ttu-id="6e890-249">Ne</span><span class="sxs-lookup"><span data-stu-id="6e890-249">No</span></span> | <span data-ttu-id="6e890-250">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-250">N\A</span></span> |
| <span data-ttu-id="6e890-251">**Project Operations ентитет извоза категорија трошкова пројекта (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="6e890-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="6e890-252">Ne</span><span class="sxs-lookup"><span data-stu-id="6e890-252">No</span></span> | <span data-ttu-id="6e890-253">Ne</span><span class="sxs-lookup"><span data-stu-id="6e890-253">No</span></span> | <span data-ttu-id="6e890-254">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-254">N\A</span></span> | <span data-ttu-id="6e890-255">Ne</span><span class="sxs-lookup"><span data-stu-id="6e890-255">No</span></span> | <span data-ttu-id="6e890-256">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-256">N\A</span></span> |
| <span data-ttu-id="6e890-257">**Project Operations ентитет извоза трошкова интеграције пројекта (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="6e890-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="6e890-258">Да</span><span class="sxs-lookup"><span data-stu-id="6e890-258">Yes</span></span> | <span data-ttu-id="6e890-259">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-259">No</span></span> | <span data-ttu-id="6e890-260">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-260">N\A</span></span> | <span data-ttu-id="6e890-261">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-261">No</span></span> | <span data-ttu-id="6e890-262">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-262">N\A</span></span> |
| <span data-ttu-id="6e890-263">**Project Operations ентитет интеграције за процене сати (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="6e890-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="6e890-264">Да</span><span class="sxs-lookup"><span data-stu-id="6e890-264">Yes</span></span> | <span data-ttu-id="6e890-265">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-265">No</span></span> | <span data-ttu-id="6e890-266">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-266">N\A</span></span> | <span data-ttu-id="6e890-267">Не</span><span class="sxs-lookup"><span data-stu-id="6e890-267">No</span></span> | <span data-ttu-id="6e890-268">Није примењиво</span><span class="sxs-lookup"><span data-stu-id="6e890-268">N\A</span></span> |


4. <span data-ttu-id="6e890-269">Да бисте освежили ентитет, изаберите назив мапе, а затим изаберите **Освежи ентитете**.</span><span class="sxs-lookup"><span data-stu-id="6e890-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Освежавање мапе](./media/20RefreshMapping.png)

5. <span data-ttu-id="6e890-271">Када се освежавање заврши, покренита мапу .</span><span class="sxs-lookup"><span data-stu-id="6e890-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="6e890-272">Пре него што омогућите следећу мапу, проверите да ли је мапа у табели у стању **Покренута**.</span><span class="sxs-lookup"><span data-stu-id="6e890-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="6e890-273">Покретање мапа са већим бројем предуслова може потрајати.</span><span class="sxs-lookup"><span data-stu-id="6e890-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="6e890-274">Да бисте покренули мапу са предусловима, омогућите преклопно дугме **Прикажи повезане мапе ентитета**.</span><span class="sxs-lookup"><span data-stu-id="6e890-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="6e890-275">Ако табела показује да **Почетна синхронизација предуслова** има вредност **Не**, проверите да ли је заставица **Почетна синхронизација** **искључена** у свим мапама предуслова пре него што је покренете.</span><span class="sxs-lookup"><span data-stu-id="6e890-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Покретање мапе](./media/21RunMap.png)

6. <span data-ttu-id="6e890-277">Потврдите да су све мапе повезане са пројектом у активном стању.</span><span class="sxs-lookup"><span data-stu-id="6e890-277">Validate all project related maps are in the running state.</span></span>

![Све мапе су покренуте](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="6e890-279">Примена података о конфигурацији у услузи CDS за Project Operations (опционално)</span><span class="sxs-lookup"><span data-stu-id="6e890-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="6e890-280">Ако сте применили демо податке на Finance окружење, погледајте чланак [Подешавање и примена података о конфигурацији у услузи Common Data Service за Project Operations](resource-apply-pro-setup-config-data.md) за примену демо података на CDS окружење.</span><span class="sxs-lookup"><span data-stu-id="6e890-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="6e890-281">Ваше Project Operations окружење је сада обезбеђено и конфигурисано.</span><span class="sxs-lookup"><span data-stu-id="6e890-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]