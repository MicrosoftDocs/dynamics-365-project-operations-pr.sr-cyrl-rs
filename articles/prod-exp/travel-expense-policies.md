---
title: Подешавање смерница трошкова
description: Можете да подесите смернице трошкова које ваши радници морају следити приликом уношења и подношења извештаја о трошковима и путних захтева у услузи Microsoft Dynamics 365 Finance.
author: suvaidya
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: fa4f628a918e6e099a723ed05994f63d6ad847f5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005764"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="e1dd8-103">Подешавање смерница трошкова</span><span class="sxs-lookup"><span data-stu-id="e1dd8-103">Set up expense policies</span></span>

<span data-ttu-id="e1dd8-104">Можете да дефинишете смернице које ваши радници морају следити приликом уношења и подношења извештаја о трошковима и путних захтева.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="e1dd8-105">Спровођење смерница трошкова може вам помоћи да ефикасно управљате трошковима.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="e1dd8-106">На пример, можете да поставите смерницу за хотелске трошкове у Њујорку, која наводи да трошак по ноћењу не може премашити 250 USD.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="e1dd8-107">Ако радник поднесе извештај о трошку или захтев за путовање када цена собе прелази овај износ, систем ће о томе обавестити</span><span class="sxs-lookup"><span data-stu-id="e1dd8-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="e1dd8-108">радника да је прекорачен износ смернице за трошак.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="e1dd8-109">Можете да конфигуришете поруку коју ће радник добити када</span><span class="sxs-lookup"><span data-stu-id="e1dd8-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="e1dd8-110">дефинишете смерницу.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-110">define the policy.</span></span>      
        
<span data-ttu-id="e1dd8-111">Можете да дефинишете три типа смерница:</span><span class="sxs-lookup"><span data-stu-id="e1dd8-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="e1dd8-112">Упозорење – Омогућава раднику да поднесе извештај о трошку или захтев за путовање, али ће трошак бити означен за све даваоце одобрења и</span><span class="sxs-lookup"><span data-stu-id="e1dd8-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="e1dd8-113">за касније извештавање.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-113">for later reporting.</span></span>        

- <span data-ttu-id="e1dd8-114">Грешка – Захтева од радника да ревидира трошкове како би се придржавао смерница пре подношења извештаја о трошковима или захтева за путовање.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="e1dd8-115">Оправдање – Захтева од радника или менаџера да унесе образложење за прекорачење износа полисе пре подношења извештаја о трошковима или захтева за путовање.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="e1dd8-116">Савети за смернице</span><span class="sxs-lookup"><span data-stu-id="e1dd8-116">Policy tips</span></span>
<span data-ttu-id="e1dd8-117">Ево неколико предлога који вам могу помоћи при креирању нових смерница за управљање трошковима.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="e1dd8-118">Смернице важе на датум и неће ступити на снагу ако су креиране са датумом после датума настанка трошкова.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="e1dd8-119">На пример, ако данас креирате нове смернице за примену максималног трошка оброка од 50 USD, сви постојећи трошкови унети од јуче неће бити проверени у складу са овим смерницама.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="e1dd8-120">Приликом креирања смерница за категорију трошкова која се може поделити, размислите о додавању услова за врсту линије трошкова.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="e1dd8-121">Неке смернице, попут захтева за признаницу, можда неће имати смисла за разврстане ставке и треба их применити само на заглавље или неразврстане ставке.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="e1dd8-122">Смернице за управљање трошковима подразумевано се вреднују према изворном ентитету.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="e1dd8-123">У случају интеркомпанијских сценарија, можете да подесите да се смернице вреднују према одредишном ентитету (ентитету задуживања).</span><span class="sxs-lookup"><span data-stu-id="e1dd8-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="e1dd8-124">Да бисте покренули смернице према одредишном ентитету, укључите функцију „Процените смернице трошкова у односу на задуживања правног лица“ у радном простору **Управљање функцијама**.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="e1dd8-125">Када се процењују смернице</span><span class="sxs-lookup"><span data-stu-id="e1dd8-125">When to evaluate policies</span></span>

<span data-ttu-id="e1dd8-126">У параметрима управљања трошковима постоји опција да процените политике управљања трошковима када се линија сачува или када се поднесе извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="e1dd8-127">Ако одлучите да процените када је линија сачувана, корисници ће имати ранији увид у оно што треба да ураде да би одједном комплетирали свој извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="e1dd8-128">У супротном, можете одложити процену смерница и уштедети време ако се потврђивање обавља на крају, током предаје у радни ток.</span><span class="sxs-lookup"><span data-stu-id="e1dd8-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]