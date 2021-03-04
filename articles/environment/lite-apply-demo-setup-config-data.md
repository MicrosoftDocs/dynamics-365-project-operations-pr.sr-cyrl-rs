---
title: Примена демо подешавања и података о конфигурацији – једноставно
description: Ова тема пружа информације о томе како да примените демо подешавања и податке о конфигурацији за Project Operations.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 762b0cf317d442565a033f56033a53a5b5cc435c
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089137"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="e8a5f-103">Примена демо подешавања и података о конфигурацији за Project Operations – једноставно</span><span class="sxs-lookup"><span data-stu-id="e8a5f-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="e8a5f-104">_\*\*Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="e8a5f-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="e8a5f-105">Предуслови</span><span class="sxs-lookup"><span data-stu-id="e8a5f-105">Prerequisites</span></span>

<span data-ttu-id="e8a5f-106">Пре него што започнете конфигурацију, морате имати Common Data Service (CDS) окружење предвиђено за Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="e8a5f-107">Упутства</span><span class="sxs-lookup"><span data-stu-id="e8a5f-107">Instructions</span></span>

1. <span data-ttu-id="e8a5f-108">Преузмите [Пакет главних података](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="e8a5f-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="e8a5f-109">Идите у фасциклу *ProjOpsDemoDataSetupAndMaster - Integrated CMT* и покрените извршну датотеку *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="e8a5f-110">На 1. страници Common Data Service чаробњака за конфигурисање миграције (CMT) изаберите **Увези податке**, а затим изаберите **Настави**.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![Миграција конфигурације](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="e8a5f-112">На 2. страници CMT чаробњака изаберите **Microsoft 365** као **Тип примене**.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="e8a5f-113">Изаберите поља за потврду **Прикажи листу доступних организација** и **Прикажи напредно**.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="e8a5f-114">Изаберите регион вашег закупца, унесите своје акредитиве, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![Пријављивање у конфигурацију](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="e8a5f-116">На страници 3, са листе организација у закупцу, изаберите у коју организацију желите да увезете демо податке, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="e8a5f-117">На 4. страници изаберите zip датотеку *MasterAndSetupData* из распаковане фасцикле *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

   ![Компримована датотека](./media/3ZipFile.png)

   ![Избор датотеке](./media/4SelectAFile.png)

9. <span data-ttu-id="e8a5f-120">Када изаберете zip датотеку, изаберите **Увоз података**.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-120">After the zip file is selected, select **Import Data**.</span></span>

   ![Увоз података](./media/5ImportData.png)

10. <span data-ttu-id="e8a5f-122">Увоз ће трајати отприлике од два до десет минута, у зависности од брзине ваше мреже.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="e8a5f-123">По завршетку изађите из CMT чаробњака.</span><span class="sxs-lookup"><span data-stu-id="e8a5f-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="e8a5f-124">Потражите у својој организацији податке за следећих 20 ентитета:</span><span class="sxs-lookup"><span data-stu-id="e8a5f-124">Check your organization for data in the following 20 entities:</span></span>

    -   <span data-ttu-id="e8a5f-125">Валута</span><span class="sxs-lookup"><span data-stu-id="e8a5f-125">Currency</span></span>
    -   <span data-ttu-id="e8a5f-126">Налог</span><span class="sxs-lookup"><span data-stu-id="e8a5f-126">Account</span></span>
    -   <span data-ttu-id="e8a5f-127">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="e8a5f-127">Organizational Unit</span></span>
    -   <span data-ttu-id="e8a5f-128">Контакт</span><span class="sxs-lookup"><span data-stu-id="e8a5f-128">Contact</span></span>
    -   <span data-ttu-id="e8a5f-129">Јединица</span><span class="sxs-lookup"><span data-stu-id="e8a5f-129">Unit</span></span>
    -   <span data-ttu-id="e8a5f-130">Група јединица</span><span class="sxs-lookup"><span data-stu-id="e8a5f-130">Unit Group</span></span>
    -   <span data-ttu-id="e8a5f-131">Ценовник</span><span class="sxs-lookup"><span data-stu-id="e8a5f-131">Price List</span></span>
    -   <span data-ttu-id="e8a5f-132">Ценовник параметара пројекта</span><span class="sxs-lookup"><span data-stu-id="e8a5f-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="e8a5f-133">Учесталост фактурисања</span><span class="sxs-lookup"><span data-stu-id="e8a5f-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="e8a5f-134">Категорија ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="e8a5f-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="e8a5f-135">Категорија трансакције</span><span class="sxs-lookup"><span data-stu-id="e8a5f-135">Transaction Category</span></span>
    -   <span data-ttu-id="e8a5f-136">Категорија трошка</span><span class="sxs-lookup"><span data-stu-id="e8a5f-136">Expense Category</span></span>
    -   <span data-ttu-id="e8a5f-137">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="e8a5f-137">Role Price</span></span>
    -   <span data-ttu-id="e8a5f-138">Цена категорије трансакције</span><span class="sxs-lookup"><span data-stu-id="e8a5f-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="e8a5f-139">Карактеристика</span><span class="sxs-lookup"><span data-stu-id="e8a5f-139">Characteristic</span></span>
    -   <span data-ttu-id="e8a5f-140">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="e8a5f-140">Bookable Resource</span></span>
    -   <span data-ttu-id="e8a5f-141">Повезивање категорије ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="e8a5f-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="e8a5f-142">Карактеристика ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="e8a5f-142">Bookable Resource Characteristic</span></span>

    ![Комплетан увоз](./media/6CompleteImport.png)
