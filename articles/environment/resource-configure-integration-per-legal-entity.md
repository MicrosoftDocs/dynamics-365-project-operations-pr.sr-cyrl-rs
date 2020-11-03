---
title: Конфигурисање интеграције за Project Operations по правном лицу
description: Ова тема пружа информације о томе како да подесите интеграцију по правном лицу у услузи Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c0e02ef2d17bf49209369f7adad681d9a5981e2a
ms.sourcegitcommit: 91ad491e94a421f256a378b0f4b26ed48c67bc93
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/22/2020
ms.locfileid: "4096770"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="b8a88-103">Конфигурисање интеграције за Project Operations по правном лицу</span><span class="sxs-lookup"><span data-stu-id="b8a88-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="b8a88-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="b8a88-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b8a88-105">Ова тема вас води кроз кораке потребне за конфигурисање услуге Dynamics 365 Project Operations по правном лицу.</span><span class="sxs-lookup"><span data-stu-id="b8a88-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="b8a88-106">Омогућите кључне функције у услузи Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="b8a88-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="b8a88-107">Довршите следеће кораке да бисте омогућили потребне функције.</span><span class="sxs-lookup"><span data-stu-id="b8a88-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="b8a88-108">У услузи Dynamics 365 Finance идите на радни простор **Управљање подацима**.</span><span class="sxs-lookup"><span data-stu-id="b8a88-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="b8a88-109">У одељку **Листа функција** , пронађите и омогућите следеће функције:</span><span class="sxs-lookup"><span data-stu-id="b8a88-109">In **Feature list** , find and enable the following features:</span></span>
  
    - <span data-ttu-id="b8a88-110">**Омогућите више предмета уговора за пројекат**</span><span class="sxs-lookup"><span data-stu-id="b8a88-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="b8a88-111">**Омогућите Project Operations у услузи Dynamics 365 Customer Engagement**</span><span class="sxs-lookup"><span data-stu-id="b8a88-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="b8a88-112">Ако не видите **Кључне функције** , проверите да ли ваша верзија услуге Finance испуњава минимални захтев за верзију (верзија апликације 10.0.13 са примењеним свим исправкама квалитета или новија).</span><span class="sxs-lookup"><span data-stu-id="b8a88-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="b8a88-113">Изаберите **Провери да ли има ажурирања** да бисте освежили листу функција.</span><span class="sxs-lookup"><span data-stu-id="b8a88-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="b8a88-114">Дефинишите сценарио примене услуге Project Operations за правно лице</span><span class="sxs-lookup"><span data-stu-id="b8a88-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="b8a88-115">Project Operations можете да омогућите у услузи Dynamics 365 Customer Engagement на нивоу правног лица.</span><span class="sxs-lookup"><span data-stu-id="b8a88-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="b8a88-116">Можете да имате једно правно лице које користи Project Operations у услузи Dynamics 365 Customer Engagement за сценарије засноване на ресурсима/који нису засновани на залихама.</span><span class="sxs-lookup"><span data-stu-id="b8a88-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="b8a88-117">У истом окружењу можете имати друго правно лице које користи Project Operations за сценарије засноване на залихама/поруџбеницама.</span><span class="sxs-lookup"><span data-stu-id="b8a88-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="b8a88-118">У услузи Dynamics 365 Finance идите на **Управљање пројектима и рачуноводство** > **Подешавање** > **Глобално управљање пројектима и рачуноводствени параметри**.</span><span class="sxs-lookup"><span data-stu-id="b8a88-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="b8a88-119">На листи доступних правних лица изаберите ентитете у којима ће бити омогућено више предмета уговора и функције Project Operations у услузи Dynamics 365 Customer Engagement.</span><span class="sxs-lookup"><span data-stu-id="b8a88-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="b8a88-120">Немојте бирати правна лица која ће користити Project Operations за сценарије засноване на залихама/поруџбеницама.</span><span class="sxs-lookup"><span data-stu-id="b8a88-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="b8a88-121">Правно лице се може одабрати само ако нема постојеће пројекте.</span><span class="sxs-lookup"><span data-stu-id="b8a88-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="b8a88-122">Конфигурисање параметара управљања пројектима и рачуноводства</span><span class="sxs-lookup"><span data-stu-id="b8a88-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="b8a88-123">Свако правно лице које користи Project Operations у услузи Dynamics 365 Customer Engagement мора да има скуп подразумеваних параметара.</span><span class="sxs-lookup"><span data-stu-id="b8a88-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="b8a88-124">Ови параметри су конфигурисани на картици **Project Operations** на страници **Управљање пројектом и рачуноводствени параметри**.</span><span class="sxs-lookup"><span data-stu-id="b8a88-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="b8a88-125">Параметри су:</span><span class="sxs-lookup"><span data-stu-id="b8a88-125">The parameters are:</span></span>

  - <span data-ttu-id="b8a88-126">**Подразумеване вредности типова обрачуна** : Project Operations користи фиксни скуп подразумеваних задатака типа наплате који се морају мапирати са својствима ставки услуге Finance.</span><span class="sxs-lookup"><span data-stu-id="b8a88-126">**Billing type defaults** : Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="b8a88-127">Направите запис за сваку врсту обрачуна: **Није наведено** , **Наплативо** , **Ненаплативо** , **Бесплатно** и **Није доступно**.</span><span class="sxs-lookup"><span data-stu-id="b8a88-127">Create a record for each billing type: **Not specified** , **Chargeable** , **Non-chargeable** , **Complimentary** , and **Not available**.</span></span>
  - <span data-ttu-id="b8a88-128">**Подразумеване категорије пројеката** : Изаберите подразумеване категорије пројеката које ће се користити за сваку врсту трансакције.</span><span class="sxs-lookup"><span data-stu-id="b8a88-128">**Project category defaults** : Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="b8a88-129">Ове подразумеване вредности ће се користити у **Project Operations дневнику интеграције** и у проценама где није наведена категорија трансакције за стварни пројекат.</span><span class="sxs-lookup"><span data-stu-id="b8a88-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="b8a88-130">**Прогнозе** : Изаберите модел прогнозе који ће се користити за процену времена и трошкова.</span><span class="sxs-lookup"><span data-stu-id="b8a88-130">**Forecasts** : Select the forecast model to be used for time and expense estimates.</span></span>
