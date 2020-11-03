---
title: Подешавање и примена података о конфигурацији у услузи Common Data Service за Project Operations
description: Ова тема пружа информације о томе како да подесите и примените податке о конфигурацији у услузи Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e72b88a4dae1eb89859fdfd55f6d5e6ee5befcd
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083845"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="9bb9d-103">Подешавање и примена података о конфигурацији у услузи Common Data Service за Project Operations</span><span class="sxs-lookup"><span data-stu-id="9bb9d-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="9bb9d-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="9bb9d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="9bb9d-105">Подаци о подешавању и конфигурацији инсталирања</span><span class="sxs-lookup"><span data-stu-id="9bb9d-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="9bb9d-106">Преузмите, деблокирајте и распакујте [Пакет података за подешавање и конфигурацију](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="9bb9d-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="9bb9d-107">Идите у фасциклу са распакованим садржајем и покрените извршну датотеку *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="9bb9d-108">На 1. страници Common Data Service чаробњака за конфигурисање миграције (CMT) изаберите **Увези податке** , а затим изаберите **Настави**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Миграција конфигурације](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="9bb9d-110">На 2. страници CMT чаробњака изаберите **Microsoft 365** као **Тип примене**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-110">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="9bb9d-111">Изаберите поља за потврду **Прикажи листу доступних организација** и **Прикажи напредно**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="9bb9d-112">Изаберите регион вашег закупца, унесите своје акредитиве, па изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Пријављивање у конфигурацију](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="9bb9d-114">На 3. страници, са листе организација у закупцу, изаберите у коју организацију желите да увезете демо податке, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="9bb9d-115">На 4. страници, изаберите zip датотеку *SampleSetupAndConfigData* из распаковане фасцикле.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Избор zip датотеке](./media/3ZipFile.png)

![Избор датотеке](./media/4SelectAFile.png)

9. <span data-ttu-id="9bb9d-118">Када изаберете zip датотеку, изаберите **Увоз података**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-118">After the zip file is selected, select **Import Data**.</span></span>

![Увези податке](./media/5ImportData.png)

10. <span data-ttu-id="9bb9d-120">Увоз ће трајати отприлике од два до десет минута, у зависности од брзине ваше мреже.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="9bb9d-121">По завршетку увоза, изађите из CMT чаробњака.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="9bb9d-122">Потражите у својој организацији податке за следећих 19 ентитета:</span><span class="sxs-lookup"><span data-stu-id="9bb9d-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="9bb9d-123">Валута</span><span class="sxs-lookup"><span data-stu-id="9bb9d-123">Currency</span></span>
  - <span data-ttu-id="9bb9d-124">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="9bb9d-124">Organizational Unit</span></span>
  - <span data-ttu-id="9bb9d-125">Контакт</span><span class="sxs-lookup"><span data-stu-id="9bb9d-125">Contact</span></span>
  - <span data-ttu-id="9bb9d-126">Пореска група</span><span class="sxs-lookup"><span data-stu-id="9bb9d-126">Tax Group</span></span>
  - <span data-ttu-id="9bb9d-127">Група клијената</span><span class="sxs-lookup"><span data-stu-id="9bb9d-127">Customer Group</span></span>
  - <span data-ttu-id="9bb9d-128">Јединица</span><span class="sxs-lookup"><span data-stu-id="9bb9d-128">Unit</span></span>
  - <span data-ttu-id="9bb9d-129">Група јединица</span><span class="sxs-lookup"><span data-stu-id="9bb9d-129">Unit Group</span></span>
  - <span data-ttu-id="9bb9d-130">Ценовник</span><span class="sxs-lookup"><span data-stu-id="9bb9d-130">Price List</span></span>
  - <span data-ttu-id="9bb9d-131">Ценовник параметара пројекта</span><span class="sxs-lookup"><span data-stu-id="9bb9d-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="9bb9d-132">Учесталост фактурисања</span><span class="sxs-lookup"><span data-stu-id="9bb9d-132">Invoice Frequency</span></span>
  - <span data-ttu-id="9bb9d-133">Категорија ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="9bb9d-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="9bb9d-134">Категорија трансакције</span><span class="sxs-lookup"><span data-stu-id="9bb9d-134">Transaction Category</span></span>
  - <span data-ttu-id="9bb9d-135">Категорија трошка</span><span class="sxs-lookup"><span data-stu-id="9bb9d-135">Expense Category</span></span>
  - <span data-ttu-id="9bb9d-136">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="9bb9d-136">Role Price</span></span>
  - <span data-ttu-id="9bb9d-137">Цена категорије трансакције</span><span class="sxs-lookup"><span data-stu-id="9bb9d-137">Transaction Category Price</span></span>
  - <span data-ttu-id="9bb9d-138">Карактеристика</span><span class="sxs-lookup"><span data-stu-id="9bb9d-138">Characteristic</span></span>
  - <span data-ttu-id="9bb9d-139">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="9bb9d-139">Bookable Resource</span></span>
  - <span data-ttu-id="9bb9d-140">Повезивање категорије ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="9bb9d-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="9bb9d-141">Карактеристика ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="9bb9d-141">Bookable Resource Characteristic</span></span>

![Комплетан увоз](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="9bb9d-143">Ажурирање Project Operations конфигурације</span><span class="sxs-lookup"><span data-stu-id="9bb9d-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="9bb9d-144">Идите у CE окружење.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-144">Navigate to the CE environment.</span></span> <span data-ttu-id="9bb9d-145">Можете га пронаћи ако отворите [Power Platform центар администрације](https://admin.powerplatform.microsoft.com/environments), изаберете окружење, а затим изаберете **Отворено окружење**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Отворено окружење](./media/7OpenEnvironment.png)

2. <span data-ttu-id="9bb9d-147">Идите на **Пројекти** > **Ресурси** , а затим изаберите **Ново** да бисте креирали ресурс који може да се резервише за вашег корисника.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Ресурси који могу да се резервишу](./media/8BookableResources.png)

3. <span data-ttu-id="9bb9d-149">На картици **Општи подаци** изаберите свог администратора.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="9bb9d-150">Проверите да ли се временска зона подудара са оном у којој се налазите.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-150">Verify that the time zone matches the one you are in.</span></span> 

![Нови ресурс који може да се резервише](./media/9NewBookableResource.png)

4. <span data-ttu-id="9bb9d-152">На картици **Заказивање** , у пољу **Компанија** одаберите компанију **USPM** , а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Картица „Заказивање“](./media/10SchedulingTab.png)

5. <span data-ttu-id="9bb9d-154">Изаберите картицу **Радно време**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-154">Select the **Work hours** tab.</span></span>  

![Радно време](./media/11WorkHours.png)

6. <span data-ttu-id="9bb9d-156">Двапут кликните било коју вредност у календару и изаберите **Уређивање** > **Сви догађаји у серији**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Календар посла](./media/12WorkCalendar.png)

