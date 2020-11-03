---
title: Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха
description: Ова тема пружа информације о начину претплате и примене услуге Project Operations за сценарије засноване на ресурсима / без залиха.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7a03f021b1ae0a87dfc947976b8a16c8246e1684
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083858"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Ова тема објашњава како се претплатити на верзију за преглед / партнерску понуду и примену Project Operations окружења за сценарије засноване на ресурсима / без залиха.

## <a name="prerequisites"></a>Предуслови

- Добићете е-поруку са позивом да учествујете у прегледу. Можете затражити верзију за преглед на [Project Operations веб-локацији](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Корисник који примени верзију за преглед мора да има глобална администраторска права у Azure закупцу.
- За примену Finance окружења потребна је важећа Azure претплата која ће се наплаћивати по окружењу. Можете да користите постојећу претплату у својим организацијама или да користите [Azure пробну верзију](https://azure.microsoft.com/en-us/free/) да бисте започели. CDS окружење ће бити бесплатно за ограничен период од 30 дана.

## <a name="subscribe"></a>Претплати се

Када ваш [захтев за преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) буде одобрен, добићете три понуде од компаније Microsoft е-поштом. Ове понуде вам омогућавају да примените верзију за преглед услуге Project Operations:

- Dynamics 365 Project Operations (CRM) – Пробна верзија за преглед
- Office 365 Project Operations – Пробна верзија за преглед
- Dynamics 365 Finance – Пробна верзија за преглед

> [!IMPORTANT]
> Само једна особа, администратор закупца, у организацији треба да извршава овај задатак. Ако нисте претплатник на ово издање, сачекајте док се ваша организација не региструје и не примите своје корисничке акредитиве.

### <a name="dynamics-365-project-operations-crm---preview-trial"></a>Dynamics 365 Project Operations (CRM) – Пробна верзија за преглед 

Пре него што започнете, уверите се да сте пријављени у прегледач са корисничким пословним налогом у закупцу где желите преглед услуге Project Operations.

1. Искористите прву шифру понуде, **Dynamics 365 Project Operations (CRM) – Пробна верзија за преглед** њеним лепљењем у URL прегледача.

![Искористите понуду](./media/16RedeemFirstOfferNew.png)

2. Потврдите поруџбину.

![Потврдите поруџбину](./media/17ConfirmOrderNew.png)

Видећете да је понуда за потврду успешно искоришћена.

![Потврда](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a>Office 365 Project Operations – Пробна верзија за преглед

Поновите исте кораке као код прве шифре понуде. Обавезно додајте другу шифру понуде користећи исти кориснички налог који је коришћен са првом шифром понуде.

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance пробна верзија за преглед

Поновите исте кораке са последњом понудом из е-поруке добродошлице.

## <a name="assign-licenses"></a>Додељивање лиценци

> [!IMPORTANT]
> Требаће вам административни приступ Microsoft 365 порталу ваше организације да бисте извршили следеће кораке.

1. Идите у [Microsoft 365 центар администрације](https://portal.office.com/) да доделите лиценце својим корисницима.

![Почетна страница центра администрације](./media/14AdminPortal.png)

2. На страници **Активни корисници** , изаберите кориснике којима желите да доделите лиценцу.

![Доделите лиценце](./media/15AssignLicenses.png)

3. Проверите да ли су изабране лиценце за **Dynamics 365 Project Operations (CRM) верзију за преглед** и **Office 365 Project Operations – верзију за преглед** и изаберите **Сачувај промене**.

> [!NOTE]
> Понуду за пробну верзију услуге Finance не треба доделити кориснику.

## <a name="start-a-new-project-in-lcs"></a>Започните нови пројекат у LCS

Направите нови LCS пројекат како је описано у теми [Започните нови пројекат у LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>Додајте Azure претплату у LCS пројекат

Да бисте довршили овај задатак, следите кораке у теми [Додавање Azure претплате у LCS пројекат](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>Примените Finance демо окружење са услугом Project Operations за сценарије ресурса / без залиха

Следите смернице у теми [Обезбеђење новог окружења](resource-provision-new-environment.md) да бисте завршили примену. Користите [демо окружење](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) тип примене за преглед. 

## <a name="install-cds-setup-and-configuration-data"></a>Инсталирајте податке о подешавању и конфигурацији CDS

Инсталирајте податке о подешавању и конфигурацији CDS како је описано у теми [Подесите и примените податке о конфигурацији у услузи Common Data Service](resource-apply-pro-setup-config-data.md).
Довршите овај корак тек након што се примени демо окружење услуге Finance и демо подаци у FO буду спремни.
