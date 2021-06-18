---
title: Подешавање и примена података о конфигурацији у услузи Common Data Service
description: Ова тема пружа информације о томе како да подесите и примените податке о конфигурацији у услузи Project Operations.
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ea00df6112fb69b61f1889463424fdfee79aec9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001309"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="37622-103">Подешавање и примена података о конфигурацији у услузи Common Data Service</span><span class="sxs-lookup"><span data-stu-id="37622-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="37622-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="37622-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="37622-105">Предуслови</span><span class="sxs-lookup"><span data-stu-id="37622-105">Prerequisites</span></span>

<span data-ttu-id="37622-106">Пре него што почнете да конфигуришете податке у услузи Common Data Service (CDS), морају бити испуњени следећи предуслови:</span><span class="sxs-lookup"><span data-stu-id="37622-106">Before you begin to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="37622-107">Обезбедите CDS окружење и Dynamics 365 Finance окружење за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="37622-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="37622-108">Информације о правном лицу из услуге Dynamics 365 Finance се деле са CDS окружењем.</span><span class="sxs-lookup"><span data-stu-id="37622-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="37622-109">То значи да ентитет **Компанија** у CDS-у има следеће евиденције предузећа:</span><span class="sxs-lookup"><span data-stu-id="37622-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="37622-110">THPM</span><span class="sxs-lookup"><span data-stu-id="37622-110">THPM</span></span>
  - <span data-ttu-id="37622-111">USPM</span><span class="sxs-lookup"><span data-stu-id="37622-111">USPM</span></span>
  - <span data-ttu-id="37622-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="37622-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="37622-113">Подаци о подешавању и конфигурацији инсталирања</span><span class="sxs-lookup"><span data-stu-id="37622-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="37622-114">Преузмите, деблокирајте и распакујте [Пакет података за подешавање и конфигурацију](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span><span class="sxs-lookup"><span data-stu-id="37622-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span></span>
