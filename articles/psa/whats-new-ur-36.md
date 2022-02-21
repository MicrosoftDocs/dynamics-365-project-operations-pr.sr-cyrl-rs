---
title: Шта је ново или промењено у издању 36 исправке Project Service Automation верзије 3
description: У овој теми наведене су функције и исправке које су доступне у издању 36 исправке услуге Microsoft Dynamics 365 Project Service Automation верзије 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/06/2021
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
ms.openlocfilehash: 9b85aed79acb7e7784a23f54a2e9af1cc83f5f4d
ms.sourcegitcommit: 6d9fc4dc851814664bf71729904ab4bedd85fe70
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/06/2021
ms.locfileid: "7606815"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-36-v3"></a>Шта је ново или промењено у издању 36 исправке Project Service Automation верзије 3

[!include [banner](../includes/psa-now-project-operations.md)]

Задовољство нам је да најавимо најновију исправку за апликацију Microsoft Dynamics 365 Project Service Automation. Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Компатибилна је са системом Dynamics 365 9.x. Да бисте се ажурирали на ово издање, посетите страницу центра администрације за Dynamics 365 мрежна решења и инсталирајте исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

У овој теми наведене су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 36. Ова верзија има број верзије V3.10.57.152 и опште је доступна путем само-исправке у октобру 2021. године.

## <a name="update-release-36"></a>Издање исправке 36

### <a name="bug-fixes"></a>Исправке грешака

Поправљени су следећи проблеми.

**Опште**
- Назив поља **Подразумевани предложак радних часова** погрешно је преведен на страници **Параметри пројекта**.
- Додатне компоненте за асинхронизацију не управљају исправно са изузецима везаним за **SharedVariableService**.

**Време и трошак**
- Када ставке у главној књизи недостају или корисник нема одговарајуће привилегије за читање ставки у главној књизи, долази до грешке при отказивању одобрења пројекта.
- Корисници не могу да откажу одобрење ако ставка трошкова или времена има више од једног придруженог одобрења пројекта.
- **Одсуство** и **Годишњи одмор** су погрешно преведени за кинески језик у претрази на страници за брзо креирање **Ставка времена**.

**Управљање ресурсима**
- Корисник не може тражити ресурсе у **Помоћнику за заказивање** када је режим приказа подешен на **Дан**, **Недеља** или **Месец**.
- Генеричким ресурсима је погрешно дозвољено да имају празна имена радних места. 
- Затварање уговора као неоствареног не отказује будуће резервације.

**Продаја**
- Када окружење има велику количину производа, перформансе се смањују у табели **Процена материјала**.
- Приликом креирања пројекта из предлошка, валута пројекта није подразумевана за одговарајућу уговорну јединицу одговарајућег вође пројекта.
- Стварни износи не одговарају увек ономе што се се налази у доспелом пројекту, или износи постају негативни у специфичним сценаријима опозива.
- До грешке долази када пројекат који сте креирали из предлошка пројекта повежете са предметом уговора.
- Корисници могу да обришу предмет уговора са контролним тачкама, **Спремно за фактурисање** и **Фактура је направљена**. Ово не би требало дозволити.
- Када се процене увезу из пројекта, могућност наплате детаља ставке понуде је погрешно подешена када је за ставку понуде омогућена наплата заснована на задацима.
- Када додате контролну тачку у наплати по фиксној цени, та контролна тачка се не одражава у подмрежи контролних тачака све док се страница не освежи.
- Изузетак нулте референце генерише се када креирате уговор о пројекту са називом понуде који је без вредности.
- Задаци у ручном режиму у којима се валута пројекта разликује од валуте извора доводе до погрешних процена цене.
- Корисници не могу да се сете трансакције која је успешно исправљена корективном фактуром.
- Деактивиране категорије трансакција појављују се у мрежи **Процене трошкова**.


