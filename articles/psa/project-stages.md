---
title: Типови фаза пројеката
description: Ова тема пружа информације о стварним фазама пројекта.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: aa423979a794b07a8bd27440f47a29480b74b518
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123080"
---
# <a name="project-stage-types"></a>Типови фаза пројеката 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Фазе пројекта се дизајнирају тако да одражавају статус пројекта током његовом напретка. Прилагођавања се могу користити за аутоматско ажурирање фаза са токовима пословних процеса, Power Automate или проширења додатних компоненти.

Следеће фазе су дефинисане у подразумеваном току пословног процеса:

- Нови
- Понуда
- План
- Испорука
- Довршено
- Затворите 

## <a name="new"></a>Ново

Када креирате пројекат, фаза пројекта се подешава на **Ново**. Ако је пројекат креиран из предлошка, можда ће имати распоред, процену и податке о тиму. У супротном, то је само скица пројекта, а преостале компоненте морају бити унете.

## <a name="quote"></a>Понуда

Када повежете пројекат са понудом или га креирате из понуде, фаза пројекта се подешава на **Понуда**, а процењени датум почетка и завршетка се ажурирају. Док је пројекат је у фази **понуде**, картица **Продаја** на страници **Ентитет пројекта** приказује детаље понуде.

## <a name="plan"></a>План

Када вам буде одобрена понуда повезана са пројектом и када се пројекат пребаци у фазу **уговора**, фаза пројекта се ажурира на **План**. Док је пројекат је у фази **плана**, на страници **Ентитет пројекта** се приказују детаљи уговора.

## <a name="deliver"></a>Испорука

Када је пројектни план завршен, а ви сте спремни за почетак пројекта, менаџер пројекта треба да ажурира фазу пројекта на **Испорука** да би показао да је пројекат започет.

## <a name="complete"></a>Довршено 

Када је посао за пројекат завршен, менаџер пројекта може да ажурира фазу на **Довршено**. Ажурирањем фазе пројекта на **Довршено**, менаџер пројекта показује да је посао завршен 100%, али да је пројекат и даље отворен тако да се могу евидентирати било какве ставке времена или трошкова на чекању.

## <a name="close"></a>Затворите

Када се све трансакције евидентирају за пројекат, менаџер пројекта може да ажурира фазу на **Затворено**. У том тренутку не могу се евидентирати никакве трансакције и пројект се подешава на „само за читање“.