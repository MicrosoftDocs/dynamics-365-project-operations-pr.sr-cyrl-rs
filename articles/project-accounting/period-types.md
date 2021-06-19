---
title: Типови периода
description: У овој теми се пружају информације о томе како да конфигуришете типове периода за процену прихода.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 07cc9cde5fab10accb1fd6efede58926918f614c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013504"
---
# <a name="period-types"></a><span data-ttu-id="a7c87-103">Типови периода</span><span class="sxs-lookup"><span data-stu-id="a7c87-103">Period types</span></span>

<span data-ttu-id="a7c87-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="a7c87-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a7c87-105">Тип периода дефинише колико се често процењује приход од пројекта.</span><span class="sxs-lookup"><span data-stu-id="a7c87-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="a7c87-106">У овој теми се пружају информације о томе како да конфигуришете типове периода за процену прихода.</span><span class="sxs-lookup"><span data-stu-id="a7c87-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="a7c87-107">Креирање и рад са типовима периода</span><span class="sxs-lookup"><span data-stu-id="a7c87-107">Create and work with period types</span></span>
<span data-ttu-id="a7c87-108">Да бисте креирали и радили са типовима периода, извршите следеће кораке:</span><span class="sxs-lookup"><span data-stu-id="a7c87-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="a7c87-109">У Dynamics 365 Finance окружењу, идите на **Управљање пројектима и рачуноводство** > **Подешавање** > **Процене** > **Типови периода**.</span><span class="sxs-lookup"><span data-stu-id="a7c87-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="a7c87-110">Да бисте креирали нови тип периода, изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="a7c87-110">Select **New** to create new period type.</span></span> <span data-ttu-id="a7c87-111">Унесите назив и опис.</span><span class="sxs-lookup"><span data-stu-id="a7c87-111">Enter a name and description.</span></span>
3. <span data-ttu-id="a7c87-112">У пољу **Учесталост**, изаберите вредност:</span><span class="sxs-lookup"><span data-stu-id="a7c87-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="a7c87-113">Ако изаберете **седмица**, **Двонедељно**, **Полумесечно**, **Месец**, **Дан**, **Квартал** или **Година**, календар ће се користити за генерисање периода.</span><span class="sxs-lookup"><span data-stu-id="a7c87-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="a7c87-114">Ако изаберете **Период књиге**, периоди књиге из конфигурације главне књиге ће се користити за генерисање периода.</span><span class="sxs-lookup"><span data-stu-id="a7c87-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="a7c87-115">Ако изаберете **Неограничено**, можете одредити прилагођене периоде.</span><span class="sxs-lookup"><span data-stu-id="a7c87-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="a7c87-116">Изаберите запис типа периода, а затим изаберите **Генериши периоде** да бисте креирали периоде за тип периода.</span><span class="sxs-lookup"><span data-stu-id="a7c87-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="a7c87-117">На основу учесталости периода коју сте изабрали, можда ћете моћи да одредите датум почетка или број периода који треба генерисати.</span><span class="sxs-lookup"><span data-stu-id="a7c87-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="a7c87-118">Изаберите **Периоди** да бисте прегледали генерисане периоде.</span><span class="sxs-lookup"><span data-stu-id="a7c87-118">Select **Periods** to review generated periods.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]