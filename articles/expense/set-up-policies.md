---
title: Дефинисање смерница трошкова
description: Можете да дефинишете смернице трошкова које ваши радници морају следити приликом уношења и подношења извештаја о трошковима и путних захтева.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 30b3a0e1547ca7043b1433da2b4ebf02f2b473a1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084042"
---
# <a name="define-expense-policies"></a><span data-ttu-id="7399a-103">Дефинисање смерница трошкова</span><span class="sxs-lookup"><span data-stu-id="7399a-103">Define expense policies</span></span>

<span data-ttu-id="7399a-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="7399a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7399a-105">Можете да дефинишете смернице које ваши радници морају следити приликом уношења и подношења извештаја о трошковима и путних захтева.</span><span class="sxs-lookup"><span data-stu-id="7399a-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="7399a-106">Спровођење смерница трошкова може вам помоћи да ефикасно управљате трошковима.</span><span class="sxs-lookup"><span data-stu-id="7399a-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="7399a-107">На пример, можете да поставите смерницу за хотелске трошкове у Њујорку, која наводи да трошак по ноћењу не може премашити 250 USD.</span><span class="sxs-lookup"><span data-stu-id="7399a-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="7399a-108">Ако радник поднесе извештај о трошку или захтев за путовање када цена собе прелази овај износ, систем ће о томе обавестити</span><span class="sxs-lookup"><span data-stu-id="7399a-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="7399a-109">радника да је прекорачен износ смернице за трошак.</span><span class="sxs-lookup"><span data-stu-id="7399a-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="7399a-110">Можете да конфигуришете поруку коју ће радник добити када</span><span class="sxs-lookup"><span data-stu-id="7399a-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="7399a-111">дефинишете смерницу.</span><span class="sxs-lookup"><span data-stu-id="7399a-111">define the policy.</span></span>      
        
<span data-ttu-id="7399a-112">Можете да дефинишете три типа смерница:</span><span class="sxs-lookup"><span data-stu-id="7399a-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="7399a-113">**Упозорење** : Омогућава раднику да поднесе извештај о трошку или захтев за путовање, али ће трошак бити означен за све даваоце одобрења и</span><span class="sxs-lookup"><span data-stu-id="7399a-113">**Warning** : Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="7399a-114">за касније извештавање.</span><span class="sxs-lookup"><span data-stu-id="7399a-114">for later reporting.</span></span>        

- <span data-ttu-id="7399a-115">**Грешка** : Захтева од радника да ревидира трошкове како би се придржавао смерница пре подношења извештаја о трошковима или захтева за путовање.</span><span class="sxs-lookup"><span data-stu-id="7399a-115">**Error** : Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="7399a-116">**Оправдање** : Захтева од радника или менаџера да унесе образложење за прекорачење износа полисе пре подношења извештаја о трошковима или захтева за путовање.</span><span class="sxs-lookup"><span data-stu-id="7399a-116">**Justification** : Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="7399a-117">Савети за смернице</span><span class="sxs-lookup"><span data-stu-id="7399a-117">Policy tips</span></span>
<span data-ttu-id="7399a-118">Ево неколико предлога који вам могу помоћи при креирању нових смерница за управљање трошковима:</span><span class="sxs-lookup"><span data-stu-id="7399a-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="7399a-119">Смернице важе на датум, што значи да смернице неће ступити на снагу ако су креиране са датумом после датума настанка трошкова.</span><span class="sxs-lookup"><span data-stu-id="7399a-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="7399a-120">На пример, данас креирате нову политику за примену максималних трошкова оброка од 50 USD.</span><span class="sxs-lookup"><span data-stu-id="7399a-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="7399a-121">Сви постојећи трошкови који су унети од јуче неће бити проверени у складу са овом политиком.</span><span class="sxs-lookup"><span data-stu-id="7399a-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="7399a-122">Приликом креирања смерница за категорију трошкова која се може поделити, размислите о додавању услова за врсту линије трошкова.</span><span class="sxs-lookup"><span data-stu-id="7399a-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="7399a-123">Неке смернице, попут захтева за признаницом, можда неће имати смисла за детаљне линије.</span><span class="sxs-lookup"><span data-stu-id="7399a-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="7399a-124">У овој ситуацији, смернице се примењују само на линију заглавља или линију која није стављена у ставке.</span><span class="sxs-lookup"><span data-stu-id="7399a-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="7399a-125">Смернице за управљање трошковима подразумевано се вреднују према изворном ентитету.</span><span class="sxs-lookup"><span data-stu-id="7399a-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="7399a-126">У случају интеркомпанијских сценарија, можете да подесите да се смернице вреднују према одредишном ентитету (ентитету задуживања).</span><span class="sxs-lookup"><span data-stu-id="7399a-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="7399a-127">Да бисте покренули смернице према одредишном ентитету, укључите функцију **Процените смернице трошкова у односу на задуживања правног лица** у радном простору **Управљање функцијама**.</span><span class="sxs-lookup"><span data-stu-id="7399a-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="7399a-128">Када се процењују смернице</span><span class="sxs-lookup"><span data-stu-id="7399a-128">When to evaluate policies</span></span>

<span data-ttu-id="7399a-129">У параметрима управљања трошковима можете изабрати да процените политике управљања трошковима када се линија сачува или када се поднесе извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="7399a-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="7399a-130">Ако одлучите да процените када је линија сачувана, корисници ће имати ранији увид у оно што треба да ураде да би одједном комплетирали свој извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="7399a-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="7399a-131">У супротном, можете одложити процену смерница и уштедети време потврђивањем на крају, током предаје у радни ток.</span><span class="sxs-lookup"><span data-stu-id="7399a-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>
