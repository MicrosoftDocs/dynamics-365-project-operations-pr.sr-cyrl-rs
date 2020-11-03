---
title: Резервације у односу на доделе
description: Ова тема пружа информације о разликама између резервисања ресурса и додељивања ресурса.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fa99783e52dbcdeaf80bbfd03df0f458f86b5e99
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083821"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="034ad-103">Резервације у односу на доделе</span><span class="sxs-lookup"><span data-stu-id="034ad-103">Bookings vs assignments</span></span>

<span data-ttu-id="034ad-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="034ad-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="034ad-105">Резервације представљају фиксну или условну расподелу ресурса за пројекат.</span><span class="sxs-lookup"><span data-stu-id="034ad-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="034ad-106">Фиксне резервације троше капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="034ad-106">Hard bookings consume a resource's capacity.</span></span> 

<span data-ttu-id="034ad-107">Доделе представљају додела ресурса пројектним задацима у распореду пројеката.</span><span class="sxs-lookup"><span data-stu-id="034ad-107">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="034ad-108">Ресурси могу бити стварни или генерички.</span><span class="sxs-lookup"><span data-stu-id="034ad-108">The resources can be real or generic.</span></span> 

<span data-ttu-id="034ad-109">Идеално би било да се за стварне ресурсе слажу резервације и доделе, јер се не разликују.</span><span class="sxs-lookup"><span data-stu-id="034ad-109">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="034ad-110">Међутим, Microsoft Dynamics Project Operations не спроводи овај договор.</span><span class="sxs-lookup"><span data-stu-id="034ad-110">However, Microsoft Dynamics Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="034ad-111">Приказ **Усаглашеност** показује менаџеру пројеката места где се резервације и доделе ресурса не слажу.</span><span class="sxs-lookup"><span data-stu-id="034ad-111">The **Reconciliation** view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>
