---
title: Пријавите се за претплату на преглед
description: Ова тема пружа информације о томе како да се претплатите и примените услугу Project Operations Lite – од погодбе до профактуре.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5342466f308ab62a9f73a85fbd838d7c33bb1f47
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4083835"
---
# <a name="sign-up-for-a-preview-subscription-for-lite-deployment--deal-to-proforma-invoicing"></a>Пријавите се за претплату на верзију за преглед за лагану примену – од погодбе до профактуре

Ова тема објашњава како да се претплатите на партнерску понуду за верзију за преглед и примените услугу Dynamics 365 Project Operations Lite у једноставној примени – од погодбе до профактуре.

> [!NOTE]
> Овај поступак ће се променити у предстојећим издањима услуге Project Operations.

## <a name="prerequisites"></a>Предуслови

- Добићете е-поруку са позивом да учествујете у прегледу. Можете затражити верзију за преглед на [Project Operations веб-локацији](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Корисник који примени верзију за преглед мора да има глобална администраторска права у Azure закупцу.
- Прегледајте све услове и одредбе.

## <a name="subscribe"></a>Претплати се

Када добијете [захтев за преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) одобрење, добићете две понуде од компаније Microsoft е-поштом. Ове понуде вам омогућавају да примените верзију за преглед услуге Project Operations:

- Dynamics 365 Project Operations (CRM) – Пробна верзија за преглед
- Office 365 Project Operations – Пробна верзија за преглед

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

## <a name="assign-licenses"></a>Додељивање лиценци

> [!IMPORTANT]
> Требаће вам административни приступ Microsoft 365 порталу ваше организације да бисте извршили следеће кораке.


1. Идите у [Microsoft 365 центар администрације](https://portal.office.com/) да доделите лиценце својим корисницима.

![Почетна страница центра администрације](./media/14AdminPortal.png)

2. На страници **Активни корисници** , изаберите кориснике којима желите да доделите лиценцу.

![Доделите лиценце](./media/15AssignLicenses.png)

3. Проверите да ли су изабране лиценце за **Dynamics 365 Project Operations (CRM) верзију за преглед** и **Office 365 Project Operations – верзију за преглед**. 
4. Изаберите **Сачувај промене**.

## <a name="create-a-new-cds-environment"></a>Направите ново CDS окружење

1. Обезбедите ново окружење за примену услуге Project Operations CDS пратећи упутства у теми [Модел примене CDS-а](lite-deployment.md). Када одаберете тип окружења, обавезно користите **пробну верзију (засновано на претплати)**.
![Ново окружење](./media/19CreateEnvironment.png)

2. Изаберите подешавање **Омогућите Dynamics 365 апликације** и оставите **Аутоматски примени ове апликације** празно.  
3. Изаберите **Сачувај** да бисте креирали окружење.

![Додај базу података](./media/20CreateEnvironment1.png)

4. Након креирања окружења, инсталирајте решење **Microsoft Dynamics 365 Project Operations**. 

![Инсталирање решења](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>Инсталирање CDS конфигурације и подешавање демо података

Инсталирајте CDS конфигурацију и подесите демо податке пратећи упутства у теми [Примените демо подешавања и података о конфигурацији](lite-apply-demo-setup-config-data.md).
