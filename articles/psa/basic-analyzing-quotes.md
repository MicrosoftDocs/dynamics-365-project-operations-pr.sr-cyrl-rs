---
title: Анализа понуда за пројекат
description: Ова тема пружа информације о анализи понуда за пројекат.
author: rumant
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
ms.openlocfilehash: b50f419d2c13cff4914f4b589c8d7ad9099c8734834d75f8d17104d2db40049b
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "7002844"
---
# <a name="analysis-of-project-quotes"></a>Анализа понуда за пројекат

[!include [banner](../includes/psa-now-project-operations.md)]

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


[!INCLUDE[footer-include](../includes/footer-banner.md)]