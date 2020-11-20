---
title: Ажурирање процене по завршетку
description: Ова тема пружа информације о ажурирању пројекције ангажовања на пројекту.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 59d04869839cebd6e197f94f2ada8ab12c495c3b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127221"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="b2dbd-103">Ажурирање процене по завршетку</span><span class="sxs-lookup"><span data-stu-id="b2dbd-103">Update estimate at completion</span></span>

<span data-ttu-id="b2dbd-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="b2dbd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b2dbd-105">Уобичајено је да менаџер пројекта ревидира оригиналне процене задатка.</span><span class="sxs-lookup"><span data-stu-id="b2dbd-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="b2dbd-106">Поновне пројекције пројеката представљају начин на који менаџер пројекта перципира процене, с обзиром на тренутни статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="b2dbd-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="b2dbd-107">Међутим, не препоручујемо да менаџери пројекта мењају основне вредности зато што основне вредности пројекта представљају успостављен извор истине за распоред пројекта и процену трошкова, а сви заинтересовани за пројекат су је прихватили.</span><span class="sxs-lookup"><span data-stu-id="b2dbd-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="b2dbd-108">Постоје два начина на које менаџер пројекта може поново да пројектује ангажовање на задацима:</span><span class="sxs-lookup"><span data-stu-id="b2dbd-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="b2dbd-109">Измените подразумевану процену завршетка (ETC) новом проценом стварног преосталог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="b2dbd-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="b2dbd-110">Измените подразумевани проценат напретка новом проценом стварног напретка задатка.</span><span class="sxs-lookup"><span data-stu-id="b2dbd-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="b2dbd-111">Сваки од ових приступа доводи до тога да се поново израчунају ETC, процена завршетка (EAC) и проценат напретка задатка, као и одступање од пројектованог ангажовања на задатку.</span><span class="sxs-lookup"><span data-stu-id="b2dbd-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="b2dbd-112">EAC, ETC и проценат напретка у резимираним задацима се поново израчунавају и стварају нову пројекцију одступања од ангажовања.</span><span class="sxs-lookup"><span data-stu-id="b2dbd-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
