---
title: Ажурирање атрибута додатних компоненти тако да укључују нове димензије за одређивање цена
description: Ова тема пружа информације о ажурирању атрибута додатних компоненти за димензије одређивања цена.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: project-operations
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 603b0e9a10dc2fe23c9fa0fa7065bc3f500dc540
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147086"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="f1ad3-103">Ажурирање атрибута додатних компоненти тако да укључују нове димензије за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="f1ad3-103">Update plug-in attributes to include new pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!NOTE]
> <span data-ttu-id="f1ad3-104">Ако не користите Project Service Automation (PSA) функције за давања понуда и уговарање, можете прескочити ову тему.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="f1ad3-105">Ова тема претпоставља да сте довршили процедуре у темама, [Креирање прилагођених поља и ентитета](create-custom-fields-entities.md), [Додавање прилагођених поља у подешавање цена и ентитете трансакције](field-references.md) и [Подешавање прилагођених поља као димензија за одређивање цена](set-up-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="f1ad3-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="f1ad3-106">Ако нисте довршили те процедуре, вратите се и довршите их, а затим се вратите на ову тему.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="f1ad3-107">Када се на страници **Ставка понуде** креира детаљ ставке понуде за ставку понуде за пројекат, систем креира две ставке процене у позадини, једну ставку за трошковни део процене и једну за продајну страну.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="f1ad3-108">Ово је исто за предмете уговора о пројекту.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="f1ad3-109">Када промените количину или поље на страни трошкова, та промена се преноси на страну продаје.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="f1ad3-110">Ово је могуће због следећих додатних компоненти које морају бити поново регистроване после промене димензија за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="f1ad3-111">PreOperationContractLineDetailUpdate - Исправке **msdyn_orderlinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="f1ad3-112">PreOperationQuoteLineDetailUpdate - Исправке **msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="f1ad3-113">Следећи кораци вас воде кроз процес регистрације додатних компоненти.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="f1ad3-114">Отворите **PluginRegistrationTool** и повежите се са инстанцом на мрежи.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="f1ad3-115">Кликните на **Претрага** и потражите додатну компоненту за ажурирање.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![Снимак екрана стабла за претрагу](media/PRT-1.png)

3. <span data-ttu-id="f1ad3-117">Након што пронађете додатну компоненту, изаберите је, а затим кликните на **Изабери у главном обрасцу**.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="f1ad3-118">Изаберите корак додатне компоненте за ажурирање, кликните десним тастером миша, а затим изаберите **Ажурирај**.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![Снимак екрана додатне компоненте за ажурирање](media/PRT-2.png)
 
5. <span data-ttu-id="f1ad3-120">У прозору за ажурирање кликните на три тачке (**...**) у атрибутима филтрирања.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-120">In the update window, click the ellipsis (**...**) in the filtering attributes.</span></span>

 ![Снимак екрана са информацијама за конфигурисање ажурирања постојећег корака](media/PRT-3.png)
 
6. <span data-ttu-id="f1ad3-122">Изаберите поља за потврду атрибута за одређивање цена.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-122">Select the pricing attribute check boxes.</span></span>

 ![Снимак екрана који приказује избор у пољу за потврду за атрибуте одређивања цена](media/PRT-4.png)

7. <span data-ttu-id="f1ad3-124">Кликните на **У реду** да затворите страницу, а затим изаберите **Ажурирај корак**.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 ![Снимак екрана који приказује дугме „Ажурирај корак“](media/PRT-5.png)
 
8. <span data-ttu-id="f1ad3-126">Поновите овај поступак за другу додатну компоненту, **PreOperationQuoteLineDetail - Исправка за msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="f1ad3-127">Затворите алатку за регистровање додатне компоненте.</span><span class="sxs-lookup"><span data-stu-id="f1ad3-127">Close the plug-in registration tool.</span></span>

