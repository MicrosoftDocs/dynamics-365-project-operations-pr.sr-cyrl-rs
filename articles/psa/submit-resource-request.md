---
title: Прослеђивање захтева за ресурс
description: Ова тема пружа информације о прослеђивању захтева за ресурс пројекта.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: 173572be43149aea253bf7beddb993f8c50ab337
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149741"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="203e7-103">Прослеђивање захтева за ресурс</span><span class="sxs-lookup"><span data-stu-id="203e7-103">Submitting a resource request</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="203e7-104">Генерисану потребу за ресурсом можете проследити као захтев за ресурс.</span><span class="sxs-lookup"><span data-stu-id="203e7-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="203e7-105">Захтев се затим шаље менаџеру ресурса ради испуњавања.</span><span class="sxs-lookup"><span data-stu-id="203e7-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="203e7-106">У апликацији Project Service Automation (PSA), на страници **Пројекти** кликните на картицу **Тим** да бисте видели листу ресурса који се могу резервисати.</span><span class="sxs-lookup"><span data-stu-id="203e7-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="203e7-107">Са листе изаберите генерички ресурс који има потребу за ресурсом, а затим кликните на **Проследи захтев**.</span><span class="sxs-lookup"><span data-stu-id="203e7-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![Прослеђивање захтева за ресурс](media/RM-how-to-18.png)

<span data-ttu-id="203e7-109">Статус захтева генеричког члана тима ће се променити у **Прослеђен**.</span><span class="sxs-lookup"><span data-stu-id="203e7-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="203e7-110">Када менаџер ресурса испуни захтев, генерички ресурс ће бити замењен именованим ресурсом ако менаџер ресурса испуни захтев резервисањем именованог ресурса.</span><span class="sxs-lookup"><span data-stu-id="203e7-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="203e7-111">У супротном, генерички ресурс ће остати у тиму и статус захтева ће се променити у **Захтева преглед** ако је менаџер ресурса предложио именовани ресурс.</span><span class="sxs-lookup"><span data-stu-id="203e7-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review**, if the resource manager has proposed a named resource.</span></span>
