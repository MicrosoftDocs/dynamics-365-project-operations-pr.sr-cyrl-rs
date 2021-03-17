---
title: Креирање ручног предрачуна – једноставно
description: Ова тема пружа информације о креирању ручног предрачуна у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 104c2f3f7f0ca0682158d0f7fa0f50a4967e6dd0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274206"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="266aa-103">Креирање ручног предрачуна – једноставно</span><span class="sxs-lookup"><span data-stu-id="266aa-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="266aa-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="266aa-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="266aa-105">У услузи Dynamics 365 Project Operations, профактуре се по потреби могу креирати ручно.</span><span class="sxs-lookup"><span data-stu-id="266aa-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="266aa-106">Можете ручно да креирате предрачун са странице листа **Уговори о пројекту** или са странице са детаљима **Уговор о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="266aa-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="266aa-107">Страница листе уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="266aa-107">Project Contracts list page</span></span>

<span data-ttu-id="266aa-108">Са странице листе **Уговори о пројекту** одаберите један или више пројектних уговора и креирајте фактуре за све изабране записе.</span><span class="sxs-lookup"><span data-stu-id="266aa-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="266aa-109">Систем проверава који од изабраних пројектних уговора има заостатак **Спремно за фактурисање** датиран пре данашњег датума.</span><span class="sxs-lookup"><span data-stu-id="266aa-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="266aa-110">Од тих уговора систем креира радне верзије предрачуна.</span><span class="sxs-lookup"><span data-stu-id="266aa-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="266aa-111">Ако пројектни уговор има више клијената, може се креирати једна фактура по клијенту и више фактура по уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="266aa-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="266aa-112">Све креиране фактуре пројекта су доступне на страници **Фактура** у одељку **Наплата** области **Продаја**.</span><span class="sxs-lookup"><span data-stu-id="266aa-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="266aa-113">Страница са детаљима уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="266aa-113">Project Contract details page</span></span>

<span data-ttu-id="266aa-114">Профактура се такође може креирати на страници са детаљима **Уговор о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="266aa-114">A proforma invoice can also be created from the **Project Contract** details page.</span></span> <span data-ttu-id="266aa-115">Систем проверава да ли пројектни уговор има заостатак **Спремно за фактурисање** датиран пре данашњег датума.</span><span class="sxs-lookup"><span data-stu-id="266aa-115">The system verifies the project contract has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="266aa-116">Од ових уговора систем креира радне верзије предрачуна на основу броја клијената у сваком предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="266aa-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="266aa-117">Када се креира један предрачун, отвара се страница **Фактура**.</span><span class="sxs-lookup"><span data-stu-id="266aa-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="266aa-118">Ако се креира више фактура за тај уговор о пројекту, отвара се страница листа **Фактуре** са приказом свих креираних фактура.</span><span class="sxs-lookup"><span data-stu-id="266aa-118">If multiple invoices are created for that project contract, the **Invoices** list page opens to show all of the created invoices.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]