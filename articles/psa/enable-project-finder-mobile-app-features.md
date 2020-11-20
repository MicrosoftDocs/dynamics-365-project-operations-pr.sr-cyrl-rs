---
title: Омогућавање функција апликације Project Finder Mobile
description: Како да омогућите функције апликације Project Finder Mobile за апликацију Project Service
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: af267b5adc48b6edec57de196f91e338c058558c
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4132981"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a><span data-ttu-id="ab6e5-103">Омогућавање функција апликације Project Finder Mobile (Project Service)</span><span class="sxs-lookup"><span data-stu-id="ab6e5-103">Enable Project Finder Mobile app features (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="ab6e5-104">Ваши ресурси могу да користе апликацију Project Finder Mobile на телефону уз [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] да проналазе нове пројекте на којима ће радити и да ажурирају скупове вештина.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-104">Your resources can use the Project Finder Mobile app on their phone with [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to find new projects to work on and update their skill sets.</span></span>  
  
 <span data-ttu-id="ab6e5-105">Апликација је доступна за [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] телефоне и [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].</span><span class="sxs-lookup"><span data-stu-id="ab6e5-105">The app is available for [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] phones, and [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].</span></span>  
  
 <span data-ttu-id="ab6e5-106">Треба да подесите неколико опција у поставкама параметара за организациону јединицу да бисте омогућили корисницима преглед захтева за ресурсима у пројектима и ажурирање њихових вештина.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-106">You need to set a couple of options in the parameters setting for your organizational unit to allow users to view projects' resource requirements and update their skills.</span></span>  
  
> [!NOTE]
>  <span data-ttu-id="ab6e5-107">Апликација Project Finder Mobile ради само са системом [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], а не са локалним инсталацијама.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-107">The Project Finder Mobile app only works with [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], not with on-premises installations.</span></span>  
  
1. <span data-ttu-id="ab6e5-108">Идите на **Project Service > Параметри**.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-108">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="ab6e5-109">Кликните на поставку параметара које желите да користите да бисте омогућили функције апликације Project Finder Mobile.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-109">Click the parameters setting you want to use for allowing the Project Finder Mobile app features.</span></span>  
  
3. <span data-ttu-id="ab6e5-110">У области **Општи подаци**, поставите **Захтеви у погледу ресурса видљиви ресурсима** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-110">In the **General** area, set **Resource requirements visible to resources** to **Yes**.</span></span>  
  
4. <span data-ttu-id="ab6e5-111">Подесите **Дозволи да ресурси освеже вештине** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-111">Set **Allow skill update by resource** to **Yes**.</span></span>  
  
   <span data-ttu-id="ab6e5-112">![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span><span class="sxs-lookup"><span data-stu-id="ab6e5-112">![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span></span>  
  
   <span data-ttu-id="ab6e5-113">Ово је глобално подешавање.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-113">This is a global setting.</span></span> <span data-ttu-id="ab6e5-114">Менаџери пројекта треба да подесе да ли ће појединачни пројекат бити видљив на страници **Пројектни тим** тог пројекта.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-114">Project managers can set whether an individual project will be visible on that project's **Project Team** page.</span></span>  
  
   <span data-ttu-id="ab6e5-115">![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span><span class="sxs-lookup"><span data-stu-id="ab6e5-115">![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span></span>  
  
## <a name="email-notifications"></a><span data-ttu-id="ab6e5-116">Обавештења путем е-поште</span><span class="sxs-lookup"><span data-stu-id="ab6e5-116">Email notifications</span></span>  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="ab6e5-117">шаље е-поруке које се односе на захтеве за ресурсима следећим примаоцима следећим терминима:</span><span class="sxs-lookup"><span data-stu-id="ab6e5-117">sends emails regarding resource requests to the following recipients at the following times:</span></span>  
  
|<span data-ttu-id="ab6e5-118">Прималац</span><span class="sxs-lookup"><span data-stu-id="ab6e5-118">Recipient</span></span>|<span data-ttu-id="ab6e5-119">Догађај</span><span class="sxs-lookup"><span data-stu-id="ab6e5-119">Event</span></span>|  
|---------------|-----------|  
|<span data-ttu-id="ab6e5-120">Менаџер пројекта</span><span class="sxs-lookup"><span data-stu-id="ab6e5-120">Project manager</span></span>|<span data-ttu-id="ab6e5-121">-   Када је ресурс пријављен за пројекат преко апликације Project Finder Mobile.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-121">-   When a resource signs up for a project with the Project Finder Mobile app.</span></span>|  
|<span data-ttu-id="ab6e5-122">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ab6e5-122">Resource</span></span>|<span data-ttu-id="ab6e5-123">-   Када је посао на пројекту за који се ресурс пријавио већ испуњен од стране другог ресурса.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-123">-   When the project work the resource has signed up for has already been fulfilled by another resource.</span></span><br /><span data-ttu-id="ab6e5-124">-   Када њихови захтеви за одобрењем вештине буду одобрени или одбачени.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-124">-   When their skill approval request has been approved or rejected.</span></span><br /><span data-ttu-id="ab6e5-125">-   Када њихови захтеви за пријављивање у пројекат буду одобрени или одбачени.</span><span class="sxs-lookup"><span data-stu-id="ab6e5-125">-   When their project sign up request has been approved or rejected.</span></span>|  
  
## <a name="privacy-notice"></a><span data-ttu-id="ab6e5-126">Обавештење о приватности</span><span class="sxs-lookup"><span data-stu-id="ab6e5-126">Privacy notice</span></span>  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a><span data-ttu-id="ab6e5-127">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="ab6e5-127">See Also</span></span>  
 [<span data-ttu-id="ab6e5-128">Подешавање ресурса</span><span class="sxs-lookup"><span data-stu-id="ab6e5-128">Set up resources</span></span>](../psa/set-up-resources.md)
