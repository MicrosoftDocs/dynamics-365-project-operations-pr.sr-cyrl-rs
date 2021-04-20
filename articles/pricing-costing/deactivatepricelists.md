---
title: Деактивирање ценовника
description: Ова тема објашњава како да деактивирате или уклоните неискоришћене или старе ценовнике.
author: rumant
manager: AnnBe
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 3fa902e93815002be7d6915880cd7759dbbde5ef
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701970"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="f9857-103">Деактивирање ценовника</span><span class="sxs-lookup"><span data-stu-id="f9857-103">Deactivate price lists</span></span> 

<span data-ttu-id="f9857-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="f9857-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f9857-105">Да бисте уклонили старе или неискоришћене ценовнике из услуге Dynamics 365 Project Operations, постоје два корака која морате извршити.</span><span class="sxs-lookup"><span data-stu-id="f9857-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="f9857-106">Уклоните или избришите ценовник са одређених страница.</span><span class="sxs-lookup"><span data-stu-id="f9857-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="f9857-107">Деактивирајте или избришите ценовник из активних ценовника на страници **Ценовници**.</span><span class="sxs-lookup"><span data-stu-id="f9857-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="f9857-108">Морате обавити оба корака да бисте у потпуности уклонили ценовник.</span><span class="sxs-lookup"><span data-stu-id="f9857-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="f9857-109">Није довољно да обавите само 2. корак, а то је директно брисање или деактивирање ценовника из приказа Активни ценовници.</span><span class="sxs-lookup"><span data-stu-id="f9857-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="f9857-110">Морате избрисати и повезивање овог ценовника са свих места поменутих у 1. кораку.</span><span class="sxs-lookup"><span data-stu-id="f9857-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="f9857-111">Брисање ценовника са одређених страница</span><span class="sxs-lookup"><span data-stu-id="f9857-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="f9857-112">Да бисте избрисали ценовник из услуге Project Operations, идите на следеће странице:</span><span class="sxs-lookup"><span data-stu-id="f9857-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="f9857-113">Страница **Параметри пројекта** > картица **Ценовници**</span><span class="sxs-lookup"><span data-stu-id="f9857-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="f9857-114">Страница **Организациона јединица** > мрежа **Ценовници**</span><span class="sxs-lookup"><span data-stu-id="f9857-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="f9857-115">Страница **Пословни контакт** > мрежа **Ценовници пројекта**</span><span class="sxs-lookup"><span data-stu-id="f9857-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="f9857-116">Страница **Понуде за пројекат** > мрежа **Ценовници пројекта**: Ово се односи на све активне понуде за пројекат.</span><span class="sxs-lookup"><span data-stu-id="f9857-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="f9857-117">Страница **Уговори о пројекту** > мрежа **Ценовници пројекта**: Ово се односи на све активне уговоре о пројекту.</span><span class="sxs-lookup"><span data-stu-id="f9857-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="f9857-118">За сваку страницу, морате изабрати ценовник који желите да избришете, а затим изаберите **Избриши**.</span><span class="sxs-lookup"><span data-stu-id="f9857-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="f9857-119">Брисање или деактивирање ценовника са странице Ценовници</span><span class="sxs-lookup"><span data-stu-id="f9857-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="f9857-120">Да бисте избрисали ценовник из активних ценовника, идите на **Продаја** > **Клијенти** > **Ценовници**.</span><span class="sxs-lookup"><span data-stu-id="f9857-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="f9857-121">Изаберите ценовник који желите да избришете, а затим изаберите **Избриши**.</span><span class="sxs-lookup"><span data-stu-id="f9857-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="f9857-122">Ако се ценовник користи у било којој трансакцији, нећете моћи да га избришете.</span><span class="sxs-lookup"><span data-stu-id="f9857-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="f9857-123">Ако се то догоди, можете деактивирати ценовник тако да се не приказује ни у једном приказу.</span><span class="sxs-lookup"><span data-stu-id="f9857-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="f9857-124">Да бисте деактивирали ценовник, поново изаберите ценовник, а затим изаберите **Деактивирај**.</span><span class="sxs-lookup"><span data-stu-id="f9857-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
