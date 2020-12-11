---
title: Поруџбенице за пројекат
description: Овај чланак описује разне методе помоћу којих можете да креирате поруџбенице за пројекат. Начин који користите зависи од сврхе поруџбенице и од тога када се купљене ставке користе и наплаћују пројекту.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083960"
---
# <a name="purchase-orders-for-a-project"></a>Поруџбенице за пројекат

[!include [banner](../includes/banner.md)]

Овај чланак описује разне методе помоћу којих можете да креирате поруџбенице за пројекат. Начин који користите зависи од сврхе поруџбенице и од тога када се купљене ставке користе и наплаћују пројекту.

### <a name="methods-for-creating-a-purchase-order"></a>Методе за креирање поруџбенице

Можете да користите један од следећих метода за креирање поруџбенице у управљању пројектима и рачуноводству. Сврха поруџбенице одређује када се поруџбеница користи и, стога, када се ставке наплаћују пројекту.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Метод</th>
<th>Сврха</th>
<th>Потрошња ставки</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Креирајте поруџбеницу директно из пројекта.</td>
<td>Ову методу користите за куповину ставки од спољног продавца за потрошњу на пројекту. Поруџбеницу можете креирати на два начина:
<ul>
<li>Из самог пројекта. У овом случају, пројекат је већ дефинисан за поруџбеницу.</li>
<li>Навигацијом до поруџбенице за пројекат. Морате изабрати продавца и пројекат за који ћете креирати поруџбеницу.</li>
</ul></td>
<td>Ставке се користе када се фактура добављача ажурира.</td>
</tr>
<tr class="even">
<td>Креирајте поруџбеницу директно из улазне поруџбине.</td>
<td>Користите овај метод за куповину ставки када креирате улазну поруџбину из пројекта.</td>
<td>Ставке се користе када се поруџбеница фактурише клијенту.</td>
</tr>
<tr class="odd">
<td>Креирајте поруџбеницу на основу захтева за ставку.</td>
<td>Користите овај метод за куповину ставки када креирате захтев за ставку из пројекта.</td>
<td>Ставке се користе када се ажурира отпремница захтева.</td>
</tr>
</tbody>
</table>

> [!NOTE] 
> Када ажурирате фактуру добављача или отпремницу, од вас ће се затражити да ажурирате отпремницу према захтеву за ставку.

За више информација погледајте [Пријем ставки по поруџбеници из захтева за ставку](tasks/receive-items-purchase-order-item-requirement.md).
