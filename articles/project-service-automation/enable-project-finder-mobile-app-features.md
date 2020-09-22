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
# <a name="enable-project-finder-mobile-app-features-project-service"></a>Омогућавање функција апликације Project Finder Mobile (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Ваши ресурси могу да користе апликацију Project Finder Mobile на телефону уз [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] да проналазе нове пројекте на којима ће радити и да ажурирају скупове вештина.  
  
 Апликација је доступна за [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] телефоне и [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].  
  
 Треба да подесите неколико опција у поставкама параметара за организациону јединицу да бисте омогућили корисницима преглед захтева за ресурсима у пројектима и ажурирање њихових вештина.  
  
> [!NOTE]
>  Апликација Project Finder Mobile ради само са системом [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], а не са локалним инсталацијама.  
  
1. Идите на **Project Service > Параметри**.  
  
2. Кликните на поставку параметара које желите да користите да бисте омогућили функције апликације Project Finder Mobile.  
  
3. У области **Општи подаци**, поставите **Захтеви у погледу ресурса видљиви ресурсима** на **Да**.  
  
4. Подесите **Дозволи да ресурси освеже вештине** на **Да**.  
  
   ![ProjectService_ProjectFinderEnable](../project-service/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")  
  
   Ово је глобално подешавање. Менаџери пројекта треба да подесе да ли ће појединачни пројекат бити видљив на страници **Пројектни тим** тог пројекта.  
  
   ![ProjectService_ProjectTeamVisible](../project-service/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")  
  
## <a name="email-notifications"></a>Обавештења путем е-поште  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] шаље е-поруке које се односе на захтеве за ресурсима следећим примаоцима следећим терминима:  
  
|Прималац|Догађај|  
|---------------|-----------|  
|Менаџер пројекта|-   Када је ресурс пријављен за пројекат преко апликације Project Finder Mobile.|  
|Ресурс|-   Када је посао на пројекту за који се ресурс пријавио већ испуњен од стране другог ресурса.<br />-   Када њихови захтеви за одобрењем вештине буду одобрени или одбачени.<br />-   Када њихови захтеви за пријављивање у пројекат буду одобрени или одбачени.|  
  
## <a name="privacy-notice"></a>Обавештење о приватности  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a>Такође погледајте  
 [Подешавање ресурса](../project-service/set-up-resources.md)
