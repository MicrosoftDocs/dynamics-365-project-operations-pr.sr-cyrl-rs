---
title: Шта је ново или промењено у Project Service Automation издању исправке 20 у верзији 3
description: У овој теми дате су функције и исправке које су доступне у Project Service Automation издању исправке 20 у верзији 3
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: ef24c20f3fa520b25a14773a15363a0f04f98d36
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126771"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="bcb14-103">Project Service Automation издање исправке 20, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="bcb14-103">Project Service Automation Update Release 20, V3</span></span>

<span data-ttu-id="bcb14-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="bcb14-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="bcb14-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="bcb14-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="bcb14-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="bcb14-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="bcb14-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="bcb14-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="bcb14-108">За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="bcb14-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="bcb14-109">У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 20.</span><span class="sxs-lookup"><span data-stu-id="bcb14-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="bcb14-110">Број израде ове верзије је V 3.10.31.37 и углавном је доступна путем самосталног ажурирања у јуну 2020. године.</span><span class="sxs-lookup"><span data-stu-id="bcb14-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="bcb14-111">Издање исправке 20</span><span class="sxs-lookup"><span data-stu-id="bcb14-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="bcb14-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="bcb14-112">Bug fixes</span></span>

<span data-ttu-id="bcb14-113">**Управљање пројектима**</span><span class="sxs-lookup"><span data-stu-id="bcb14-113">**Project Management**</span></span>

<span data-ttu-id="bcb14-114">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="bcb14-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="bcb14-115">Увоз чланова пројектног тима методом расподеле која захтева сате резултира нејасном поруком о грешци када су наведени сати нула.</span><span class="sxs-lookup"><span data-stu-id="bcb14-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="bcb14-116">Корисници добијају погрешну грешку када је у поље **Опис** унет максималан број знакова за пројектни задатак.</span><span class="sxs-lookup"><span data-stu-id="bcb14-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="bcb14-117">Страница **Преузимање Microsoft Dynamics 365 Project Service Automation програмског додатка** се преусмерава на енглеску страницу за преузимање када су подешавања језика корисника подешене на јапански.</span><span class="sxs-lookup"><span data-stu-id="bcb14-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="bcb14-118">Када дође до грешке на серверу, ознака синхронизације на картици **Распоред** обрасца **Пројекти** понекад остаје.</span><span class="sxs-lookup"><span data-stu-id="bcb14-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="bcb14-119">Сувишна ажурирања задатака се шаљу серверу када је задатак измењен.</span><span class="sxs-lookup"><span data-stu-id="bcb14-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="bcb14-120">**Sales**</span><span class="sxs-lookup"><span data-stu-id="bcb14-120">**Sales**</span></span>

<span data-ttu-id="bcb14-121">Поправљени су следећи проблеми:</span><span class="sxs-lookup"><span data-stu-id="bcb14-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="bcb14-122">На обрасцу **Уговор**, двоструки клик на **Креирај фактуру** креира две фактуре за један стварни запис.</span><span class="sxs-lookup"><span data-stu-id="bcb14-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="bcb14-123">У решењу Internet Explorer 11,корисници не могу да креирају ставке трошкова.</span><span class="sxs-lookup"><span data-stu-id="bcb14-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="bcb14-124">Сторнирање трошкова и сторнирање ненаплаћених стварних података о продаји нису повезани.</span><span class="sxs-lookup"><span data-stu-id="bcb14-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="bcb14-125">Дугме **Освежи стварне трошкове** на обрасцу **Пројекат** не освежава ставку **Стварни сати за задатак**.</span><span class="sxs-lookup"><span data-stu-id="bcb14-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="bcb14-126">Додатна компонента **PreValidateProjectTeamMemberCreate** може да креира дуплиране генеричке ресурсе који могу да се резервишу када је атрибут **msdyn_isgenericresourceprojectscoped** подешен на **Нетачно**.</span><span class="sxs-lookup"><span data-stu-id="bcb14-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="bcb14-127">**Поново израчунај** брише наплативе трошкове детаља понуде засноване на производу и детаље предмета уговора.</span><span class="sxs-lookup"><span data-stu-id="bcb14-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="bcb14-128">У одређеним сценаријима додатна компонента **PostEstimateLineUpdate** приказује грешку изузетка недефинисане референце.</span><span class="sxs-lookup"><span data-stu-id="bcb14-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="bcb14-129">Трајање временске фазе на **Графикону анализе профитабилности** се не подудара се са трајањем трошкова у детаљима линије понуде са фиксном ценом на понуди.</span><span class="sxs-lookup"><span data-stu-id="bcb14-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="bcb14-130">Вредности за јединицу и групу јединица не постају исправно подразумевано за категорије трошкова у обрасцима **Детаљи о предмету уговора** и **Детаљи ставке понуде**.</span><span class="sxs-lookup"><span data-stu-id="bcb14-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="bcb14-131">Листе **Цена коштања по јединици за организацију** дозвољавају преклапање ефикасности датума.</span><span class="sxs-lookup"><span data-stu-id="bcb14-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="bcb14-132">Корисницима није дозвољено да мењају **OrgUnit** када тип поруџбине није заснован на раду јер ће довести до грешке изузетка непостојеће референце.</span><span class="sxs-lookup"><span data-stu-id="bcb14-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="bcb14-133">При покушају кретања из обрасца **Детаљи ставке понуде** натраг на картицу **Понуда**, образац се освежава и приказује картицу **Резиме**.</span><span class="sxs-lookup"><span data-stu-id="bcb14-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>
