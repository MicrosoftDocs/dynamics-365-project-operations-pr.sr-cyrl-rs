---
title: Примена Project Operations демо података на Finance окружење које се хостује у облаку
description: Ова тема објашњава како да примените демо податке из услуге Project Operations на Dynamics 365 Finance окружење хостовано у облаку.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 1a94862d5a024eb1630f33c0c96699e8b4b49bf2
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949065"
---
# <a name="apply-project-operations-demo-data-to-a-finance-cloud-hosted-environment"></a>Примена Project Operations демо података на Finance окружење које се хостује у облаку

_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_

>[Важно] Ова тема је применљива је само на Microsoft Dynamics 365 Finance верзије 10.0.13 и може се изводити само у окружењу које хостује у облаку. Довршите кораке у овој теми **ПРЕ НЕГО ШТО** примените исправке квалитета на окружење.

1. У свом LCS пројекту, отворите страницу **Детаљи окружења**. Приметите да садржи детаље потребне за повезивање са околином помоћу протокола удаљене радне површине (RDP).

![Детаљи  окружења](./media/1EnvironmentDetails.png)

Први скуп истакнутих акредитива су акредитиви локалног налога и садрже хипервезу до везе са удаљеном радном површином. Акредитиви укључују корисничко име и лозинку администратора окружења. Други скуп акредитива се користи за пријављивање на SQL Server у овом окружењу.

2. Повежите се удаљено са окружењем користећи хипервезу у одељку **Локални налози** и употребите **Акредитиви за локални налог** за потврду идентитета.
3. Идите на **Internet Information Services** > **Групе апликација** > **AOSService** и зауставите услугу. У овом тренутку заустављате услугу да бисте могли да наставите да замењујете SQL базу података.

![Заустављање AOS](./media/2StopAOS.png)

4. Идите на **Услуге** и зауставите следеће две ставке:

- Microsoft Dynamics 365 Unified Operations: Batch Management Service
- Microsoft Dynamics 365 Unified Operations: Data Import Export Framework

![Заустављање услуга](./media/3StopServices.png)

5. Отворите Microsoft SQL Server Management Studio. Пријавите се помоћу акредитива за SQL Server и користите корисника axdbadmin и лозинку са LCS странице **Детаљи окружења**.

![SQL Server Management Studio](./media/4SSMS.png)

6. У прегледачу објеката, изаберите **Базе података** и пронађите **AXDB**. Базу података ћете заменити новом базом података која се налази у [центру за преузимање](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip). 
7. Копирајте zip датотеку у VM у који сте удаљено повезани и распакујте zip садржај.
8. У програму SQL Server Management Studio кликните десним тастером миша на **AxDB**, а затим изаберите **Задаци** > **Враћање** > **База података**.

![Враћање базе података](./media/5RestoreDatabase.png)

9. Изаберите **Изворни уређај** и дођите до датотеке извучене из zip датотеке коју сте копирали.

![Изворни уређаји](./media/6SourceDevice.png)

10. Изаберите **Опције**, а затим изаберите **Препиши постојећу базу података** и **Затворите постојеће везе са одредишном базом података**. 
11. Изаберите **У реду**.

![Враћање подешавања](./media/7RestoreSetting.png)

Добићете потврду да је враћање AXDB било успешно. Када добијете ову потврду, можете да затворите SQL Services Management Studio.

12. Вратите се на **Internet Information Services** > **Групе апликација** > **AOSService** и покрените услугу.
13. Идите на **Услуге** и покрените две услуге које сте раније зауставили.

14. Пронађите алатку AdminUserProvisioning на овом VM-у. Потражите K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.
15. Покрените .ext датотеку користећи своју корисничку адресу у пољу **Адреса е-поште**. 
16. Изаберите **Проследи**.

![Обезбеђивање корисника-администратора](./media/8AdminUserProvisioning.png)

За ово је потребно неколико минута. Требало би да примите поруку са потврдом да је корисник-администратор успешно ажуриран.

17. На крају, покрените командну линију као администратор и покрените команду iisreset

![Ресетовање IIS](./media/9IISReset.png)

18. Затворите сесију удаљене радне површине и користите страницу LCS **Детаљи окружења** да бисте се пријавили у окружење и потврдили да ради као што се очекује.

![Finance and Operations](./media/10FinanceAndOperations.png)
