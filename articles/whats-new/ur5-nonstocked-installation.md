---
title: Ажурирање услуге Project Operations у Finance окружењу
description: Ова тема пружа информације о томе како да ажурирате услугу Project Operations у Dynamics 365 Finance окружењу.
author: ruhercul
manager: tfehr
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 249b8dba17165da04596ec46a625131b9b4daeb5
ms.sourcegitcommit: f4fc6e3a81e8551da050e92f8fde85f8d7b52fbd
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 12/29/2020
ms.locfileid: "4816643"
---
# <a name="update-project-operations-in-your-finance-environment"></a>Ажурирање услуге Project Operations у Finance окружењу

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_


Ова тема пружа информације о томе како да ажурирате Dynamics 365 Project Operations у Dynamics 365 Finance окружењу. Постоје три процедуре потребне за ажурирање услуге Project Operations на исправку 5 (Microsoft Dynamics CRM 2011 Update Rollup 5):

- [Увоз пакета у пројекат прегледа](#import)
- [Примена исправке](#apply)
- [Ажурирање Dataverse окружења](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a>Увоз пакета у LCS пројекат

1. Пријавите се на [Lifecycle Services (LCS)](https://lcs.dynamics.com/) као власник пројекта или менаџер окружења.
2. Са листе пројеката одаберите LCS пројекат.
3. На страници **Пројекат** у групи **Окружења** отворите окружење које желите да ажурирате.
4. Проверите да ли је окружење покренуто. Ако није покренуто, покрените окружење.
5. У одељку **Ново издање** под **Доступне исправке** изаберите **Прикажи исправку** за 10.0.15.

![Дугме „Прикажи исправку“](media/view-update.png)

6. На страници **Бинарна ажурирања** изаберите **Сачувај пакет**.
7. На страници **Преглед и чување исправки** изаберите **Сачувај пакет**.
8. У окну **Чување пакета у библиотеци средстава** које се отвори унесите назив пакета, а затим изаберите **Сачувај пакет**.
9. Када LCS заврши чување пакета, дугме **Готово** ће бити омогућено. Изаберите **Готово**. LCS ће верификовати пакет. Верификација може трајати неколико минута, највише до сат времена.


## <a name="apply-the-package-update"></a><a name="apply"></a>Примена исправке пакета

1. У услузи LCS, на страници **Детаљи окружења** изаберите **Одржавај** > **Примени исправке**.
2. На листи изаберите пакет који сте раније сачували, а затим изаберите **Примени**.
3. Изаберите **Да** да бисте потврдили да желите да примените пакет.

![Потврдите избор у дијалогу „Примена пакета“](media/confirm-package-deployment.png)

4. Изаберите **Да** да бисте потврдили да желите да ажурирате апликацију.

![Потврдите избор у дијалогу „Ажурирање апликације“](media/confirm-application-update.png)

Покренуће се примена и ажурирање апликације. 

На страници **Детаљи окружења**, у горњем десном углу, статус окружења ће се ажурирати на **Сервисирање**. За отприлике два сата ажурирање ће бити готово. Информације о издању апликације ће се ажурирати на **Microsoft Dynamics 365 for Finance and Operations 10.0.15** а статус окружења ће се ажурирати на **Примењено**.


## <a name="update-your-dataverse-environment"></a><a name="update"></a>Ажурирање Dataverse окружења

1. Пријавите се у [Power Platform центар администрације](https://admin.powerplatform.com/).
2. На листи пронађите и отворите окружење које сте користили за инсталирање услуге Project Operations.
3. На страници **Окружења** изаберите **Ресурс** > **Dynamics 365 апликације**.
4. На листи пронађите **Microsoft Dynamics 365 Project Operations** и у колони **Статус** изаберите **Доступна исправка**.
5. Означите поље за потврду **Слажем се са условима коришћења услуге**, а затим изаберите **Ажурирај**. Биће инсталирана најновија верзија решења.

По завршетку инсталације имаћете инсталирану верзију 4.5.0.134.

## <a name="configure-new-features"></a>Конфигурисање нових функција

### <a name="enable-dual-write-mapping"></a>Омогућавање мапирања двоструког уписивања

Након што довршите ажурирање Finance и Dataverse окружења, можете омогућити потребна мапирања двоструког уписивања. Обавите следеће процедуре да бисте омогућили мапирање двоструког уписивања.

- [Ажурирање безбедоносних подешавања у Customer Engagement окружењу](#security)
- [Освежавање ентитета података](#refresh)
- [Ажурирање и покретање мапирања двоструког уписивања](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a>Ажурирање безбедоносних подешавања у Dataverse окружењу

Следеће исправке безбедносних привилегија за ентитете су потребне као део ажурирања на Microsoft Dynamics CRM 2011 Update Rollup 5.

1. У окружењу Dataverse идите на **Подешавања** и у групи **Систем** изаберите **Безбедност**.

![Подешавања Dataverse окружења](media/Picture21.png)

2. Изаберите **Безбедносне улоге**.
3. Са листе улога изаберите **корисник апликације за двоструко уписивање** и изаберите картицу **Прилагођени ентитети**. 
4. Проверите да ли улога има дозволе **Читање** и **Приложи у** за:

      - **Тип девизног курса валуте**
      - **Графикон пословних контаката** 
      - **Фискални календар** 
      - **Главна књига**

5. Након ажурирања безбедносне улоге, идите на **Подешавања** > **Безбедност** > **Тимови**. Проверите да ли је улога **корисник апликације за двоструко уписивање** примењена на тим. 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a>Освежавање ентитета података из исправке

1. У Finance окружењу отворите радни простор **Управљање подацима**, а затим отворите страницу **Параметри оквира**.
2. На картици **Подешавања ентитета** изаберите **Освежи листу ентитета**.
3. Изаберите **Затвори** да бисте потврдили освежавање ентитета.

 > [!NOTE]
 > Овај поступак ће се завршити за око 20 минута. Бићете обавештени када се освежавање заврши.

### <a name="update-dual-write-mappings"></a><a name="run"></a>Ажурирање мапирања двоструког уписивања

1. У радном простору **Управљање подацима** изаберите **Двоструко уписивање**.
2. Изаберите **Примени решења**, изаберите оба решења са листе, а затим изаберите **Примени**.
3. На страници **Двоструко уписивање** изаберите следеће мапе табела, а затим изаберите **Заустави**.

    - **Project Operations стварне вредности интеграције (msdyn_actuals)**
    - **Project Operations интеграција категорија трошкова пројеката (msdyn_expensecategories)**
    - **Ентитет за извоз трошкова пројеката за Project Operations стварне вредности интеграције (msdyn_expenses)**

4. На страници **Верзија мапе табеле** примените нову верзију мапе на сваки од три ентитета.
5. На страници **Двоструко уписивање** изаберите „Покрени“ да бисте поново покренули мапе.
6. На листи мапа одаберите мапу **Главна књига (msdyn_ledgers)** са свим предусловима и означите поље за потврду **Почетна синхронизација**. 
7. У пољу **Мастер за почетну синхронизацију** изаберите **Finance and Operations апликације**, а затим изаберите **Покрени**.
 
 ![Синхронизација мапе главне књиге](media/DW6.png)
 