2. <span data-ttu-id="37622-115">Идите у фасциклу са распакованим садржајем и покрените извршну датотеку *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="37622-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="37622-116">На 1. страници Common Data Service чаробњака за конфигурисање миграције (CMT) изаберите **Увези податке**, а затим изаберите **Настави**.</span><span class="sxs-lookup"><span data-stu-id="37622-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Миграција конфигурације](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="37622-118">На 2. страници CMT чаробњака изаберите **Microsoft 365** као **Тип примене**.</span><span class="sxs-lookup"><span data-stu-id="37622-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="37622-119">Изаберите поља за потврду **Прикажи листу доступних организација** и **Прикажи напредно**.</span><span class="sxs-lookup"><span data-stu-id="37622-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="37622-120">Изаберите регион вашег закупца, унесите своје акредитиве, па изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="37622-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Пријављивање у конфигурацију](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="37622-122">На 3. страници, са листе организација у закупцу, изаберите у коју организацију желите да увезете демо податке, а затим изаберите **Пријављивање**.</span><span class="sxs-lookup"><span data-stu-id="37622-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="37622-123">На 4. страници, изаберите zip датотеку *SampleSetupAndConfigData* из распаковане фасцикле.</span><span class="sxs-lookup"><span data-stu-id="37622-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Избор zip датотеке](./media/3ZipFile.png)

![Избор датотеке](./media/4SelectAFile.png)

9. <span data-ttu-id="37622-126">Када изаберете zip датотеку, изаберите **Увоз података**.</span><span class="sxs-lookup"><span data-stu-id="37622-126">After the zip file is selected, select **Import Data**.</span></span>

![Увези податке](./media/5ImportData.png)

10. <span data-ttu-id="37622-128">Увоз ће трајати отприлике од два до десет минута, у зависности од брзине ваше мреже.</span><span class="sxs-lookup"><span data-stu-id="37622-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="37622-129">По завршетку увоза, изађите из CMT чаробњака.</span><span class="sxs-lookup"><span data-stu-id="37622-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="37622-130">Потражите у својој организацији податке за следећих 26 ентитета:</span><span class="sxs-lookup"><span data-stu-id="37622-130">Check your organization for data in the following 26 entities:</span></span>

  - <span data-ttu-id="37622-131">Валута</span><span class="sxs-lookup"><span data-stu-id="37622-131">Currency</span></span>
  - <span data-ttu-id="37622-132">Графикон пословних контаката</span><span class="sxs-lookup"><span data-stu-id="37622-132">Chart of Accounts</span></span>
  - <span data-ttu-id="37622-133">Фискални календар</span><span class="sxs-lookup"><span data-stu-id="37622-133">Fiscal Calendar</span></span>
  - <span data-ttu-id="37622-134">Врсте девизних курсева валута</span><span class="sxs-lookup"><span data-stu-id="37622-134">Currency Exchange Rate Types</span></span>
  - <span data-ttu-id="37622-135">Дан за плаћање</span><span class="sxs-lookup"><span data-stu-id="37622-135">Payment Day</span></span>
  - <span data-ttu-id="37622-136">Распоред плаћања</span><span class="sxs-lookup"><span data-stu-id="37622-136">Payment Schedule</span></span>
  - <span data-ttu-id="37622-137">Услови плаћања</span><span class="sxs-lookup"><span data-stu-id="37622-137">Payment Term</span></span>
  - <span data-ttu-id="37622-138">Организациона јединица</span><span class="sxs-lookup"><span data-stu-id="37622-138">Organizational Unit</span></span>
  - <span data-ttu-id="37622-139">Контакт</span><span class="sxs-lookup"><span data-stu-id="37622-139">Contact</span></span>
  - <span data-ttu-id="37622-140">Пореска група</span><span class="sxs-lookup"><span data-stu-id="37622-140">Tax Group</span></span>
  - <span data-ttu-id="37622-141">Група клијената</span><span class="sxs-lookup"><span data-stu-id="37622-141">Customer Group</span></span>
  - <span data-ttu-id="37622-142">Група продаваца</span><span class="sxs-lookup"><span data-stu-id="37622-142">Vendor Group</span></span>
  - <span data-ttu-id="37622-143">Јединица</span><span class="sxs-lookup"><span data-stu-id="37622-143">Unit</span></span>
  - <span data-ttu-id="37622-144">Група јединица</span><span class="sxs-lookup"><span data-stu-id="37622-144">Unit Group</span></span>
  - <span data-ttu-id="37622-145">Ценовник</span><span class="sxs-lookup"><span data-stu-id="37622-145">Price List</span></span>
  - <span data-ttu-id="37622-146">Ценовник параметара пројекта</span><span class="sxs-lookup"><span data-stu-id="37622-146">Project Parameter Price List</span></span>
  - <span data-ttu-id="37622-147">Учесталост фактурисања</span><span class="sxs-lookup"><span data-stu-id="37622-147">Invoice Frequency</span></span>
  - <span data-ttu-id="37622-148">Категорија ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="37622-148">Bookable Resource Category</span></span>
  - <span data-ttu-id="37622-149">Категорија трансакције</span><span class="sxs-lookup"><span data-stu-id="37622-149">Transaction Category</span></span>
  - <span data-ttu-id="37622-150">Категорија трошка</span><span class="sxs-lookup"><span data-stu-id="37622-150">Expense Category</span></span>
  - <span data-ttu-id="37622-151">Цена улоге</span><span class="sxs-lookup"><span data-stu-id="37622-151">Role Price</span></span>
  - <span data-ttu-id="37622-152">Цена категорије трансакције</span><span class="sxs-lookup"><span data-stu-id="37622-152">Transaction Category Price</span></span>
  - <span data-ttu-id="37622-153">Карактеристика</span><span class="sxs-lookup"><span data-stu-id="37622-153">Characteristic</span></span>
  - <span data-ttu-id="37622-154">Ресурс који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="37622-154">Bookable Resource</span></span>
  - <span data-ttu-id="37622-155">Повезивање категорије ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="37622-155">Bookable resource category Assn</span></span>
  - <span data-ttu-id="37622-156">Карактеристика ресурса који може да се резервише</span><span class="sxs-lookup"><span data-stu-id="37622-156">Bookable Resource Characteristic</span></span>

![Комплетан увоз](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="37622-158">Ажурирање Project Operations конфигурације</span><span class="sxs-lookup"><span data-stu-id="37622-158">Update Project Operations configurations</span></span>

1. <span data-ttu-id="37622-159">Идите у CE окружење.</span><span class="sxs-lookup"><span data-stu-id="37622-159">Navigate to the CE environment.</span></span> <span data-ttu-id="37622-160">Можете га пронаћи ако отворите [Power Platform центар администрације](https://admin.powerplatform.microsoft.com/environments), изаберете окружење, а затим изаберете **Отворено окружење**.</span><span class="sxs-lookup"><span data-stu-id="37622-160">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Отворено окружење](./media/7OpenEnvironment.png)

2. <span data-ttu-id="37622-162">Идите на **Пројекти** > **Ресурси**, а затим изаберите **Ново** да бисте креирали ресурс који може да се резервише за вашег корисника.</span><span class="sxs-lookup"><span data-stu-id="37622-162">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Ресурси који могу да се резервишу](./media/8BookableResources.png)

3. <span data-ttu-id="37622-164">На картици **Општи подаци** изаберите свог администратора.</span><span class="sxs-lookup"><span data-stu-id="37622-164">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="37622-165">Проверите да ли се временска зона подудара са оном у којој се налазите.</span><span class="sxs-lookup"><span data-stu-id="37622-165">Verify that the time zone matches the one you are in.</span></span> 

![Нови ресурс који може да се резервише](./media/9NewBookableResource.png)

4. <span data-ttu-id="37622-167">На картици **Заказивање**, у пољу **Компанија** одаберите компанију **USPM**, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="37622-167">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Картица „Заказивање“](./media/10SchedulingTab.png)

5. <span data-ttu-id="37622-169">Изаберите картицу **Радно време**.</span><span class="sxs-lookup"><span data-stu-id="37622-169">Select the **Work hours** tab.</span></span>  

![Радно време](./media/11WorkHours.png)

6. <span data-ttu-id="37622-171">Двапут кликните било коју вредност у календару и изаберите **Уређивање** > **Сви догађаји у серији**.</span><span class="sxs-lookup"><span data-stu-id="37622-171">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Календар посла](./media/12WorkCalendar.png)

