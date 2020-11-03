---
title: Ажурирање процене по завршетку
description: Ова тема пружа информације о ажурирању пројекције ангажовања на пројекту.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 16393133a5de17308caceb069d7bca670caa04c8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084155"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="439e7-103">Ажурирање процене по завршетку</span><span class="sxs-lookup"><span data-stu-id="439e7-103">Update estimate at completion</span></span>

<span data-ttu-id="439e7-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="439e7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="439e7-105">Уобичајено је да менаџер пројекта ревидира оригиналне процене задатка.</span><span class="sxs-lookup"><span data-stu-id="439e7-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="439e7-106">Поновне пројекције пројеката представљају начин на који менаџер пројекта перципира процене, с обзиром на тренутни статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="439e7-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="439e7-107">Међутим, не препоручујемо да менаџери пројекта мењају основне вредности зато што основне вредности пројекта представљају успостављен извор истине за распоред пројекта и процену трошкова, а сви заинтересовани за пројекат су је прихватили.</span><span class="sxs-lookup"><span data-stu-id="439e7-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="439e7-108">Постоје два начина на које менаџер пројекта може поново да пројектује ангажовање на задацима:</span><span class="sxs-lookup"><span data-stu-id="439e7-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="439e7-109">Измените подразумевану процену завршетка (ETC) новом проценом стварног преосталог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="439e7-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="439e7-110">Измените подразумевани проценат напретка новом проценом стварног напретка задатка.</span><span class="sxs-lookup"><span data-stu-id="439e7-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="439e7-111">Сваки од ових приступа доводи до тога да се поново израчунају ETC, процена завршетка (EAC) и проценат напретка задатка, као и одступање од пројектованог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="439e7-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="439e7-112">EAC, ETC и проценат напретка у резимираним задацима се поново израчунавају и стварају нову пројекцију одступања од ангажовања.</span><span class="sxs-lookup"><span data-stu-id="439e7-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
