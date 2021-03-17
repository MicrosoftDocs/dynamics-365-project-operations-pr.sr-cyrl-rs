---
title: Типови периода
description: У овој теми се пружају информације о томе како да конфигуришете типове периода за процену прихода.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 107cecbc1dabdf13147d847bf1816f44cc2703c5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287301"
---
# <a name="period-types"></a><span data-ttu-id="56124-103">Типови периода</span><span class="sxs-lookup"><span data-stu-id="56124-103">Period types</span></span>

<span data-ttu-id="56124-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="56124-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="56124-105">Тип периода дефинише колико се често процењује приход од пројекта.</span><span class="sxs-lookup"><span data-stu-id="56124-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="56124-106">У овој теми се пружају информације о томе како да конфигуришете типове периода за процену прихода.</span><span class="sxs-lookup"><span data-stu-id="56124-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="56124-107">Креирање и рад са типовима периода</span><span class="sxs-lookup"><span data-stu-id="56124-107">Create and work with period types</span></span>
<span data-ttu-id="56124-108">Да бисте креирали и радили са типовима периода, извршите следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="56124-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="56124-109">У Dynamics 365 Finance окружењу, идите на **Управљање пројектима и рачуноводство** > **Подешавање** > **Процене** > **Типови периода**.</span><span class="sxs-lookup"><span data-stu-id="56124-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="56124-110">Да бисте креирали нови тип периода, изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="56124-110">Select **New** to create new period type.</span></span> <span data-ttu-id="56124-111">Унесите назив и опис.</span><span class="sxs-lookup"><span data-stu-id="56124-111">Enter a name and description.</span></span>
3. <span data-ttu-id="56124-112">У пољу **Учесталост**, изаберите вредност:</span><span class="sxs-lookup"><span data-stu-id="56124-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="56124-113">Ако изаберете **седмица**, **Двонедељно**, **Полумесечно**, **Месец**, **Дан**, **Квартал** или **Година**, календар ће се користити за генерисање периода.</span><span class="sxs-lookup"><span data-stu-id="56124-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="56124-114">Ако изаберете **Период књиге**, периоди књиге из конфигурације главне књиге ће се користити за генерисање периода.</span><span class="sxs-lookup"><span data-stu-id="56124-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="56124-115">Ако изаберете **Неограничено**, можете одредити прилагођене периоде.</span><span class="sxs-lookup"><span data-stu-id="56124-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="56124-116">Изаберите запис типа периода, а затим изаберите **Генериши периоде** да бисте креирали периоде за тип периода.</span><span class="sxs-lookup"><span data-stu-id="56124-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="56124-117">На основу учесталости периода коју сте изабрали, можда ћете моћи да одредите датум почетка или број периода који треба генерисати.</span><span class="sxs-lookup"><span data-stu-id="56124-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="56124-118">Изаберите **Периоди** да бисте прегледали генерисане периоде.</span><span class="sxs-lookup"><span data-stu-id="56124-118">Select **Periods** to review generated periods.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]