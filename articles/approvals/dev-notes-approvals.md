---
title: Напомене програмера за одобрења
description: У овој теми се пружају додатне информације програмера о раду са одобрењима.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996809"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="8456e-103">Напомене програмера за одобрења</span><span class="sxs-lookup"><span data-stu-id="8456e-103">Developer notes for Approvals</span></span>

<span data-ttu-id="8456e-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="8456e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8456e-105">Dynamics 365 Project Operations укључује логику провере која осигурава тачан прелаз записа кроз фазе одобрења.</span><span class="sxs-lookup"><span data-stu-id="8456e-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="8456e-106">Тачни прелази записа осигуравају:</span><span class="sxs-lookup"><span data-stu-id="8456e-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="8456e-107">Сви подржани редови се креирају у повезаним табелама, као што су дневници и стварне вредности.</span><span class="sxs-lookup"><span data-stu-id="8456e-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="8456e-108">Давалац одобрења се означава као **Давалац одобрења за пројекат** у пројекту пре него што наставите.</span><span class="sxs-lookup"><span data-stu-id="8456e-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]