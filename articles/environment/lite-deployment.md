---
title: Примена лите пројектних операција
description: Овај чланак пружа информације о томе како да инсталирате примену услуге Project Operations једноставна примена – од погодбе до профактуре.
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810997"
---
# <a name="deploy-project-operations-lite"></a>Примена лите пројектних операција

_**Односи се на:** Једноставна примена – од погодбе до профактуре_



Project Operations подржава више модела примене. Да бисте утврдили најбољи модел примене, погледајте чланак [Врсте примена](determine-deployment-type.md).


> [!IMPORTANT]
> Ова примена, Lite примена – од погодбе до профактуре, резултира **само у Project Operations примени у услузи Dataverse**.

- [Инсталирање услуге Project Operations у ново Dataverse окружење](#new)
- [Инсталирајте у постојеће Dataverse окружење](#existing)
- [Инсталирање у постојеће окружење  Dataverse  које има Дуал wрите компоненте](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a> Инсталирање програма Пројецт Оператионс Лите у ново  Dataverse  окружење

1. Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, креирајте ново Dataverse окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com). Уверите се да су омогућени **Креирање базе података за ово окружење** и **Dynamics 365 апликације**. За више информација, погледајте одељак [Креирање и управљање окружењима у Power Platform центру администрације](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
1. Изаберите **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a> Инсталирање програма Пројецт Оператионс Лите у постојеће  Dataverse  окружење 
1. Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, лоцирајте окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com) где желите да инсталирате Project Operations.
1. Инсталирајте **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација. Више информација потражите у чланку [Управљање Dynamics 365 апликацијама](/power-platform/admin/manage-apps).

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a> Инсталирање програма Пројецт Оператионс Лите у постојеће окружење где  Dataverse  су дуална решења за писање већ присутна

Ако желите да наставите са покретањем операција пројекта у режиму примене лите, требало би да следите ове кораке:

1. Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, лоцирајте окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com) где желите да инсталирате Project Operations.
1. Инсталирајте **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација. Више информација потражите у чланку [Управљање Dynamics 365 апликацијама](/power-platform/admin/manage-apps).
1. Пошто ваше окружење има инсталиране Дуал wрите компоненте које помажу у интеграцији апликација за финансирање и операције, инсталација операција пројекта ће такође инсталирати могућности и проширења потребна за интегрисање података везаних за пројекат за финансирање и операције апликација. Пошто желите да покренете операције пројекта у лите распоређивању, ове компоненте интеграције би требало да буду уклоњене јер ће креирати ограничења и индиректне трошкове за сценарије примене лите. Ручно деинсталирајте решења Дуал  **Dynamics 365 Project Operations  Wрите**  и  **Dynamics 365 Project Operations  Дуал Wрите Ентитy Мапс да бисте**  уклонили ове компоненте.
1. Идите на  **локацију Пројецт Оператионс -> Сеттингс -> Параметерс**. Отворите страницу  **"Детаљи параметра**  пројекта" и поставите поље  **Понашање надоградње**  решења на опцију  **"Само лите"**. Овим се обезбеђује да наредне надоградње операција пројекта неће вратити компоненте интеграције у операције пројекта.  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
