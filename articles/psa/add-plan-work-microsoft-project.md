---
title: Користите програмски додатак Project Service за планирање вашег рада у програму Microsoft Project | MicrosoftDocs
description: Ова тема пружа информације о додавању, конфигурисању и коришћењу програмског додатка Microsoft Project у програму Microsoft Project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 6bc74442866caccc02e53afc913a55aab81f9629
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129696"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="8f357-103">Користите програмски додатак Project Service Automation за планирање вашег рада у програму Microsoft Project</span><span class="sxs-lookup"><span data-stu-id="8f357-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="8f357-104">вам олакшава да обављате планирање пројеката, укључујући процене.</span><span class="sxs-lookup"><span data-stu-id="8f357-104">makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="8f357-105">Можете да дефинишете рад тако да трошкови, ангажовање и продајна вредност буду јасни када коначан предлог буде прослеђен.</span><span class="sxs-lookup"><span data-stu-id="8f357-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="8f357-106">Сада можете да инсталирате систем [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] и да послове планирања обављате у познатом окружења програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="8f357-107">Користите робусне могућности планирања и управљања програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], а затим ажурирајте план пројекта у програму Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="8f357-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="8f357-108">Да бисте користили SharePoint управљање документима за складиштење у вашим [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотекама за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекте, ваш [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] администратор ће морати да укључи управљање документима.</span><span class="sxs-lookup"><span data-stu-id="8f357-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> 
> - <span data-ttu-id="8f357-109">[!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] је компатибилан само са [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional издањем.</span><span class="sxs-lookup"><span data-stu-id="8f357-109">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="8f357-110">Преузмите и инсталирајте програмски додатак</span><span class="sxs-lookup"><span data-stu-id="8f357-110">Download and install the add-in</span></span>  
 <span data-ttu-id="8f357-111">Припремите ваше информације за пријављивање у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-111">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="8f357-112">Те информације ће вам бити потребне да бисте се повезали са програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] на функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-112">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="8f357-113">Из центра за преузимање преузмите програмски додатак за подржану верзију услуге of Project Service, верзије [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) или [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span><span class="sxs-lookup"><span data-stu-id="8f357-113">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="8f357-114">Кликните на везу за преузимање.</span><span class="sxs-lookup"><span data-stu-id="8f357-114">Click the download link.</span></span>  

3.  <span data-ttu-id="8f357-115">Након преузимања, кликните на **Да** да бисте инсталирали програмски додатак.</span><span class="sxs-lookup"><span data-stu-id="8f357-115">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="8f357-116">Конфигуришите програмски додатак</span><span class="sxs-lookup"><span data-stu-id="8f357-116">Configure the add-in</span></span>  

1. <span data-ttu-id="8f357-117">Отворите [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и кликните на картицу **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="8f357-117">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="8f357-118">Кликните на дугме **Повежи**.</span><span class="sxs-lookup"><span data-stu-id="8f357-118">Click **Connect**.</span></span>  

3. <span data-ttu-id="8f357-119">Унесите своје информације за пријављивање и кликните на дугме **Пријави се**.</span><span class="sxs-lookup"><span data-stu-id="8f357-119">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="8f357-120">Сада можете почети са коришћењем програмског додатка.</span><span class="sxs-lookup"><span data-stu-id="8f357-120">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="8f357-121">Читање из предлошка</span><span class="sxs-lookup"><span data-stu-id="8f357-121">Read from a template</span></span>  
 <span data-ttu-id="8f357-122">Читајте из предлошка који сте креирали у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] и копирали у програм [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] да бисте започели планирање пројекта.</span><span class="sxs-lookup"><span data-stu-id="8f357-122">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="8f357-123">[Креирање предлошка за пројекат (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="8f357-123">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1.  <span data-ttu-id="8f357-124">Са картице **Project Service** кликните на дугме **Читање** > **Предложак Project Service Automation пројекта**.</span><span class="sxs-lookup"><span data-stu-id="8f357-124">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="8f357-125">Са листе изаберите предложак пројекта и кликните на дугме **Отвори**.</span><span class="sxs-lookup"><span data-stu-id="8f357-125">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="8f357-126">Подразумевано, задаци који су копирани из предлошка у пројекат су подешени као ручно заказани.</span><span class="sxs-lookup"><span data-stu-id="8f357-126">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="8f357-127">Додељивање [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] улога ресурсима пројекта</span><span class="sxs-lookup"><span data-stu-id="8f357-127">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="8f357-128">Отворите пројекат и кликните на траку **Задатак**.</span><span class="sxs-lookup"><span data-stu-id="8f357-128">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="8f357-129">Кликните на мени **Гантов графикон**, а затим изаберите **Листа ресурса**.</span><span class="sxs-lookup"><span data-stu-id="8f357-129">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="8f357-130">На листу ресурса кликните на дугме у падајућем менију **Улога ресурса за Project Service** и одаберите улогу за Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="8f357-130">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="8f357-131">Обезбедите радну снагу за пројекат помоћу ресурса</span><span class="sxs-lookup"><span data-stu-id="8f357-131">Staff your project with resources</span></span>  

1.  <span data-ttu-id="8f357-132">На картици „Project Service“ изаберите ред и кликните на дугме **Пронађи ресурсе**.</span><span class="sxs-lookup"><span data-stu-id="8f357-132">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="8f357-133">На екрану **Резервација ресурса** изаберите ресурс који желите да користите за пројекат.</span><span class="sxs-lookup"><span data-stu-id="8f357-133">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="8f357-134">Кликните на дугме **Резервиши**, а затим на **У реду**.</span><span class="sxs-lookup"><span data-stu-id="8f357-134">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="8f357-135">Објавите ваш пројекат</span><span class="sxs-lookup"><span data-stu-id="8f357-135">Publish your project</span></span>  
<span data-ttu-id="8f357-136">Када се планирање пројекта заврши, следећи корак је увоз и објављивање пројекта у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-136">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="8f357-137">Пројекат ће се увести у функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-137">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="8f357-138">Примењују се процеси одређивања цена и генерисања тима.</span><span class="sxs-lookup"><span data-stu-id="8f357-138">The pricing and team generation process are applied.</span></span> <span data-ttu-id="8f357-139">Отворите пројекат у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] да бисте видели да ли су тим, процене за пројекат и структурна анализа посла генерисани.</span><span class="sxs-lookup"><span data-stu-id="8f357-139">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="8f357-140">У следећој табели је приказано где да пронађете резултате:</span><span class="sxs-lookup"><span data-stu-id="8f357-140">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="8f357-141">**Гантов графикон**</span><span class="sxs-lookup"><span data-stu-id="8f357-141">**Gantt Chart**</span></span>   | <span data-ttu-id="8f357-142">Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Структурна анализа посла**.</span><span class="sxs-lookup"><span data-stu-id="8f357-142">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="8f357-143">**Листа ресурса**</span><span class="sxs-lookup"><span data-stu-id="8f357-143">**Resource Sheet**</span></span> |   <span data-ttu-id="8f357-144">Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Чланови пројектног тима**.</span><span class="sxs-lookup"><span data-stu-id="8f357-144">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="8f357-145">**Користите употребу**</span><span class="sxs-lookup"><span data-stu-id="8f357-145">**Use Usage**</span></span>    |    <span data-ttu-id="8f357-146">Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Процене пројекта**.</span><span class="sxs-lookup"><span data-stu-id="8f357-146">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="8f357-147">**Да бисте увозили и објављивали пројекте**</span><span class="sxs-lookup"><span data-stu-id="8f357-147">**To import and publish your project**</span></span>  
1. <span data-ttu-id="8f357-148">Са картице **Project Service** кликните на **Објави** > **Нови Project Service Automation пројекат**.</span><span class="sxs-lookup"><span data-stu-id="8f357-148">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="8f357-149">У дијалогу **Објави у нови пројекат у програму Project Service** унесите **Име пројекта** и изаберите **Клијент**.</span><span class="sxs-lookup"><span data-stu-id="8f357-149">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="8f357-150">Опционално означите **Повежи план пројекта са функцијом Project Service Automation** да бисте повезали датотеку пројекта плана са функцијом Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="8f357-150">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="8f357-151">Изаберите дугме **Објави**</span><span class="sxs-lookup"><span data-stu-id="8f357-151">Click **Publish**.</span></span>  

   <span data-ttu-id="8f357-152">Повезивање датотеке пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] од датотеке пројекта прави главну датотеку и подешава структурну анализу посла у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на само за читање.</span><span class="sxs-lookup"><span data-stu-id="8f357-152">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="8f357-153">Да бисте унели измене у план пројекта, потребно је да их направите у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да их објавите као исправке за функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-153">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="8f357-154">Уредите пројекат који је увезен</span><span class="sxs-lookup"><span data-stu-id="8f357-154">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="8f357-155">Да бисте унели промене у план пројекта који је увезен у функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], имате две опције:</span><span class="sxs-lookup"><span data-stu-id="8f357-155">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="8f357-156">Отворите главну датотеку и измените је у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-156">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="8f357-157">Опозовите везу датотеке и уредите је директно у функцији Project Service.</span><span class="sxs-lookup"><span data-stu-id="8f357-157">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="8f357-158">Подразумевано, пројекат који је био отпремљен из програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] је закључан и може се уређивати само у функцији Project.</span><span class="sxs-lookup"><span data-stu-id="8f357-158">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="8f357-159">Да бисте уредили датотеку у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], потребно је опозвати везу датотеке.</span><span class="sxs-lookup"><span data-stu-id="8f357-159">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="8f357-160">Уређивање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="8f357-160">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="8f357-161">У главном менију кликните на **Project Service** > **Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="8f357-161">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="8f357-162">Са листе пројеката отворите онај који сте креирали у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-162">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="8f357-163">Кликните на дугме **Отвори у програму MS Project** са траке.</span><span class="sxs-lookup"><span data-stu-id="8f357-163">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="8f357-164">То ће отворити повезану главну датотеку у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-164">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="8f357-165">Раскините везу датотеке и уредите је у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span><span class="sxs-lookup"><span data-stu-id="8f357-165">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="8f357-166">У главном менију кликните на **Project Service** > **Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="8f357-166">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="8f357-167">Са листе пројеката отворите онај који сте креирали у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-167">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="8f357-168">Кликните на дугме **Раскини везу са програмом MS Project** са траке.</span><span class="sxs-lookup"><span data-stu-id="8f357-168">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="8f357-169">Отпремање датотеке пројекта у SharePoint или Office групе</span><span class="sxs-lookup"><span data-stu-id="8f357-169">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="8f357-170">Датотеку пројекта можете да отпремите у SharePoint и да је пронађете у оквиру опције „Повезани документи“ за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.</span><span class="sxs-lookup"><span data-stu-id="8f357-170">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="8f357-171">Администратор мора да конфигурише SharePoint управљање документима и да га укључите за ентитет Пројекат.</span><span class="sxs-lookup"><span data-stu-id="8f357-171">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> 

 <span data-ttu-id="8f357-172">Можете и да отпремите датотеку пројекта у [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] ако имате подешену опцију Office групе.</span><span class="sxs-lookup"><span data-stu-id="8f357-172">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span>

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="8f357-173">Отпремање датотеке за SharePoint</span><span class="sxs-lookup"><span data-stu-id="8f357-173">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="8f357-174">У главном менију кликните на **Project Service** > **Отпреми**.</span><span class="sxs-lookup"><span data-stu-id="8f357-174">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="8f357-175">Изаберите **У документа пројекта Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="8f357-175">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="8f357-176">У дијалогу **Омогући отварање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изаберите **Да** или **Не**.</span><span class="sxs-lookup"><span data-stu-id="8f357-176">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="8f357-177">Ако кликнете на **Да**, моћи ћете да изаберете дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** у решењу Project Service Automation, да покренете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и учитате датотеку пројекта из SharePoint библиотеке докумената.</span><span class="sxs-lookup"><span data-stu-id="8f357-177">If you click **Yes**, you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="8f357-178">Ако кликнете на **Не**, веза за дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** неће радити.</span><span class="sxs-lookup"><span data-stu-id="8f357-178">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="8f357-179">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотеку можете да пронађете у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у оквиру опције **Документи** за одређени [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.</span><span class="sxs-lookup"><span data-stu-id="8f357-179">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="8f357-180">Отпремање датотеке за Office групе</span><span class="sxs-lookup"><span data-stu-id="8f357-180">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="8f357-181">У главном менију кликните на **Project Service** > **Отпреми**.</span><span class="sxs-lookup"><span data-stu-id="8f357-181">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="8f357-182">Изаберите **У документа пројекта Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="8f357-182">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="8f357-183">У дијалогу **Омогући отварање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изаберите **Да** или **Не**.</span><span class="sxs-lookup"><span data-stu-id="8f357-183">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="8f357-184">Ако кликнете на **Да**, моћи ћете да изаберете дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** у решењу Project Service Automation, да покренете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и учитате датотеку пројекта из SharePoint библиотеке докумената.</span><span class="sxs-lookup"><span data-stu-id="8f357-184">If you click **Yes**, you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="8f357-185">Ако кликнете на **Не**, веза за дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** неће радити.</span><span class="sxs-lookup"><span data-stu-id="8f357-185">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="8f357-186">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотеку можете да пронађете у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у оквиру опције **Документи** за одређени [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.</span><span class="sxs-lookup"><span data-stu-id="8f357-186">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="8f357-187">Објавите своје пројекте као предложак</span><span class="sxs-lookup"><span data-stu-id="8f357-187">Publish  your project as a template</span></span>  
 <span data-ttu-id="8f357-188">Можете да сачувате ваш пројекат и да га поново употребите тако што ћете га сачувати ка предложак пројекта у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-188">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="8f357-189">Предлошци пројеката су планови пројекта који могу поново да се користе у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-189">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="8f357-190">[Креирање предлошка за пројекат (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="8f357-190">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1. <span data-ttu-id="8f357-191">Са картице **Project Service** кликните на дугме **Објави** > **Нови Project Service Automation шаблон пројекта**.</span><span class="sxs-lookup"><span data-stu-id="8f357-191">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="8f357-192">У дијалогу **Објави у нови пројекат у предлошку Project Service** унесите **Име предлошка пројекта**.</span><span class="sxs-lookup"><span data-stu-id="8f357-192">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="8f357-193">Опционално означите **Повежи план пројекта са функцијом Project Service Automation** да бисте повезали датотеку пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-193">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="8f357-194">Изаберите дугме **Објави**</span><span class="sxs-lookup"><span data-stu-id="8f357-194">Click **Publish**.</span></span>  

<span data-ttu-id="8f357-195">Повезивање датотеке пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] од датотеке пројекта прави главну датотеку и подешава структурну анализу посла у предлошку за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на само за читање.</span><span class="sxs-lookup"><span data-stu-id="8f357-195">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="8f357-196">Да бисте унели измене у план пројекта, потребно је да их направите у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да их објавите као исправке за функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="8f357-196">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="8f357-197">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="8f357-197">See Also</span></span>  
 [<span data-ttu-id="8f357-198">Водич за менаџера пројекта</span><span class="sxs-lookup"><span data-stu-id="8f357-198">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