7. <span data-ttu-id="37622-173">Промените радно време у радни дан од осам (8) сати, обележите викенде као нерадне дане и уверите се да временска зона одговара вашем.</span><span class="sxs-lookup"><span data-stu-id="37622-173">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="37622-174">Изаберите **Сачувај и затвори**.</span><span class="sxs-lookup"><span data-stu-id="37622-174">Select **Save and close**.</span></span>

![Ажурирање календара](./media/13UpdateCalendar.png)

9. <span data-ttu-id="37622-176">Идите на **Подешавања** > **Предлошци календара** и изаберите **Нови**.</span><span class="sxs-lookup"><span data-stu-id="37622-176">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Предлошци календара](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="37622-178">Унесите назив, изаберите ресурс шаблона који сте креирали, а затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="37622-178">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Чување предлошка календара](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="37622-180">Идите на **Параметри** и двапут кликните на запис.</span><span class="sxs-lookup"><span data-stu-id="37622-180">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Параметри пројекта](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="37622-182">Ажурирајте следећа поља:</span><span class="sxs-lookup"><span data-stu-id="37622-182">Update the following fields:</span></span>

 - <span data-ttu-id="37622-183">**Подразумевана компанија**: USPM</span><span class="sxs-lookup"><span data-stu-id="37622-183">**Default company**: USPM</span></span>
 - <span data-ttu-id="37622-184">**Подразумевана организациона јединица**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="37622-184">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="37622-185">**Учесталост фактурисања**: Седми и последњи дан</span><span class="sxs-lookup"><span data-stu-id="37622-185">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="37622-186">**Предложак радног времена**: Промените на предложак који сте креирали.</span><span class="sxs-lookup"><span data-stu-id="37622-186">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="37622-187">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="37622-187">Select **Save**.</span></span> 

![Ажурирани параметри пројекта](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
