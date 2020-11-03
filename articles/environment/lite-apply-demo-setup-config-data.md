---
title: Примена демо подешавања и података о конфигурацији
description: Ова тема пружа информације о томе како да примените демо подешавања и податке о конфигурацији за Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 33b85115963f3561718b8951e5b518fd34de7723
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083837"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="4c364-103">Примените демо подешавања и податке о конфигурацији за једноставну примену услуге Project Operations – од погодбе до профактуре</span><span class="sxs-lookup"><span data-stu-id="4c364-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="4c364-104">_\*\*Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="4c364-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="4c364-105">Преузмите [Пакет главних података](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="4c364-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="4c364-106">Идите у фасциклу *ProjOpsDemoDataSetupAndMaster - Integrated CMT* и покрените извршну датотеку *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="4c364-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="4c364-107">На 1. страници Common Data Service чаробњака за конфигурисање миграције (CMT) изаберите **Увези податке** , а затим изаберите **Настави**.</span><span class="sxs-lookup"><span data-stu-id="4c364-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Миграција конфигурације](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="4c364-109">На 2. страници CMT чаробњака изаберите **Microsoft 365** као **Тип примене**.</span><span class="sxs-lookup"><span data-stu-id="4c364-109">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="4c364-110">Изаберите поља за потврду **Прикажи листу доступних организација** и **Прикажи напредно**.</span><span class="sxs-lookup"><span data-stu-id="4c364-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="4c364-111">Изаберите регион вашег закупца, унесите своје акредитиве, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="4c364-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Пријављивање у конфигурацију](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="4c364-113">На страници 3, са листе организација у закупцу, изаберите у коју организацију желите да увезете демо податке, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="4c364-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="4c364-114">На 4. страници изаберите zip датотеку *MasterAndSetupData* из распаковане фасцикле *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="4c364-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Компримована датотека](./media/3ZipFile.png)

![Избор датотеке](./media/4SelectAFile.png)

9. <span data-ttu-id="4c364-117">Када изаберете zip датотеку, изаберите **Увоз података**.</span><span class="sxs-lookup"><span data-stu-id="4c364-117">After the zip file is selected, select **Import Data**.</span></span>

![Увоз података](./media/5ImportData.png)

10. <span data-ttu-id="4c364-119">Увоз ће трајати отприлике од два до десет минута, у зависности од брзине ваше мреже.</span><span class="sxs-lookup"><span data-stu-id="4c364-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="4c364-120">По завршетку изађите из CMT чаробњака.</span><span class="sxs-lookup"><span data-stu-id="4c364-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="4c364-121">Потражите у својој организацији податке за следећих 20 ентитета:</span><span class="sxs-lookup"><span data-stu-id="4c364-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="4c364-122">Валута</span><span class="sxs-lookup"><span data-stu-id="4c364-122">Currency</span></span>
- <span data-ttu-id="4c364-123">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="4c364-123">Organizational Unit</span></span>
- <span data-ttu-id="4c364-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="4c364-124">Contact</span></span>
- <span data-ttu-id="4c364-125">Пореска група</span><span class="sxs-lookup"><span data-stu-id="4c364-125">Tax Group</span></span>
- <span data-ttu-id="4c364-126">Група клијената</span><span class="sxs-lookup"><span data-stu-id="4c364-126">Customer Group</span></span>
- <span data-ttu-id="4c364-127">Јединица</span><span class="sxs-lookup"><span data-stu-id="4c364-127">Unit</span></span>
- <span data-ttu-id="4c364-128">Група јединица</span><span class="sxs-lookup"><span data-stu-id="4c364-128">Unit Group</span></span>
- <span data-ttu-id="4c364-129">Ценовник</span><span class="sxs-lookup"><span data-stu-id="4c364-129">Price List</span></span>
- <span data-ttu-id="4c364-130">Ценовник параметара пројекта</span><span class="sxs-lookup"><span data-stu-id="4c364-130">Project Parameter Price List</span></span>
- <span data-ttu-id="4c364-131">Учесталост фактурисања</span><span class="sxs-lookup"><span data-stu-id="4c364-131">Invoice Frequency</span></span>
- <span data-ttu-id="4c364-132">Детаљ о учесталости фактурисања</span><span class="sxs-lookup"><span data-stu-id="4c364-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="4c364-133">Категорија ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="4c364-133">Bookable Resource Category</span></span>
- <span data-ttu-id="4c364-134">Категорија трансакције</span><span class="sxs-lookup"><span data-stu-id="4c364-134">Transaction Category</span></span>
- <span data-ttu-id="4c364-135">Категорија трошка</span><span class="sxs-lookup"><span data-stu-id="4c364-135">Expense Category</span></span>
- <span data-ttu-id="4c364-136">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="4c364-136">Role Price</span></span>
- <span data-ttu-id="4c364-137">Цена категорије трансакције</span><span class="sxs-lookup"><span data-stu-id="4c364-137">Transaction Category Price</span></span>
- <span data-ttu-id="4c364-138">Карактеристика</span><span class="sxs-lookup"><span data-stu-id="4c364-138">Characteristic</span></span>
- <span data-ttu-id="4c364-139">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="4c364-139">Bookable Resource</span></span>
- <span data-ttu-id="4c364-140">Повезивање категорије ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="4c364-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="4c364-141">Карактеристика ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="4c364-141">Bookable Resource Characteristic</span></span>

![Комплетан увоз](./media/6CompleteImport.png)
