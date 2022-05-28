---
title: Примена услуге Project Operations – једноставно
description: Ова тема пружа информације о томе како да инсталирате примену услуге Project Operations Lite – од погодбе до профактуре.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: e33506504665f2e7ef7ad48469082f9f64a2a44b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580750"
---
# <a name="deploy-project-operations---lite"></a>Примена услуге Project Operations – једноставно

_**Односи се на:** Једноставна примена – од погодбе до профактуре_



Project Operations подржава више модела примене. Да бисте утврдили најбољи модел примене, погледајте чланак [Врсте примена](determine-deployment-type.md).


> [!IMPORTANT]
> Ова примена, Lite примена – од погодбе до профактуре, резултира **само у Project Operations примени у услузи Dataverse**.

- [Инсталирање операција пројекта у ново Dataverse окружење](#new)
- [Инсталирање у постојеће Dataverse окружење](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a> Инсталирање операција пројекта у ново Dataverse окружење

1. Као глобални [или администратор са Power Platform лиценцом](/power-platform/admin/global-service-administrators-can-administer-without-license) за пројектне операције, креирајте ново Dataverse окружење у [ПоwерПлатформ админ центру](https://admin.powerplatform.com). Уверите се да **је омогућено креирање базе података** за **ово окружење и Дyнамицс 365** апликације. За више информација, погледајте одељак [Креирање и управљање окружењима у Power Platform центру администрације](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Изаберите **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a> Инсталирање пројектних операција у постојеће Dataverse окружење
1. Уверите се да окружење није конфигурисано са двоструким [уписивања као](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) инсталацијом, а затим ћете [инсталирати операције пројекта за могућности сценарија заснованих на ресурсима/неодовршеним](project-operations-integrated-deployment-overview.md) сценаријима.
2. Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, лоцирајте окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com) где желите да инсталирате Project Operations.
3. Инсталирајте **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација. Више информација потражите у чланку [Управљање Dynamics 365 апликацијама](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
