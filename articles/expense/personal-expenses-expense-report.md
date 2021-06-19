---
title: Ред са личним трошковима у извештају о трошковима
description: Ова тема пружа информације о начину рада са личним трошковима које су остварили запослен на пословним путовањима.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025702"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="777be-103">Ред са личним трошковима у извештају о трошковима</span><span class="sxs-lookup"><span data-stu-id="777be-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="777be-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="777be-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="777be-105">Током пословног пута запосленик може наплатити личне трошкове са кредитне картице предузећа.</span><span class="sxs-lookup"><span data-stu-id="777be-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="777be-106">Ако није дефинисан поступак за управљање личним трошковима, поступак одобравања извештаја о трошковима може бити прекинут када запослени преда детаљни извештај о трошковима.</span><span class="sxs-lookup"><span data-stu-id="777be-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="777be-107">Постоје две методе које можете користити за рад са личним трошковима запосленог:</span><span class="sxs-lookup"><span data-stu-id="777be-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="777be-108">**Плаћа запослени**: Ваша организација не плаћа личне трошкове који се појављују на рачуну за кредитну картицу предузећа.</span><span class="sxs-lookup"><span data-stu-id="777be-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="777be-109">Уместо тога, запослени директно плаћа добављачу кредитне картице за трошкове.</span><span class="sxs-lookup"><span data-stu-id="777be-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="777be-110">**Плаћа предузеће**: Ваша организација плаћа цео рачун за кредитну картицу предузећа, а затим терети рачун радника за личне трошкове.</span><span class="sxs-lookup"><span data-stu-id="777be-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="777be-111">Можете одабрати метод који ваша организација користи на страници **Параметри управљања трошковима**.</span><span class="sxs-lookup"><span data-stu-id="777be-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="777be-112">Омогућите функцију подељених трошкова када поље за лични износ има дефинисану вредност</span><span class="sxs-lookup"><span data-stu-id="777be-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="777be-113">Функција, **Омогућите функцију подељених трошкова када поље за лични износ има дефинисану вредност** односи се само на извештаје о трошковима који су одобрени коришћењем тока посла на нивоу ставке.</span><span class="sxs-lookup"><span data-stu-id="777be-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="777be-114">Извештаји се одобравају одласком на **Обрада извештаја о трошковима** > **Извештаји о трошковима који су ми додељени** > **Отвори извештај о трошковима**.</span><span class="sxs-lookup"><span data-stu-id="777be-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="777be-115">Да бисте омогућили ову функцију, идите на **Радни простори** > **Управљање функцијама**, изаберите **Омогући функцију подељених трошкова када поље за лични износ има дефинисану вредност**, а затим изаберите **Омогући одмах**.</span><span class="sxs-lookup"><span data-stu-id="777be-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="777be-116">Када је функција омогућена, ставке трошкова које користе ову функцију генеришу две ставке када се извештај поднесе.</span><span class="sxs-lookup"><span data-stu-id="777be-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="777be-117">Две ставке се генеришу тако да давалац одобрења може да одобри сваки ред засебно.</span><span class="sxs-lookup"><span data-stu-id="777be-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
