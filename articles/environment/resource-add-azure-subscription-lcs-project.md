---
title: Додајте Azure претплату у LCS пројекат
description: Ова тема пружа информације о томе како да повежете своју Azure претплату са LCS пројектом.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0b5703542ac58adcc710890d9676dd0090a82f25
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949061"
---
# <a name="add-an-azure-subscription-to-lcs-project"></a><span data-ttu-id="466d1-103">Додајте Azure претплату у LCS пројекат</span><span class="sxs-lookup"><span data-stu-id="466d1-103">Add an Azure subscription to LCS project</span></span>

<span data-ttu-id="466d1-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="466d1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="466d1-105">Окружења у хосту у облаку морају се применити помоћу постојеће Azure претплате.</span><span class="sxs-lookup"><span data-stu-id="466d1-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="466d1-106">Ова тема објашњава како да повежете своју постојећу Azure претплату са LCS пројектом.</span><span class="sxs-lookup"><span data-stu-id="466d1-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="466d1-107">Дајте пристанак администратора</span><span class="sxs-lookup"><span data-stu-id="466d1-107">Grant admin consent</span></span>

1. <span data-ttu-id="466d1-108">У вашем LCS пројекту, у одељку **Окружења**, изаберите **Microsoft Azure подешавања**.</span><span class="sxs-lookup"><span data-stu-id="466d1-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![Подешавања програма Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="466d1-110">На страници **Подешавања пројекта**, на картици **Azure конектори**, изаберите **Одобри**.</span><span class="sxs-lookup"><span data-stu-id="466d1-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="466d1-111">То омогућава да се окружења примене на овај пројекат.</span><span class="sxs-lookup"><span data-stu-id="466d1-111">This allows environments to be deployed to this project.</span></span>

![Azure конектори](./media/2AzureConnectors.png)

3. <span data-ttu-id="466d1-113">Поново изаберите **Одобри** да бисте пружили пристанак администратора.</span><span class="sxs-lookup"><span data-stu-id="466d1-113">Select **Authorize** again to provide admin consent.</span></span>

![Дајте пристанак администратора](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="466d1-115">Прихватите захтев за дозволе.</span><span class="sxs-lookup"><span data-stu-id="466d1-115">Accept the permissions request.</span></span>

![Прихватите захтев за дозволе](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="466d1-117">Овлашћење је сада завршено.</span><span class="sxs-lookup"><span data-stu-id="466d1-117">The authorization is now complete.</span></span> 

![Одобрење је успешно](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="466d1-119">Омогућите приступ услуге Dynamics Deployment Services вашој Azure претплати</span><span class="sxs-lookup"><span data-stu-id="466d1-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="466d1-120">Идите на [Microsoft Azure обрачун](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) и изаберите своју претплату.</span><span class="sxs-lookup"><span data-stu-id="466d1-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="466d1-121">Услуга Dynamics Deployment Services треба да приступи овој претплати да би могла да примени окружења.</span><span class="sxs-lookup"><span data-stu-id="466d1-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![Детаљи претплате на услугу Azure](./media/6AzureSubscription.png)

2. <span data-ttu-id="466d1-123">Изаберите **Контрола приступа (IAM)** у окну за навигацију, а затим изаберите **Додајте додељивање улога**.</span><span class="sxs-lookup"><span data-stu-id="466d1-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="466d1-124">У клизачу са десне стране изаберите **Улога сарадника** и на приложеној листи пронађите и изаберите **Dynamics Deployment Services**.</span><span class="sxs-lookup"><span data-stu-id="466d1-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="466d1-125">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="466d1-125">Select **Save**.</span></span>

![Приступ претплати](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="466d1-127">Додавање конектора за претплату у LCS пројекат</span><span class="sxs-lookup"><span data-stu-id="466d1-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="466d1-128">У вашем LCS пројекту, на страници **Microsoft Azure подешавања** изаберите **Додај** да бисте додали нови конектор.</span><span class="sxs-lookup"><span data-stu-id="466d1-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="466d1-129">Унесите свој ID Azure претплате.</span><span class="sxs-lookup"><span data-stu-id="466d1-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="466d1-130">ID Azure претплате можете пронаћи у [Azure порталу](https://ms.portal.azure.com/), у одељку  **Подешавања**  у доњем левом углу екрана.</span><span class="sxs-lookup"><span data-stu-id="466d1-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="466d1-131">У пољу **Конфигуриши да се користи Azure Resource Manager**, изаберите **Да**.</span><span class="sxs-lookup"><span data-stu-id="466d1-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="466d1-132">Уверите се да се Azure домен закупца AAD претплате подудара са Azure претплатом у власништву домена коју користите, па изаберите **Следећи**.</span><span class="sxs-lookup"><span data-stu-id="466d1-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="466d1-133">На екрану **Microsoft Azure подешавање**, изаберите **Следећи** за потврду.</span><span class="sxs-lookup"><span data-stu-id="466d1-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="466d1-134">Ако на овом екрану добијете грешку, вратите се у одељак [Омогућите приступ услузи Dynamics Deployment Services у Azure претплату](#provide) у овој теми и уверите се да сте завршили све кораке.</span><span class="sxs-lookup"><span data-stu-id="466d1-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="466d1-135">Преузмите Azure цертификат за управљање у локалну фасциклу на рачунару, а затим га отпремите на портал за управљање услугом Azure тако што ћете отићи на **Подешавања** > **Сертификати о управљању**.</span><span class="sxs-lookup"><span data-stu-id="466d1-135">Download the Azure Management Certificate to a local folder on your computer, and then upload it to Azure Management Portal by going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="466d1-136">Овај цертификат ће омогућити LCS да комуницира са платформом Azure у ваше име.</span><span class="sxs-lookup"><span data-stu-id="466d1-136">This certificate will enable LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="466d1-137">Овај корак можете прескочити ако ваш корисник има приступ претплати.</span><span class="sxs-lookup"><span data-stu-id="466d1-137">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="466d1-138">Изаберите **Следеће**.</span><span class="sxs-lookup"><span data-stu-id="466d1-138">Select  **Next**.</span></span>
8. <span data-ttu-id="466d1-139">Изаберите Azure регион за примену и изаберите центар података који је близу места где планирате да користите овај систем.</span><span class="sxs-lookup"><span data-stu-id="466d1-139">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="466d1-140">Изаберите **Повежи се**.</span><span class="sxs-lookup"><span data-stu-id="466d1-140">Select  **Connect**.</span></span>

<span data-ttu-id="466d1-141">Успешно сте повезали своју Azure претплату.</span><span class="sxs-lookup"><span data-stu-id="466d1-141">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="466d1-142">Сада можете да примените Dynamics 365 Finance окружења хостована у облаку.</span><span class="sxs-lookup"><span data-stu-id="466d1-142">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>


