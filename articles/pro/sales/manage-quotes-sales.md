---
title: Управљање понудама за пројекат
description: Ова тема пружа информације о понудама за пројекат.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3c33adabbd03cca19ae5e7f401f08a716e9242b2
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177844"
---
# <a name="manage-project-quotes"></a><span data-ttu-id="69d79-103">Управљање понудама за пројекат</span><span class="sxs-lookup"><span data-stu-id="69d79-103">Manage project quotes</span></span>

<span data-ttu-id="69d79-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="69d79-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="69d79-105">У услузи Dynamics 365 Project Operations, понуде за пројекат се праве тако да помогну у изради предлога за пројектни задатак.</span><span class="sxs-lookup"><span data-stu-id="69d79-105">In Dynamics 365 Project Operations, project quotes are designed to help build proposals for project work.</span></span> <span data-ttu-id="69d79-106">Структура понуде за пројекат у услузи Project Operations структурирана је за предлоге за пројекат са следећим компонентама:</span><span class="sxs-lookup"><span data-stu-id="69d79-106">The structure of a project quote in Project Operations is structured for project proposals with the following components:</span></span>

  - <span data-ttu-id="69d79-107">Ставке понуде које идентификују дискретне компоненте посла које ће бити представљене као компоненте на високом нивоу.</span><span class="sxs-lookup"><span data-stu-id="69d79-107">Quote lines that identify the discrete components of work that will be presented as high-level components.</span></span>
  - <span data-ttu-id="69d79-108">Детаљи ставке понуде који идентификују и процењују посао за сваку компоненту или ставку понуде на високом нивоу.</span><span class="sxs-lookup"><span data-stu-id="69d79-108">Quote line details that identify and estimate the work for each high-level component or quote line.</span></span> <span data-ttu-id="69d79-109">Процене распореда или датума у финансијски аспекти посла су повезани са том ставком понуде.</span><span class="sxs-lookup"><span data-stu-id="69d79-109">Schedule or date estimates and the financial aspects for the work are tied to that quote line.</span></span>
  - <span data-ttu-id="69d79-110">Модели уговарања и наплативе компоненте постављају се за сваку ставку понуде.</span><span class="sxs-lookup"><span data-stu-id="69d79-110">Contracting models and chargeable components are set up for each quote line.</span></span> <span data-ttu-id="69d79-111">Ова поставка помаже у процени ширења прихода, потрошње и исплативости за сваку ставку понуде и укупну цену.</span><span class="sxs-lookup"><span data-stu-id="69d79-111">This set up helps estimate the spread of revenue, spend, and profitability for each quote line and the overall quote.</span></span>

## <a name="view-all-project-based-quotes"></a><span data-ttu-id="69d79-112">Приказ свих понуда заснованих на пројекту</span><span class="sxs-lookup"><span data-stu-id="69d79-112">View all project-based quotes</span></span>

<span data-ttu-id="69d79-113">Листа свих понуда за пројекат може се видети на страници листе **Понуде**.</span><span class="sxs-lookup"><span data-stu-id="69d79-113">A list of all the project quotes can be seen from the **Quotes** list page.</span></span> 

1. <span data-ttu-id="69d79-114">Идите на ставку **Продаја** > **Понуде**.</span><span class="sxs-lookup"><span data-stu-id="69d79-114">Go to **Sales** > **Quotes**.</span></span> <span data-ttu-id="69d79-115">Приказана је листа свих ваших понуда за пројекат у систему.</span><span class="sxs-lookup"><span data-stu-id="69d79-115">A list of all your project quotes in the system are shown.</span></span> 
2. <span data-ttu-id="69d79-116">Користите **Пребацивач приказа** да бисте изабрали друге филтриране приказе понуда.</span><span class="sxs-lookup"><span data-stu-id="69d79-116">Use the **View Switcher** to select other filtered views of the quotes.</span></span> <span data-ttu-id="69d79-117">Користећи прилагођене критеријуме филтера, можете да конфигуришете своје приказе и опције навигације.</span><span class="sxs-lookup"><span data-stu-id="69d79-117">Using custom filter criteria, you can configure your own views and navigation options.</span></span>

<span data-ttu-id="69d79-118">Понуде се могу креирати или избрисати са ове странице листе или страница са детаљима.</span><span class="sxs-lookup"><span data-stu-id="69d79-118">Quotes can be created or deleted from this list page or detail pages.</span></span>
