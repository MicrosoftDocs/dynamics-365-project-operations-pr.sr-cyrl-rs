---
title: Project Operations интеграција двоструког уписивања
description: Ова тема пружа преглед Project Operations интеграцији двоструког уписивања.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ce4f7bf8185e6f3f942df14d30d7b8d0a3e4444a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998699"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="31d23-103">Преглед Project Operations интеграције двоструког уписивања</span><span class="sxs-lookup"><span data-stu-id="31d23-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="31d23-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="31d23-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="31d23-105">Project Operations користи [могућности двоструког уписивања](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) за синхронизацију података у Microsoft Dataverse и Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="31d23-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="31d23-106">Следећа илустрација показује како се подаци синхронизују као део ове интеграције између Dataverse и Finance.</span><span class="sxs-lookup"><span data-stu-id="31d23-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![Преглед Project Operations токова података](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="31d23-108">Project Operations у Dataverse пружа модеран кориснички интерфејс (UI) и једноставну проширивост без кодирања/са мало кодирања помоћу Power Platform могућности.</span><span class="sxs-lookup"><span data-stu-id="31d23-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="31d23-109">Менаџери пројеката, менаџери ресурса, чланови пројектног тима и особе које раде са клијентима обављају своје активности у Project Operations у Dataverse.</span><span class="sxs-lookup"><span data-stu-id="31d23-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="31d23-110">Project Operations у Finance пружа подршку пројектном рачуноводству и признавању прихода.</span><span class="sxs-lookup"><span data-stu-id="31d23-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="31d23-111">Project Operations се укључују у финансијски оквир у Finance за обрачун пореза на промет, курсеве валута, извештавање о финансијској димензији и још много тога.</span><span class="sxs-lookup"><span data-stu-id="31d23-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="31d23-112">Искуства рачуновођа на пројекту углавном се темеље на Finance.</span><span class="sxs-lookup"><span data-stu-id="31d23-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="31d23-113">Project Operations интеграција састоји се од следеће интеграције компонената:</span><span class="sxs-lookup"><span data-stu-id="31d23-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="31d23-114">Project Operations подешавање и интеграција података о конфигурацији</span><span class="sxs-lookup"><span data-stu-id="31d23-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="31d23-115">Процене и стварне вредности у пројекту</span><span class="sxs-lookup"><span data-stu-id="31d23-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="31d23-116">Фактуре пројекта</span><span class="sxs-lookup"><span data-stu-id="31d23-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="31d23-117">Управљање трошковима</span><span class="sxs-lookup"><span data-stu-id="31d23-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="31d23-118">Фактура продавца</span><span class="sxs-lookup"><span data-stu-id="31d23-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
