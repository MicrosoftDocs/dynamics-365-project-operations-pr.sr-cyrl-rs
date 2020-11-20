---
title: Анализа понуда за пројекат
description: Ова тема пружа информације о анализи понуда за пројекат.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 6ed900620f92e76d293f6b533b101be94b25cff3
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127041"
---
# <a name="analysis-of-project-quotes"></a>Анализа понуда за пројекат

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation анализира понуде за пројекат ради процене профитабилности. Такође анализира колико је понуда усаглашена са очекивањима клијента о датуму испоруке или завршетка, као и са буџетом.

## <a name="profitability-analysis"></a>Анализа исплативости

Project Service Automation анализира профитабилност коришћењем бруто марже и кориговане бруто маргине.

- Бруто марже се израчунавају помоћу следеће формуле:

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- Коригована бруто маржа се израчунавају помоћу следеће формуле:

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

Ако се вредности бруто марже и кориговане бруто марже значајно разликују, већи део посла у понуди је класификован као ненаплатив.

## <a name="analysis-of-customer-expectations"></a>Анализа очекивања клијента

Можете анализирати понуде и генерисати графиконе за очекивања клијената у вези са распоредом и буџетом ако унесете вредности за следећа поља:

- Поље **Захтевани датум испоруке** у заглављу понуде.
- Поље **Буџет клијента** за сваку ставку понуде (за ставке засноване на пројекту и ставке засноване на производу).

Анализа очекивања клијената у вези са распоредом се врши поређењем најновијег датума завршетка детаља ставке понуде са захтеваним датумом испоруке за све ставке понуде у понуди.

Анализа очекивања клијената у вези са буџетом врши се поређењем збира укупног буџета клијента са понуђеним износом у свим ставкама понуде.
