---
title: Пословне трансакције
description: Ова тема пружа информације о пословним трансакцијама.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: 048bd2d98e6332e6c48a24f4eacee5b937ef04a9
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126996"
---
# <a name="business-transactions"></a>Пословне трансакције

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

У апликацији Dynamics 365 Project Service Automation *пословна трансакција* је апстрактни концепт који не представља ниједан ентитет. Међутим, нека уобичајена поља и процеси у ентитетима су дизајнирани да користе концепт пословних трансакција. Следећи ентитети користе ову апстракцију:

- Детаљи ставке понуде
- Детаљи предмета уговора
- Ставке процене
- Ставке у главној књизи
- Стварне вредности

Од ових ентитета, Детаљи ставке понуде, Детаљи предмета уговора и Ставке процене се мапирају на фазу процене у животном циклусу пројекта. Ставке у главној књизи и ентитети стварних вредности се мапирају на фазу извршавања у животном циклусу пројекта.

PSA третира записе у ових пет еититета као пословне трансакције. Једина разлика је у томе што се записи у ентитетима који су мапирани на фазу процене сматрају финансијским проценама, док се записи у ентитетима који су мапирани на фазу извршења сматрају финансијским чињеницама које су се већ догодиле.

Више информација потражите у чланку [Процене](estimates.md) и [Стварне вредности](actuals.md).

## <a name="concepts-that-are-unique-to-business-transactions"></a>Концепти који су јединствени за пословне трансакције
Следећи концепти су јединствени за концепт пословних трансакција:

- Тип трансакције
- Класа трансакције
- Порекло трансакције
- Веза трансакције

### <a name="transaction-type"></a>Тип трансакције

Врста трансакције представља трајање и контекст финансијског утицаја на пројекат. Представља је скуп опција са следећим подржаним вредности у апликацији PSA:
- Трошкови
- Уговор за пројекат
- Ненаплаћена продаја
- Наплаћена продаја
- Продаја између организација
- Трошкови јединице за обезбеђивање ресурса

### <a name="transaction-class"></a>Класа трансакције

Класа трансакције представља различите врсте трошкова који се остварују на пројектима. Представља је скуп опција са следећим подржаним вредности у апликацији PSA:

- Time
- Трошак
- Материјал
- Накнада
- Контролна тачка
- Порез

Вредност **Контролна тачка** обично користи пословна логика за наплату фиксне цене у апликацији PSA.

### <a name="transaction-origin"></a>Порекло трансакције

Порекло трансакције је ентитет који складишти порекло сваке пословне трансакције. Како се извршава пројекат, свака пословна трансакција ће створити још једну пословну трансакцију, која ће заузврат створити другу, и тако даље. Ентитет порекла трансакције дизајниран је за складиштење података о пореклу сваке трансакције, како би се олакшало извештавање и праћење ентитета. 

### <a name="transaction-connection"></a>Веза трансакције

Веза трансакције је ентитет који складишти однос између две сличне пословне трансакције, као што су трошкови и припадајуће стварне вредности продаје или сторнирање трансакција које активирају активности наплате као што су потврда фактуре или корекције фактура.

Порекло трансакције и Веза трансакције вам заједно помажу да пратите односе између пословних трансакција и радњи које су довеле до креирања одређене пословне трансакције.

### <a name="example-how-transaction-origin-works-with-transaction-connection"></a>Пример: Како порекло трансакције функционише са везом трансакције

Следећи пример приказује типичну обраду ставки времена у животном циклусу пројекта у апликацији PSA.

> ![Обрада ставки времена у животном циклусу услуге Project Service](media/basic-guide-17.png)
 
1. Прослеђивање ставке времена узрокује креирање две ставке у главној књизи: једне за трошкове и једне за ненаплаћену продају.
2. Крајње одобравање ставке времена узрокује креирање две стварне вредности: једне за трошкове и једне за ненаплаћену продају.
3. Када корисник креира фактуру за пројекат, трансакција ставке фактуре се креира коришћењем података из стварне вредности ненаплаћене продаје. 
4. Када је фактура потврђена, креирају се две нове стварне вредности: сторнирање ненаплаћене продаје и стварна вредност наплаћене продаје.

Сваки од ових догађаја покреће креирање записа у ентитетима Порекло трансакције и Веза трансакције да би могли да се прате односи између ових записа који су креирани у детаљима ставке времена, ставке у главној књизи, стварних вредности и ставке фактуре.

Следећа табела приказује записе у ентитету Порекло трансакције за претходни ток посла.

