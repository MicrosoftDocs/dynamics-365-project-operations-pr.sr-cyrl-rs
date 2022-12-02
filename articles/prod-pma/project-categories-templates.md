---
title: Синхронизовање категорија трошкова пројеката између финансија и операција и услуге Project Service Automation
description: Овај чланак описује предлошке и основне задатке који се користе за синхронизацију категорија задатака пројекта између услуга Microsoft Dynamics 365 Finance и Dynamics 365 Project Service Automation.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 8eba7defb93bd880db4b0e8fe425d07312cf5cb9
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028950"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a>Синхронизовање категорија трошкова пројеката између финансија и операција и услуге Project Service Automation

[!include[banner](../includes/banner.md)]

Овај чланак описује предлошке и основне задатке који се користе за синхронизацију категорија задатака пројекта између услуга Dynamics 365 Finance и Dynamics 365 Project Service Automation.

> [!NOTE]
> - Интеграција пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и закључавање функционалности доступни су у верзији 8.0.
> - Интеграција стварних података доступна је у верзији 8.0.1 или новијој.
> - Ако користите Enterprise Edition 7.3.0, када инсталирате KB 4132657 и KB 4132660, моћи ћете да користите предлошке за интегрисање пројектних задатака, категорије трансакција трошкова, процене сати, процене трошкова и стварних података, као и да конфигуришите закључавање функционалности. Ако морате да ресетујете рачуноводствене дистрибуције, препоручујемо да инсталирате и KB 4131710.

## <a name="data-flow-for-project-service-automation-and-finance"></a>Ток података за Project Service Automation и Finance

Решење за интеграцију услуга Project Service Automation и Finance користи функцију интеграције података за синхронизацију података у свим инстанцама услуга Project Service Automation и Finance. Предлошци за интеграцију који су доступни са функцијом Интеграција података омогућава ток података о категоријама пројектних задатака између услуга Finance и Project Service Automation.

Ако се категорије трошкова пројекта савладају у услузи Finance, ток интеграције је први из услуге Finance у Project Service Automation. ID-ови интеграције категорија трошкова пројекта се затим ажурирају синхронизацијом из услуге Project Service Automation у Finance.

Ако се категорије трошкова пројекта савладају у услузи Project Service Automation, ток интеграције је први из услуге Project Service Automation у Finance. Категорије пројеката морају већ бити конфигурисане у услузи Finance пре синхронизације из услуге Project Service Automation. Затим синхронизујте из услуге Finance назад у Project Service Automation, а затим поново из услуге Project Service Automation у Finance. На овај начин гарантујете да ће се категорије повезати и да се неће направити дупликати.

> [!NOTE]
> Категорије трошкова пројекта обично се савладавају у услузи Finance. Међутим, ако није такав случај или ако су категорије трошкова већ креиране у услузи Project Service Automation, прво морате синхронизовати помоћу предлошка категорија трансакција трошкова (из PSA у Fin and Ops). Затим синхронизујте помоћу предлошка категорија трансакција трошкова пројекта (из Fin and Ops у PSA). Затим би требало да још једном покренете синхронизацију из услуге Project Service Automation у Finance.
>
> Ако прво извршите синхронизацију из услуге Project Service Automation, у услузи Finance морају бити испуњени следећи захтеви:
>
> - Дељена категорија која се подудара са категоријом пројекта која је постављена у услузи Project Service Automation мора постојати и мора бити омогућена и за **Пројекат** и за **Трошак**.
> - За свако правно лице у услузи Finance са којим се мора интегрисати, морају постојати следеће категорије пројеката:
>
>     - **Категорија пројекта** постоји. 
>     - **Користи у трошку** је омогућено.
>     - **Активно у дневнику** је омогућено.
>     - **Тип трансакције** је подешен на **Трошак**.

Следећа илустрација приказује како се подаци синхронизују између услуга Project Service Automation и Finance.

[![Ток података за интеграцију услуге Project Service Automation са услугом Finance.](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a>Синхронизација категорије трошкова пројекта из услуге Finance у Project Service Automation

### <a name="template-and-task"></a>Предложак и задатак

Да бисте приступили предлошку, у Microsoft Power Apps центру администрације изаберите **Пројекти**, а затим у горњем десном углу изаберите **Нови пројекат** за одабир јавних образаца.

Следећи предложак и основни задатак који се користе за синхронизацију категорија трошкова пројекта из услуге Finance у Project Service Automation:

- **Назив предлошка у услузи Data Integration:** Категорије трансакција трошкова пројекта (из Fin and Ops у PSA)
- **Назив задатка у пројекту:** Синхронизујте категорије са PSA

### <a name="entity-set"></a>Скуп ентитета

| Finance                           | Project Service Automation |
|-----------------------------------|----------------------------|
| Ентитет интеграције за категорије | Категорије трансакција     |

### <a name="entity-flow"></a>Ток ентитета

Категоријама пројектних задатака се управља у услузи Finance и они се синхронизују са услугом Project Service Automation као категорија трансакција.

### <a name="power-query"></a>Power Query

Када се синхронизујете са услугом Project Service Automation, морате да користите Microsoft Power Query за Excel да бисте поставили врсту наплате за категорију трансакција. Предложак категорија трансакција трошкова пројекта (из Fin and Ops у PSA) пружају подразумевану колону и мапирање. Ако креирате сопствени образац, морате додати ову условну колону у услузи Power Query. Пратите ове кораке.

1. Кликните на стрелицу да бисте отворили мапирање задатка категорија пројектних трошкова у предлошку категорија трансакција трошкова пројекта (из Fin and Ops у PSA).
2. Кликните на везу **Напредни упит и филтрирање** да бисте отворили Power Query.
2. Изаберите **Додај условну колону**.
3. Унесите име за нову колону, као што је **BillingType**.
4. Унесите следећи услов: **if CATEGORYID not equal to null then 19235001, Otherwise null**.
5. Кликните на **У реду** на колони.
6. Обавезно мапирајте ову нову колону на страницу за мапирање.

Следећа илустрација приказује пример мапирања задатака предлошка у услузи Data Integration. Мапирање приказује информације о пољу које ће се синхронизовати из услуге Finance у Project Service Automation.

[![Мапирање категорије трошкова пројекта са Project Service Automation предлошком.](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a>Синхронизација категорије трошкова пројекта из услуге Project Service Automation у Finance

### <a name="template-and-task"></a>Предложак и задатак

Следећи предложак и основни задатак који се користе за синхронизацију категорија трошкова пројекта из услуге Project Service Automation у Finance:

- **Назив предлошка у услузи Data Integration:** Категорије трансакција трошкова пројекта (из PSA у Fin and Ops)
- **Назив задатка у пројекту:** Синхронизујте категорије са Fin Ops

### <a name="entity-set"></a>Скуп ентитета

| Project Service Automation | Finance                           |
|----------------------------|-----------------------------------|
| Категорије трансакција     | Ентитет интеграције за категорије |

### <a name="entity-flow"></a>Ток ентитета

Категоријама пројектних задатака се управља у услузи Finance и они се синхронизују са услугом Project Service Automation као категорија трансакција. Повратна синхронизација у Finance ажурира категорију пројекта у услузи Finance са ID-ом интеграције из услуге Project Service Automation.

### <a name="template-mapping-in-data-integration"></a>Мапирање предложака у услузи Data Integration

Следећа илустрација приказује пример мапирања задатака предлошка у услузи Data Integration.

> [!NOTE]
> Мапирање приказује информације о терену које ће се синхронизовати из услуге Project Service Automation у Finance.

[![Мапирање услуге Project Service Automation са Finance предлошком.](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]