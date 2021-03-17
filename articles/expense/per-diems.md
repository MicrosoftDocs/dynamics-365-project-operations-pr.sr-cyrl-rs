---
title: Дневнице
description: Ова тема пружа информације о правилима дневница која се користе у управљању трошковима.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 70e26a5e0f9a06730a2166318006429195335d4d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276321"
---
# <a name="per-diems"></a><span data-ttu-id="d1a83-103">Дневнице</span><span class="sxs-lookup"><span data-stu-id="d1a83-103">Per diems</span></span>

<span data-ttu-id="d1a83-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="d1a83-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="d1a83-105">Дневница је накнада која се исплаћује раднику који путује због посла.</span><span class="sxs-lookup"><span data-stu-id="d1a83-105">A per diem is an allowance that is paid to a worker who is traveling for work.</span></span> <span data-ttu-id="d1a83-106">У управљању трошковима можете креирати правила за дневнице за различите ситуације путовања.</span><span class="sxs-lookup"><span data-stu-id="d1a83-106">In Expense management, you can create per diem rules for  various travel situations.</span></span> <span data-ttu-id="d1a83-107">Износи дневница могу се заснивати на добу године, локацији путовања или обоје.</span><span class="sxs-lookup"><span data-stu-id="d1a83-107">Per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="d1a83-108">Када креирате правило за дневницу, можете да одредите да се проценат дневнице задржава ако радник добије бесплатне оброке или услуге.</span><span class="sxs-lookup"><span data-stu-id="d1a83-108">When you create a per diem  rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="d1a83-109">Такође можете да одредите минимални и максимални број сати за који дневница може да се примењује на путовање радника.</span><span class="sxs-lookup"><span data-stu-id="d1a83-109">You can also set a minimum and maximum number of hours that the per diem rate can apply to a worker's travel.</span></span>

## <a name="configuration"></a><span data-ttu-id="d1a83-110">Конфигурисање</span><span class="sxs-lookup"><span data-stu-id="d1a83-110">Configuration</span></span> 

1. <span data-ttu-id="d1a83-111">Да бисте додали локације за дневнице, идите на **Подешавање** > **Прорачуни и шифре** > **Локације за дневнице**.</span><span class="sxs-lookup"><span data-stu-id="d1a83-111">To add per diem locations, go to **Set up** > **Calculations and codes** > **Per diem locations**.</span></span>
2. <span data-ttu-id="d1a83-112">За сваку од горе додатих локација изаберите износ дневнице и валуту која важи између одређеног датума почетка и завршетка за хотел, оброке и остале трошкове.</span><span class="sxs-lookup"><span data-stu-id="d1a83-112">For each of the locations added above, select a per diem rate and currency that is valid between a specific start and end date for hotel, meals, and other expenses.</span></span> <span data-ttu-id="d1a83-113">Стопе дневница и валуте су конфигурисане у одељку **Подешавање** > **Прорачуни и шифре** > **Дневнице**.</span><span class="sxs-lookup"><span data-stu-id="d1a83-113">Per diem rates and currencies are configured under **Set up** > **Calculations and codes** > **Per diems**.</span></span>
3. <span data-ttu-id="d1a83-114">На страници **Локације за дневнице**, конфигуришите нивое износа дневница.</span><span class="sxs-lookup"><span data-stu-id="d1a83-114">On the **Per diem locations** page, configure per diem rate tiers.</span></span> <span data-ttu-id="d1a83-115">Нивои износа дневница омогућавају вам да дефинишете процентуалну поделу дневне накнаде за хотел, оброке и друге трошкове.</span><span class="sxs-lookup"><span data-stu-id="d1a83-115">Per diem rate tiers allow you to define the percentage split of a daily allowance for hotel, meal, and other expenses.</span></span> 
4. <span data-ttu-id="d1a83-116">Да бисте одредили смањење процента оброка за доручак, ручак или вечеру, ажурирајте поља на страници **Параметри управљања трошковима** на картици **Дневнице**.</span><span class="sxs-lookup"><span data-stu-id="d1a83-116">To specify the meal percentage reduction for breakfast, lunch, or dinner, update the fields on the **Expense management parameters** page on the **Per diem** tab.</span></span> 
    
## <a name="submit-expenses-using-per-diem"></a><span data-ttu-id="d1a83-117">Прослеђивање трошкова коришћењем дневница</span><span class="sxs-lookup"><span data-stu-id="d1a83-117">Submit expenses using per diem</span></span>
<span data-ttu-id="d1a83-118">Да бисте проследили трошкове користећи дневнице, користите категорију трошка **Дневница** када креирате извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="d1a83-118">To submit expenses utilizing per diems, use the **Per diem** expense category when you create an expense report.</span></span> <span data-ttu-id="d1a83-119">Унесите **почетни датум дневнице**, **крајњи датум дневнице** и **локацију дневнице**.</span><span class="sxs-lookup"><span data-stu-id="d1a83-119">Enter the **Per diem from date**, **Per diem to date**,  and the **Per diem location**.</span></span> <span data-ttu-id="d1a83-120">Износ ће се израчунати на основу износа дневнице за изабрану локацију, а смањење оброка на основу нивоа дневница.</span><span class="sxs-lookup"><span data-stu-id="d1a83-120">The amount will be calculated based on the per diem rates for the selected location and meal reduction will be calculated based on the per diem rate tiers.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]