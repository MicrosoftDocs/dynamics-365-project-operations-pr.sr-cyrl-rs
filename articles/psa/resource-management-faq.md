---
title: Најчешћа питања о управљању ресурсима
description: Ова тема нуди одговоре на најчешћа питања о управљању ресурсима.
author: ruhercul
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: d335a12a9b478bff63b6c93809c89dac9718a4be
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144386"
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
