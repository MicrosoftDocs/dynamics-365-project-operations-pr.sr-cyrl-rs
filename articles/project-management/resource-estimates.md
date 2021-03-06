---
title: Процене ресурса
description: Ова тема пружа информације о томе како се израчунавају процене ресурса у услузи Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: f255b2cbf290973ce62fe2c1c121bd1df15a7392
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/01/2020
ms.locfileid: "3928604"
---
# <a name="resource-estimates"></a>Процене ресурса

_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_

Процене ресурса потичу из ангажовања у времену које је дефинисано у структурној анализи посла заједно са применљивим димензијама за одређивање цена. Типично, прорачун је **сатница за сваку улогу x број сати.** Ангажовање у времену за сваки ресурс ускладиштено је у запису о додели ресурса. Одређивање цена се складишти у унапред дефинисаном ценовнику. Конверзија јединица примењује се на основу важећег ценовника.

![Процене ресурса](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a>Подразумевана цена коштања и валута трошкова

Цене трошкова подразумевано долазе из организационе јединице.

## <a name="default-bill-rate-and-sales-currency"></a>Подразумевана стопа наплате и продајна валута

Продајне цене се примењују једном по погодби. Хијерархија продајног ценовника подразумевано је следећа:

1. Организација
2. Клијент
3. Понуда/уговор
