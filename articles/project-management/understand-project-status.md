---
title: Разумевање статуса пројекта
description: Ова тема пружа информације о статусу додељеном пројектима у услузи Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bc5bc174518e46b32cf88ea7231bb2df10fde292
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127311"
---
# <a name="understand-project-status"></a><span data-ttu-id="4576b-103">Разумевање статуса пројекта</span><span class="sxs-lookup"><span data-stu-id="4576b-103">Understand project status</span></span>

<span data-ttu-id="4576b-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="4576b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="4576b-105">Одељак **Статус** на страници **Ентитет пројекта** пружа резиме стања исправности пројекта на основу трошкова и ангажовања.</span><span class="sxs-lookup"><span data-stu-id="4576b-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="4576b-106">Поља резимеа статуса</span><span class="sxs-lookup"><span data-stu-id="4576b-106">Status summary fields</span></span>

- <span data-ttu-id="4576b-107">Поље **Општи статус пројекта** је поље које може да се уређује и које показује општи статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="4576b-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="4576b-108">Ово поље користи кодирање у боји, као што су зелена, жута и црвена, да укаже на повећани ризик.</span><span class="sxs-lookup"><span data-stu-id="4576b-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="4576b-109">Поље **Коментари** омогућава менаџеру пројекта да унесе конкретне коментаре о статусу.</span><span class="sxs-lookup"><span data-stu-id="4576b-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="4576b-110">Поље **Датум ажурирања статуса** није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="4576b-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="4576b-111">Вредност у овом пољу је временска ознака која показује када је статус последњи пут ажуриран.</span><span class="sxs-lookup"><span data-stu-id="4576b-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="4576b-112">Поља **Перформансе распореда** и **Перформансе трошкова** су подешена из мреже за праћење.</span><span class="sxs-lookup"><span data-stu-id="4576b-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="4576b-113">Када су одступања од распореда и трошкова за основни чвор у приказу **Праћење ангажовања** позитивна, ова поља се ажурирају на **Пре плана**.</span><span class="sxs-lookup"><span data-stu-id="4576b-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="4576b-114">Када су одступања од распореда и трошкова за основни чвор негативна, ова поља се подешавају на **Заостаје за планом**.</span><span class="sxs-lookup"><span data-stu-id="4576b-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
