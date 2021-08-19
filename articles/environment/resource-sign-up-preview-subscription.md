---
title: Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха
description: Ова тема пружа информације о начину претплате и примене услуге Project Operations за сценарије засноване на ресурсима / без залиха.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 75ee31e67018fe2a7655d8a8f11e40b433a9a5db6f8f2addac27844f18fffe8d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007884"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Ова тема објашњава како да се претплатите на понуду пробне верзије и применити Project Operations окружење за сценарије засноване на ресурсима / без залиха.

## <a name="prerequisites"></a>Предуслови
- Корисник који примени верзију за преглед мора да има глобална администраторска права у Azure закупцу. Закупца можете креирати током првог искоришћавања понуде. 
- За примену Finance окружења потребна је важећа Azure претплата која ће се наплаћивати по окружењу. Можете да користите постојећу претплату у својим организацијама или да користите [Azure пробну верзију](https://azure.microsoft.com/en-us/free/) да бисте започели. CDS окружење ће бити бесплатно за ограничен период од 30 дана.

> [!IMPORTANT]
> Само једна особа, администратор закупца, у организацији треба да извршава овај задатак. Ако нисте претплатник на ово издање, сачекајте док се ваша организација не региструје и не примите своје корисничке акредитиве.
> 
> Пробне верзије се користе једнократно у закупцу. Пробну верзију можете покренути само једном. Препоручујемо вам да креирате новог закупца у сврху пробне верзије.


### <a name="dynamics-365-project-operations-ce---preview-trial"></a>Dynamics 365 Project Operations (CE) – Пробна верзија за преглед 

Пре него што започнете, уверите се да сте пријављени у прегледач са корисничким пословним налогом у закупцу где желите преглед услуге Project Operations.

1. Искористите прву шифру понуде, **Dynamics 365 Project Operations** овде [Project Operations пробна верзија](https://aka.ms/try-po).
2. Потврдите поруџбину.

  Видећете да је понуда за потврду успешно искоришћена.

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance пробна верзија за преглед

Идите на [пробну верзију за преглед услуге Dynamics 365 for Finance](https://aka.ms/trypoche) и поновите кораке из претходног одељка са понудом, Пријавите се за окружење које се хостује у облаку.  

## <a name="assign-licenses"></a>Додељивање лиценци

> [!IMPORTANT]
> Требаће вам административни приступ Microsoft 365 порталу ваше организације да бисте извршили следеће кораке.

1. Идите у [Microsoft 365 центар администрације](https://portal.office.com/) да доделите лиценце својим корисницима.

2. На страници **Активни корисници**, изаберите кориснике којима желите да доделите лиценцу.

3. Проверите да ли је изабрана лиценца **Dynamics 365 Project Operations**, па изаберите **Сачувај промене**.

> [!NOTE]
> Понуду за пробну верзију услуге Finance не треба доделити кориснику.

## <a name="start-a-new-project-in-lcs"></a>Започните нови пројекат у LCS

Направите нови LCS пројекат како је описано у теми [Започните нови пројекат у LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>Додајте Azure претплату у LCS пројекат

Да бисте довршили овај задатак, следите кораке у теми [Додавање Azure претплате у LCS пројекат](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>Примените Finance демо окружење са услугом Project Operations за сценарије ресурса / без залиха

Следите смернице у теми [Обезбеђење новог окружења](resource-provision-new-environment.md) да бисте завршили примену. Користите [демо окружење](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) тип примене за преглед. 

## <a name="install-cds-setup-and-configuration-data"></a>Инсталирајте податке о подешавању и конфигурацији CDS

Инсталирајте податке о подешавању и конфигурацији CDS како је описано у теми [Подесите и примените податке о конфигурацији у услузи Common Data Service](resource-apply-pro-setup-config-data.md).
Довршите овај корак тек након што се примени демо окружење услуге Finance и демо подаци буду спремни.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
