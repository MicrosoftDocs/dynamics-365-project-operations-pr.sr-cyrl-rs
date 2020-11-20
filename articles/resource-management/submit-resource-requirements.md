---
title: Прослеђивање захтева за ресурсом
description: Генерисану потребу за ресурсом можете проследити као захтев за ресурс. Захтев се затим шаље менаџеру ресурса ради испуњавања.
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 18f43acc64ed72b1543a2d7d91a2648e7e185fc4
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128841"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="a04d3-104">Прослеђивање захтева за ресурсом</span><span class="sxs-lookup"><span data-stu-id="a04d3-104">Submit a resource request</span></span>

<span data-ttu-id="a04d3-105">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="a04d3-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a04d3-106">Генерисану потребу за ресурсом можете проследити као захтев за ресурс.</span><span class="sxs-lookup"><span data-stu-id="a04d3-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="a04d3-107">Захтев се затим шаље менаџеру ресурса ради испуњавања.</span><span class="sxs-lookup"><span data-stu-id="a04d3-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="a04d3-108">У услузи Dynamics 365 Project Operations, на страници **Пројекти** изаберите картицу **Тим** да бисте видели листу ресурса који се могу резервисати.</span><span class="sxs-lookup"><span data-stu-id="a04d3-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="a04d3-109">Са листе изаберите генерички ресурс који има потребу за ресурсом, а затим кликните на **Проследи захтев**.</span><span class="sxs-lookup"><span data-stu-id="a04d3-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="a04d3-110">Статус захтева генеричког члана тима ће се променити у **Прослеђен**.</span><span class="sxs-lookup"><span data-stu-id="a04d3-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="a04d3-111">Када се захтев испуни, генерички ресурс се мења именованим ресурсом ако менаџер ресурса испуни захтев резервисањем именованог ресурса.</span><span class="sxs-lookup"><span data-stu-id="a04d3-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="a04d3-112">У супротном, ако менаџер ресурса предложи именовани ресурс, генерички ресурс остаје у тиму и статус захтева ће се променити у **Захтева преглед**.</span><span class="sxs-lookup"><span data-stu-id="a04d3-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>
