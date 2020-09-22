---
title: Омогућавање функција апликације Project Finder Mobile
description: Како да омогућите функције апликације Project Finder Mobile за апликацију Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 038c5c66-f136-4c7e-88c2-30ada80bbf38
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 9265ee78b20899026277e5af8e589112cd9fac74
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 03/24/2020
ms.locfileid: "3755310"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a><span data-ttu-id="ed614-103">Омогућавање функција апликације Project Finder Mobile (Project Service)</span><span class="sxs-lookup"><span data-stu-id="ed614-103">Enable Project Finder Mobile app features (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="ed614-104">Ваши ресурси могу да користе апликацију Project Finder Mobile на телефону уз [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] да проналазе нове пројекте на којима ће радити и да ажурирају скупове вештина.</span><span class="sxs-lookup"><span data-stu-id="ed614-104">Your resources can use the Project Finder Mobile app on their phone with [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to find new projects to work on and update their skill sets.</span></span>  
  
 <span data-ttu-id="ed614-105">Апликација је доступна за [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] телефоне и [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].</span><span class="sxs-lookup"><span data-stu-id="ed614-105">The app is available for [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] phones, and [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].</span></span>  
  
 <span data-ttu-id="ed614-106">Треба да подесите неколико опција у поставкама параметара за организациону јединицу да бисте омогућили корисницима преглед захтева за ресурсима у пројектима и ажурирање њихових вештина.</span><span class="sxs-lookup"><span data-stu-id="ed614-106">You need to set a couple of options in the parameters setting for your organizational unit to allow users to view projects' resource requirements and update their skills.</span></span>  
  
> [!NOTE]
>  <span data-ttu-id="ed614-107">Апликација Project Finder Mobile ради само са системом [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], а не са локалним инсталацијама.</span><span class="sxs-lookup"><span data-stu-id="ed614-107">The Project Finder Mobile app only works with [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], not with on-premises installations.</span></span>  
  
1. <span data-ttu-id="ed614-108">Идите на **Project Service > Параметри**.</span><span class="sxs-lookup"><span data-stu-id="ed614-108">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="ed614-109">Кликните на поставку параметара које желите да користите да бисте омогућили функције апликације Project Finder Mobile.</span><span class="sxs-lookup"><span data-stu-id="ed614-109">Click the parameters setting you want to use for allowing the Project Finder Mobile app features.</span></span>  
  
3. <span data-ttu-id="ed614-110">У области **Општи подаци**, поставите **Захтеви у погледу ресурса видљиви ресурсима** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="ed614-110">In the **General** area, set **Resource requirements visible to resources** to **Yes**.</span></span>  
  
4. <span data-ttu-id="ed614-111">Подесите **Дозволи да ресурси освеже вештине** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="ed614-111">Set **Allow skill update by resource** to **Yes**.</span></span>  
  
   <span data-ttu-id="ed614-112">![ProjectService_ProjectFinderEnable](../project-service/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span><span class="sxs-lookup"><span data-stu-id="ed614-112">![ProjectService_ProjectFinderEnable](../project-service/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span></span>  
  
   <span data-ttu-id="ed614-113">Ово је глобално подешавање.</span><span class="sxs-lookup"><span data-stu-id="ed614-113">This is a global setting.</span></span> <span data-ttu-id="ed614-114">Менаџери пројекта треба да подесе да ли ће појединачни пројекат бити видљив на страници **Пројектни тим** тог пројекта.</span><span class="sxs-lookup"><span data-stu-id="ed614-114">Project managers can set whether an individual project will be visible on that project's **Project Team** page.</span></span>  
  
   <span data-ttu-id="ed614-115">![ProjectService_ProjectTeamVisible](../project-service/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span><span class="sxs-lookup"><span data-stu-id="ed614-115">![ProjectService_ProjectTeamVisible](../project-service/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span></span>  
  
## <a name="email-notifications"></a><span data-ttu-id="ed614-116">Обавештења путем е-поште</span><span class="sxs-lookup"><span data-stu-id="ed614-116">Email notifications</span></span>  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="ed614-117">шаље е-поруке које се односе на захтеве за ресурсима следећим примаоцима следећим терминима:</span><span class="sxs-lookup"><span data-stu-id="ed614-117">sends emails regarding resource requests to the following recipients at the following times:</span></span>  
  
|<span data-ttu-id="ed614-118">Прималац</span><span class="sxs-lookup"><span data-stu-id="ed614-118">Recipient</span></span>|<span data-ttu-id="ed614-119">Догађај</span><span class="sxs-lookup"><span data-stu-id="ed614-119">Event</span></span>|  
|---------------|-----------|  
|<span data-ttu-id="ed614-120">Менаџер пројекта</span><span class="sxs-lookup"><span data-stu-id="ed614-120">Project manager</span></span>|<span data-ttu-id="ed614-121">-   Када је ресурс пријављен за пројекат преко апликације Project Finder Mobile.</span><span class="sxs-lookup"><span data-stu-id="ed614-121">-   When a resource signs up for a project with the Project Finder Mobile app.</span></span>|  
|<span data-ttu-id="ed614-122">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ed614-122">Resource</span></span>|<span data-ttu-id="ed614-123">-   Када је посао на пројекту за који се ресурс пријавио већ испуњен од стране другог ресурса.</span><span class="sxs-lookup"><span data-stu-id="ed614-123">-   When the project work the resource has signed up for has already been fulfilled by another resource.</span></span><br /><span data-ttu-id="ed614-124">-   Када њихови захтеви за одобрењем вештине буду одобрени или одбачени.</span><span class="sxs-lookup"><span data-stu-id="ed614-124">-   When their skill approval request has been approved or rejected.</span></span><br /><span data-ttu-id="ed614-125">-   Када њихови захтеви за пријављивање у пројекат буду одобрени или одбачени.</span><span class="sxs-lookup"><span data-stu-id="ed614-125">-   When their project sign up request has been approved or rejected.</span></span>|  
  
## <a name="privacy-notice"></a><span data-ttu-id="ed614-126">Обавештење о приватности</span><span class="sxs-lookup"><span data-stu-id="ed614-126">Privacy notice</span></span>  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a><span data-ttu-id="ed614-127">Такође погледајте</span><span class="sxs-lookup"><span data-stu-id="ed614-127">See Also</span></span>  
 [<span data-ttu-id="ed614-128">Подешавање ресурса</span><span class="sxs-lookup"><span data-stu-id="ed614-128">Set up resources</span></span>](../project-service/set-up-resources.md)
