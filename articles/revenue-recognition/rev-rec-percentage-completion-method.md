---
title: Процена прихода пројеката са фиксном ценом
description: Ова тема пружа информације о процени прихода са фиксном ценом у пројектима.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7cf4d7853f7fedaeeeba99bc589f39989b924423
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278931"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="84b0e-103">Процена прихода пројеката са фиксном ценом</span><span class="sxs-lookup"><span data-stu-id="84b0e-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="84b0e-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="84b0e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="84b0e-105">Када креирате предмет пројектног уговора са следећим атрибутима у услузи Dynamics 365 Project Operations на платформи Microsoft Dataverse, систем аутоматски креира пројекат процене прихода са фиксном ценом.</span><span class="sxs-lookup"><span data-stu-id="84b0e-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="84b0e-106">Информације у овом пројекту заснивају се на следећем:</span><span class="sxs-lookup"><span data-stu-id="84b0e-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="84b0e-107">Начин обрачуна са фиксном ценом.</span><span class="sxs-lookup"><span data-stu-id="84b0e-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="84b0e-108">Везани пројекат.</span><span class="sxs-lookup"><span data-stu-id="84b0e-108">An associated project.</span></span>
  - <span data-ttu-id="84b0e-109">Најмање једна контролна тачка дефинисана на картици **Распоред фактура** на страници **Предмет пројектног уговора**.</span><span class="sxs-lookup"><span data-stu-id="84b0e-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="84b0e-110">Преглед процена прихода пројеката са фиксном ценом</span><span class="sxs-lookup"><span data-stu-id="84b0e-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="84b0e-111">Да бисте прегледали процене прихода пројеката са фиксном ценом, довршите следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="84b0e-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="84b0e-112">У Dynamics 365 Finance окружењу, идите на **Управљање пројектима и рачуноводство** > **Пројекти** > **Процена прихода пројеката са фиксном ценом**.</span><span class="sxs-lookup"><span data-stu-id="84b0e-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="84b0e-113">Изаберите пројекат који желите да прикажете и двапут кликните на **ID процене пројекта** како бисте отворили запис и прегледали детаље пројекта.</span><span class="sxs-lookup"><span data-stu-id="84b0e-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="84b0e-114">РАзвијте картицу **Пројекат**. Видећете један пројекат у мрежи **Изабрани пројекти**.</span><span class="sxs-lookup"><span data-stu-id="84b0e-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="84b0e-115">Систем ово користи као подразумевани пројекат, јер је то пројекат повезан са предметом пројектног уговора.</span><span class="sxs-lookup"><span data-stu-id="84b0e-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="84b0e-116">Да бисте променили повезивање, изаберите додатне пројекте и додајте их у мрежу **Изабрани пројекти**.</span><span class="sxs-lookup"><span data-stu-id="84b0e-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="84b0e-117">Ако је у овој мрежи изабрано више пројеката, проценат довршења пројекта и процене прихода израчунавају се заједно за све изабране пројекте.</span><span class="sxs-lookup"><span data-stu-id="84b0e-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="84b0e-118">Трошак пројекта, профил прихода, предложак трошкова и кôд периода могу се ручно подесити.</span><span class="sxs-lookup"><span data-stu-id="84b0e-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="84b0e-119">Ако их не поставите ручно, вредности ће бити подразумеване на прво израчунавање процене за пројекат користећи правила конфигурисана за профиле трошкова и прихода пројекта.</span><span class="sxs-lookup"><span data-stu-id="84b0e-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]