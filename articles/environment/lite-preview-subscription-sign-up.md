---
title: Пријављивање за претплату на преглед – једноставно
description: Ова тема пружа информације о томе како да се претплатите и примените услугу Project Operations Lite – од погодбе до профактуре.
author: sigitac
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4de51277e5a08690cc16497e3916f40498b39fb8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997439"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>Пријављивање за претплату на преглед – једноставно 

Ова тема објашњава како да се претплатите на понуду партнера за преглед и примените посао везан за Dynamics 365 Project Operations једноставну примену на профактуру.

> [!NOTE]
> Овај поступак ће се променити у предстојећим издањима услуге Project Operations.

## <a name="prerequisites"></a>Предуслови

- Добићете е-поруку са позивом да учествујете у прегледу. Можете затражити верзију за преглед на [Project Operations веб-локацији](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Корисник који примени верзију за преглед мора да има глобална администраторска права у Azure закупцу.
- Прегледајте све услове и одредбе.

## <a name="subscribe"></a>Претплати се

Када добијете [захтев за преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) одобрење, добићете две понуде од компаније Microsoft е-поштом. Ове понуде вам омогућавају да примените верзију за преглед услуге Project Operations:

- Dynamics 365 Project Operations (CRM) – пробна верзија за преглед
- Office 365 Project Operations – Пробна верзија за преглед

> [!IMPORTANT]
> Само једна особа, администратор закупца, у организацији треба да извршава овај задатак. Ако нисте претплатник на ово издање, сачекајте док се ваша организација не региструје и не примите своје корисничке акредитиве.

### <a name="dynamics-365-project-operations-crm---preview-trial"></a>Dynamics 365 Project Operations (CRM) – пробна верзија за преглед 

Пре него што започнете, уверите се да сте пријављени у прегледач са корисничким пословним налогом у закупцу где желите преглед услуге Project Operations.

1. Искористите први кôд понуде, **Dynamics 365 Project Operations (CRM) – преглед пробне верзије** тако што ћете га налепити у URL прегледача.

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

2. На страници **Активни корисници**, изаберите кориснике којима желите да доделите лиценцу.

![Доделите лиценце](./media/15AssignLicenses.png)

3. Проверите да ли су изабране лиценце за **Dynamics 365 Project Operations (CRM) верзију за преглед** и **Office 365 Project Operations – верзију за преглед**. 
4. Изаберите **Сачувај промене**.

## <a name="create-a-new-cds-environment"></a>Направите ново CDS окружење

1. Обезбедите ново окружење за примену услуге Project Operations CDS пратећи упутства у теми [Модел примене CDS-а](lite-deployment.md). Када одаберете тип окружења, обавезно користите **пробну верзију (засновано на претплати)**.
![Ново окружење](./media/19CreateEnvironment.png)

2. Изаберите подешавање **Омогућите Dynamics 365 апликације** и оставите **Аутоматски примени ове апликације** празно.  
3. Изаберите **Сачувај** да бисте креирали окружење.

![Додај базу података](./media/20CreateEnvironment1.png)

4. Када креирате окружење, инсталирајте **Microsoft Dynamics 365 Project Operations** решење. 

![Инсталирање решења](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>Инсталирање CDS конфигурације и подешавање демо података

Инсталирајте CDS конфигурацију и подесите демо податке пратећи упутства у теми [Примените демо подешавања и података о конфигурацији](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]