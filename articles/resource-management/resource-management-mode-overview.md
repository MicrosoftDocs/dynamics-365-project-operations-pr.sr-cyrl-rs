---
title: Преглед режима управљања ресурсима
description: У овој теми дате су информације о функцији управљања ресурсима у услузи Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 5c0f98a6f08129ebef9b6d3fed1cc85969aa347c815a643d3c8dd639b42c0e8c
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "7008244"
---
# <a name="resource-management-modes-overview"></a>Преглед режима управљања ресурсима

_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_


Dynamics 365 Project Operations подржава два режима како бисте извршавали укупан ток резервације. Режим управљања дефинисан је као параметар пројекта и може се изменити ако ваше пословање треба променити.    

## <a name="central-mode"></a>Централни режим
За организације које централизују додељивање ресурса пројектима, централни режим пружа начин да менаџери пројеката могу да дефинишу захтеве за ресурсима на нивоу пројекта. Испуњавање захтева за ресурсима делегира се менаџеру ресурса. Менаџери пројеката могу прихватити или одбити ресурсе које предложи менаџер ресурса.

![Централни режим.](./media/resource-management-central.png)

Да бисте управљали ресурсима у централном режиму, погледајте:

- [Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима](/dynamics365/project-service/assign-generic-bookable-resource)
- [Резервисање именованих ресурса из потребе за ресурсима](/dynamics365/project-service/book-named-resource)
- [Прослеђивање захтева за ресурсом](/dynamics365/project-service/submit-resource-request)
- [Испуњавање захтева за ресурсима](/dynamics365/project-service/resource-management-fulfill-requests)
- [Прихватање или одбацивање предложеног ресурса пројекта у захтеву за ресурс](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>Хибридни режим
За организације којима је потребна флексибилност у расподели ресурса, хибридни режим омогућава менаџерима пројеката и менаџерима ресурса могућност да резервишу ресурсе.

![Хибридни режим.](./media/resource-management-hybrid.png)

Поред подржаног процеса централног режима, погледајте следеће теме да бисте управљали свим осталим подржаним токовима резервација у хибридном режиму:

Резервисање ресурса директно у пројекту:
- [Резервисање именованих ресурса које је могуће резервисати за пројектни тим и додељивање задатака](/dynamics365/project-service/assign-named-bookable-resource)

Резервисање ресурса из захтева за ресурсима:
- [Додељивање генеричких ресурса који се могу резервисати задатку и генерисање потреба за ресурсима](/dynamics365/project-service/assign-generic-bookable-resource)
- [Резервисање именованих ресурса из потребе за ресурсима](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]