---
title: Матична страница за извештавање
description: Ова тема пружа информације о извештавању у апликацији Dynamics 365 Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 32b504a862f98dac4b1d9b54289476026d988c13
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5951497"
---
# <a name="reporting-home-page"></a><span data-ttu-id="dcc70-103">Почетна страница за извештавање</span><span class="sxs-lookup"><span data-stu-id="dcc70-103">Reporting home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="dcc70-104">Microsoft Dynamics 365 Project Service Automation омогућава да организације засноване на пројектима ефикасно управљају пословним операцијама предузећа.</span><span class="sxs-lookup"><span data-stu-id="dcc70-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="dcc70-105">На било којем пројекту, чланови тима морају да управљају могућностима за пословање, дају пословну понуду и планирају посао, обезбеђују ресурсе за пројекте, управљају послом према плану, наплаћују за посао, а затим обављају остале послове како би пројекат привели крају.</span><span class="sxs-lookup"><span data-stu-id="dcc70-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="dcc70-106">Могућност извештавања о пословним операцијама је кључна за утврђивање стања организације и предузимање било каквих корективних поступака који су потребни.</span><span class="sxs-lookup"><span data-stu-id="dcc70-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="dcc70-107">PSA користи Microsoft Dynamics 365 методе и технологије извештавања за целокупно извештавање.</span><span class="sxs-lookup"><span data-stu-id="dcc70-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="dcc70-108">Још информација о опцијама за извештавање потражите у одељку [Водич за писање извештаја за Dynamics 365 Customer Engagement (on-premises), верзију 9](/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span><span class="sxs-lookup"><span data-stu-id="dcc70-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="dcc70-109">Чаробњак за извештаје</span><span class="sxs-lookup"><span data-stu-id="dcc70-109">Report Wizard</span></span>

<span data-ttu-id="dcc70-110">Чаробњак за извештаје омогућава онима који нису програмери да креирају једноставне извештаје.</span><span class="sxs-lookup"><span data-stu-id="dcc70-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="dcc70-111">Будући да је апликација развијена на постојећој платформи, искуство је исто као искуство документовано у чланку [Креирање или измена извештаја помоћу чаробњака за извештаје](/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span><span class="sxs-lookup"><span data-stu-id="dcc70-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span></span> <span data-ttu-id="dcc70-112">Међутим, користићете ентитете специфичне за Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="dcc70-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="dcc70-113">Прилагођени извештаји за SQL Server Reporting Services</span><span class="sxs-lookup"><span data-stu-id="dcc70-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="dcc70-114">Ако ваше предузеће захтева одређени извештај који се не може креирати помоћу чаробњака за извештаје, можете да креирате прилагођени извештај.</span><span class="sxs-lookup"><span data-stu-id="dcc70-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="dcc70-115">Морате инсталирати Microsoft Visual Studio, уз одговарајуће Microsoft SQL Server Data Tools и додатке за креирање извештаја.</span><span class="sxs-lookup"><span data-stu-id="dcc70-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="dcc70-116">За више информација о алаткама и верзијама погледајте чланак [Окружење за писање извештаја које користи SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="dcc70-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span></span> <span data-ttu-id="dcc70-117">Информације о креирању прилагођеног извештаја потражите у чланку [Креирање новог извештаја помоћу услуге SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="dcc70-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="dcc70-118">Power BI апликације за увиде</span><span class="sxs-lookup"><span data-stu-id="dcc70-118">Power BI insights apps</span></span>

<span data-ttu-id="dcc70-119">Microsoft Power BI и Dynamics 365 заједно пружају моћан начин рада са подацима, у виду апликација за увиде.</span><span class="sxs-lookup"><span data-stu-id="dcc70-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="dcc70-120">Информације о доступности апликација за увиде потражите у чланку [Power BI страница са апликацијама за увиде](https://powerbi.microsoft.com/power-bi-insights-apps/).</span><span class="sxs-lookup"><span data-stu-id="dcc70-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="dcc70-121">Додатни ресурси</span><span class="sxs-lookup"><span data-stu-id="dcc70-121">Additional resources</span></span>
<span data-ttu-id="dcc70-122">За више информација о извештавању у апликацији PSA, погледајте следеће теме:</span><span class="sxs-lookup"><span data-stu-id="dcc70-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="dcc70-123">Рад са Project Service моделом података</span><span class="sxs-lookup"><span data-stu-id="dcc70-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="dcc70-124">Контролне табле</span><span class="sxs-lookup"><span data-stu-id="dcc70-124">Dashboards</span></span>](reports-dashboards.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]