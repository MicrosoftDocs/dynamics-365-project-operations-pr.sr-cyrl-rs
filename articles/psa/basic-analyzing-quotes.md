---
title: Анализа понуда за пројекат
description: Овај чланак пружа информације о анализи понуда за пројекат.
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 9db924c16c5eca17e7962ff1d88b09e581347fa5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8919296"
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
