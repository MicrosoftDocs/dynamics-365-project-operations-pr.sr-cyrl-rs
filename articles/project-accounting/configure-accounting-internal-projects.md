---
title: Конфигурисање рачуноводства за интерне пројекте
description: Ова тема пружа информације о томе како поставити рачуноводствене праксе за интерне пројекте у услузи Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 504e7481cb2aee6310cb4ace2d0791d1c7fe360d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083906"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="c1ce1-103">Конфигурисање рачуноводства за интерне пројекте</span><span class="sxs-lookup"><span data-stu-id="c1ce1-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="c1ce1-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="c1ce1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c1ce1-105">Интерни пројекти омогућавају компанијама да прате трошкове повезане са активностима које се не наплаћују клијенту.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="c1ce1-106">Примери интерних пројеката укључују:</span><span class="sxs-lookup"><span data-stu-id="c1ce1-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="c1ce1-107">Развој производа, као што је апликација за мобилне уређаје, и праћење трошкова повезаних са развојем.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="c1ce1-108">Управљање временом и трошковима претпродаје.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="c1ce1-109">Овај интерни пројекат у претпродаји може се касније претворити у наплативи пројекат ако се добије понуда.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="c1ce1-110">Било који пројекат који није повезан са уговором у производу Dynamics 365 Project Operations се третира као интерни.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="c1ce1-111">Профили трошкова и прихода пројекта не користе се за одређивање рачуноводствених правила за пројекат.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="c1ce1-112">Интерни трошкови пројекта се увек књиже према принципима добити и губитка.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="c1ce1-113">Књиговодствени рачуни за књижења дефинисани су на страници **Подешавање књижења у књизи**.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="c1ce1-114">Временске трансакције се књиже задуживањем налога **Трошак** и кредитирањем налога **Расподела зарада**.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="c1ce1-115">Трансакције трошкова се књиже задуживањем налога **Цена** и кредитирањем налога **Рачун за пребијање дуговања и потраживања за трошкове**.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>

<span data-ttu-id="c1ce1-116">Након што су трансакције књижене у пројекат, ако је пројекат повезан са пројектним уговором, систем поништава све акумулиране трансакције и креира нове наплативе трансакције.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-116">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="c1ce1-117">Трансакције које се наплаћују прате рачуноводствена правила дефинисана у одговарајућем профилу трошкова и прихода пројекта.</span><span class="sxs-lookup"><span data-stu-id="c1ce1-117">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>


