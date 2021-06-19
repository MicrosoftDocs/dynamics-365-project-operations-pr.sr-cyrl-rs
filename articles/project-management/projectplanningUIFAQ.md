---
title: Решавање проблема са радом у мрежи података
description: Ова тема пружа информације о решавању проблема потребне за рад у мрежи задатака.
author: ruhercul
ms.date: 01/19/2021
ms.topic: article
ms.product: ''
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a15a4752de7537b3f60d5ee3269c846257a1fe4a
ms.sourcegitcommit: 72fa1f09fe406805f7009fc68e2f3eeeb9b7d5fc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/09/2021
ms.locfileid: "6213418"
---
# <a name="troubleshoot-working-in-the-task-grid"></a><span data-ttu-id="e304d-103">Решавање проблема са радом у мрежи података</span><span class="sxs-lookup"><span data-stu-id="e304d-103">Troubleshoot working in the Task grid</span></span> 

<span data-ttu-id="e304d-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="e304d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e304d-105">Ова тема описује како да решите проблеме на које бисте могли наићи током рада са управљањем трошковима.</span><span class="sxs-lookup"><span data-stu-id="e304d-105">This topic describes how to fix issues that you might encounter while working with cost management.</span></span>

## <a name="enable-cookies"></a><span data-ttu-id="e304d-106">Омогућавање колачића</span><span class="sxs-lookup"><span data-stu-id="e304d-106">Enable cookies</span></span>

<span data-ttu-id="e304d-107">Project Operations захтева да независни колачићи буду омогућени како би се приказивала структурна анализа посла.</span><span class="sxs-lookup"><span data-stu-id="e304d-107">Project Operations requires that third-party cookies be enabled in order to render the work breakdown structure.</span></span> <span data-ttu-id="e304d-108">Када независни колачићи нису омогућени, уместо да видите задатке, видећете празну страницу када одаберете картицу **Задаци** на страници **Пројекат**.</span><span class="sxs-lookup"><span data-stu-id="e304d-108">When third-party cookies aren't enabled, instead of seeing tasks, you will see a blank page when you select the **Tasks** tab on the **Project** page.</span></span>

![Празна картица када независни колачићи нису омогућени](media/blankschedule.png)


### <a name="workaround"></a><span data-ttu-id="e304d-110">Заобилазно решење</span><span class="sxs-lookup"><span data-stu-id="e304d-110">Workaround</span></span>
<span data-ttu-id="e304d-111">За прегледаче Microsoft Edge или Google Chrome, следећи поступци описују како да ажурирате подешавања прегледача како бисте омогућили независне колачиће.</span><span class="sxs-lookup"><span data-stu-id="e304d-111">For Microsoft Edge or Google Chrome browsers, the following procedures outline how to update your browser setting to enable third-party cookies.</span></span>

#### <a name="microsoft-edge"></a><span data-ttu-id="e304d-112">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e304d-112">Microsoft Edge</span></span>

1. <span data-ttu-id="e304d-113">Отворите прегледач Edge.</span><span class="sxs-lookup"><span data-stu-id="e304d-113">Open your Edge browser.</span></span>
2. <span data-ttu-id="e304d-114">У горњем десном углу изаберите **три тачке** (...), а затим изаберите **Подешавања**.</span><span class="sxs-lookup"><span data-stu-id="e304d-114">In the upper-right corner, select the **ellipsis** (...), and then select **Settings**.</span></span>
3. <span data-ttu-id="e304d-115">У делу **Колачићи и дозволе за локације** изаберите **Колачићи и подаци о локацијама**.</span><span class="sxs-lookup"><span data-stu-id="e304d-115">Under **Cookies and site permissions**, select **Cookies and site data**.</span></span>
4. <span data-ttu-id="e304d-116">Искључите **Блокирај колачиће треће стране**.</span><span class="sxs-lookup"><span data-stu-id="e304d-116">Turn off **Block third-party cookies**.</span></span>

#### <a name="google-chrome"></a><span data-ttu-id="e304d-117">Google Chrome</span><span class="sxs-lookup"><span data-stu-id="e304d-117">Google Chrome</span></span>

