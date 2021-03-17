---
title: Како прилагођавате ток пословног процеса за фазе пројекта?
description: Преглед начина прилагођавања тока пословног процеса за фазе пројекта.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
author: JohnPBurrows
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0f95677c56b745bf7900ad503596c93f1e722281
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286176"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="cd21d-103">Како прилагођавате ток пословног процеса за фазе пројекта?</span><span class="sxs-lookup"><span data-stu-id="cd21d-103">How do I customize the Project Stages business process flow?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="cd21d-104">Постоји познато ограничење у ранијим верзијама апликације Project Service да имена фаза у току пословног процеса за фазе пројекта морају бити потпуно иста са очекиваним енглеским именима (**Quote**, **Plan**, **Close**).</span><span class="sxs-lookup"><span data-stu-id="cd21d-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="cd21d-105">У супротном, пословна логика, која се ослања на енглеско име фазе, не ради како је очекивано.</span><span class="sxs-lookup"><span data-stu-id="cd21d-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="cd21d-106">Зато не видите да су познате радње, као што су **Пребаци процес** или **Уреди процес** доступне у обрасцу пројекта, а прилагођавање тока пословног процеса се не подстиче.</span><span class="sxs-lookup"><span data-stu-id="cd21d-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="cd21d-107">Ово ограничење је отклоњено у верзији 2.4.5.48 и новијим.</span><span class="sxs-lookup"><span data-stu-id="cd21d-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="cd21d-108">У овом чланку дата су предложена заобилазна решења уколико морате да прилагодите подразумевани ток пословног процеса за старије верзије.</span><span class="sxs-lookup"><span data-stu-id="cd21d-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="cd21d-109">Пословна логика захтева потпуно подударање са енглеским именима фазе</span><span class="sxs-lookup"><span data-stu-id="cd21d-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="cd21d-110">Ток пословног процеса за фазе пројекта садржи пословну логику која управља следећим понашањима у апликацији:</span><span class="sxs-lookup"><span data-stu-id="cd21d-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="cd21d-111">Када је пројекат повезан са понудом, кôд поставља ток пословног процеса на фазу **Quote**.</span><span class="sxs-lookup"><span data-stu-id="cd21d-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="cd21d-112">Када је пројекат повезан са контактом, кôд поставља ток пословног процеса на фазу **Plan**.</span><span class="sxs-lookup"><span data-stu-id="cd21d-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="cd21d-113">Када је ток пословног процеса напредовао до фазе **Close**, запис пројекат се деактивира.</span><span class="sxs-lookup"><span data-stu-id="cd21d-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="cd21d-114">Када је пројекат деактивиран, образац пројекта и структурна анализа посла (САП) су подешени на само за читање, резервације именованог ресурса се укидају и сви повезани ценовници се деактивирају.</span><span class="sxs-lookup"><span data-stu-id="cd21d-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="cd21d-115">Ова пословна логика се ослања имена на енглеском језику за фазе пројекта.</span><span class="sxs-lookup"><span data-stu-id="cd21d-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="cd21d-116">Ова зависност од имена на енглеском језику представља главни разлог зашто се не подстиче прилагођавање тока пословног процеса за фазе пројекта, као и зашто не видите уобичајене радње тока пословног процеса као што су **Пребаци процес** или **Уреди процес** у ентитету Пројекат.</span><span class="sxs-lookup"><span data-stu-id="cd21d-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="cd21d-117">Шта се догађа ако се имена фаза не подударају са именима на енглеском?</span><span class="sxs-lookup"><span data-stu-id="cd21d-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="cd21d-118">У апликацији Project Service, верзија 1.x на платформи 8.2, када се имена фаза у току пословног процеса не подударају тачно са енглеским именима за фазе, прескаче се пословна логика која подешава прави фазу за понуде или уговоре или која затвара пројекат.</span><span class="sxs-lookup"><span data-stu-id="cd21d-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="cd21d-119">Неће се приказивати поруке о грешци.</span><span class="sxs-lookup"><span data-stu-id="cd21d-119">No error messages are displayed.</span></span> <span data-ttu-id="cd21d-120">Због тога делује да можете да прилагодите ток пословног процеса за фазе пројекта.</span><span class="sxs-lookup"><span data-stu-id="cd21d-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="cd21d-121">Међутим, нећете видети да иједан аутоматски процес функционише за понуде, уговоре и затварање пројекта.</span><span class="sxs-lookup"><span data-stu-id="cd21d-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="cd21d-122">У апликацији Project Service, верзија 2.4.4.30 или ранија на платформи 9.0, дошло је до значајне архитектонске промене токова пословних процеса, што је захтевало поновно писање пословне логике тока пословног процеса.</span><span class="sxs-lookup"><span data-stu-id="cd21d-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="cd21d-123">Као последица тога, ако се имена фазе процеса не подударају са очекиваним именима на енглеском језику, примићете поруку о грешци.</span><span class="sxs-lookup"><span data-stu-id="cd21d-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="cd21d-124">Стога, ако желите да прилагодите ток пословног процеса за фазе пројекта за ентитет пројекта, можете само да додате потпуно нове фазе у подразумевани ток пословног процеса за ентитет пројекта задржавајући фазе **Понуда**, **План** и **Затвори** непромењене.</span><span class="sxs-lookup"><span data-stu-id="cd21d-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="cd21d-125">Ово ограничење осигурава да не добијате грешке од пословне логике која очекује имена на енглеском језику у току пословног процеса.</span><span class="sxs-lookup"><span data-stu-id="cd21d-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="cd21d-126">У верзији 2.4.5.48 или новијој, пословна логика описана у овом чланку је уклоњена из подразумеваног тока пословног процеса за ентитет пројекта.</span><span class="sxs-lookup"><span data-stu-id="cd21d-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="cd21d-127">Надоградња на ту верзију или каснију ће вам омогућити да прилагодите или замените подразумевани ток пословног процеса сопственим.</span><span class="sxs-lookup"><span data-stu-id="cd21d-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="cd21d-128">Заобилазна решења за раније верзије</span><span class="sxs-lookup"><span data-stu-id="cd21d-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="cd21d-129">Ако надоградња не представља опцију, можете да прилагодите ток пословног процеса за фазе пројекта за ентитет пројекта на један од ова два начина:</span><span class="sxs-lookup"><span data-stu-id="cd21d-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="cd21d-130">Додајте додатне фазе подразумеваној конфигурацији истовремено задржавајући енглеска имена фаза за опције **Понуда**, **План** и **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="cd21d-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>


