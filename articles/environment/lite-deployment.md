---
title: Примена услуге Project Operations – једноставно
description: Овај чланак пружа информације о томе како да инсталирате примену услуге Project Operations једноставна примена – од погодбе до профактуре.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 86293b725e86db3d4b8bdaf5810b16b7c670e8a3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930336"
---
# <a name="deploy-project-operations---lite"></a>Примена услуге Project Operations – једноставно

_**Односи се на:** Једноставна примена – од погодбе до профактуре_



Project Operations подржава више модела примене. Да бисте утврдили најбољи модел примене, погледајте чланак [Врсте примена](determine-deployment-type.md).


> [!IMPORTANT]
> Ова примена, Lite примена – од погодбе до профактуре, резултира **само у Project Operations примени у услузи Dataverse**.

- [Инсталирање услуге Project Operations у ново Dataverse окружење](#new)
- [Инсталирајте у постојеће Dataverse окружење](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a>Инсталирање услуге Project Operations у ново Dataverse окружење

1. Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, креирајте ново Dataverse окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com). Уверите се да су омогућени **Креирање базе података за ово окружење** и **Dynamics 365 апликације**. За више информација, погледајте одељак [Креирање и управљање окружењима у Power Platform центру администрације](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Изаберите **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a>Инсталирање услуге Project Operations у постојеће Dataverse окружење
1. Уверите се да окружење није конфигурисано са [двоструким уписивањем](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) јер ће инсталација,тада инсталирати могућности [Project Operations за сценарије засноване на ресурсима/без залиха](project-operations-integrated-deployment-overview.md).
2. Као [глобални или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) са лиценцом за Project Operations, лоцирајте окружење у [PowerPlatform центру администрације](https://admin.powerplatform.com) где желите да инсталирате Project Operations.
3. Инсталирајте **Microsoft Dynamics 365 Project Operations** са листе за примену Dynamics 365 апликација. Више информација потражите у чланку [Управљање Dynamics 365 апликацијама](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
