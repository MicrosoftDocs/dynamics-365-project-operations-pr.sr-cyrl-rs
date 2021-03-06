---
title: Додајте Azure претплату у LCS пројекат
description: Ова тема пружа информације о томе како да повежете своју Azure претплату са LCS пројектом.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0b5703542ac58adcc710890d9676dd0090a82f25
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949061"
---
# <a name="add-an-azure-subscription-to-lcs-project"></a>Додајте Azure претплату у LCS пројекат

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

Окружења у хосту у облаку морају се применити помоћу постојеће Azure претплате. Ова тема објашњава како да повежете своју постојећу Azure претплату са LCS пројектом. 

## <a name="grant-admin-consent"></a>Дајте пристанак администратора

1. У вашем LCS пројекту, у одељку **Окружења**, изаберите **Microsoft Azure подешавања**.

![Подешавања програма Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. На страници **Подешавања пројекта**, на картици **Azure конектори**, изаберите **Одобри**. То омогућава да се окружења примене на овај пројекат.

![Azure конектори](./media/2AzureConnectors.png)

3. Поново изаберите **Одобри** да бисте пружили пристанак администратора.

![Дајте пристанак администратора](./media/3GrantAdminConsent.png)

4. Прихватите захтев за дозволе.

![Прихватите захтев за дозволе](./media/4AcceptPermissionRequest.png)

Овлашћење је сада завршено. 

![Одобрење је успешно](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a>Омогућите приступ услуге Dynamics Deployment Services вашој Azure претплати

1. Идите на [Microsoft Azure обрачун](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) и изаберите своју претплату. Услуга Dynamics Deployment Services треба да приступи овој претплати да би могла да примени окружења.

![Детаљи претплате на услугу Azure](./media/6AzureSubscription.png)

2. Изаберите **Контрола приступа (IAM)** у окну за навигацију, а затим изаберите **Додајте додељивање улога**.
3. У клизачу са десне стране изаберите **Улога сарадника** и на приложеној листи пронађите и изаберите **Dynamics Deployment Services**. 
4. Изаберите ставку **Сачувај**.

![Приступ претплати](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a>Додавање конектора за претплату у LCS пројекат

1. У вашем LCS пројекту, на страници **Microsoft Azure подешавања** изаберите **Додај** да бисте додали нови конектор.
2. Унесите свој ID Azure претплате. ID Azure претплате можете пронаћи у [Azure порталу](https://ms.portal.azure.com/), у одељку  **Подешавања**  у доњем левом углу екрана.
3. У пољу **Конфигуриши да се користи Azure Resource Manager**, изаберите **Да**.
4. Уверите се да се Azure домен закупца AAD претплате подудара са Azure претплатом у власништву домена коју користите, па изаберите **Следећи**.
5. На екрану **Microsoft Azure подешавање**, изаберите **Следећи** за потврду. Ако на овом екрану добијете грешку, вратите се у одељак [Омогућите приступ услузи Dynamics Deployment Services у Azure претплату](#provide) у овој теми и уверите се да сте завршили све кораке.
6. Преузмите Azure цертификат за управљање у локалну фасциклу на рачунару, а затим га отпремите на портал за управљање услугом Azure тако што ћете отићи на **Подешавања** > **Сертификати о управљању**. Овај цертификат ће омогућити LCS да комуницира са платформом Azure у ваше име. Овај корак можете прескочити ако ваш корисник има приступ претплати.
7. Изаберите **Следеће**.
8. Изаберите Azure регион за примену и изаберите центар података који је близу места где планирате да користите овај систем.
9.  Изаберите **Повежи се**.

Успешно сте повезали своју Azure претплату. Сада можете да примените Dynamics 365 Finance окружења хостована у облаку.


