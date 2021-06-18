---
title: Разумевање статуса пројекта
description: Ова тема пружа информације о статусу додељеном пројектима у услузи Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ad8c012b93bc65595dca33df1770562916c557e0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993434"
---
# <a name="understand-project-status"></a><span data-ttu-id="07b9b-103">Разумевање статуса пројекта</span><span class="sxs-lookup"><span data-stu-id="07b9b-103">Understand project status</span></span>

<span data-ttu-id="07b9b-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="07b9b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="07b9b-105">Одељак **Статус** на страници **Ентитет пројекта** пружа резиме стања исправности пројекта на основу трошкова и ангажовања.</span><span class="sxs-lookup"><span data-stu-id="07b9b-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="07b9b-106">Поља резимеа статуса</span><span class="sxs-lookup"><span data-stu-id="07b9b-106">Status summary fields</span></span>

- <span data-ttu-id="07b9b-107">Поље **Општи статус пројекта** је поље које може да се уређује и које показује општи статус пројекта.</span><span class="sxs-lookup"><span data-stu-id="07b9b-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="07b9b-108">Ово поље користи кодирање у боји, као што су зелена, жута и црвена, да укаже на повећани ризик.</span><span class="sxs-lookup"><span data-stu-id="07b9b-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="07b9b-109">Поље **Коментари** омогућава менаџеру пројекта да унесе конкретне коментаре о статусу.</span><span class="sxs-lookup"><span data-stu-id="07b9b-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="07b9b-110">Поље **Датум ажурирања статуса** није могуће уређивати.</span><span class="sxs-lookup"><span data-stu-id="07b9b-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="07b9b-111">Вредност у овом пољу је временска ознака која показује када је статус последњи пут ажуриран.</span><span class="sxs-lookup"><span data-stu-id="07b9b-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="07b9b-112">Поља **Перформансе распореда** и **Перформансе трошкова** су подешена из мреже за праћење.</span><span class="sxs-lookup"><span data-stu-id="07b9b-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="07b9b-113">Када су одступања од распореда и трошкова за основни чвор у приказу **Праћење ангажовања** позитивна, ова поља се ажурирају на **Пре плана**.</span><span class="sxs-lookup"><span data-stu-id="07b9b-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="07b9b-114">Када су одступања од распореда и трошкова за основни чвор негативна, ова поља се подешавају на **Заостаје за планом**.</span><span class="sxs-lookup"><span data-stu-id="07b9b-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]