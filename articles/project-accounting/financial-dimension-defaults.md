---
title: Подразумеване вредности финансијске димензије
description: Ова тема пружа информације о начину постављања подразумеваних вредности финансијске димензије.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: aa6771ba5346fd4133b82c3e670badfa7655299f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131901"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="e8844-103">Подразумеване вредности финансијске димензије</span><span class="sxs-lookup"><span data-stu-id="e8844-103">Financial dimension defaults</span></span>

<span data-ttu-id="e8844-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="e8844-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e8844-105">Dynamics 365 Project Operations користи радни оквир за [финансијске димензије](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) у услузи Dynamics 365 Finance да пружи додатни увид у трансакције поткњиге и главне књиге.</span><span class="sxs-lookup"><span data-stu-id="e8844-105">Dynamics 365 Project Operations uses the [Financial dimensions](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="e8844-106">Подразумеване финансијске димензије могу се поставити на основу клијента, извора финансирања пројекта, контролне тачке, предмета уговора за пројекат или пројекта.</span><span class="sxs-lookup"><span data-stu-id="e8844-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="e8844-107">Дефинисање подразумеваних финансијских димензија за клијента</span><span class="sxs-lookup"><span data-stu-id="e8844-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="e8844-108">Подразумеване вредности за димензију клијента наведене су у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="e8844-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="e8844-109">Довршите следеће кораке да бисте подесили подразумеване вредности димензија.</span><span class="sxs-lookup"><span data-stu-id="e8844-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="e8844-110">Идите на **Потраживања** > **Клијенти** > **Сви клијенти**.</span><span class="sxs-lookup"><span data-stu-id="e8844-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="e8844-111">На страници **Клијенти**, на картици **Финансијске димензије**, подесите вредности финансијске димензије за одређеног клијента.</span><span class="sxs-lookup"><span data-stu-id="e8844-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="e8844-112">Дефинисање подразумеваних финансијских димензија за уговоре за пројекат</span><span class="sxs-lookup"><span data-stu-id="e8844-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="e8844-113">Уговори за пројекат се креирају и одржавају у услузи Common Data Service (CDS).</span><span class="sxs-lookup"><span data-stu-id="e8844-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="e8844-114">Атрибути рачуноводства за уговоре за пројекат постављени су у модул **Управљање пројектима и рачуноводство** у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="e8844-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="e8844-115">Подесите финансијске димензије за извор финансирања пројекта</span><span class="sxs-lookup"><span data-stu-id="e8844-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="e8844-116">Идите на **Управљање пројектима и рачуноводство** > **Пројекти** > **Уговори за пројекат**.</span><span class="sxs-lookup"><span data-stu-id="e8844-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="e8844-117">Изаберите запис који желите да ажурирате, а затим на картици **Уговор о пројекту** изаберите **Прикажи подразумевано рачуноводство**.</span><span class="sxs-lookup"><span data-stu-id="e8844-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="e8844-118">Проширите **Сродне информације** и изаберите картицу **Извори финансирања**.</span><span class="sxs-lookup"><span data-stu-id="e8844-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="e8844-119">Подесите подразумеване вредности финансијских димензија.</span><span class="sxs-lookup"><span data-stu-id="e8844-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="e8844-120">Имајте у виду да се подразумеване вредности финансијских димензија узимају са налога клијента.</span><span class="sxs-lookup"><span data-stu-id="e8844-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="e8844-121">Подесите финансијске димензије за предмет уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="e8844-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="e8844-122">Идите на **Управљање пројектима и рачуноводство** > **Пројекти** > **Уговори за пројекат**.</span><span class="sxs-lookup"><span data-stu-id="e8844-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="e8844-123">Изаберите запис који желите да ажурирате, а затим на картици **Уговор о пројекту** изаберите **Прикажи подразумевано рачуноводство**.</span><span class="sxs-lookup"><span data-stu-id="e8844-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="e8844-124">Проширите **Сродне информације** и изаберите картицу **Предмети уговора**.</span><span class="sxs-lookup"><span data-stu-id="e8844-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="e8844-125">Подесите подразумеване вредности финансијских димензија.</span><span class="sxs-lookup"><span data-stu-id="e8844-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="e8844-126">Подразумеване финансијске димензије су применљиве и могу се користити само са предметима уговора са фиксном ценом (контролном тачком).</span><span class="sxs-lookup"><span data-stu-id="e8844-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="e8844-127">Ове подразумеване вредности се користе за повезане трансакције за пословног клијента на пројекту и ставке фактура.</span><span class="sxs-lookup"><span data-stu-id="e8844-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="e8844-128">Дефинисање подразумеваних финансијских димензија за пројекте</span><span class="sxs-lookup"><span data-stu-id="e8844-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="e8844-129">Пројекти се креирају и одржавају у услузи CDS.</span><span class="sxs-lookup"><span data-stu-id="e8844-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="e8844-130">Атрибути рачуноводства за пројекат постављени су у модул **Управљање пројектима и рачуноводство** у услузи Finance.</span><span class="sxs-lookup"><span data-stu-id="e8844-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="e8844-131">Идите на **Управљање пројектима и рачуноводство** > **Пројекти** > **Сви пројекти**.</span><span class="sxs-lookup"><span data-stu-id="e8844-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="e8844-132">Изаберите запис који желите да ажурирате, а затим на картици **Пројекат** изаберите **Прикажи подразумевано рачуноводство**.</span><span class="sxs-lookup"><span data-stu-id="e8844-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="e8844-133">Проширите **Сродне информације** и изаберите картицу **Подешавање**.</span><span class="sxs-lookup"><span data-stu-id="e8844-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="e8844-134">Подесите подразумеване вредности финансијских димензија.</span><span class="sxs-lookup"><span data-stu-id="e8844-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="e8844-135">Имајте у виду да се подразумеване вредности финансијских димензија узимају са налога клијента.</span><span class="sxs-lookup"><span data-stu-id="e8844-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="e8844-136">Ако је пројекат повезан са предметом уговора са више клијената уговора за пројекат, примарни клијент се користи за подразумеване финансијске димензије.</span><span class="sxs-lookup"><span data-stu-id="e8844-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="e8844-137">Подразумеване финансијске димензије пројекта користе се за постављање подразумеваних вредности ставке у главној књизи за трансакције времена, трошкова и накнада у **Project Operations дневнику интеграције** и на повезаним ставкама фактуре пројекта.</span><span class="sxs-lookup"><span data-stu-id="e8844-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>
