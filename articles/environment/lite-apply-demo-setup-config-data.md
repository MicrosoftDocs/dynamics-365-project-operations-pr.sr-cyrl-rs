---
title: Примена демо подешавања и података о конфигурацији – једноставно
description: Ова тема пружа информације о томе како да примените демо подешавања и податке о конфигурацији за Project Operations.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7729b4a9ef5f498b78af298f7233d7dd45434bb3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997169"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="c4866-103">Примена демо подешавања и података о конфигурацији за Project Operations – једноставно</span><span class="sxs-lookup"><span data-stu-id="c4866-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="c4866-104">_\*\*Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="c4866-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="c4866-105">Предуслови</span><span class="sxs-lookup"><span data-stu-id="c4866-105">Prerequisites</span></span>

<span data-ttu-id="c4866-106">Пре него што започнете конфигурацију, морате имати Common Data Service (CDS) окружење предвиђено за Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="c4866-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="c4866-107">Упутства</span><span class="sxs-lookup"><span data-stu-id="c4866-107">Instructions</span></span>

1. <span data-ttu-id="c4866-108">Преузмите [Пакет главних података](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip).</span><span class="sxs-lookup"><span data-stu-id="c4866-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip).</span></span> 
2. <span data-ttu-id="c4866-109">Дођите до фасцикле *ProjOpsSampleSetupData - CE only CMT* и покрените извршну датотеку *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="c4866-109">Navigate to the folder *ProjOpsSampleSetupData - CE only CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="c4866-110">На 1. страници Common Data Service чаробњака за конфигурисање миграције (CMT) изаберите **Увези податке**, а затим изаберите **Настави**.</span><span class="sxs-lookup"><span data-stu-id="c4866-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![Миграција конфигурације](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="c4866-112">На 2. страници CMT чаробњака изаберите **Microsoft 365** као **Тип примене**.</span><span class="sxs-lookup"><span data-stu-id="c4866-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="c4866-113">Изаберите поља за потврду **Прикажи листу доступних организација** и **Прикажи напредно**.</span><span class="sxs-lookup"><span data-stu-id="c4866-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="c4866-114">Изаберите регион вашег закупца, унесите своје акредитиве, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="c4866-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![Пријављивање у конфигурацију](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="c4866-116">На страници 3, са листе организација у закупцу, изаберите у коју организацију желите да увезете демо податке, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="c4866-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="c4866-117">На страници 4 изаберите zip датотеку, *SampleSetupAndConfigData* из распаковане фасцикле, *ProjOpsSampleSetupData - CE only CMT*.</span><span class="sxs-lookup"><span data-stu-id="c4866-117">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder, *ProjOpsSampleSetupData - CE only CMT*.</span></span>

   ![Компримована датотека](./media/3ZipFile.png)

   ![Изаберите датотеку](./media/4SelectAFile.png)

9. <span data-ttu-id="c4866-120">Када изаберете zip датотеку, изаберите **Увоз података**.</span><span class="sxs-lookup"><span data-stu-id="c4866-120">After the zip file is selected, select **Import Data**.</span></span>

   ![Увоз података](./media/5ImportData.png)

10. <span data-ttu-id="c4866-122">Увоз ће трајати отприлике од два до десет минута, у зависности од брзине ваше мреже.</span><span class="sxs-lookup"><span data-stu-id="c4866-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="c4866-123">По завршетку изађите из CMT чаробњака.</span><span class="sxs-lookup"><span data-stu-id="c4866-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="c4866-124">Потражите у својој организацији податке за следећих 18 ентитета:</span><span class="sxs-lookup"><span data-stu-id="c4866-124">Check your organization for data in the following 18 entities:</span></span>

    -   <span data-ttu-id="c4866-125">Валута</span><span class="sxs-lookup"><span data-stu-id="c4866-125">Currency</span></span>
    -   <span data-ttu-id="c4866-126">Налог</span><span class="sxs-lookup"><span data-stu-id="c4866-126">Account</span></span>
    -   <span data-ttu-id="c4866-127">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="c4866-127">Organizational Unit</span></span>
    -   <span data-ttu-id="c4866-128">Контакт</span><span class="sxs-lookup"><span data-stu-id="c4866-128">Contact</span></span>
    -   <span data-ttu-id="c4866-129">Јединица</span><span class="sxs-lookup"><span data-stu-id="c4866-129">Unit</span></span>
    -   <span data-ttu-id="c4866-130">Група јединица</span><span class="sxs-lookup"><span data-stu-id="c4866-130">Unit Group</span></span>
    -   <span data-ttu-id="c4866-131">Ценовник</span><span class="sxs-lookup"><span data-stu-id="c4866-131">Price List</span></span>
    -   <span data-ttu-id="c4866-132">Ценовник параметара пројекта</span><span class="sxs-lookup"><span data-stu-id="c4866-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="c4866-133">Учесталост фактурисања</span><span class="sxs-lookup"><span data-stu-id="c4866-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="c4866-134">Категорија ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="c4866-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="c4866-135">Категорија трансакције</span><span class="sxs-lookup"><span data-stu-id="c4866-135">Transaction Category</span></span>
    -   <span data-ttu-id="c4866-136">Категорија трошка</span><span class="sxs-lookup"><span data-stu-id="c4866-136">Expense Category</span></span>
    -   <span data-ttu-id="c4866-137">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="c4866-137">Role Price</span></span>
    -   <span data-ttu-id="c4866-138">Цена категорије трансакције</span><span class="sxs-lookup"><span data-stu-id="c4866-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="c4866-139">Карактеристика</span><span class="sxs-lookup"><span data-stu-id="c4866-139">Characteristic</span></span>
    -   <span data-ttu-id="c4866-140">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="c4866-140">Bookable Resource</span></span>
    -   <span data-ttu-id="c4866-141">Повезивање категорије ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="c4866-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="c4866-142">Карактеристика ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="c4866-142">Bookable Resource Characteristic</span></span>

    ![Комплетан увоз](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
