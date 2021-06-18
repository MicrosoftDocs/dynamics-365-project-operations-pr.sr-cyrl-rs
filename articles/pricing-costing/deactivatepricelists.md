---
title: Деактивирање ценовника
description: Ова тема објашњава како да деактивирате или уклоните неискоришћене или старе ценовнике.
author: rumant
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d5d6cf6b4b097c08edca5a3235ed1b438a0eae2d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001354"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="98499-103">Деактивирање ценовника</span><span class="sxs-lookup"><span data-stu-id="98499-103">Deactivate price lists</span></span> 

<span data-ttu-id="98499-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="98499-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="98499-105">Да бисте уклонили старе или неискоришћене ценовнике из услуге Dynamics 365 Project Operations, постоје два корака која морате извршити.</span><span class="sxs-lookup"><span data-stu-id="98499-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="98499-106">Уклоните или избришите ценовник са одређених страница.</span><span class="sxs-lookup"><span data-stu-id="98499-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="98499-107">Деактивирајте или избришите ценовник из активних ценовника на страници **Ценовници**.</span><span class="sxs-lookup"><span data-stu-id="98499-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="98499-108">Морате обавити оба корака да бисте у потпуности уклонили ценовник.</span><span class="sxs-lookup"><span data-stu-id="98499-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="98499-109">Није довољно да обавите само 2. корак, а то је директно брисање или деактивирање ценовника из приказа Активни ценовници.</span><span class="sxs-lookup"><span data-stu-id="98499-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="98499-110">Морате избрисати и повезивање овог ценовника са свих места поменутих у 1. кораку.</span><span class="sxs-lookup"><span data-stu-id="98499-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="98499-111">Брисање ценовника са одређених страница</span><span class="sxs-lookup"><span data-stu-id="98499-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="98499-112">Да бисте избрисали ценовник из услуге Project Operations, идите на следеће странице:</span><span class="sxs-lookup"><span data-stu-id="98499-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="98499-113">Страница **Параметри пројекта** > картица **Ценовници**</span><span class="sxs-lookup"><span data-stu-id="98499-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="98499-114">Страница **Организациона јединица** > мрежа **Ценовници**</span><span class="sxs-lookup"><span data-stu-id="98499-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="98499-115">Страница **Пословни контакт** > мрежа **Ценовници пројекта**</span><span class="sxs-lookup"><span data-stu-id="98499-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="98499-116">Страница **Понуде за пројекат** > мрежа **Ценовници пројекта**: Ово се односи на све активне понуде за пројекат.</span><span class="sxs-lookup"><span data-stu-id="98499-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="98499-117">Страница **Уговори о пројекту** > мрежа **Ценовници пројекта**: Ово се односи на све активне уговоре о пројекту.</span><span class="sxs-lookup"><span data-stu-id="98499-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="98499-118">За сваку страницу, морате изабрати ценовник који желите да избришете, а затим изаберите **Избриши**.</span><span class="sxs-lookup"><span data-stu-id="98499-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="98499-119">Брисање или деактивирање ценовника са странице Ценовници</span><span class="sxs-lookup"><span data-stu-id="98499-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="98499-120">Да бисте избрисали ценовник из активних ценовника, идите на **Продаја** > **Клијенти** > **Ценовници**.</span><span class="sxs-lookup"><span data-stu-id="98499-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="98499-121">Изаберите ценовник који желите да избришете, а затим изаберите **Избриши**.</span><span class="sxs-lookup"><span data-stu-id="98499-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="98499-122">Ако се ценовник користи у било којој трансакцији, нећете моћи да га избришете.</span><span class="sxs-lookup"><span data-stu-id="98499-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="98499-123">Ако се то догоди, можете деактивирати ценовник тако да се не приказује ни у једном приказу.</span><span class="sxs-lookup"><span data-stu-id="98499-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="98499-124">Да бисте деактивирали ценовник, поново изаберите ценовник, а затим изаберите **Деактивирај**.</span><span class="sxs-lookup"><span data-stu-id="98499-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
