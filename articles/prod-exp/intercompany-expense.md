---
title: Интерни трошкови у оквиру предузећа
description: Радник који је запослен у једном правном лицу у организацији може обављати посао за друго правно лице у истој организацији. У овој ситуацији можете да користите функцију трошкова у оквиру предузећа за додељивање трошкова радника правном лицу за које је посао изведен.
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
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084123"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="e4c9e-104">Интерни трошкови у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="e4c9e-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e4c9e-105">Радник који је запослен у једном правном лицу у организацији може обављати посао за друго правно лице у истој организацији.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="e4c9e-106">У овој ситуацији можете да користите функцију трошкова у оквиру предузећа за додељивање трошкова радника правном лицу за које је посао изведен.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="e4c9e-107">Правно лице које запошљава радника назива се правно лице које позајмљује.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="e4c9e-108">Правно лице за које радник сноси трошкове назива се правно лице којем се позајмљује.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="e4c9e-109">Пре него што радник може креирати и поднети трошкове за рад који се обавља за друго правно лице, у правном лицу које позајмљује, на страници **Параметри управљања трошковима** изаберите **Омогућите ставке трошкова у оквиру предузећа**.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="e4c9e-110">Пореско књижење за трошкове у оквиру предузећа</span><span class="sxs-lookup"><span data-stu-id="e4c9e-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e4c9e-111">Ако у извештају о трошковима желите да користите пореске групе које су повезане са правним лицем које позајмљује (изворно правно лице) уместо са правним лицем којем се позајмљује (одредишно правно лице), мораћете то да конфигуришете у подешавању пореза на промет у главној књизи.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="e4c9e-112">Када је параметар главне књиге **Правно лице за пореско књижење у оквиру предузећа** подешен на **Извор** и опција **Примени правила опорезивања за порез на промет** подешена на **Не** , користиће се комбинација пореза за правно лице које позајмљује.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="e4c9e-113">Када је исти параметар постављен на **Одредиште** , користиће се пореска комбинација за правно лице којем се позајмљује.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="e4c9e-114">За правна лица у Сједињеним Државама, када је параметар постављен на **Извор** , поље **Потраживање пореза на промет** такође мора бити конфигурисано на новој страници **Групе за књижење главне књиге**.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="e4c9e-115">Рачуноводствени механизам ће користити податке из овог поља за рачуноводствено књижење у вези са порезом.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="e4c9e-116">Понашање је доследно за ставке трошкова објављене са пројектом или без њега.</span><span class="sxs-lookup"><span data-stu-id="e4c9e-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