7. <span data-ttu-id="9bb9d-158">Промените радно време у радни дан од осам (8) сати, обележите викенде као нерадне дане и уверите се да временска зона одговара вашем.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="9bb9d-159">Изаберите **Сачувај и затвори**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-159">Select **Save and close**.</span></span>

![Ажурирање календара](./media/13UpdateCalendar.png)

9. <span data-ttu-id="9bb9d-161">Идите на **Подешавања** > **Предлошци календара** и изаберите **Нови**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Предлошци календара](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="9bb9d-163">Унесите назив, изаберите ресурс шаблона који сте креирали, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Чување предлошка календара](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="9bb9d-165">Идите на **Параметри** и двапут кликните на запис.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Параметри пројекта](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="9bb9d-167">Ажурирајте следећа поља:</span><span class="sxs-lookup"><span data-stu-id="9bb9d-167">Update the following fields:</span></span>

 - <span data-ttu-id="9bb9d-168">**Подразумевана компанија** : USPM</span><span class="sxs-lookup"><span data-stu-id="9bb9d-168">**Default company** : USPM</span></span>
 - <span data-ttu-id="9bb9d-169">**Подразумевана организациона јединица** : Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="9bb9d-169">**Default Organizational Unit** : Contoso Robotics Global</span></span>
 - <span data-ttu-id="9bb9d-170">**Учесталост фактурисања** : Седми и последњи дан</span><span class="sxs-lookup"><span data-stu-id="9bb9d-170">**Invoice Frequency** : Seventh and Last day</span></span>
 - <span data-ttu-id="9bb9d-171">**Предложак радног времена** : Промените на предложак који сте креирали.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-171">**Work hour template** : Change to the template you created.</span></span>

13. <span data-ttu-id="9bb9d-172">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="9bb9d-172">Select **Save**.</span></span> 

![Ажурирани параметри пројекта](./media/17UpdatedProjectParameters.png)
