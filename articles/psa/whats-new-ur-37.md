---
title: Шта је ново или промењено у издању 37 исправке за Project Service Automation верзије 3
description: У овом чланку наведене су функције и исправке које су доступне у издању 37 исправке услуге Microsoft Dynamics 365 Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 11/01/2021
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
ms.openlocfilehash: bdbb125b4f41bb9970f5bd8a01cf0bb863c34738
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922516"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-37-v3"></a>Шта је ново или промењено у издању 37 исправке за Project Service Automation верзије 3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Компатибилна је са системом Dynamics 365 9.x. Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

У овом чланку дате су функције које су нове или су промењене у издању исправке 37 у решењу Project Service Automation у верзији 3. Ова верзија има број V3.10.58.120 и опште је доступна кроз самосталну исправку у новембру 2021.

## <a name="update-release-37"></a>Издање исправке 37

### <a name="bug-fixes"></a>Исправке грешака

Поправљени су следећи проблеми.

**Време и трошак**
- Корисници не могу да бришу унос времена тако што ће обрисати ћелију.
- Приказ **Моје неуспело одобрење** садржи само одобрења пројеката са статусом **Послато**.

**Управљање пројектима**
- Корисници добијају грешку у изузетку без референце приликом отварања пројекта у програмском додатку Microsoft за рачунаре ако је назив позиције члана пројектног тима празан.
- Не постоји дугме **Сачувај** на страници **Пројектни задатак** тако да корисници не могу да сачувају промене на записима пројекта.
- Корисници не могу да избришу пројекат који има задатак повезан са понудом са статусом **Освојено**.

**Продаја**
- Поље **Валута** на страници **Пројекат** се ажурира тако да се подудара са примењеном валутом предлошка.
- Цена се неправилно израчунава за задатке који имају више валута.
