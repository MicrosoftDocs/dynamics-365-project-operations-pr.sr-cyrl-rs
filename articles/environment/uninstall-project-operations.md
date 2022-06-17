---
title: Деинстралирање Dynamics 365 Project Operations
description: Овај чланак пружа информације о деинсталирању Dynamics 365 Project Operations.
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 33a505594d6db47b4f8a0c8a630a0836f424e7d5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911982"
---
# <a name="uninstall-dynamics-365-project-operations"></a>Деинстралирање Dynamics 365 Project Operations 

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Да бисте деинсталирали услугу Dynamics 365 Project Operations, мора вам бити додељена улога администратора.

1. Идите на ставку **Подешавања** > **Решења**.

    ![Страница Подешавања.](./media/uninstall-proj-ops-solutions.png)
  
2. Уклоните решења тачном редоследом којим су наведена у следећој табели. 

    | Корак | Назив решења                                    | Белешка                                                                                         |
    |------|----------------------------------------------------|----------------------------------------------------------------------------------------------|
    | 1 | msdyn_ProjectServiceUpgrade_managed.cab            | Ако га не нађете, прескочите ово решење.                                                            |
    | 2 | ProjectOperations_Anchor                           | Ако га не нађете, прескочите ово решење.                                                            |
    | 3 | Dynamics365ProjectOperationsDualWriteEntityMaps    | Ако га не нађете, прескочите ово решење.                                                            |
    | 4 | Dynamics365ProjectOperationsDualWrite              | Ако га не нађете, прескочите ово решење.                                                            |
    | 5 | ProjectService                                     | Нема додатних белешки.                                                                         |
    | 6 | ProjectServiceCore_Patch                           | Нема додатних белешки.                                                                         |
    | 7 | ProjectServiceCore                                 | Нема додатних белешки.                                                                         |
    | 8 | ProjectServiceDeprecatedComponents                 | Ако га не нађете, прескочите ово решење.                                                            |
    | 9 | FieldServiceCommon                                 | Потребно за двоструко писање са Дyнамицс 365 Финанце или Dynamics 365 Supply Chain Management.   |
    | 1.0. | msdyn_AssetCommon                                  | Потребно за двоструко писање са Дyнамицс 365 Финанце или Dynamics 365 Supply Chain Management.   |
    | 11. | msdyn_TESA_Anchor                                  | Обавезно за Dynamics 365 Field Service.                                                     |
    | 12 | msdyn_TESA_Patch                                   | Обавезно за Dynamics 365 Field Service.                                                     |
    | 13 | msdyn_TESA                                         | Обавезно за Dynamics 365 Field Service.                                                     |
    | 14 | ResourceSchedulingControls                         | Обавезно за Dynamics 365 Field Service.                                                     |
    | 15 | MicrosoftDynamicsScheduling3_CumulativePatch       | Обавезно за Dynamics 365 Field Service.                                                     |
    | 16 | MicrosoftDynamicsScheduling_Patch_xx               | Обавезно за Dynamics 365 Field Service.                                                     |
    | 17 | MicrosoftDynamicsScheduling                        | Обавезно за Dynamics 365 Field Service.                                                     |
    | 18 | Dynamics365FinanceAndOperationsAnchor              | Ако га не нађете, прескочите ово решење.                                                            |
    | 19 | Dynamics365Notes                                   | Ако га не нађете, прескочите ово решење.                                                            |
    | 20 | Dynamics365FinanceAndOperationsDualWriteEntityMaps | Ако га не нађете, прескочите ово решење.                                                            |
    | 21 | DualWriteCore                                      | Ако га не нађете, прескочите ово решење.                                                            |
    | 22 | Dynamics365AssetManagementApp                      | Ако га не нађете, прескочите ово решење.                                                            |
    | 23 | Dynamics365AssetManagement                         | Ако га не нађете, прескочите ово решење.                                                            |
    | 24 | Dynamics365SupplyChainExtended                     | Ако га не нађете, прескочите ово решење.                                                            |
    | 25 | Dynamics365FinanceExtended                         | Ако га не нађете, прескочите ово решење.                                                            |
    | 26 | HCMCommon                                          | Ако га не нађете, прескочите ово решење.                                                            |
    | 27 | Dynamics365FinanceAndOperationsCommon              | Ако га не нађете, прескочите ово решење.                                                            |
    | 28 | Извођач                                              | Ако га не нађете, прескочите ово решење.                                                            |
    | 29 | Dynamics365Company                                 | Ако га не нађете, прескочите ово решење.                                                            |
    | 30 | CurrencyExchangeRates                              | Ако га не нађете, прескочите ово решење.                                                            |
    | 31 | AssetCommon                                        | Ако га не нађете, прескочите ово решење.                                                            |
