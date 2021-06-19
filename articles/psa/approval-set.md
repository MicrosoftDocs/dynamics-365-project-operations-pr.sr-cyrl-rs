---
title: Скупови одобрења
description: Ова тема пружа информације о скупу одобрења, захтевима и подскуповима тих операција.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116889"
---
# <a name="approval-sets"></a><span data-ttu-id="3849f-103">Скупови одобрења</span><span class="sxs-lookup"><span data-stu-id="3849f-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3849f-104">Скупови одобрења групишу захтеве за одобрење заједно у мање подскупове операција.</span><span class="sxs-lookup"><span data-stu-id="3849f-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="3849f-105">Ово груписање омогућава обраду одобрења у редоследу по пројекту и омогућава поновне покушаје и секвенцирања.</span><span class="sxs-lookup"><span data-stu-id="3849f-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="3849f-106">Груписање побољшава поузданост и следљивост обраде одобрења за велике количине одобрења.</span><span class="sxs-lookup"><span data-stu-id="3849f-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="3849f-107">Скупови одобрења указују на целокупни статус обраде њихових повезаних записа.</span><span class="sxs-lookup"><span data-stu-id="3849f-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="3849f-108">Када се запис о одобрењу обрађује помоћу скупа одобрења, запис се премешта са **Прослеђено** на **Одобрено** и раскида се његова веза са скупом одобрења.</span><span class="sxs-lookup"><span data-stu-id="3849f-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="3849f-109">Ако запис не успе када се поднесе на одобрење, остаће у статусу **Прослеђено**, а скуп одобрења се означава као неуспешан.</span><span class="sxs-lookup"><span data-stu-id="3849f-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="3849f-110">Скуп одобрења евидентира поруку о грешци неуспеха.</span><span class="sxs-lookup"><span data-stu-id="3849f-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="3849f-111">Обрада одобрења и скупова одобрења</span><span class="sxs-lookup"><span data-stu-id="3849f-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="3849f-112">Одобрења која су у реду за обраду видљива су у приказу **Одобрења обраде**.</span><span class="sxs-lookup"><span data-stu-id="3849f-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="3849f-113">Систем покушава да обради све ставке више пута асинхроно, укључујући поновни покушај одобрења ако претходни покушаји нису успели.</span><span class="sxs-lookup"><span data-stu-id="3849f-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="3849f-114">Поље **Трајање скупа одобрења** евидентира број покушаја обраде скупа пре него што се означи као неуспешан.</span><span class="sxs-lookup"><span data-stu-id="3849f-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="3849f-115">Неуспела одобрења и скупови одобрења</span><span class="sxs-lookup"><span data-stu-id="3849f-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="3849f-116">Приказ **Неуспела одобрења** наводи сва одобрења која захтевају интервенцију корисника.</span><span class="sxs-lookup"><span data-stu-id="3849f-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="3849f-117">Отворите повезане евиденције скупова одобрења да бисте идентификовали узрок неуспеха.</span><span class="sxs-lookup"><span data-stu-id="3849f-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="3849f-118">Избор **Покушај поново** повећава трајни број скупова одобрења, враћа скуп одобрења натраг у статус **Обрада** и покушава да обради преостале записе.</span><span class="sxs-lookup"><span data-stu-id="3849f-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="3849f-119">Конфигурисање скупова одобрења</span><span class="sxs-lookup"><span data-stu-id="3849f-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="3849f-120">Омогућавање функције скупова одобрења</span><span class="sxs-lookup"><span data-stu-id="3849f-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="3849f-121">Да бисте омогућили функцију Скупови одобрења, уверите се да тренутно нема одобрења која се обрађују.</span><span class="sxs-lookup"><span data-stu-id="3849f-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="3849f-122">Идите на страницу **Параметри пројекта** и изаберите **Контрола функција** > **Омогућавање модерних одобрења**.</span><span class="sxs-lookup"><span data-stu-id="3849f-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="3849f-123">Искључивање функције скупова одобрења</span><span class="sxs-lookup"><span data-stu-id="3849f-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="3849f-124">Да бисте искључили функцију Скупови одобрења, уверите се да тренутно нема одобрења која се обрађују.</span><span class="sxs-lookup"><span data-stu-id="3849f-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="3849f-125">Идите на страницу **Параметри пројекта** и изаберите **Контрола функција** > **Онемогућавање модерних одобрења**.</span><span class="sxs-lookup"><span data-stu-id="3849f-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="3849f-126">Конфигурисање асинхроне граничне вредности</span><span class="sxs-lookup"><span data-stu-id="3849f-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="3849f-127">Када се креирају скупови одобрења, обрада се премешта у позадину када изабрани број записа за одобрење пређе назначену граничну вредност.</span><span class="sxs-lookup"><span data-stu-id="3849f-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="3849f-128">Користите поље **Асинхрона гранична вредност** да конфигуришете када обраду одобрења треба изводити синхроно или асинхроно.</span><span class="sxs-lookup"><span data-stu-id="3849f-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="3849f-129">Важеће вредности су:</span><span class="sxs-lookup"><span data-stu-id="3849f-129">Valid values are:</span></span>

  - <span data-ttu-id="3849f-130">Нула: Сви захтеви треба да се обрађују асинхроно.</span><span class="sxs-lookup"><span data-stu-id="3849f-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="3849f-131">Бројеви већи од нуле: Одобрења се обрађују асинхроно само када пријављени број одобрења премаши ову вредност.</span><span class="sxs-lookup"><span data-stu-id="3849f-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