1. <span data-ttu-id="e304d-118">Отворите прегледач Chrome.</span><span class="sxs-lookup"><span data-stu-id="e304d-118">Open your Chrome browser.</span></span>
2. <span data-ttu-id="e304d-119">У горњем десном углу изаберите три вертикалне тачке, а затим изаберите **Подешавања**.</span><span class="sxs-lookup"><span data-stu-id="e304d-119">In the upper-right corner, select the three vertical dots, and then select **Settings**.</span></span>
3. <span data-ttu-id="e304d-120">У делу **Приватност и безбедност** изаберите **Колачићи и други подаци о локацијама**.</span><span class="sxs-lookup"><span data-stu-id="e304d-120">Under **Privacy and security**, select **Cookies and other site data**.</span></span>
4. <span data-ttu-id="e304d-121">Изаберите **Дозволи све колачиће**.</span><span class="sxs-lookup"><span data-stu-id="e304d-121">Select **Allow all cookies**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e304d-122">Ако блокирате независне колачиће, сви колачићи и подаци о локацијама са других локација биће блокирани, чак и ако је локација дозвољена на листи изузетака.</span><span class="sxs-lookup"><span data-stu-id="e304d-122">If you block third-party cookies, all cookies and site data from other sites will be blocked, even if the site is allowed on your exceptions list.</span></span>

## <a name="pex-endpoint"></a><span data-ttu-id="e304d-123">PEX крајња тачка</span><span class="sxs-lookup"><span data-stu-id="e304d-123">PEX Endpoint</span></span>

<span data-ttu-id="e304d-124">Project Operations захтева да параметар пројекта упућује на PEX крајњу тачку.</span><span class="sxs-lookup"><span data-stu-id="e304d-124">Project Operations requires that a project parameter reference the PEX Endpoint.</span></span> <span data-ttu-id="e304d-125">Ова крајња тачка је потребан за комуникацију са услугом која се користи за приказивање структурне анализе посла.</span><span class="sxs-lookup"><span data-stu-id="e304d-125">This endpoint is required to communicate with the service used to render the work breakdown structure.</span></span> <span data-ttu-id="e304d-126">Ако параметар није омогућен, добићете грешку „Параметар пројекта није важећи“.</span><span class="sxs-lookup"><span data-stu-id="e304d-126">If the parameter isn't enabled, you will receive the error, "The project parameter is not valid".</span></span> 

### <a name="workaround"></a><span data-ttu-id="e304d-127">Заобилазно решење</span><span class="sxs-lookup"><span data-stu-id="e304d-127">Workaround</span></span>
 ![Поље „PEX крајња тачка“ у параметру пројекта](media/projectparameter.png)

1. <span data-ttu-id="e304d-129">Додајте поље **PEX крајња тачка** на страницу **Параметри пројекта**.</span><span class="sxs-lookup"><span data-stu-id="e304d-129">Add the **PEX Endpoint** field to the **Project Parameters** page.</span></span>
2. <span data-ttu-id="e304d-130">Ажурирајте поље следећом вредности: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=/<id>&type=2`</span><span class="sxs-lookup"><span data-stu-id="e304d-130">Update the field with the following value: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=/<id>&type=2`</span></span>
3. <span data-ttu-id="e304d-131">Уклоните поље са странице **Параметри пројекта**.</span><span class="sxs-lookup"><span data-stu-id="e304d-131">Remove the field from the **Project Parameters** page.</span></span>

## <a name="privileges-for-project-for-the-web"></a><span data-ttu-id="e304d-132">Привилегије за пројекат за веб</span><span class="sxs-lookup"><span data-stu-id="e304d-132">Privileges for Project for the Web</span></span>

