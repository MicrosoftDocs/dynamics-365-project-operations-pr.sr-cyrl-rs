---
title: Додајте Azure претплату у LCS пројекат
description: Ова тема пружа информације о томе како да повежете своју Azure претплату са LCS пројектом.
author: sigitac
manager: Annbe
ms.date: 04/12/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a80c926ba67a1620e39d8c7677a05678454e6340
ms.sourcegitcommit: 7468d668c48c1d87934aab9a034decd51e56dec6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/13/2021
ms.locfileid: "5880556"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="83190-103">Додајте Azure претплату у LCS пројекат</span><span class="sxs-lookup"><span data-stu-id="83190-103">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="83190-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="83190-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="83190-105">Окружења у хосту у облаку морају се применити помоћу постојеће Azure претплате.</span><span class="sxs-lookup"><span data-stu-id="83190-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="83190-106">Ова тема објашњава како да повежете своју постојећу Azure претплату са LCS пројектом.</span><span class="sxs-lookup"><span data-stu-id="83190-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="83190-107">Дајте пристанак администратора</span><span class="sxs-lookup"><span data-stu-id="83190-107">Grant admin consent</span></span>

1. <span data-ttu-id="83190-108">У вашем LCS пројекту, у одељку **Окружења**, изаберите **Microsoft Azure подешавања**.</span><span class="sxs-lookup"><span data-stu-id="83190-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![Подешавања програма Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="83190-110">На страници **Подешавања пројекта**, на картици **Azure конектори**, изаберите **Одобри**.</span><span class="sxs-lookup"><span data-stu-id="83190-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="83190-111">То омогућава да се окружења примене на овај пројекат.</span><span class="sxs-lookup"><span data-stu-id="83190-111">This allows environments to be deployed to this project.</span></span>

![Azure конектори](./media/2AzureConnectors.png)

3. <span data-ttu-id="83190-113">Поново изаберите **Одобри** да бисте пружили пристанак администратора.</span><span class="sxs-lookup"><span data-stu-id="83190-113">Select **Authorize** again to provide admin consent.</span></span>

![Дајте пристанак администратора](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="83190-115">Прихватите захтев за дозволе.</span><span class="sxs-lookup"><span data-stu-id="83190-115">Accept the permissions request.</span></span>

![Прихватите захтев за дозволе](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="83190-117">Овлашћење је сада завршено.</span><span class="sxs-lookup"><span data-stu-id="83190-117">The authorization is now complete.</span></span> 

![Одобрење је успешно](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="83190-119">Омогућите приступ услуге Dynamics Deployment Services вашој Azure претплати</span><span class="sxs-lookup"><span data-stu-id="83190-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="83190-120">Идите на [Microsoft Azure обрачун](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) и изаберите своју претплату.</span><span class="sxs-lookup"><span data-stu-id="83190-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="83190-121">Услуга Dynamics Deployment Services треба да приступи овој претплати да би могла да примени окружења.</span><span class="sxs-lookup"><span data-stu-id="83190-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![Детаљи претплате на услугу Azure](./media/6AzureSubscription.png)

2. <span data-ttu-id="83190-123">Изаберите **Контрола приступа (IAM)** у окну за навигацију, а затим изаберите **Додајте додељивање улога**.</span><span class="sxs-lookup"><span data-stu-id="83190-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="83190-124">У клизачу са десне стране изаберите **Улога сарадника** и на приложеној листи пронађите и изаберите **Dynamics Deployment Services**.</span><span class="sxs-lookup"><span data-stu-id="83190-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="83190-125">Изаберите ставку **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="83190-125">Select **Save**.</span></span>

![Приступ претплати](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="83190-127">Додавање конектора за претплату у LCS пројекат</span><span class="sxs-lookup"><span data-stu-id="83190-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="83190-128">У вашем LCS пројекту, на страници **Microsoft Azure подешавања** изаберите **Додај** да бисте додали нови конектор.</span><span class="sxs-lookup"><span data-stu-id="83190-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="83190-129">Унесите свој ID Azure претплате.</span><span class="sxs-lookup"><span data-stu-id="83190-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="83190-130">ID Azure претплате можете пронаћи у [Azure порталу](https://ms.portal.azure.com/), у одељку  **Подешавања**  у доњем левом углу екрана.</span><span class="sxs-lookup"><span data-stu-id="83190-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="83190-131">У пољу **Конфигуриши да се користи Azure Resource Manager**, изаберите **Да**.</span><span class="sxs-lookup"><span data-stu-id="83190-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="83190-132">Уверите се да се Azure домен закупца AAD претплате подудара са Azure претплатом у власништву домена коју користите, па изаберите **Следећи**.</span><span class="sxs-lookup"><span data-stu-id="83190-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="83190-133">На екрану **Microsoft Azure подешавање**, изаберите **Следећи** за потврду.</span><span class="sxs-lookup"><span data-stu-id="83190-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="83190-134">Ако на овом екрану добијете грешку, вратите се у одељак [Омогућите приступ услузи Dynamics Deployment Services у Azure претплату](#provide) у овој теми и уверите се да сте завршили све кораке.</span><span class="sxs-lookup"><span data-stu-id="83190-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="83190-135">Преузмите Azure цертификат за управљање у локалну фасциклу на рачунару.</span><span class="sxs-lookup"><span data-stu-id="83190-135">Download the Azure Management Certificate to a local folder on your computer.</span></span> <span data-ttu-id="83190-136">Замолите администратора претплате за Azure да отпреми сертификат на портал за управљање услугом Azure тако што ће одабрати претплату и отићи на **Подешавања** > **Сертификати о управљању**.</span><span class="sxs-lookup"><span data-stu-id="83190-136">Ask your Azure subscription administrator to upload the certificate to Azure Management Portal by selecting the subscription and going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="83190-137">Овај сертификат омогућава LCS-у да у ваше име комуницира са услугом Azure.</span><span class="sxs-lookup"><span data-stu-id="83190-137">This certificate enables LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="83190-138">Овај корак можете прескочити ако ваш корисник има приступ претплати.</span><span class="sxs-lookup"><span data-stu-id="83190-138">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="83190-139">Изаберите **Следеће**.</span><span class="sxs-lookup"><span data-stu-id="83190-139">Select  **Next**.</span></span>
8. <span data-ttu-id="83190-140">Изаберите Azure регион за примену и изаберите центар података који је близу места где планирате да користите овај систем.</span><span class="sxs-lookup"><span data-stu-id="83190-140">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="83190-141">Изаберите **Повежи се**.</span><span class="sxs-lookup"><span data-stu-id="83190-141">Select  **Connect**.</span></span>

<span data-ttu-id="83190-142">Успешно сте повезали своју Azure претплату.</span><span class="sxs-lookup"><span data-stu-id="83190-142">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="83190-143">Сада можете да примените Dynamics 365 Finance окружења хостована у облаку.</span><span class="sxs-lookup"><span data-stu-id="83190-143">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
