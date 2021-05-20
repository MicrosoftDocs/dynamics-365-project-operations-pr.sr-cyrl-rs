---
title: Купујте нескладиштени материјал користећи фактуру добављача на чекању
description: Ова тема објашњава како да снимите фактуре добављача на чекању.
author: sigitac
manager: tfehr
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7a706f419443dcdf92ce3b247d719943272907d0
ms.sourcegitcommit: 7468d668c48c1d87934aab9a034decd51e56dec6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/13/2021
ms.locfileid: "5880682"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="e57a6-103">Купујте нескладиштени материјал користећи фактуру добављача на чекању</span><span class="sxs-lookup"><span data-stu-id="e57a6-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="e57a6-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="e57a6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e57a6-105">Како компанија набавља не-залихе материјала за пројекат, трошкови се могу одмах евидентирати у односу на пројекат.</span><span class="sxs-lookup"><span data-stu-id="e57a6-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="e57a6-106">На пример, Contoso Robotics US изводи пројекат обнове опреме и потребне су софтверске лиценце.</span><span class="sxs-lookup"><span data-stu-id="e57a6-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="e57a6-107">Ове лиценце се набављају од независног добављача.</span><span class="sxs-lookup"><span data-stu-id="e57a6-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="e57a6-108">Користећи Dynamics 365 Finance, службеник за дуговања евидентира документ фактуре добављача на чекању и приписује трошкове лиценце директно пројекту обнове опреме.</span><span class="sxs-lookup"><span data-stu-id="e57a6-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="e57a6-109">Пре него што употребите функционалност описану у овој теми, прегледајте и примените потребне конфигурације.</span><span class="sxs-lookup"><span data-stu-id="e57a6-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="e57a6-110">За више информација погледајте [Омогућите нескладиштени материјал и фактуре добављача на чекању](configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="e57a6-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="e57a6-111">Пошаљите фактуру добављача на чекању у вези са пројектом</span><span class="sxs-lookup"><span data-stu-id="e57a6-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="e57a6-112">Фактуре добављача на чекању могу се евидентирати на страници **Фактуре добављача на чекању** (**Дуговања** > **Фактуре** > **Фактуре добављача на чекању**).</span><span class="sxs-lookup"><span data-stu-id="e57a6-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="e57a6-113">Довршите следеће кораке да бисте књижили фактуру добављача на чекању у вези са пројектом:</span><span class="sxs-lookup"><span data-stu-id="e57a6-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="e57a6-114">Идите на **Дуговања** > **Фактуре** и изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="e57a6-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="e57a6-115">У пољу **Рачун фактуре** изаберите добављача и у поље **Број** унесите идентификацију рачуна добављача.</span><span class="sxs-lookup"><span data-stu-id="e57a6-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="e57a6-116">Додајте ред на фактуру добављача и у поље **Број предмета** изаберите артикал на залихама купљен од добављача.</span><span class="sxs-lookup"><span data-stu-id="e57a6-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="e57a6-117">Редови фактура добављача који се заснивају на категорији набавке не могу се евидентирати у пројекту.</span><span class="sxs-lookup"><span data-stu-id="e57a6-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="e57a6-118">Додајте купљену количину.</span><span class="sxs-lookup"><span data-stu-id="e57a6-118">Add the quantity purchased.</span></span> <span data-ttu-id="e57a6-119">Систем ће попунити јединичну цену на основу конфигурације цене залиха на залихама.</span><span class="sxs-lookup"><span data-stu-id="e57a6-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="e57a6-120">Потврдите укупан износ и остале потребне детаље на линији.</span><span class="sxs-lookup"><span data-stu-id="e57a6-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="e57a6-121">На линији детаљи, на картици **Пројекат** одаберите ID пројекта на који ће се снимати ова ставка.</span><span class="sxs-lookup"><span data-stu-id="e57a6-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="e57a6-122">По жељи одаберите број активности и ажурирајте категорију пројекта и својство линије.</span><span class="sxs-lookup"><span data-stu-id="e57a6-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="e57a6-123">Пошаљите фактуру добављача на чекању.</span><span class="sxs-lookup"><span data-stu-id="e57a6-123">Post pending vendor invoice.</span></span> <span data-ttu-id="e57a6-124">Када је фактура књижена, систем бележи:</span><span class="sxs-lookup"><span data-stu-id="e57a6-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="e57a6-125">Износ биланса добављача.</span><span class="sxs-lookup"><span data-stu-id="e57a6-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="e57a6-126">Износ пореза на промет.</span><span class="sxs-lookup"><span data-stu-id="e57a6-126">The sales tax amount.</span></span>
    - <span data-ttu-id="e57a6-127">Трошкови пројекта евидентирају се на рачун интеграције набавки.</span><span class="sxs-lookup"><span data-stu-id="e57a6-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="e57a6-128">Стварна трансакција пројекта у Dataverse.</span><span class="sxs-lookup"><span data-stu-id="e57a6-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="e57a6-129">Ова трансакција се даље обрађује помоћу [Project Operations дневника интеграције](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="e57a6-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="e57a6-130">Објављивањем овог дневника премешта се износ са рачуна интеграције набавки на рачун трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="e57a6-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