<span data-ttu-id="e304d-133">Project Operations се ослања на екстерну услугу заказивања.</span><span class="sxs-lookup"><span data-stu-id="e304d-133">Project Operations relies on an external scheduling service.</span></span> <span data-ttu-id="e304d-134">Услуга захтева да корисник има неколико улога додељених за читање и писање у ентитете повезане са структурном анализом посла.</span><span class="sxs-lookup"><span data-stu-id="e304d-134">The service requires that a user have several roles assigned to read and write to entities related to the work breakdown structure.</span></span> <span data-ttu-id="e304d-135">Ти ентитети укључују пројектне задатке, додељивање ресурса и зависне елементе задатака.</span><span class="sxs-lookup"><span data-stu-id="e304d-135">These entities include project tasks, resource assignments, and task dependencies.</span></span> <span data-ttu-id="e304d-136">Ако корисник не може да прикаже структурну анализу посла када дође на картицу **Задаци**, то је вероватно зато што Project Operations није омогућен.</span><span class="sxs-lookup"><span data-stu-id="e304d-136">If a user can't render the work breakdown structure when they go to the **Tasks** tab, it's probably because Project for Project Operations hasn't been enabled.</span></span> <span data-ttu-id="e304d-137">Корисник може да добије грешку за безбедоносну улогу или грешку повезану са ускраћивањем приступа.</span><span class="sxs-lookup"><span data-stu-id="e304d-137">A user might receive either a security role error, or an error related to a denial of access.</span></span>


## <a name="workaround"></a><span data-ttu-id="e304d-138">Заобилазно решење</span><span class="sxs-lookup"><span data-stu-id="e304d-138">Workaround</span></span>

1. <span data-ttu-id="e304d-139">Идите на **Подешавања > Безбедност > Корисници > Корисници апликација**.</span><span class="sxs-lookup"><span data-stu-id="e304d-139">Go to **Setting > Security > Users > Application Users**.</span></span>  

   ![Читач апликације](media/applicationuser.jpg)
   
2. <span data-ttu-id="e304d-141">Двапут кликните на запис корисника апликације да бисте проверили следеће:</span><span class="sxs-lookup"><span data-stu-id="e304d-141">Double-click the application user record to verify the following:</span></span>

 - <span data-ttu-id="e304d-142">Корисник има приступ пројекту.</span><span class="sxs-lookup"><span data-stu-id="e304d-142">The user has access to the project.</span></span> <span data-ttu-id="e304d-143">Ова верификација се обично обавља тако што се осигурава да корисник има безбедносну улогу **Менаџер пројекта**.</span><span class="sxs-lookup"><span data-stu-id="e304d-143">This verification is typically done by ensuring that the user has **Project Manager** security role.</span></span>
 - <span data-ttu-id="e304d-144">Корисник апликације Microsoft Project постоји и правилно је конфигурисан.</span><span class="sxs-lookup"><span data-stu-id="e304d-144">The Microsoft Project application user exists and is configured correctly.</span></span>
 
3. <span data-ttu-id="e304d-145">Ако овај корисник не постоји, можете креирати запис новог корисника.</span><span class="sxs-lookup"><span data-stu-id="e304d-145">If this user doesn't exist, you can create a new user record.</span></span> <span data-ttu-id="e304d-146">Изаберите **Нови корисници**.</span><span class="sxs-lookup"><span data-stu-id="e304d-146">Select **New Users**.</span></span> <span data-ttu-id="e304d-147">Промените образац за унос у **Корисник апликације**, а затим додајте **ID апликације**.</span><span class="sxs-lookup"><span data-stu-id="e304d-147">Change the entry form to **Application User**, and then add the **Application ID**.</span></span>

   ![Детаљи о кориснику апликације](media/applicationuserdetails.jpg)

