---
title: Примена услуге Project Operations – једноставно
description: Ова тема пружа информације о томе како да инсталирате примену услуге Project Operations Lite – од погодбе до профактуре.
author: stsporen
ms.date: 10/02/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb1f1ad86e19d84d68a40b32b2fdb08dc4777a78
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995549"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="17560-103">Примена услуге Project Operations – једноставно</span><span class="sxs-lookup"><span data-stu-id="17560-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="17560-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="17560-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="17560-105">Project Operations подржава више модела примене.</span><span class="sxs-lookup"><span data-stu-id="17560-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="17560-106">Да бисте утврдили најбољи модел примене, погледајте чланак [Врсте примена](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="17560-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="17560-107">Ова примена, Lite примена – од погодбе до профактуре, резултира **само у Project Operations примени у услузи Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="17560-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="17560-108">Инсталирање услуге Project Operations у ново CDS окружење</span><span class="sxs-lookup"><span data-stu-id="17560-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="17560-109">Инсталирајте у постојеће CDS окружење</span><span class="sxs-lookup"><span data-stu-id="17560-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="17560-110">Инсталирање услуге Project Operations у ново CDS окружење</span><span class="sxs-lookup"><span data-stu-id="17560-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="17560-111">Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, креирајте ново CDS окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="17560-111">As the [Global or Power Platform Administrator](/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="17560-112">Уверите се да су омогућене **CDS база података** и **Dynamics 365 апликације**.</span><span class="sxs-lookup"><span data-stu-id="17560-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="17560-113">За више информација, погледајте одељак [Креирање и управљање окружењима у Power Platform центру администрације](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="17560-113">For more information, see [Create and manage environments in the Power Platform admin center](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="17560-114">Изаберите **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација.</span><span class="sxs-lookup"><span data-stu-id="17560-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="17560-115">Инсталирање услуге Project Operations у постојеће CDS окружење</span><span class="sxs-lookup"><span data-stu-id="17560-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="17560-116">Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, лоцирајте окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com) где желите да инсталирате Project Operations.</span><span class="sxs-lookup"><span data-stu-id="17560-116">As the [Global or Power Platform Administrator](/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="17560-117">Инсталирајте **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација.</span><span class="sxs-lookup"><span data-stu-id="17560-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="17560-118">Више информација потражите у чланку [Управљање Dynamics 365 апликацијама](/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="17560-118">For more information, see [Manage Dynamics 365 apps](/power-platform/admin/manage-apps).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]