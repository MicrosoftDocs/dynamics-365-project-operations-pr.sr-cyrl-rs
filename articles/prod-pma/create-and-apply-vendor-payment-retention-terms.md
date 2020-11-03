---
title: Креирајте и примените услове задржавања плаћања продавца
description: Ова тема пружа информације о томе како подесити и одржавати услове задржавања за плаћања продаваца.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 1970a24a5073de6af43db1f1c068332c9ba9c8fe
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084109"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="5e099-103">Креирајте и примените услове задржавања плаћања продавца</span><span class="sxs-lookup"><span data-stu-id="5e099-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="5e099-104">Постављање услова задржавања за плаћања продаваца за пројекат корисно је када ваша организација жели да задржи део уплата извршених продавцу.</span><span class="sxs-lookup"><span data-stu-id="5e099-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="5e099-105">На пример, када желите да задржите плаћање продавцу док испоручени производи не испуне ваша очекивања.</span><span class="sxs-lookup"><span data-stu-id="5e099-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="5e099-106">Услови задржавања за плаћања продаваца могу се одредити када преговарате о уговору продавца.</span><span class="sxs-lookup"><span data-stu-id="5e099-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="5e099-107">Креирајте услове задржавања плаћања продавца</span><span class="sxs-lookup"><span data-stu-id="5e099-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="5e099-108">Можете да унесете проценат плаћања продавца за задржавање и проценат претходно задржаних износа који ће се ослободити.</span><span class="sxs-lookup"><span data-stu-id="5e099-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="5e099-109">Износи се аутоматски задржавају на фактурама продаваца све док уговор не достигне одређени статус завршености.</span><span class="sxs-lookup"><span data-stu-id="5e099-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="5e099-110">Након што поставите услове задржавања, можете их применити на било који пројекат тог продавца.</span><span class="sxs-lookup"><span data-stu-id="5e099-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="5e099-111">Користите следеће кораке за постављање и одржавање услова задржавања за плаћања продавца.</span><span class="sxs-lookup"><span data-stu-id="5e099-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="5e099-112">Идите на **Управљање пројектима и рачуноводство** > **Задржавање** > **Услови задржавања за плаћања продаваца**.</span><span class="sxs-lookup"><span data-stu-id="5e099-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="5e099-113">Изаберите **Ново** да бисте додали нови услов задржавања за продавце.</span><span class="sxs-lookup"><span data-stu-id="5e099-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="5e099-114">Вредност **ID правила** за нови услов се аутоматски уноси.</span><span class="sxs-lookup"><span data-stu-id="5e099-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="5e099-115">Унесите кратак опис у поље **Опис** , а на брзој картици **Услови** изаберите **Додај линију** да бисте унели вредности услова за следеће:</span><span class="sxs-lookup"><span data-stu-id="5e099-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="5e099-116">**Проценат испоручених јединица** : Унесите проценат завршетка за услов.</span><span class="sxs-lookup"><span data-stu-id="5e099-116">**Percentage of units delivered** : Enter a percentage of completion for the term.</span></span> <span data-ttu-id="5e099-117">Износи се аутоматски задржавају на фактурама продаваца све док фаза довршетка пројекта не буде иста као наведени проценат.</span><span class="sxs-lookup"><span data-stu-id="5e099-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="5e099-118">На пример, ако унесете 50,00, износи се задржавају све док пројекат не буде завршен 50 одсто.</span><span class="sxs-lookup"><span data-stu-id="5e099-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="5e099-119">**Проценат за задржавање** : Унесите проценат износа фактуре добављача који ће се задржати.</span><span class="sxs-lookup"><span data-stu-id="5e099-119">**Percentage to retain** : Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="5e099-120">На пример, ако унесете 10,00, тада се задржава 10 процената износа на фактури добављача све док пројекат не достигне проценат завршетка како је постављено у поље **Проценат испоручених јединица**.</span><span class="sxs-lookup"><span data-stu-id="5e099-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="5e099-121">**Проценат за ослобађање** : Изаберите **Додај линију** да бисте унели проценат свих претходно задржаних износа који ће се ослободити за изабрани ниво завршетка пројекта.</span><span class="sxs-lookup"><span data-stu-id="5e099-121">**Percentage to release** : Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="5e099-122">Ако имате више од једне контролне тачке за различите нивое завршетка пројекта, унесите засебну линију услова задржавања за продавца за свако правило задржавања.</span><span class="sxs-lookup"><span data-stu-id="5e099-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="5e099-123">Свака линија може наводити различити проценат задржавања и другачији проценат издавања за сваки назначени ниво завршетка пројекта.</span><span class="sxs-lookup"><span data-stu-id="5e099-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="5e099-124">Након што креирате услове задржавања за продавца, можете их применити на пројекат.</span><span class="sxs-lookup"><span data-stu-id="5e099-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="5e099-125">Примените услове задржавања за продавца на пројекат</span><span class="sxs-lookup"><span data-stu-id="5e099-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="5e099-126">Идите на **Управљање пројектима и рачуноводство** > **Пројекти** > **Сви пројекти** и отворите пројекат са странице листе пројеката.</span><span class="sxs-lookup"><span data-stu-id="5e099-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="5e099-127">На брзој картици **Уговори са продавцима** изаберите **Додај линију**.</span><span class="sxs-lookup"><span data-stu-id="5e099-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="5e099-128">У пољу **Кôд пословног контакта** изаберите једну од следећих опција:</span><span class="sxs-lookup"><span data-stu-id="5e099-128">In the **Account code field** , select one of the following options:</span></span> 

   - <span data-ttu-id="5e099-129">**Табела** : Услови задржавања за продавце се примењују на једног продавца.</span><span class="sxs-lookup"><span data-stu-id="5e099-129">**Table** : The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="5e099-130">**Група** – Услови задржавања за продавце важе за све продавце у групи.</span><span class="sxs-lookup"><span data-stu-id="5e099-130">**Group** : The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="5e099-131">**Све** : Услови задржавања за продавце се примењују на све продавце.</span><span class="sxs-lookup"><span data-stu-id="5e099-131">**All** : The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="5e099-132">У **пољу Добављач/група продаваца** , изаберите продавца или групу продаваца на које се примењују услови задржавања за продавце.</span><span class="sxs-lookup"><span data-stu-id="5e099-132">In the **Vendor/Vendor group field** , select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="5e099-133">Ако сте изабрали **Све** у претходном кораку, ово поље није доступно.</span><span class="sxs-lookup"><span data-stu-id="5e099-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="5e099-134">У пољу **Услови задржавања за продавце** изаберите услове задржавања које сте креирали у претходном поступку.</span><span class="sxs-lookup"><span data-stu-id="5e099-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="5e099-135">Ако пројекат такође има услове за плаћање након уплате (PWP) за продавца, унесите проценат прага за пројекат у поље **Проценат PWP прага**.</span><span class="sxs-lookup"><span data-stu-id="5e099-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="5e099-136">Услови задржавања за продавце се такође приказују на поруџбеницама које креирате за продавца.</span><span class="sxs-lookup"><span data-stu-id="5e099-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>
