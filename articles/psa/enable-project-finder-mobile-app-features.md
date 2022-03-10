---
title: Омогућавање функција апликације Project Finder Mobile
description: Како да омогућите функције апликације Project Finder Mobile за апликацију Project Service
author: JohnPBurrows
ms.prod: ''
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
ms.openlocfilehash: 8651ba591853faf648587dcbd4c50625ba94360958d7b418e89aa0bf09464a89
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "7004914"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a>Омогућавање функција апликације Project Finder Mobile (Project Service)

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Ваши ресурси могу да користе апликацију Project Finder Mobile на телефону уз [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] да проналазе нове пројекте на којима ће радити и да ажурирају скупове вештина.  
  
 Апликација је доступна за [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] телефоне и [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].  
    
 Да бисте омогућили корисницима преглед захтева за ресурсе у пројектима и ажурирање њихових вештина, морате да изаберете опције у подешавањима параметара за организациону јединицу.
  
> [!NOTE]
>  Апликација Project Finder Mobile ради само са системом [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], а не са локалним инсталацијама.  
  
1. Идите на **Project Service > Параметри**.  
  
2. Кликните на поставку параметара које желите да користите да бисте омогућили функције апликације Project Finder Mobile.  
  
3. У области **Општи подаци**, поставите **Захтеви у погледу ресурса видљиви ресурсима** на **Да**.  
  
4. Подесите **Дозволи да ресурси освеже вештине** на **Да**.  
  
   ![ProjectService_ProjectFinderEnable.](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")  
  
   Ово је глобално подешавање. Менаџери пројекта треба да подесе да ли ће појединачни пројекат бити видљив на страници **Пројектни тим** тог пројекта.  
  
   ![ProjectService_ProjectTeamVisible.](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")  
  
## <a name="email-notifications"></a>Обавештења путем е-поште  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] шаље е-поруке које се односе на захтеве за ресурсима следећим примаоцима следећим терминима:  
  
|Прималац|Догађај|  
|---------------|-----------|  
|Менаџер пројекта|- Ресурс се пријављује за пројекат преко апликације Project Finder Mobile.|  
|Ресурс|- Посао на пројекту за који се ресурс пријавио је већ испуњен од стране другог ресурса.<br />- Захтеви за одобрење вештине су одобрени или одбачени.<br />- Захтеви за пријављивање у пројекат су одобрени или одбачени.|  
  
## <a name="privacy-notice"></a>Обавештење о приватности  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a>Такође погледајте  
 [Подешавање ресурса](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]