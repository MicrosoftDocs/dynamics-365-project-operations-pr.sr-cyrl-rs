---
title: Шта је ново или промењено у издању 40 исправке Project Service Automation верзије 3
description: У овом чланку наведене су функције и исправке које су доступне у издању 40 исправке услуге Microsoft Dynamics 365 Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/31/2022
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
ms.openlocfilehash: dca7f340b8d544b183aa0390ac3c11a38f536ed0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912810"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>Шта је ново или промењено у издању 40 исправке Project Service Automation верзије 3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Компатибилна је са системом Dynamics 365 9.x. Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

У овом чланку дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 40. Ова верзија има број верзије V3.10.61.61 и генерално је доступна путем самосталног ажурирања у фебруаре 2022.

## <a name="update-release-40"></a>Издање исправке 40

### <a name="features"></a>Функције
Прва фаза надоградње 1 са Project Service Automation на Project Operations – једноставном применом биће објављена у фебруару 2022. године за све клијенте. Да бисте проверили да ли испуњавате услове, погледајте [Надоградња са апликације Project Service Automation на услугу Project Operations](upgrade-project-operations-non-stocked.md). Ако се апликација не појави у вашој инстанци у Power Platform центру администрације, обратите се подршци и затражите да то буде омогућено за ваша окружења. Ваш захтев мора да садржи листу ID-ова окружења где је потребно омогућити апликацију.

### <a name="bug-fixes"></a>Исправке грешака

Поправљени су следећи проблеми.

**Време и трошак**
- Ставка белешке недостаје када је ставка времена одбијена или отказана. 

**Продаја**

- Када ажурирате процену цене или продаје коришћењем готових додатних компоненти, неисправно вам је дозвољено да шаљете JSON корисне податке који нису важећи изван корисничког интерфејса.
- Када ажурирате редове понуде помоћу брзог приказа, дозвољено вам је да активирате понуде.
