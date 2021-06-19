---
title: Вештине и модели стручности
description: Ова тема пружа информације о томе како да користите вештине и моделе стручности.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/13/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 976650cc71b0cdb75d5ce2d7532cd78bd91d3670
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6008689"
---
# <a name="skills-and-proficiency-models"></a><span data-ttu-id="b4fdb-103">Вештине и модели стручности</span><span class="sxs-lookup"><span data-stu-id="b4fdb-103">Skills and proficiency models</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b4fdb-104">Вештине су карактеристике ресурса које се деле између услуга Dynamics 365 Project Service Automation и Dynamics 365 Field Service (ако постоји).</span><span class="sxs-lookup"><span data-stu-id="b4fdb-104">Skills are resource characteristics that are shared between Dynamics 365 Project Service Automation and if present, Dynamics 365 Field Service.</span></span> 

<span data-ttu-id="b4fdb-105">Да бисте одржали спремиште вештина у услузи Project Service Automation, идите на **Ресурси** \> **Вештине ресурса**.</span><span class="sxs-lookup"><span data-stu-id="b4fdb-105">To maintain the repository of skills in Project Service Automation, go to **Resources** \> **Resource Skills**.</span></span> 

> ![Вештине ресурса](media/Resource-Management-image84.png)

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="b4fdb-107">Користите моделе стручности да бисте оценили ресурсе</span><span class="sxs-lookup"><span data-stu-id="b4fdb-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="b4fdb-108">Вештине за ресурсе оцењују се према моделима стручности.</span><span class="sxs-lookup"><span data-stu-id="b4fdb-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="b4fdb-109">Појединачне оцене су у моделу стручности.</span><span class="sxs-lookup"><span data-stu-id="b4fdb-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="b4fdb-110">Да бисте креирали модел стручности, идите на **Ресурси** \> **Модели стручности**, а затим изаберите **Нови**.</span><span class="sxs-lookup"><span data-stu-id="b4fdb-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="b4fdb-111">У новом моделу оцењивања наведите минималну вредност оцењивања, максималну вредност оцењивања и ентитет који се оцењује.</span><span class="sxs-lookup"><span data-stu-id="b4fdb-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="b4fdb-112">У подформи **Вредности оцена** можете дефинисати различите вредности оцењивања, од минималне до максималне.</span><span class="sxs-lookup"><span data-stu-id="b4fdb-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>

> ![Дефинисане су минималне и максималне вредности оцењивања](media/Resource-Management-image85.png)

<span data-ttu-id="b4fdb-114">Те вредности оцењивања су приказане у филтерима **Потребе за ресурсима**, **Табела распореда** и **Помоћник за заказивање**.</span><span class="sxs-lookup"><span data-stu-id="b4fdb-114">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]