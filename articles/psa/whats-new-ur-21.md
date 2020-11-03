---
title: Шта је ново или промењено у издању 21 исправке за Project Service Automation у верзији 3
description: У овој теми дате су функције и исправке које су доступне у издању 21 исправке за Project Service Automation у верзији 3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: e8a15d5f723da528640c62c1892bac0d801c2bee
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083923"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="8d0a9-103">Project Service Automation издање исправке 21, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="8d0a9-103">Project Service Automation Update Release 21, V3</span></span>

<span data-ttu-id="8d0a9-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="8d0a9-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="8d0a9-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="8d0a9-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="8d0a9-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="8d0a9-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="8d0a9-109">У овој теми дате су функције које су нове или су промењене у издању 21 исправке за Project Service Automation у верзији 3.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="8d0a9-110">Број израде ове верзије је V 3.10.32.50 и углавном је доступна путем самосталног ажурирања у јуну 2020. године.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="8d0a9-111">Издање исправке 21</span><span class="sxs-lookup"><span data-stu-id="8d0a9-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="8d0a9-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="8d0a9-112">Bug fixes</span></span>

<span data-ttu-id="8d0a9-113">**Време и трошак**</span><span class="sxs-lookup"><span data-stu-id="8d0a9-113">**Time and Expense**</span></span>

<span data-ttu-id="8d0a9-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="8d0a9-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="8d0a9-115">Приликом хостовања **Контроле мреже ставке времена** на контролној табли, мрежа не користи пуну ширину контејнера мреже контролне табле.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="8d0a9-116">За одређене временске зоне, контрола мреже **Ставка времена** не приказује записе.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="8d0a9-117">Ставке времена које су после 21:00 појављују се погрешног дана.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="8d0a9-118">Корисници не могу да пошаљу трошкове ако категорија трошкова, **Потребна је признаница за трошкове** нема вредност.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="8d0a9-119">**Управљање ресурсима**</span><span class="sxs-lookup"><span data-stu-id="8d0a9-119">**Resource Management**</span></span>

<span data-ttu-id="8d0a9-120">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="8d0a9-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="8d0a9-121">Неактивне резервације се приказују у приказу **Сравњење**.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="8d0a9-122">Недостаје валидација генеричког ресурса како би се осигурало да постоји важећи статус резервације.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="8d0a9-123">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="8d0a9-123">**Project Management**</span></span>

<span data-ttu-id="8d0a9-124">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="8d0a9-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="8d0a9-125">Мреже обрасца за **Пројекат** ( **Додела ресурса** , **Задатак** , приказ **Сравњење** , **Процене трошкова** ) се могу уређивати чак и када пројекат није активан.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-125">The **Project** form grids ( **Resource Assignment** , **Task** , **Reconciliation** view, **Expense Estimates** ) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="8d0a9-126">Дуплирани клијенти се не могу објединити са клијентима који су повезани са потврђеним уговорима за пројекат.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="8d0a9-127">Када се дода ресурс који нема важећи календар, систем не враћа поруку о грешци прилагођену кориснику.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="8d0a9-128">Дугме **Додај задатак** на мрежи задатака је омогућено када је пројекат повезан на **програмски додатака за Microsoft Project**.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="8d0a9-129">Напор неконтролисано расте када је задатак са категоријом додељен ресурсу са улогом за коју је дефинисана цена коштања.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="8d0a9-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="8d0a9-130">**Sales**</span></span>

<span data-ttu-id="8d0a9-131">Унета су следећа побољшања:</span><span class="sxs-lookup"><span data-stu-id="8d0a9-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="8d0a9-132">**Учесталост фактурисања** и **Почетак наплате** су пресељени на картицу **Распоред фактурисања**.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="8d0a9-133">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="8d0a9-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="8d0a9-134">**Укупна продајна цена** је нула (0) за **Категорију** , мада **Улога** има укупну продајну цену која није нула.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="8d0a9-135">Клијенти не могу да мењају вредност поља **Статус фактуре** на **Спремно за фактурисање** када неки други прилагођени процес ажурира додатно поље.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="8d0a9-136">Дугме **Освежи ставке фактуре** може да креира више дуплираних ставки ако се више пута изаберу.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="8d0a9-137">Дугме **Ажурирај цене** не ради на подобрасцу **Цене улога** у обрасцу **Брзи преглед**.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-137">The **Update Prices** button doesn't work on the **Role Prices** sub-grid in the **Quick View** form.</span></span>
- <span data-ttu-id="8d0a9-138">Логика **Решење продајног ценовника** неправилно рукује временским зонама, што резултира погрешним одабиром ценовника.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="8d0a9-139">**Укупни стварни трошак** пројекта се може искључити једним делом након што се одобри једна ставка времена.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="8d0a9-140">Логика **Решење цена** не даје поруку о грешци прилагођену кориснику ако **Враћена цена улоге** нема вредности у пољима **'Примарна јединица'** и **'Цена у основној јединици'**.</span><span class="sxs-lookup"><span data-stu-id="8d0a9-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>
