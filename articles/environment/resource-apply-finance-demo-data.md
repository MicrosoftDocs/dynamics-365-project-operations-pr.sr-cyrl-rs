---
title: Примена демо података на Finance окружење које се хостује у облаку
description: Ова тема објашњава како да примените демо податке из услуге Project Operations на Dynamics 365 Finance окружење хостовано у облаку.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a7239301dc8b775dc4a53a1cf6c0bcba3956125a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289882"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="000ff-103">Примена демо података на Finance окружење које се хостује у облаку</span><span class="sxs-lookup"><span data-stu-id="000ff-103">Apply demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="000ff-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="000ff-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="000ff-105">Ова тема је применљива је само на Microsoft Dynamics 365 Finance верзије 10.0.13 и може се изводити само у окружењу које се хостује у облаку.</span><span class="sxs-lookup"><span data-stu-id="000ff-105">This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="000ff-106">Довршите кораке у овој теми **ПРЕ НЕГО ШТО** примените исправке квалитета на окружење.</span><span class="sxs-lookup"><span data-stu-id="000ff-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="000ff-107">У свом LCS пројекту, отворите страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="000ff-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="000ff-108">Приметите да садржи детаље потребне за повезивање са околином помоћу протокола удаљене радне површине (RDP).</span><span class="sxs-lookup"><span data-stu-id="000ff-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![Детаљи  окружења](./media/1EnvironmentDetails.png)

<span data-ttu-id="000ff-110">Први скуп истакнутих акредитива су акредитиви локалног налога и садрже хипервезу до везе са удаљеном радном површином.</span><span class="sxs-lookup"><span data-stu-id="000ff-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="000ff-111">Акредитиви укључују корисничко име и лозинку администратора окружења.</span><span class="sxs-lookup"><span data-stu-id="000ff-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="000ff-112">Други скуп акредитива се користи за пријављивање на SQL Server у овом окружењу.</span><span class="sxs-lookup"><span data-stu-id="000ff-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="000ff-113">Повежите се удаљено са окружењем користећи хипервезу у одељку **Локални налози** и употребите **Акредитиви за локални налог** за потврду идентитета.</span><span class="sxs-lookup"><span data-stu-id="000ff-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="000ff-114">Идите на **Internet Information Services** > **Групе апликација** > **AOSService** и зауставите услугу.</span><span class="sxs-lookup"><span data-stu-id="000ff-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="000ff-115">У овом тренутку заустављате услугу да бисте могли да наставите да замењујете SQL базу података.</span><span class="sxs-lookup"><span data-stu-id="000ff-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![Заустављање AOS](./media/2StopAOS.png)

4. <span data-ttu-id="000ff-117">Идите на **Услуге** и зауставите следеће две ставке:</span><span class="sxs-lookup"><span data-stu-id="000ff-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="000ff-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span><span class="sxs-lookup"><span data-stu-id="000ff-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="000ff-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span><span class="sxs-lookup"><span data-stu-id="000ff-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![Заустављање услуга](./media/3StopServices.png)

5. <span data-ttu-id="000ff-121">Отворите Microsoft SQL Server Management Studio.</span><span class="sxs-lookup"><span data-stu-id="000ff-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="000ff-122">Пријавите се помоћу акредитива за SQL Server и користите корисника axdbadmin и лозинку са LCS странице **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="000ff-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server Management Studio](./media/4SSMS.png)

6. <span data-ttu-id="000ff-124">У прегледачу објеката, изаберите **Базе података** и пронађите **AXDB**.</span><span class="sxs-lookup"><span data-stu-id="000ff-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="000ff-125">Базу података ћете заменити новом базом података која се налази у [центру за преузимање](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span><span class="sxs-lookup"><span data-stu-id="000ff-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="000ff-126">Копирајте zip датотеку у VM у који сте удаљено повезани и распакујте zip садржај.</span><span class="sxs-lookup"><span data-stu-id="000ff-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="000ff-127">У програму SQL Server Management Studio кликните десним тастером миша на **AxDB**, а затим изаберите **Задаци** > **Враћање** > **База података**.</span><span class="sxs-lookup"><span data-stu-id="000ff-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![Враћање базе података](./media/5RestoreDatabase.png)

9. <span data-ttu-id="000ff-129">Изаберите **Изворни уређај** и дођите до датотеке извучене из zip датотеке коју сте копирали.</span><span class="sxs-lookup"><span data-stu-id="000ff-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![Изворни уређаји](./media/6SourceDevice.png)

10. <span data-ttu-id="000ff-131">Изаберите **Опције**, а затим изаберите **Препиши постојећу базу података** и **Затворите постојеће везе са одредишном базом података**.</span><span class="sxs-lookup"><span data-stu-id="000ff-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="000ff-132">Изаберите **У реду**.</span><span class="sxs-lookup"><span data-stu-id="000ff-132">Select **OK**.</span></span>

![Враћање подешавања](./media/7RestoreSetting.png)

<span data-ttu-id="000ff-134">Добићете потврду да је враћање AXDB било успешно.</span><span class="sxs-lookup"><span data-stu-id="000ff-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="000ff-135">Када добијете ову потврду, можете да затворите SQL Services Management Studio.</span><span class="sxs-lookup"><span data-stu-id="000ff-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="000ff-136">Вратите се на **Internet Information Services** > **Групе апликација** > **AOSService** и покрените услугу.</span><span class="sxs-lookup"><span data-stu-id="000ff-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="000ff-137">Идите на **Услуге** и покрените две услуге које сте раније зауставили.</span><span class="sxs-lookup"><span data-stu-id="000ff-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="000ff-138">Пронађите алатку AdminUserProvisioning на овом VM-у.</span><span class="sxs-lookup"><span data-stu-id="000ff-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="000ff-139">Потражите K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span><span class="sxs-lookup"><span data-stu-id="000ff-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="000ff-140">Покрените .ext датотеку користећи своју корисничку адресу у пољу **Адреса е-поште**.</span><span class="sxs-lookup"><span data-stu-id="000ff-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="000ff-141">Изаберите **Проследи**.</span><span class="sxs-lookup"><span data-stu-id="000ff-141">Select **Submit**.</span></span>

![Обезбеђивање корисника-администратора](./media/8AdminUserProvisioning.png)

<span data-ttu-id="000ff-143">За ово је потребно неколико минута.</span><span class="sxs-lookup"><span data-stu-id="000ff-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="000ff-144">Требало би да примите поруку са потврдом да је корисник-администратор успешно ажуриран.</span><span class="sxs-lookup"><span data-stu-id="000ff-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="000ff-145">На крају, покрените командну линију као администратор и покрените команду iisreset</span><span class="sxs-lookup"><span data-stu-id="000ff-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![Ресетовање IIS](./media/9IISReset.png)

18. <span data-ttu-id="000ff-147">Затворите сесију удаљене радне површине и користите страницу LCS **Детаљи окружења** да бисте се пријавили у окружење и потврдили да ради као што се очекује.</span><span class="sxs-lookup"><span data-stu-id="000ff-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]