---
title: Преглед режима управљања ресурсима
description: Ова тема пружа информације о функционалности управљања ресурсима у услузи Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4a8e605109e48b50da68abeee989f8ac8d3d659c
ms.sourcegitcommit: cf79185c8c84c55fbae55f9cfc1b17840e072b49
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3930109"
---
# <a name="resource-management-modes-overview"></a>Преглед режима управљања ресурсима

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_


Dynamics 365 Project Operations подржава два режима како бисте извршили укупан ток резервације. Режим управљања дефинисан је као параметар пројекта и може се изменити ако ваше пословање треба променити.    

## <a name="central-mode"></a>Централни режим
За организације које централизују додељивање ресурса пројектима, централни режим пружа начин да менаџери пројеката могу да дефинишу захтеве за ресурсима на нивоу пројекта. Испуњавање захтева за ресурсима делегира се менаџеру ресурса. Менаџери пројеката могу прихватити или одбити ресурсе које предложи менаџер ресурса.

![Централни режим](./media/resource-management-central.png)

Да бисте управљали ресурсима у централном режиму, погледајте:

- [Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [Резервисање именованих ресурса из потребе за ресурсима](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [Прослеђивање захтева за ресурсом](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [Испуњавање захтева за ресурсима](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [Прихватање или одбацивање предложеног ресурса пројекта у захтеву за ресурс](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>Хибридни режим
За организације којима је потребна флексибилност у расподели ресурса, хибридни режим омогућава менаџерима пројеката и менаџерима ресурса могућност да резервишу ресурсе.

![Хибридни режим](./media/resource-management-hybrid.png)

Поред подржаног процеса централног режима, погледајте следеће теме да бисте управљали свим осталим подржаним токовима резервација у хибридном режиму:

Резервисање ресурса директно у пројекту:
- [Резервисање именованих ресурса које је могуће резервисати за пројектни тим и додељивање задатака](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

Резервисање ресурса из захтева за ресурсима:
- [Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [Резервисање именованих ресурса из потребе за ресурсима](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
