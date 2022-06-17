---
title: Најчешћа питања о управљању ресурсима
description: Овај чланак пружа одговоре на најчешћа питања о управљању ресурсима.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 6610098737b79d76b38c3d467135b9118c2a8ec7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8913362"
---
# <a name="resource-management-faq"></a>Најчешћа питања о управљању ресурсима

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a>Која је разлика између члана тима и потребе за ресурсом?

Члан пројектног тима може бити додељен задацима, резервисан или пребукиран, као и подешен као давалац одобрења. Потреба за ресурсом може постојати без члана пројектног тима, као радна верзија напомене о потражњи. 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a>Која је разлика између предложених и условно резервираних сати?

Предложени сати и условно резервисани сати разликују се по видљивости. Предложени сати су видљиви само менаџерима ресурса и менаџеру пројеката који су покренули потражњу користећи захтев за ресурс. Условно резервисани сати су видљиви свима који имају приступ табели распореда.

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a>Како могу да видим условно резервисане сате за ресурсе у тиму?

Условне резервације можете да обавите када резервишете потребу за ресурсом. Ресурси који су условно резервисани у пројектном тиму приказују се као чланови тима који имају условно резервисане сате. Приказују се и на табели распореда.

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a>Како да променим захтеване сате, датум почетка и завршетка за (генерички или именовани) ресурс који је резервисан?

Након резервисања ресурса, изаберите **Одржавање резервација** да унесете промене које су неопходне.

## <a name="what-resources-types-does-project-service-automation-support"></a>Које врсте ресурса подржава Project Service Automation?

**Корисник** и **Контакт** су једине врсте ресурса које подржава Dynamics 365 Project Service Automation. Иако можете да креирате друге врсте ресурса (на пример, **Опрема** и **Група**), ниједан случај њиховог комплетног коришћења није подржан.

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a>Која је разлика између доделе и резервације?

Доделе представљају додела ресурса пројектним задацима у распореду пројеката. Ресурси могу бити стварни или генерички ресурси. Резервације представљају фиксну или условну расподелу ресурса за пројекат. Фиксне резервације троше капацитет ресурса. Идеално би било да се за стварне ресурсе слажу резервације и доделе, јер се не разликују. Међутим, PSA не спроводи овај договор. Приказ Усаглашеност показује менаџеру пројеката места где се резервације и доделе ресурса не слажу.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
