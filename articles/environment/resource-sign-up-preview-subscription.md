---
title: Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха
description: Ова тема пружа информације о начину претплате и примене услуге Project Operations за сценарије засноване на ресурсима / без залиха.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d35a8bf9e8a841b45808b26ae2587c5b7d99d72
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949062"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Пријављивање за претплате на верзију за преглед услуге Project Operations за сценарије ресурса / без залиха

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Ова тема објашњава како се претплатити на верзију за преглед / партнерску понуду и примену Project Operations окружења за сценарије засноване на ресурсима / без залиха.

## <a name="prerequisites"></a>Предуслови

- Добићете е-поруку са позивом да учествујете у прегледу. Можете затражити верзију за преглед на [Project Operations веб-локацији](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Корисник који примени верзију за преглед мора да има глобална администраторска права у Azure закупцу.
- За примену Finance окружења потребна је важећа Azure претплата која ће се наплаћивати по окружењу. Можете да користите постојећу претплату у својим организацијама или да користите [Azure пробну верзију](https://azure.microsoft.com/en-us/free/) да бисте започели. CDS окружење ће бити бесплатно за ограничен период од 30 дана.

## <a name="subscribe"></a>Претплати се

Када ваш [захтев за преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) буде одобрен, добићете две понуде од компаније Microsoft е-поштом. Ове понуде вам омогућавају да примените верзију за преглед услуге Project Operations:

- Dynamics 365 Project Operations – Пробна верзија за преглед
- Dynamics 365 for Finance and Operations пробна верзија за преглед.

> [!IMPORTANT]
> Само једна особа, администратор закупца, у организацији треба да извршава овај задатак. Ако нисте претплатник на ово издање, сачекајте док се ваша организација не региструје и не примите своје корисничке акредитиве.

### <a name="dynamics-365-project-operations--preview-trial"></a>Dynamics 365 Project Operations – Пробна верзија за преглед

1. Искористите прву понуду, **Пробна верзија услуге Dynamics 365 Project Operations**, са URL-ом наведеним у е-поруци добродошлице.

![Прва понуда](./media/1FirstOffer.png)

2. Потврдите да сте пријављени као корисник који припада организацији која ће се претплатити на услугу.
3. Наставите са искоришћавањем понуде. 
4. Изаберите **Да, додај на мој налог**.

![Искористите понуду](./media/2RedeemFirstOffer.png)

![Потврдите понуду](./media/3ConfirmFirstOffer.png)

![Понуда је искоришћена](./media/4OfferSuccessfulyRedeemed.png)

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance пробна верзија за преглед

Поновите исте кораке са другом понудом из е-поруке добродошлице.

## <a name="assign-licenses"></a>Доделите лиценце

> [!IMPORTANT]
> Требаће вам административни приступ Office 365 порталу ваше организације да бисте извршили следеће кораке.

1. Идите у [Microsoft 365 центар администрације](https://portal.office.com/) да доделите лиценце својим корисницима.

![Office портал за администрацију](./media/5OfficeAdminPortal.png)

2. На страници **Активни корисници**, изаберите кориснике којима желите да доделите лиценцу.

![Доделите лиценце](./media/6AssignLicenses.png)

3. Проверите да ли је изабрана Project Operations лиценца и изаберите **Сачувај промене**. 

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

