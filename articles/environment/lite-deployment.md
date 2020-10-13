---
title: Примена услуге Project Operations Lite – од погодбе до профактуре
description: Ова тема пружа информације о томе како да инсталирате примену услуге Project Operations Lite – од погодбе до профактуре.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e938876d459b3f6dfedd90e57e3042cda96bffb7
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949056"
---
# <a name="deploy-project-operations-lite-deployment--deal-to-proforma-invoicing"></a><span data-ttu-id="a0549-103">Примена услуге Project Operations Lite – од погодбе до профактуре</span><span class="sxs-lookup"><span data-stu-id="a0549-103">Deploy Project Operations Lite deployment – deal to proforma invoicing</span></span>

<span data-ttu-id="a0549-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="a0549-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a0549-105">Project Operations подржава више модела примене.</span><span class="sxs-lookup"><span data-stu-id="a0549-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="a0549-106">Да бисте утврдили најбољи модел примене, погледајте чланак [Врсте примена](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="a0549-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="a0549-107">Ова примена, Lite примена – од погодбе до профактуре, резултира **само у Project Operations примени у услузи Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="a0549-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="a0549-108">Инсталирање услуге Project Operations у ново CDS окружење</span><span class="sxs-lookup"><span data-stu-id="a0549-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="a0549-109">Инсталирајте у постојеће CDS окружење</span><span class="sxs-lookup"><span data-stu-id="a0549-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="a0549-110">Инсталирање услуге Project Operations у ново CDS окружење</span><span class="sxs-lookup"><span data-stu-id="a0549-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="a0549-111">Као [глобални или Power Platform администратор](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, креирајте ново CDS окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="a0549-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="a0549-112">Уверите се да су омогућене **CDS база података** и **Dynamics 365 апликације**.</span><span class="sxs-lookup"><span data-stu-id="a0549-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="a0549-113">За више информација, погледајте одељак [Креирање и управљање окружењима у Power Platform центру администрације](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a0549-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="a0549-114">Изаберите **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација.</span><span class="sxs-lookup"><span data-stu-id="a0549-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="a0549-115">Инсталирање услуге Project Operations у постојеће CDS окружење</span><span class="sxs-lookup"><span data-stu-id="a0549-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="a0549-116">Као [глобални или Power Platform администратор](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, лоцирајте окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com) где желите да инсталирате Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a0549-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="a0549-117">Инсталирајте **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација.</span><span class="sxs-lookup"><span data-stu-id="a0549-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="a0549-118">Више информација потражите у чланку [Управљање Dynamics 365 апликацијама](https://docs.microsoft.com/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="a0549-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>