![Снимак екрана за додавање фаза подразумеваној конфигурацији](media/FAQ-Customize-BPF-1.png)
 
2. <span data-ttu-id="cd21d-132">Креирајте сопствени ток пословног процеса и нека он буде ваш примарни ток пословног процеса за ентитет пројекта, што вам омогућава да имате било која имена фазе по жељи.</span><span class="sxs-lookup"><span data-stu-id="cd21d-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="cd21d-133">Међутим, ако желите да користите исте стандардне фазе пројекта **Понуда**, **План** и **Затвори**, потребно је да извршите још нека прилагођавања која се покрећу на основу ваших прилагођених имена за фазе.</span><span class="sxs-lookup"><span data-stu-id="cd21d-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="cd21d-134">Сложенија логика се налази у затварању пројекта, коју и даље можете да покрећете простим деактивирањем записа пројекта.</span><span class="sxs-lookup"><span data-stu-id="cd21d-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

![BPF прилагођавање](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="cd21d-136">Додатна разматрања за апликацију Project Service, верзија 2.4.4.30 или раније на платформи 9.0</span><span class="sxs-lookup"><span data-stu-id="cd21d-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="cd21d-137">У апликацији Project Service 2.4.4.30 или ранијој на платформи 9.0, са прилагођеним током пословног процеса, поље **Име фазе** у ентитету Пројекат којег користи графикон **Пројеката према фази** и приказ листе пројекта се неће исправљати, јер су повезани са током пословног процеса за подразумеване фазе пројекта.</span><span class="sxs-lookup"><span data-stu-id="cd21d-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="cd21d-138">Овај проблем можете да решите са следећим корацима:</span><span class="sxs-lookup"><span data-stu-id="cd21d-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="cd21d-139">Додајте прилагођено поље да бисте прибележили тренутну фазу тока пословног процеса која се ажурира како корисник прилази кроз прилагођени ток пословног процеса.</span><span class="sxs-lookup"><span data-stu-id="cd21d-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="cd21d-140">Измените графикон **Пројекат према фази** како бисте радили са прилагођеним пољем уместо са подразумеваном конфигурацијом.</span><span class="sxs-lookup"><span data-stu-id="cd21d-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="cd21d-141">Кораци за креирање сопственог тока пословног процеса за ентитет пројекта</span><span class="sxs-lookup"><span data-stu-id="cd21d-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="cd21d-142">Поступите на следећи начин да бисте креирали сопствени ток пословног процеса за ентитет пројекта:</span><span class="sxs-lookup"><span data-stu-id="cd21d-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="cd21d-143">Идите на ставку **Подешавања** > **Центар за процесе**.</span><span class="sxs-lookup"><span data-stu-id="cd21d-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="cd21d-144">Немојте да копирате ток пословног пројекта за фазе пројекта јер то копира и пословну логику апликације Project Service.</span><span class="sxs-lookup"><span data-stu-id="cd21d-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

  ![Креирај процес](media/FAQ-Customize-BPF-3.png)

2. <span data-ttu-id="cd21d-146">Користите дизајнер процеса за креирање жељених имена за фазе.</span><span class="sxs-lookup"><span data-stu-id="cd21d-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="cd21d-147">Ако желите исту функционалност као подразумеване фазе за ставке **Понуда**, **План** и **Затвори**, мораћете да је креирате на основу имена за фазе прилагођеног тока пословног процеса.</span><span class="sxs-lookup"><span data-stu-id="cd21d-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   ![Снимак екрана дизајнера процеса који се користи за прилагођавање BPF](media/FAQ-Customize-BPF-4.png) 

3. <span data-ttu-id="cd21d-149">У дизајнеру процеса, кликните на ставку **Редослед тока процеса** како би прилагођени ток пословног процеса постао примарни ток пословног процеса за ентитет пројекта његовим премештањем изнад тока пословног процеса за фазе пројекта на врх листе.</span><span class="sxs-lookup"><span data-stu-id="cd21d-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>


   [<span data-ttu-id="cd21d-150">Снимак екрана коришћења Редоследа тока процеса</span><span class="sxs-lookup"><span data-stu-id="cd21d-150">Screenshot of using Order Process Flow</span></span>](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="cd21d-151">Следећи кораци се примењују на апликацију Project Service 2.4.4.30 или ранију на платформи 9.0</span><span class="sxs-lookup"><span data-stu-id="cd21d-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="cd21d-152">Додајте ново прилагођено поље у ентитет пројекта да бисте прибележили прилагођене фазе у свом прилагођеном току пословног процеса.</span><span class="sxs-lookup"><span data-stu-id="cd21d-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="cd21d-153">Потребно је да додате пословну логику (додатну компоненту/ток посла) да бисте исправили ово поље када се исправља фаза у прилагођеном току пословног процеса.</span><span class="sxs-lookup"><span data-stu-id="cd21d-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   ![Снимак екрана за прилагођавање ентитета Пројекат](media/FAQ-Customize-BPF-6-720.png)

5. <span data-ttu-id="cd21d-155">Измените графикон **Пројекат према фази** да бисте користили ново прилагођено поље за фазе.</span><span class="sxs-lookup"><span data-stu-id="cd21d-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   ![Снимак екрана коришћења графикона Пројекат према фази](media/FAQ-Customize-BPF-7-720.png)

6. <span data-ttu-id="cd21d-157">Измените све приказе за ентитет Пројекат да бисте обухватили ново прилагођено поље за фазе.</span><span class="sxs-lookup"><span data-stu-id="cd21d-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   ![Снимак екрана измене приказа у ентитету Пројекат](media/FAQ-Customize-BPF-8-720.png)



[!INCLUDE[footer-include](../includes/footer-banner.md)]