4. <span data-ttu-id="e304d-149">Проверите да ли је кориснику додељена исправна лиценца и да ли је услуга омогућена у детаљима планова услуге лиценце.</span><span class="sxs-lookup"><span data-stu-id="e304d-149">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
5. <span data-ttu-id="e304d-150">Проверите да ли корисник може да отвори project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="e304d-150">Verify that the user can open project.microsoft.com.</span></span>
6. <span data-ttu-id="e304d-151">Проверите кроз параметре пројекта да ли систем показује на исправну крајњу тачку пројекта.</span><span class="sxs-lookup"><span data-stu-id="e304d-151">Verify through the project parameters that the system is pointing to the correct project endpoint.</span></span>
7. <span data-ttu-id="e304d-152">Проверите да ли је креиран корисник пројектне апликације.</span><span class="sxs-lookup"><span data-stu-id="e304d-152">Verify that the project application user is created.</span></span>
8. <span data-ttu-id="e304d-153">Примените следеће безбедносне улоге на корисника:</span><span class="sxs-lookup"><span data-stu-id="e304d-153">Apply the following security roles to the user:</span></span>

  - <span data-ttu-id="e304d-154">Корисник услуге Dataverse</span><span class="sxs-lookup"><span data-stu-id="e304d-154">Dataverse User</span></span>
  - <span data-ttu-id="e304d-155">Project Operations систем</span><span class="sxs-lookup"><span data-stu-id="e304d-155">Project Operations System</span></span>
  - <span data-ttu-id="e304d-156">Пројектни систем</span><span class="sxs-lookup"><span data-stu-id="e304d-156">Project System</span></span>

## <a name="error-when-updating-the-work-breakdown-structure"></a><span data-ttu-id="e304d-157">Грешка при ажурирању структурне анализе посла</span><span class="sxs-lookup"><span data-stu-id="e304d-157">Error when updating the work breakdown structure</span></span>

<span data-ttu-id="e304d-158">Када се обави једно или више ажурирања структурне анализе посла, промене на крају не успеју и нису сачуване.</span><span class="sxs-lookup"><span data-stu-id="e304d-158">When one or more updates are made to the work breakdown structure, the changes eventually fail and aren't saved.</span></span> <span data-ttu-id="e304d-159">Долази до грешке у мрежи распореда уз напомену да „Недавна промена коју сте унели није могла бити сачувана“.</span><span class="sxs-lookup"><span data-stu-id="e304d-159">An error occurs in the schedule grid noting that “Recent change you’ve made couldn’t be saved.”</span></span>

### <a name="workaround"></a><span data-ttu-id="e304d-160">Заобилазно решење</span><span class="sxs-lookup"><span data-stu-id="e304d-160">Workaround</span></span>

1. <span data-ttu-id="e304d-161">Проверите да ли је кориснику додељена исправна лиценца и да ли је услуга омогућена у детаљима планова услуге лиценце.</span><span class="sxs-lookup"><span data-stu-id="e304d-161">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
2. <span data-ttu-id="e304d-162">Проверите да ли корисник може да отвори project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="e304d-162">Verify that the user can open project.microsoft.com.</span></span>
3. <span data-ttu-id="e304d-163">Проверите да ли систем показује на исправну крајњу тачку пројекта.</span><span class="sxs-lookup"><span data-stu-id="e304d-163">Verify that the system is pointing to the correct project endpoint,.</span></span>
4. <span data-ttu-id="e304d-164">Проверите да ли је креиран корисник пројектне апликације.</span><span class="sxs-lookup"><span data-stu-id="e304d-164">Verify that the Project Application user has been created.</span></span>
5. <span data-ttu-id="e304d-165">Примените следеће безбедносне улоге на корисника:</span><span class="sxs-lookup"><span data-stu-id="e304d-165">Apply the following security roles to the user:</span></span>
  
  - <span data-ttu-id="e304d-166">Dataverse корисник или основни корисник</span><span class="sxs-lookup"><span data-stu-id="e304d-166">Dataverse user or Base user</span></span>
  - <span data-ttu-id="e304d-167">Project Operations систем</span><span class="sxs-lookup"><span data-stu-id="e304d-167">Project Operations System</span></span>
  - <span data-ttu-id="e304d-168">Пројектни систем</span><span class="sxs-lookup"><span data-stu-id="e304d-168">Project System</span></span>
  - <span data-ttu-id="e304d-169">Project Operations систем двоструког уписивања (ова улога је потребна ако примењујете ресурс/сценарио који није заснован на залихама услуге Project Operations.)</span><span class="sxs-lookup"><span data-stu-id="e304d-169">Project Operations Dual Write System (This role is required if you are deploying the resource/non-stocked based scenario of Project Operations.)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
