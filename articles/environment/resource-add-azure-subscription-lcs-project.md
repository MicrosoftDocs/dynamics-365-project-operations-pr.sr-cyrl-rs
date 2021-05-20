---
title: Додајте Azure претплату у LCS пројекат
description: Ова тема пружа информације о томе како да повежете своју Azure претплату са LCS пројектом.
author: sigitac
manager: Annbe
ms.date: 04/12/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a80c926ba67a1620e39d8c7677a05678454e6340
ms.sourcegitcommit: 7468d668c48c1d87934aab9a034decd51e56dec6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/13/2021
ms.locfileid: "5880556"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a>Додајте Azure претплату у LCS пројекат

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
6. Преузмите Azure цертификат за управљање у локалну фасциклу на рачунару. Замолите администратора претплате за Azure да отпреми сертификат на портал за управљање услугом Azure тако што ће одабрати претплату и отићи на **Подешавања** > **Сертификати о управљању**. Овај сертификат омогућава LCS-у да у ваше име комуницира са услугом Azure. Овај корак можете прескочити ако ваш корисник има приступ претплати.
7. Изаберите **Следеће**.
8. Изаберите Azure регион за примену и изаберите центар података који је близу места где планирате да користите овај систем.
9.  Изаберите **Повежи се**.

Успешно сте повезали своју Azure претплату. Сада можете да примените Dynamics 365 Finance окружења хостована у облаку.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
