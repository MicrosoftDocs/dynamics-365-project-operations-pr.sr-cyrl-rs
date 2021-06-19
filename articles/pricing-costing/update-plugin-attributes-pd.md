---
title: Ажурирање атрибута додатних компоненти са новим аспектима за одређивање цена
description: Ова тема пружа информације о томе како да ажурирате атрибуте додатних компоненти за димензије одређивања цена.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 54b87a993929edbf89ef48741ba0a06c6c42ec4e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004639"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="2b6d4-103">Ажурирајте атрибуте додатних компоненти са новим аспектима за одређивање цена</span><span class="sxs-lookup"><span data-stu-id="2b6d4-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="2b6d4-104">Ова тема пружа информације о томе како да ажурирате атрибуте додатних компоненти за димензије одређивања цена.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="2b6d4-105">Ова тема је применљива само на функције понуде и уговора у услузи Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b6d4-106">Предуслови</span><span class="sxs-lookup"><span data-stu-id="2b6d4-106">Prerequisites</span></span>
<span data-ttu-id="2b6d4-107">Пре него што довршите кораке у овој теми, морате довршити процедуре у следећим темама:</span><span class="sxs-lookup"><span data-stu-id="2b6d4-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="2b6d4-108">Креирање прилагођених поља и ентитета</span><span class="sxs-lookup"><span data-stu-id="2b6d4-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="2b6d4-109">Додавање прилагођених поља у подешавање цена и ентитете трансакције </span><span class="sxs-lookup"><span data-stu-id="2b6d4-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="2b6d4-110">[Подешавање прилагођених поља као димензија за одређивање цена](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="2b6d4-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="2b6d4-111">Ако нисте довршили те процедуре, довршите их, а затим се вратите на ову тему.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="2b6d4-112">Регистровање додатне компоненте</span><span class="sxs-lookup"><span data-stu-id="2b6d4-112">Register a plug-in</span></span>
<span data-ttu-id="2b6d4-113">Када креирате детаљ ставке понуде на страници **Ставка понуде** за ставку понуде пројекта, систем креира две ставке процене.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="2b6d4-114">Једна ставка је за трошковну страну процене, а друга ставка за продајну страну.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="2b6d4-115">Ово је исто за предмете уговора о пројекту.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="2b6d4-116">Када промените количину или поље на страни трошкова, та промена се врши и на страни продаје.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="2b6d4-117">То је могуће јер додатне компоненте PreOperation на Quotelinedetail и ставкама детаља за contractline повезују одређене атрибуте на трошковној страни са продајном страном трансакције.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="2b6d4-118">Ако су вам потребне измене вредности димензија формирања цена на продајној страни да би се извршиле и на трошковној страни, следеће додатне компоненте морају да се поново региструју након уношења промена у димензију формирања цене.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="2b6d4-119">Ово су додатне компоненте за ажурирање и поновну регистрацију:</span><span class="sxs-lookup"><span data-stu-id="2b6d4-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="2b6d4-120">PreOperationContractLineDetailUpdate – **Update msdyn_orderlinetransaction**</span><span class="sxs-lookup"><span data-stu-id="2b6d4-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="2b6d4-121">PreOperationQuoteLineDetailUpdate – **Updates msdyn_quotelinetransaction**</span><span class="sxs-lookup"><span data-stu-id="2b6d4-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="2b6d4-122">Довршите следеће кораке да бисте ажурирали и поново регистровали додатне компоненте.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="2b6d4-123">Отворите **PluginRegistrationTool** и повежите се са својим Project Operations Dataverse окружењем.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="2b6d4-124">Изаберите **Претрага** и откуцајте првих неколико слова додатне компоненте који треба да се ажурира.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="2b6d4-125">Након што пронађете додатну компоненту, изаберите је, а затим изаберите **Изабери у главном обрасцу**.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="2b6d4-126">Изаберите корак **Ажурирај msdyn_orderlinetransaction**, кликните десним тастером и изаберите **Ажурирај**.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="2b6d4-127">На страници са дијалогом **Ажурирај** , изаберите три тачке (**...**) у атрибутима филтрирања.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="2b6d4-128">Отвара се прозор филтрирања атрибута и наводи списак свих атрибута у ентитету и димензијама формирања цена.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="2b6d4-129">Изаберите поља за потврду за атрибуте димензије формирања цена.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="2b6d4-130">Изаберите **У реду** да затворите страницу, а затим изаберите **Ажурирај корак**.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="2b6d4-131">Поновите кораке од 2-7 за другу додатну компоненту, **PreOperationQuoteLineDetail**.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="2b6d4-132">За ову додатну компоненту, морате да ажурирате корак **Update of msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="2b6d4-133">Затворите **PluginRegistrationTool**.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-133">Close **PluginRegistrationTool**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]