---
title: Интерни трошкови у оквиру предузећа
description: Ова тема пружа информације о начину коришћења трошкова у оквиру предузећа за додељивање трошкова радника правном лицу за које је посао обављен.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 553ddbe622210169db8de4aa506dcf1ea1e9d5ef
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960850"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="62d84-103">Интерни трошкови у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="62d84-103">Intercompany expenses</span></span>

<span data-ttu-id="62d84-104">Радник који је запослен у једном правном лицу у организацији може обављати посао за друго правно лице у истој организацији.</span><span class="sxs-lookup"><span data-stu-id="62d84-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="62d84-105">Можете да користите трошкове у оквиру предузећа за додељивање трошкова радника правном лицу за које је посао обављен.</span><span class="sxs-lookup"><span data-stu-id="62d84-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="62d84-106">Правно лице које запошљава радника назива се правно лице које позајмљује.</span><span class="sxs-lookup"><span data-stu-id="62d84-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="62d84-107">Правно лице за које радник сноси трошкове назива се правно лице којем се позајмљује.</span><span class="sxs-lookup"><span data-stu-id="62d84-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="62d84-108">Да би радник могао да креира и преда трошкове у оквиру предузећа, морате омогућити редове трошкова у оквиру предузећа.</span><span class="sxs-lookup"><span data-stu-id="62d84-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="62d84-109">За правно лице које позајмљује новац, на страници **Параметри управљања трошковима** изаберите **Омогући редове трошкова у оквиру предузећа**.</span><span class="sxs-lookup"><span data-stu-id="62d84-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="62d84-110">Пореско књижење за трошкове у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="62d84-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="62d84-111">Да бисте у извештају о трошковима могли да користите пореске групе које су повезане са правним лицем које позајмљује новац (извор) уместо са правним лицем које се задужује (одредиште), морате да омогућите функционалност у подешавању пореза на промет у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="62d84-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="62d84-112">Када је параметар **Правно лице за књижење пореза у оквиру предузећа** подешен на **Извор**, а параметар **Примени правила опорезивања пореза на промет** је подешен на **Не**, користи се пореска комбинација за правно лице које позајмљује новац.</span><span class="sxs-lookup"><span data-stu-id="62d84-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="62d84-113">Када је исти параметар постављен на **Одредиште**, користиће се пореска комбинација за правно лице којем се позајмљује.</span><span class="sxs-lookup"><span data-stu-id="62d84-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="62d84-114">За правна лица у Сједињеним Државама, када је параметар постављен на **Извор**, поље **Потраживање пореза на промет** такође мора бити конфигурисано на новој страници **Групе за књижење главне књиге**.</span><span class="sxs-lookup"><span data-stu-id="62d84-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="62d84-115">Рачуноводствени механизам ће користити податке из овог поља за рачуноводствени унос у вези са порезом.</span><span class="sxs-lookup"><span data-stu-id="62d84-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="62d84-116">Понашање је доследно за ставке трошкова објављене са пројектом или без њега.</span><span class="sxs-lookup"><span data-stu-id="62d84-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
