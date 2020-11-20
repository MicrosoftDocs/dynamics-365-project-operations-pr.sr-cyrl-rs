---
title: Креирање ставки времена
description: Ова тема пружа информације о томе како да креирате ставке времена.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: d8c87f0fd2cc021bb9088d0fac73ccd52980a905
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131308"
---
# <a name="create-time-entries"></a><span data-ttu-id="b21cf-103">Креирање ставки времена</span><span class="sxs-lookup"><span data-stu-id="b21cf-103">Create time entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b21cf-104">У претходним верзијама апликације Dynamics 365 Project Service Automation, ставке времена су уношене једном недељно.</span><span class="sxs-lookup"><span data-stu-id="b21cf-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="b21cf-105">У верзији 3 апликације Project Service Automation, уносе се свакодневно.</span><span class="sxs-lookup"><span data-stu-id="b21cf-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="b21cf-106">Међутим, након што је креирано неколико ставки, можете их групно креирати или копирати.</span><span class="sxs-lookup"><span data-stu-id="b21cf-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="b21cf-107">Креирање ставке времена</span><span class="sxs-lookup"><span data-stu-id="b21cf-107">Create a time entry</span></span>

<span data-ttu-id="b21cf-108">Следите ове кораке за креирање ставке времена.</span><span class="sxs-lookup"><span data-stu-id="b21cf-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="b21cf-109">На страници **Ставке времена** изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="b21cf-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="b21cf-110">У дијалог **Брзо креирање ставке времена** унесите трајање ставке у минутима, сатима или данима.</span><span class="sxs-lookup"><span data-stu-id="b21cf-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="b21cf-111">Трајање мора да се унесе у неком од ових формата: *x* минута, *x* сати или *x* дана.</span><span class="sxs-lookup"><span data-stu-id="b21cf-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="b21cf-112">Сати и дани такође могу да се уносе као децималне вредности, на пример *x.x* сати или *x.x* дана.</span><span class="sxs-lookup"><span data-stu-id="b21cf-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="b21cf-113">Изаберите врсту ставке времена и пројекат за који је уносите.</span><span class="sxs-lookup"><span data-stu-id="b21cf-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="b21cf-114">У пољу **Пројектни задатак** пронађите задатак за ову ставку.</span><span class="sxs-lookup"><span data-stu-id="b21cf-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b21cf-115">Ако креирате ставку времена за задатак који није додељен кориснику, у пољу **Пројектни задатак** изаберите дугме **Претражи**, одаберите **Промени приказ**, а затим **Сви активни задаци пројекта** да бисте видели листу свих задатака.</span><span class="sxs-lookup"><span data-stu-id="b21cf-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View**, and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="b21cf-116">Унесите опис, ако је потребан опис, а затим изаберите **Сачувај и затвори**.</span><span class="sxs-lookup"><span data-stu-id="b21cf-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="b21cf-117">Након што је ставка времена креирана и сачувана, можете је уредити у мрежи за ставке времена.</span><span class="sxs-lookup"><span data-stu-id="b21cf-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="b21cf-118">Мрежа за ставке времена подржава два формата:</span><span class="sxs-lookup"><span data-stu-id="b21cf-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="b21cf-119">Можете унети ставке времена у формату **hh:mm**.</span><span class="sxs-lookup"><span data-stu-id="b21cf-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="b21cf-120">Овај формат се затим претвара у сате и децималне вредности.</span><span class="sxs-lookup"><span data-stu-id="b21cf-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="b21cf-121">Можете директно унети сате и децималне вредности.</span><span class="sxs-lookup"><span data-stu-id="b21cf-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="b21cf-122">Имајте на уму да децималне вредности сата нису минути.</span><span class="sxs-lookup"><span data-stu-id="b21cf-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="b21cf-123">Стога 1,5 сат представља 1 сат и 30 минута.</span><span class="sxs-lookup"><span data-stu-id="b21cf-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="b21cf-124">Исто правило важи за децималне вредности дана.</span><span class="sxs-lookup"><span data-stu-id="b21cf-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="b21cf-125">Један дан има 24 сата, па 0,5 дана представља 12 сати.</span><span class="sxs-lookup"><span data-stu-id="b21cf-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="b21cf-126">Групно креирање ставки времена</span><span class="sxs-lookup"><span data-stu-id="b21cf-126">Bulk create time entries</span></span>

<span data-ttu-id="b21cf-127">Након креирања неколико ставки времена, можете их копирати да бисте групно креирали додатне ставке времена.</span><span class="sxs-lookup"><span data-stu-id="b21cf-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="b21cf-128">На страници **Ставке времена** изаберите **Копирај недељу**.</span><span class="sxs-lookup"><span data-stu-id="b21cf-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="b21cf-129">У групи поља **Из периода** у пољима **Датум почетка** и **Датум завршетка** дефинишите опсег датума из којег треба копирати ставке времена.</span><span class="sxs-lookup"><span data-stu-id="b21cf-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="b21cf-130">У групи поља **У период**, у оквиру поља **Датум почетка**, одредите датум за који ћете креирати ставке времена.</span><span class="sxs-lookup"><span data-stu-id="b21cf-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="b21cf-131">Изаберите **Копирај** да бисте креирали копију ставки времена која одговара дану у недељи који је наведен у групи поља **У период**.</span><span class="sxs-lookup"><span data-stu-id="b21cf-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="b21cf-132">На пример, ставка времена за понедељак из прошле недеље се копира у понедељак оне седмице која је наведена у групи поља **У период**.</span><span class="sxs-lookup"><span data-stu-id="b21cf-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="b21cf-133">Увоз података за ставке времена</span><span class="sxs-lookup"><span data-stu-id="b21cf-133">Import data for time entries</span></span>

<span data-ttu-id="b21cf-134">Можете да увезете податке из резервација и задатака за пројекте.</span><span class="sxs-lookup"><span data-stu-id="b21cf-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="b21cf-135">Када увезете податке, можете одредити опсег датума резервација за увоз, а затим експлицитно одабрати резервације које би требало да буду креиране као ставке времена **Радна верзија**.</span><span class="sxs-lookup"><span data-stu-id="b21cf-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="b21cf-136">Могућности груписања према, сортирања, претраге и филтрирања</span><span class="sxs-lookup"><span data-stu-id="b21cf-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="b21cf-137">Можете груписати и филтрирати ставке времена према димензијама које су наведене у колонама.</span><span class="sxs-lookup"><span data-stu-id="b21cf-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="b21cf-138">У пољу **Групирај према** одаберите димензију за филтрирање ставки времена.</span><span class="sxs-lookup"><span data-stu-id="b21cf-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="b21cf-139">Такође можете сортирати записе ставки времена растућим или опадајућим редоследом користећи стрелицу за сортирање у називима колона.</span><span class="sxs-lookup"><span data-stu-id="b21cf-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="b21cf-140">Поред тога, ставке можете приказати или сакрити тако што ћете кликнути на дугме **Филтер** у називу колоне, а затим у пољу **Претрага** унети текст који треба да се користи за претрагу ставки времена према називу пројекта, пројектном задатку, ставци времена или ресурсу.</span><span class="sxs-lookup"><span data-stu-id="b21cf-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>
