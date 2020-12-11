---
title: Шта је ново новембра 2020. – Једноставна примена услуге Project Operations – од погодбе до профактуре
description: Ова тема пружа информације о исправкама квалитета доступним у издању једноставне примене услуге Project Operations за новембар 2020. – од погодбе до профактуре.
author: sigitac
manager: Annbe
ms.date: 11/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: fa95406a27e6d32d2be75303904547b59f24c8b2
ms.sourcegitcommit: 64d0de964a9b66c015ffcf1db62cbb6216cb3187
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 11/03/2020
ms.locfileid: "4367194"
---
# <a name="whats-new-november-2020---project-operations-lite-deployment---deal-to-proforma-invoicing"></a>Шта је ново новембра 2020. – Једноставна примена услуге Project Operations – од погодбе до профактуре

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Следећа табела наводи исправке за Project Operations у CDS окружењу верзије 4.4.0.70.

| Област функција                 | Референтни број | Исправка квалитета                                                                                                                                                                    |
|------------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   Управљање могућностима за пословање       | 2036993          | Предмети уговора за ставке процене и доделу ресурса ажурирају се на добитним понудама када ставка понуде има тип **Сви задаци**.                                                 |
|   Управљање могућностима за пословање       | 2071514          | Не могу да креирам фактуру за контролну тачку са фиксном ценом на уговору који има омогућен обрачун заснован на задатку.                                                                          |
| Наплата и одређивање цена          | 2070392          | Предмети уговора за пројекат на фактури се повећавају сваки пут када изаберете **Освежи трансакције фактуре**.                                                                       |
| Планирање пројекта             | 2043336          | Није могуће избрисати запис члана пројектног тима.                                                                                                                                    |
| Планирање пројекта             | 2046013          | Недоследно понашање за означавање колона Процене током учитавања у односу на промену типа временске фазе.                                                                                   |
| Планирање пројекта             | 2046647          | Време почетка и завршетка су померени за сат времена када захтеве за ресурсима генеришу чланови пројектног тима.                                                                      |
| Планирање пројекта             | 2053879          | (По предстојећем увођењу CDS-а) PublishUnassignedAssignments прекида покушај чувања задатка када је грешка „Вредност прослеђена за ConditionOperator.In празна“. |
| Планирање пројекта             | 2055501          | Ако **Датум почетка пројекта** остане празан, долази до неуспеха у распореду.                                                                                                      |
| Планирање пројекта             | 2066817          | Не могу да направим генерички ресурс помоћу бирача људи на картици **Задаци**.                                                                                               |
| Планирање пројекта             | 2067034          | Дугме **Приказ детаља** није доступно на страници **Детаљи задатка**.                                                                                                         |
| Управљање ресурсима          | 2046667          | Чланови генеричког тима се не бришу чак ни када се сви ресурси испуне.                                                                                                     |
| Ставка времена и брзог трошка | 2047499          | Дугме **Ново** на страници Ставка времена отвара страницу **Нов потпис е-поште**.                                                                                               |
| Ставка времена и брзог трошка | 2059859          | Отвара се неочекивани искачући прозор приликом креирања ставке трошка.                                                                                                                         |
| Други                        | 2044181          | [Деинсталација PO] – Долази до грешке „Запис није доступан“ када покушате да деинсталирате основна решења **msdyn_ProjectServiceCore_Patch** и msdyn Project Service.        |