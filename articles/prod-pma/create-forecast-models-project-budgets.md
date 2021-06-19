---
title: Креирајте моделе предвиђања за буџете пројеката
description: Ова тема описује како креирати модел предвиђања за преостале буџете.
author: Yowelle
ms.date: 04/24/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 3549b41fce72b44230ab27de081dade15a912266
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006315"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="f9aa5-103">Креирајте моделе предвиђања за буџете пројеката</span><span class="sxs-lookup"><span data-stu-id="f9aa5-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f9aa5-104">Ова тема описује како креирати модел предвиђања за преостале буџете.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="f9aa5-105">Пројекат који подлеже буџетској контроли користи две врсте буџета: оригинални и преостали.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="f9aa5-106">Када креирате буџет пројекта, морате навести моделе предвиђања првобитног и преосталог буџета који су креирани на страници **Модели предвиђања**.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="f9aa5-107">Буџети пројеката засновани на наведеним моделима креирају се када доделите буџет пројекта.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="f9aa5-108">Модел прогнозе који се користи за контролу буџета не може да има подмодел или да се користи као подмодел.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="f9aa5-109">Изаберите **Управљање пројектима и рачуноводство** > **Подешавање** > **Прогнозе**  > **Модели предвиђања**.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="f9aa5-110">Изаберите **Ново** да бисте креирали нови модел прогнозе, а затим унесите ID броја модела и име за нови модел.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="f9aa5-111">Подесите опцију **Заустављено** на **Да** како би се спречиле било какве промене линија предвиђања за модел прогнозе.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="f9aa5-112">Ако линије предвиђања са којима је модел повезан треба да генеришу предвиђања новчаног тока у главној књизи, поставите **Укључи у предвиђања новчаног тока** на **Да.**</span><span class="sxs-lookup"><span data-stu-id="f9aa5-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="f9aa5-113">Да бисте користили датум пројекта као датум фактуре, подесите **Датум фактуре прогнозе** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="f9aa5-114">У пољу **Тип буџета** изаберите један од следећих типова модела:</span><span class="sxs-lookup"><span data-stu-id="f9aa5-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="f9aa5-115">**Оригинални буџет**: Користите оригиналне износе буџета који су прослеђени при креирању и одобравању почетног буџета.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-115">**Original budget**: Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="f9aa5-116">**Преостали буџет**: Користите преостале износе буџета током трајања пројекта.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-116">**Remaining budget**: Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="f9aa5-117">Стања у овом моделу предвиђања смањују се стварним трансакцијама, а повећавају или смањују ревизијама буџета.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="f9aa5-118">**Пренос**: Користите преносне износе буџета за пројекат.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-118">**Carry-forward**: Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="f9aa5-119">Пренос је опциони поступак који се може покренути ради преноса неискоришћених износа буџета из једне фискалне године у другу.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="f9aa5-120">По потреби подесите следеће опције:</span><span class="sxs-lookup"><span data-stu-id="f9aa5-120">Set the following options as required:</span></span>

   - <span data-ttu-id="f9aa5-121">Да бисте користили датум пројекта као датум фактуре, омогућите **Датум фактуре прогнозе**.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="f9aa5-122">Омогућите **Прогноза помоћу WIP-а** за предвиђање на основу посла у току (WIP), а затим одаберите тип WIP-а.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="f9aa5-123">Можете задржати подразумевани **Тип буџета** као **Ниједан** или унесите нови тип.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="f9aa5-124">Тип буџета не може се променити након што промените запис.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="f9aa5-125">Ако промените подразумевани тип буџета, све остале опције постаће недоступне за ажурирања и не можете поново користити овај модел предвиђања.</span><span class="sxs-lookup"><span data-stu-id="f9aa5-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]