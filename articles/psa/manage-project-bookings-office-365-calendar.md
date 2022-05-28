---
title: Управљање пројектима и резервацијама у Office 365 календару
description: Како да управљате пројектима и резервацијама у Office 365 календару
author: ruhercul
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
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: cf51333179d2d972af84de7adb4b718b6e17d038
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/14/2022
ms.locfileid: "8598920"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a>Управљање пројектима и резервацијама у календару (Project Service)

> [!Note]
> ЗАСТАРЕЛО: Ова функција је застарела и није више доступна.

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

Прикажите личне заказане обавезе, резервације пројеката и посла, као и доделе радних налога у апликацији field service коришћењем [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календара.  
  
 Када је све на једном месту, лако је управљати вашим даном. Ваши састанци, заказане обавезе, резервације и задаци су сви доступни у вашем [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календару.  
  
 Ако користите [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], можете унети и ваше личне заказане обавезе у приказу уноса времена за Project Service. На тај начин менаџери пројекта и ресурса знају вашу доступност за пројекте. То вам штеди и време, јер не морате да уносите информације о вашим личним заказаним обавезама двапут. Можете једноставно да увезете личне заказане обавезе из календара у приказ уноса времена у апликацији Project Service.  
  
 Ваш календара ће синхронизовати пројекат и резервације радних налога од данас до предстојеће четири недеље. Ово подешавање не може да се промени.  
  
 Синхронизација је подржана само у једном смеру, из PSA на ваш [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календар. Можете да синхронизујете обрнутим редоследом. 
  
 Да бисте сазнали како да користите [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календар, погледајте [Календар у програму Outlook на вебу за предузећа](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936)  
  
## <a name="setup"></a>Инсталација  
 Пре него што можете да видите и управљате резервацијама у вашем [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календару, морате да подесите неколико ствари.  
  
- Биће вам потребни акредитиви [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] глобалног администратора или администратора система.  
  
- Ваш администратор ће морати да конфигурише профилу сервера е-поште и сваки корисник ће морати да конфигурише своје поштанско сандуче. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Подешавање обраде е-поште путем синхронизације на страни сервера](/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a>Укључите синхронизацију за организацију (задатак администратора)  
  
1.  У главном менију кликните на **Подешавања** > **Администрација**.  
  
2.  Кликните на **Системска подешавања**.  
  
3.  Кликните на картицу **Синхронизација**.  
  
4.  У оквиру опције **Изаберите да ли желите да омогућите синхронизацију резервације ресурса са** означите **Синхронизуј резервацију ресурса са програмом Outlook**.  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a>Укључите синхронизацију за ваш кориснички профил (задатак корисника)  
  
1.  Кликните на дугме **Подешавања** у горњем десном углу екрана.  
  
2.  Кликните на дугме **Опције**.  
  
3.  Кликните на картицу **Синхронизација**.  
  
4.  У оквиру **Синхронизација резервације ресурса са програмом Outlook**, означите **Синхронизација резервације ресурса са програмом Outlook**.  
  
## <a name="import-your-personal-appointments-user-task"></a>Увезите ваше личне заказане обавезе (задатак корисника)  
 Можете да увезете личне заказане обавезе из календара у приказ уноса времена у апликацији Project Service Automation.  
  
1. Отворите [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] календар и кликните на **Увоз података**.  
  
2. На екрану Филтери изаберите **Заказане обавезе из услуге Exchange**, а затим кликните на **Примени**.  
  
3. Систем ће извући заказане обавезе у приказу уноса времена као предложеним уносима за тренутну недељу. Да бисте додали ставке за другу недељу, кликните на дугме **Претходно** или **Следеће**.  
  
4. Изаберите заказану обавезу коју желите да додате у приказ уноса времена у апликацији Project Service Automation.  
  
5. У искачућем пољу **Унос времена** изаберите одговарајуће опције за конвертовање заказане обавезе у приказ уноса времена у апликацији Project Service Automation.  
  
6. Кликните на **Сачувај**.  
  
### <a name="see-also"></a>Такође погледајте  
 [Водич за време, трошак и сарадњу](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
