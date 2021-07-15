---
title: Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха
description: Ова тема пружа информације о начину претплате и примене услуге Project Operations за сценарије засноване на ресурсима / без залиха.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: da93fcf23ee3f255812842e31cb22b5d39daa963
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334845"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="61c6a-103">Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха</span><span class="sxs-lookup"><span data-stu-id="61c6a-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="61c6a-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="61c6a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="61c6a-105">Ова тема објашњава како да се претплатите на понуду пробне верзије и применити Project Operations окружење за сценарије засноване на ресурсима / без залиха.</span><span class="sxs-lookup"><span data-stu-id="61c6a-105">This topic explains how to subscribe to the trial offer and deploy Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61c6a-106">Предуслови</span><span class="sxs-lookup"><span data-stu-id="61c6a-106">Prerequisites</span></span>
- <span data-ttu-id="61c6a-107">Корисник који примени верзију за преглед мора да има глобална администраторска права у Azure закупцу.</span><span class="sxs-lookup"><span data-stu-id="61c6a-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="61c6a-108">Закупца можете креирати током првог искоришћавања понуде.</span><span class="sxs-lookup"><span data-stu-id="61c6a-108">You can create a tenant during the first offer redemption.</span></span> 
- <span data-ttu-id="61c6a-109">За примену Finance окружења потребна је важећа Azure претплата која ће се наплаћивати по окружењу.</span><span class="sxs-lookup"><span data-stu-id="61c6a-109">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="61c6a-110">Можете да користите постојећу претплату у својим организацијама или да користите [Azure пробну верзију](https://azure.microsoft.com/en-us/free/) да бисте започели.</span><span class="sxs-lookup"><span data-stu-id="61c6a-110">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="61c6a-111">CDS окружење ће бити бесплатно за ограничен период од 30 дана.</span><span class="sxs-lookup"><span data-stu-id="61c6a-111">The CDS environment will be provided free for a limited 30 day period.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="61c6a-112">Само једна особа, администратор закупца, у организацији треба да извршава овај задатак.</span><span class="sxs-lookup"><span data-stu-id="61c6a-112">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="61c6a-113">Ако нисте претплатник на ово издање, сачекајте док се ваша организација не региструје и не примите своје корисничке акредитиве.</span><span class="sxs-lookup"><span data-stu-id="61c6a-113">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="61c6a-114">Пробне верзије се користе једнократно у закупцу.</span><span class="sxs-lookup"><span data-stu-id="61c6a-114">Trials are single use in the tenant.</span></span> <span data-ttu-id="61c6a-115">Пробну верзију можете покренути само једном.</span><span class="sxs-lookup"><span data-stu-id="61c6a-115">You can only run a trial one time.</span></span> <span data-ttu-id="61c6a-116">Препоручујемо вам да креирате новог закупца у сврху пробне верзије.</span><span class="sxs-lookup"><span data-stu-id="61c6a-116">We recommend that you create a new tenant for the purpose of the trial.</span></span>


### <a name="dynamics-365-project-operations-ce---preview-trial"></a><span data-ttu-id="61c6a-117">Dynamics 365 Project Operations (CE) – Пробна верзија за преглед</span><span class="sxs-lookup"><span data-stu-id="61c6a-117">Dynamics 365 Project Operations (CE) - Preview Trial</span></span> 

<span data-ttu-id="61c6a-118">Пре него што започнете, уверите се да сте пријављени у прегледач са корисничким пословним налогом у закупцу где желите преглед услуге Project Operations.</span><span class="sxs-lookup"><span data-stu-id="61c6a-118">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="61c6a-119">Искористите прву шифру понуде, **Dynamics 365 Project Operations** овде [Project Operations пробна верзија](https://aka.ms/try-po).</span><span class="sxs-lookup"><span data-stu-id="61c6a-119">Redeem the first offer code, **Dynamics 365 Project Operations** here [Project Operations Trial](https://aka.ms/try-po).</span></span>
2. <span data-ttu-id="61c6a-120">Потврдите поруџбину.</span><span class="sxs-lookup"><span data-stu-id="61c6a-120">Confirm your order.</span></span>

  <span data-ttu-id="61c6a-121">Видећете да је понуда за потврду успешно искоришћена.</span><span class="sxs-lookup"><span data-stu-id="61c6a-121">You will see confirmation offer was successfully redeemed.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="61c6a-122">Dynamics 365 Finance пробна верзија за преглед</span><span class="sxs-lookup"><span data-stu-id="61c6a-122">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="61c6a-123">Идите на [пробну верзију за преглед услуге Dynamics 365 for Finance](https://aka.ms/trypoche) и поновите кораке из претходног одељка са понудом, Пријавите се за окружење које се хостује у облаку.</span><span class="sxs-lookup"><span data-stu-id="61c6a-123">Go to [Dynamics 365 for Finance Preview Trial](https://aka.ms/trypoche) and repeat the steps from the previous section with the offer, Sign up for the Cloud Hosted Environment.</span></span>  

## <a name="assign-licenses"></a><span data-ttu-id="61c6a-124">Додељивање лиценци</span><span class="sxs-lookup"><span data-stu-id="61c6a-124">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="61c6a-125">Требаће вам административни приступ Microsoft 365 порталу ваше организације да бисте извршили следеће кораке.</span><span class="sxs-lookup"><span data-stu-id="61c6a-125">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="61c6a-126">Идите у [Microsoft 365 центар администрације](https://portal.office.com/) да доделите лиценце својим корисницима.</span><span class="sxs-lookup"><span data-stu-id="61c6a-126">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

2. <span data-ttu-id="61c6a-127">На страници **Активни корисници**, изаберите кориснике којима желите да доделите лиценцу.</span><span class="sxs-lookup"><span data-stu-id="61c6a-127">On the **Active users** page, select the users that you want to assign a license to.</span></span>

3. <span data-ttu-id="61c6a-128">Проверите да ли је изабрана лиценца **Dynamics 365 Project Operations**, па изаберите **Сачувај промене**.</span><span class="sxs-lookup"><span data-stu-id="61c6a-128">Verify that the **Dynamics 365 Project Operations** license has been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="61c6a-129">Понуду за пробну верзију услуге Finance не треба доделити кориснику.</span><span class="sxs-lookup"><span data-stu-id="61c6a-129">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="61c6a-130">Започните нови пројекат у LCS</span><span class="sxs-lookup"><span data-stu-id="61c6a-130">Start a new project in LCS</span></span>

<span data-ttu-id="61c6a-131">Направите нови LCS пројекат како је описано у теми [Започните нови пројекат у LCS](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="61c6a-131">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="61c6a-132">Додајте Azure претплату у LCS пројекат</span><span class="sxs-lookup"><span data-stu-id="61c6a-132">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="61c6a-133">Да бисте довршили овај задатак, следите кораке у теми [Додавање Azure претплате у LCS пројекат](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="61c6a-133">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="61c6a-134">Примените Finance демо окружење са услугом Project Operations за сценарије ресурса / без залиха</span><span class="sxs-lookup"><span data-stu-id="61c6a-134">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="61c6a-135">Следите смернице у теми [Обезбеђење новог окружења](resource-provision-new-environment.md) да бисте завршили примену.</span><span class="sxs-lookup"><span data-stu-id="61c6a-135">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="61c6a-136">Користите [демо окружење](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) тип примене за преглед.</span><span class="sxs-lookup"><span data-stu-id="61c6a-136">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="61c6a-137">Инсталирајте податке о подешавању и конфигурацији CDS</span><span class="sxs-lookup"><span data-stu-id="61c6a-137">Install CDS setup and configuration data</span></span>

<span data-ttu-id="61c6a-138">Инсталирајте податке о подешавању и конфигурацији CDS како је описано у теми [Подесите и примените податке о конфигурацији у услузи Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="61c6a-138">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="61c6a-139">Довршите овај корак тек након што се примени демо окружење услуге Finance и демо подаци буду спремни.</span><span class="sxs-lookup"><span data-stu-id="61c6a-139">Complete this step only after Finance demo environment is deployed and demo data is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
