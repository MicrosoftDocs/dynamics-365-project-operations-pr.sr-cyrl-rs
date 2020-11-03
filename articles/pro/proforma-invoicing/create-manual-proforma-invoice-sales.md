---
title: Креирање ручног предрачуна
description: Ова тема пружа информације о креирању ручног предрачуна у услузи Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5e93206737507bf6698a9746815c790d3dfc904
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/20/2020
ms.locfileid: "4084201"
---
# <a name="creating-a-manual-proforma-invoice"></a><span data-ttu-id="19e38-103">Креирање ручног предрачуна</span><span class="sxs-lookup"><span data-stu-id="19e38-103">Creating a manual proforma invoice</span></span>

<span data-ttu-id="19e38-104">_**Односи се на:** Једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="19e38-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="19e38-105">У услузи Dynamics 365 Project Operations, предрачуни се по потреби могу креирати ручно.</span><span class="sxs-lookup"><span data-stu-id="19e38-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="19e38-106">Можете ручно да креирате предрачун са странице листа **Уговори о пројекту** или са странице са детаљима **Уговор о пројекту**.</span><span class="sxs-lookup"><span data-stu-id="19e38-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="19e38-107">Страница листе уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="19e38-107">Project Contracts list page</span></span>

<span data-ttu-id="19e38-108">Са странице листе **Уговори о пројекту** одаберите један или више пројектних уговора и креирајте фактуре за све изабране записе.</span><span class="sxs-lookup"><span data-stu-id="19e38-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="19e38-109">Систем проверава који од изабраних пројектних уговора има заостатак **Спремно за фактурисање** датиран пре данашњег датума.</span><span class="sxs-lookup"><span data-stu-id="19e38-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="19e38-110">Од тих уговора систем креира радне верзије предрачуна.</span><span class="sxs-lookup"><span data-stu-id="19e38-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="19e38-111">Ако пројектни уговор има више клијената, може се креирати једна фактура по клијенту и више фактура по уговору о пројекту.</span><span class="sxs-lookup"><span data-stu-id="19e38-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="19e38-112">Све креиране фактуре пројекта су доступне на страници **Фактура** у одељку **Наплата** области **Продаја**.</span><span class="sxs-lookup"><span data-stu-id="19e38-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="19e38-113">Страница са детаљима уговора за пројекат</span><span class="sxs-lookup"><span data-stu-id="19e38-113">Project Contract details page</span></span>

<span data-ttu-id="19e38-114">Предфактура се такође може креирати са странице са детаљима **Уговор о пројекту** , која креира фактуру за тај конкретни уговор о пројекту.</span><span class="sxs-lookup"><span data-stu-id="19e38-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="19e38-115">Систем проверава да пројектни уговор има заостатак **Спремно за фактурисање** датиран пре данашњег датума.</span><span class="sxs-lookup"><span data-stu-id="19e38-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="19e38-116">Од ових уговора систем креира радне верзије предрачуна на основу броја клијената у сваком предмету уговора.</span><span class="sxs-lookup"><span data-stu-id="19e38-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="19e38-117">Када се креира један предрачун, отвара се страница **Фактура**.</span><span class="sxs-lookup"><span data-stu-id="19e38-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="19e38-118">Ако је за тај уговор о пројекту креирано више фактура, отвара се страница листе **Фактуре** са приказом свих креираних фактура.</span><span class="sxs-lookup"><span data-stu-id="19e38-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
