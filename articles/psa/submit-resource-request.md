---
title: Прослеђивање захтева за ресурс
description: Ова тема пружа информације о прослеђивању захтева за ресурс пројекта.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: bcea3d640d7e9ee2b071c55bff9ade3268edb319
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084065"
---
# <a name="submitting-a-resource-request"></a>Прослеђивање захтева за ресурс

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Генерисану потребу за ресурсом можете проследити као захтев за ресурс. Захтев се затим шаље менаџеру ресурса ради испуњавања.

1. У апликацији Project Service Automation (PSA), на страници **Пројекти** кликните на картицу **Тим** да бисте видели листу ресурса који се могу резервисати. 
2. Са листе изаберите генерички ресурс који има потребу за ресурсом, а затим кликните на **Проследи захтев**.

![Прослеђивање захтева за ресурс](media/RM-how-to-18.png)

Статус захтева генеричког члана тима ће се променити у **Прослеђен**.

Када менаџер ресурса испуни захтев, генерички ресурс ће бити замењен именованим ресурсом ако менаџер ресурса испуни захтев резервисањем именованог ресурса. У супротном, генерички ресурс ће остати у тиму и статус захтева ће се променити у **Захтева преглед** ако је менаџер ресурса предложио именовани ресурс.
