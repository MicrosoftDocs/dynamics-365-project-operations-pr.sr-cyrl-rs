---
title: Шта је ново или промењено у издању 16 исправке Project Service Automation верзије 3
description: У овој теми дате су функције и исправке које су доступне у издању 16 исправке за Project Service Automation верзије 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
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
ms.openlocfilehash: 1f3bb4442ce1d06807f264003c930dbbee19a5c7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280911"
---
# <a name="project-service-automation-update-release-16-v3"></a><span data-ttu-id="87e4e-103">Project Service Automation издање исправке 16, у верзији 3</span><span class="sxs-lookup"><span data-stu-id="87e4e-103">Project Service Automation Update Release 16, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="87e4e-104">Задовољство нам је да објавимо најновије ажурирање за апликацију Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="87e4e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="87e4e-105">Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости.</span><span class="sxs-lookup"><span data-stu-id="87e4e-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="87e4e-106">Ово издање је компатибилно са услугом Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="87e4e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="87e4e-107">Да бисте ажурирали ово издање, посетите страницу са решењима центра за администрацију за Dynamics 365 online како бисте инсталирали исправку.</span><span class="sxs-lookup"><span data-stu-id="87e4e-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="87e4e-108">За још информација погледајте чланак [Инсталирање и исправка жељеног решења](https://docs.microsoft.com/dynamics365/project-service/upgrade-psa-home-page).</span><span class="sxs-lookup"><span data-stu-id="87e4e-108">For more information, see [Install, Update a Preferred Solution](https://docs.microsoft.com/dynamics365/project-service/upgrade-psa-home-page).</span></span>
<span data-ttu-id="87e4e-109">У овој теми дате су функције и исправке које су нове или су промењене у решењу PSA у верзији 3, издање исправке 16.</span><span class="sxs-lookup"><span data-stu-id="87e4e-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 16.</span></span> <span data-ttu-id="87e4e-110">Ова верзија има број верзије V3.10.6.34 и опште је доступна путем само-исправке у јануару 2020. године.</span><span class="sxs-lookup"><span data-stu-id="87e4e-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in January 2020.</span></span>


## <a name="update-release-16"></a><span data-ttu-id="87e4e-111">Издање исправке 16</span><span class="sxs-lookup"><span data-stu-id="87e4e-111">Update Release 16</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="87e4e-112">Исправке грешака</span><span class="sxs-lookup"><span data-stu-id="87e4e-112">Bug fixes</span></span>

-   <span data-ttu-id="87e4e-113">Време и трошак</span><span class="sxs-lookup"><span data-stu-id="87e4e-113">Time and Expense</span></span>

    -   <span data-ttu-id="87e4e-114">Исправљено: Корисници који покушавају да проследе избрисане уносе времена и трошка за одобрење ће сада примати релевантне поруке о грешци.</span><span class="sxs-lookup"><span data-stu-id="87e4e-114">Fixed: Users attempting to submit deleted time and expense entries for approvals will now receive relevant error messages.</span></span>

-   <span data-ttu-id="87e4e-115">Управљање пројектима</span><span class="sxs-lookup"><span data-stu-id="87e4e-115">Project Management</span></span>

    -   <span data-ttu-id="87e4e-116">Исправљено: јединице за обезбеђивање ресурса дефинисаних за чланове тима у шаблонима се поштују, а предлошци се примењују на нови пројекат.</span><span class="sxs-lookup"><span data-stu-id="87e4e-116">Fixed: The resourcing units defined for team members in templates are respected with the templates are applied to a new project.</span></span>

    -   <span data-ttu-id="87e4e-117">Исправљено: побољшано руковање поновним додељивањем власништва над записима.</span><span class="sxs-lookup"><span data-stu-id="87e4e-117">Fixed: Improved handling of the re-assignment of record ownership.</span></span>

    -   <span data-ttu-id="87e4e-118">Исправљено: пројекте који су у процесу копирања неће бити дозвољено копирати док се не заврше све операције копирања.</span><span class="sxs-lookup"><span data-stu-id="87e4e-118">Fixed: Projects that are in the process of being copied will not be permitted to copied until all copy operations are complete.</span></span>

-   <span data-ttu-id="87e4e-119">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="87e4e-119">Resource Management</span></span>

    -   <span data-ttu-id="87e4e-120">Исправљено: Продужи резервације сада исправно управља кратким трајањима и више не креира нула часова за продужене резервације.</span><span class="sxs-lookup"><span data-stu-id="87e4e-120">Fixed: Extend bookings now handles short durations correctly and no longer creates zero hours for extended bookings.</span></span>

    -   <span data-ttu-id="87e4e-121">Исправљено: приказ сравњења се сада приказује када је временска зона пројекта +5:30 GMT, а временска зона клијента је другачија.</span><span class="sxs-lookup"><span data-stu-id="87e4e-121">Fixed: The reconciliation view now renders when the project time zone is +5:30 GMT and the user’s time aone is different.</span></span>

-   <span data-ttu-id="87e4e-122">Sales</span><span class="sxs-lookup"><span data-stu-id="87e4e-122">Sales</span></span>

    -   <span data-ttu-id="87e4e-123">Исправљено: када се уклони пројекат мапиран на предмету уговора и мапира се нови пројекат, стварни записи о новом пројекту нису били преиспитивани на основу правила наплате и цена дефинисаних на линији уговора.</span><span class="sxs-lookup"><span data-stu-id="87e4e-123">Fixed: When a project mapped to a contract line is removed and a new project is mapped, the actual records on the new project were not getting re-evaluated based on the billing and pricing rules defined on the contract line.</span></span> <span data-ttu-id="87e4e-124">Ово је исправљено у овом издању.</span><span class="sxs-lookup"><span data-stu-id="87e4e-124">This has been fixed in this release.</span></span> <span data-ttu-id="87e4e-125">Цене и стварни записи пројекта који је скоро мапиран ће бити опозвани, па поново креирани исправно на основу правила о ценама и наплатама из предмета уговора.</span><span class="sxs-lookup"><span data-stu-id="87e4e-125">Pricing and actual records on the newly mapped project will get reversed and re-created correctly based on the pricing and billing rules of the contract line.</span></span> <span data-ttu-id="87e4e-126">Као последица овога, стварни записи о пројекту који није мапиран ће такође бити поново процењени, па поново креирани.</span><span class="sxs-lookup"><span data-stu-id="87e4e-126">The actual records of the un-mapped project will also get re-evaluated and re-created as a consequence.</span></span>

    -   <span data-ttu-id="87e4e-127">Фиксно: додата је додатна провера у ставку процене, у поље **Износ**, како би се осигурало да се нулте вредности не задржавају.</span><span class="sxs-lookup"><span data-stu-id="87e4e-127">Fixed: Additional validation has been added to an estimate line’s **Amount** field to ensure that null values are not persisted.</span></span>

    -   <span data-ttu-id="87e4e-128">Фиксно: када се на пројекту ажурира тренутно стање, у главни образац пројекта се додаје дугме за освежавање како би се корисницима омогућило да поново синхронизују тренутно стање.</span><span class="sxs-lookup"><span data-stu-id="87e4e-128">Fixed: When actuals have been updated on a project, a refresh button has been added to the project main form to allow users to re-sync the actuals.</span></span>

    -   <span data-ttu-id="87e4e-129">Фиксно: када корисници надограде са 2.X на 3.X, дозвољавају се пројекти чија је вредност за назив пројекта NULL.</span><span class="sxs-lookup"><span data-stu-id="87e4e-129">Fixed: When users upgrade from 2.X to 3.X, projects with a NULL value for project name will be permitted.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]