| Догађај                        | Порекло                   | Тип порекла                       | Трансакција                       | Тип трансакције         |
|------------------------------|--------------------------|-----------------------------------|-----------------------------------|--------------------------|
| Прослеђивање ставке времена        | GUID записа ставке времена   | Ставка времена                        | GUID записа ставке у главној књизи (трошкови)   | Ставка у главној књизи             |
| GUID записа ставке времена       | Ставка времена               | GUID записа ставке у главној књизи (продаја)  | Ставка у главној књизи                      |                          |
| Одобрење времена                | GUID записа ставке у главној књизи | Ставка у главној књизи                      | GUID записа ненаплаћене продаје        | Стварно                   |
| GUID записа ставке времена       | Ставка времена               | GUID записа ненаплаћене продаје        | Стварно                            |                          |
| GUID записа ставке у главној књизи     | Ставка у главној књизи             | GUID записа стварних вредности           | Стварно                            |                          |
| GUID записа ставке времена       | Ставка времена               | GUID записа стварних вредности           | Стварно                            |                          |
| Креирање фактуре             | GUID записа ставке времена   | Ставка времена                        | GUID трансакције ставке фактуре     | Трансакција ставке фактуре |
| GUID записа ставке у главној књизи     | Ставка у главној књизи             | GUID трансакције ставке фактуре     | Трансакција ставке фактуре          |                          |
| Потврђивање фактуре         | GUID ставке фактуре        | Ставка фактуре                      | GUID записа наплаћене продаје          | Стварно                   |
| GUID фактуре                 | Фактура                  | GUID записа наплаћене продаје          | Стварно                            |                          |
| GUID детаља ставке фактуре     | Детаљ ставке фактуре      | GUID записа наплаћене продаје          | Стварно                            |                          |
| GUID записа ставке времена       | Ставка времена               | GUID записа наплаћене продаје          | Стварно                            |                          |
| GUID записа ставке у главној књизи     | Ставка у главној књизи             | GUID записа наплаћене продаје          | Стварно                            |                          |
| GUID записа ставке времена       | Ставка времена               | GUID сторнирања ненаплаћене продаје      | Стварно                            |                          |
| GUID записа ставке у главној књизи     | Ставка у главној књизи             | GUID сторнирања ненаплаћене продаје      | Стварно                            |                          |
| Корекција радне верзије фактуре     | GUID старог детаља ставке фактуре             | Трансакција ставке фактуре          | GUID исправке детаља ставке фактуре               | Трансакција ставке фактуре |
| GUID старе ставке фактуре                  | Ставка фактуре             | GUID исправке детаља ставке фактуре               | Трансакција ставке фактуре          |                          |
| GUID старе фактуре             | Фактура                  | GUID исправке детаља ставке фактуре               | Трансакција ставке фактуре          |                          |
| GUID записа ставке времена       | Ставка времена               | GUID исправке детаља ставке фактуре               | Трансакција ставке фактуре          |                          |
| GUID записа ставке у главној књизи     | Ставка у главној књизи             | GUID исправке детаља ставке фактуре               | Трансакција ставке фактуре          |                          |
| Потврђена корекција фактуре | GUID старог детаља ставке фактуре             | Трансакција ставке фактуре          | GUID сторниране стварне вредности наплаћене продаје | Стварно                   |
| GUID старе ставке фактуре                  | Ставка фактуре             | GUID сторниране стварне вредности наплаћене продаје | Стварно                            |                          |
| GUID старе фактуре             | Фактура                  | GUID сторниране стварне вредности наплаћене продаје | Стварно                            |                          |
| GUID записа ставке времена       | Ставка времена               | GUID сторниране стварне вредности наплаћене продаје | Стварно                            |                          |
| GUID записа ставке у главној књизи     | Ставка у главној књизи             | GUID сторниране стварне вредности наплаћене продаје | Стварно                            |                          |
| GUID старог детаља ставке фактуре                 | Трансакција ставке фактуре | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |
| GUID старе ставке фактуре                  | Ставка фактуре             | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |
| GUID старе фактуре             | Фактура                  | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |
| GUID записа ставке времена       | Ставка времена               | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |
| GUID записа ставке у главној књизи     | Ставка у главној књизи             | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |
| GUID исправке детаља ставке фактуре          | Трансакција ставке фактуре | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |
| GUID исправке ставке фактуре           | Ставка фактуре             | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |
| GUID исправљене фактуре      | Фактура                  | GUID нове ненаплаћене стварне вредности продаје    | Стварно                            |                          |

Следећа табела приказује записе у ентитету Веза трансакције за претходни ток посла.

| Догађај                          | 1. трансакција                 | Улога 1. трансакције | Тип 1. трансакције           | 2. трансакција                | Улога 2. трансакције | Тип 2. трансакције |
|--------------------------------|-------------------------------|--------------------|------------------------------|------------------------------|--------------------|--------------------|
| Прослеђивање ставке времена          | GUID ставке у главној књизи (продаја)     | Ненаплаћена продаја     | msdyn_journalline            | GUID ставке у главној књизи (трошкови)     | Трошкови               | msdyn_journalline  |
| Одобрење времена                  | GUID ненаплаћене стварне вредности (продаја)  | Ненаплаћена продаја     | msdyn_actual                 | GUID стварне вредности трошкова (трошкова)       | Трошкови               | msdyn_actual       |
| Креирање фактуре               | GUID детаља ставке фактуре      | Наплаћена продаја       | msdyn_invoicelinetransaction | GUID ненаплаћене стварне вредности продаје   | Ненаплаћена продаја     | msdyn_actual       |
| Потврђивање фактуре           | GUID сторнираних стварних вредности         | Сторнирање          | msdyn_actual                 | GUID оригиналне ненаплаћене продаје | Оригинално           | msdyn_actual       |
| GUID наплаћене продаје              | Наплаћена продаја                  | msdyn_actual       | GUID ненаплаћене стварне вредности продаје   | Ненаплаћена продаја               | msdyn_actual       |                    |
| Корекција радне верзије фактуре       | GUID трансакције ставке фактуре | Замена          | msdyn_invoicelinetransaction | GUID наплаћене продаје            | Оригинално           | msdyn_actual       |
| Потврђивање корекције фактуре     | GUID сторнирања наплаћене продаје    | Сторнирање          | msdyn_actual                 | GUID наплаћене продаје            | Оригинално           | msdyn_actual       |
| GUID нове ненаплаћене стварне вредности продаје | Замена                     | msdyn_actual       | GUID наплаћене продаје            | Оригинално                     | msdyn_actual       |                    |