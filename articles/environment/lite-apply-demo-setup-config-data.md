---
title: Примена демо подешавања и података о конфигурацији – једноставно
description: Ова тема пружа информације о томе како да примените демо подешавања и податке о конфигурацији за Project Operations.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 694dbc74591de74895095a9da6e590069711fc83
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290152"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>Примена демо подешавања и података о конфигурацији за Project Operations – једноставно 

_**Једноставна примена – од погодбе до профактуре_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a>Предуслови

Пре него што започнете конфигурацију, морате имати Common Data Service (CDS) окружење предвиђено за Dynamics 365 Project Operations.


## <a name="instructions"></a>Упутства

1. Преузмите [Пакет главних података](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip). 
2. Идите у фасциклу *ProjOpsDemoDataSetupAndMaster - Integrated CMT* и покрените извршну датотеку *DataMigrationUtility*.
3. На 1. страници Common Data Service чаробњака за конфигурисање миграције (CMT) изаберите **Увези податке**, а затим изаберите **Настави**.

    ![Миграција конфигурације](./media/1ConfigurationMigration.png)

4. На 2. страници CMT чаробњака изаберите **Microsoft 365** као **Тип примене**.
5. Изаберите поља за потврду **Прикажи листу доступних организација** и **Прикажи напредно**.
6. Изаберите регион вашег закупца, унесите своје акредитиве, а затим изаберите **Пријављивање**.

   ![Пријављивање у конфигурацију](./media/2ConfigurationSignin.png)

7. На страници 3, са листе организација у закупцу, изаберите у коју организацију желите да увезете демо податке, а затим изаберите **Пријављивање**.
8. На 4. страници изаберите zip датотеку *MasterAndSetupData* из распаковане фасцикле *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.

   ![Компримована датотека](./media/3ZipFile.png)

   ![Избор датотеке](./media/4SelectAFile.png)

9. Када изаберете zip датотеку, изаберите **Увоз података**.

   ![Увоз података](./media/5ImportData.png)

10. Увоз ће трајати отприлике од два до десет минута, у зависности од брзине ваше мреже. По завршетку изађите из CMT чаробњака. 
11. Потражите у својој организацији податке за следећих 20 ентитета:

    -   Валута
    -   Налог
    -   Организациона јединица
    -   Контакт
    -   Јединица
    -   Група јединица
    -   Ценовник
    -   Ценовник параметара пројекта 
    -   Учесталост фактурисања
    -   Категорија ресурса који може да се резервише
    -   Категорија трансакције
    -   Категорија трошка
    -   Цена улоге
    -   Цена категорије трансакције
    -   Карактеристика
    -   Ресурс који може да се резервише
    -   Повезивање категорије ресурса који може да се резервише
    -   Карактеристика ресурса који може да се резервише

    ![Комплетан увоз](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]