---
title: Планирање рада у програму Microsoft Project помоћу програмског додатка за Project Service
description: Ова тема пружа информације о томе како да користите програмски додатак Microsoft Project у програму Microsoft Project Service.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 01/07/2021
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c9628fcaf40f33d75f70ae15e37f422e65337d2c51d0d803178f8bcdfe10c7bd
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 08/06/2021
ms.locfileid: "6993889"
---
# <a name="plan-your-work-in-microsoft-project-with-the-project-service-add-in"></a>Планирање рада у програму Microsoft Project помоћу програмског додатка за Project Service

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3x](../includes/cc-applies-to-psa-app-3x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] вам олакшава да обављате планирање пројеката, укључујући процене. Можете да дефинишете рад тако да трошкови, ангажовање и продајна вредност буду јасни када коначан предлог буде прослеђен.  

Можете да инсталирате систем [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] и да послове планирања обављате у познатом окружења програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. Користите робусне могућности планирања и управљања програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], а затим ажурирајте план пројекта у програму Project Service Automation.  

> [!IMPORTANT]
> - Да бисте користили SharePoint управљање документима за складиштење у вашим [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотекама за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекте, ваш [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] администратор ће морати да укључи управљање документима. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] је компатибилан само са [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional издањем.  

## <a name="download-and-install-the-add-in"></a>Преузмите и инсталирајте програмски додатак  
 Припремите ваше информације за пријављивање у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Те информације ће вам бити потребне да бисте се повезали са програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] на функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  Из центра за преузимање преузмите програмски додатак за подржану верзију услуге of Project Service, верзије [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) или [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  Изаберите везу за преузимање.  

3.  Након преузимања, изаберите **Да** да бисте инсталирали програмски додатак.  

## <a name="configure-the-add-in"></a>Конфигуришите програмски додатак  

1. Отворите [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и изаберите картицу **Project Service**.  

2. Изаберите **Повежи се**.  

3. Унесите информације за пријављивање, а затим изаберите **Пријави се**.  

   Сада можете почети са коришћењем програмског додатка.  

## <a name="read-from-a-template"></a>Читање из предлошка  
 Читајте из предлошка који сте креирали у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] и копирали у програм [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] да бисте започели планирање пројекта. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Креирање предлошка за пројекат (Project Service Automation)](../psa/create-project-template.md)  

1.  Са картице **Project Service** изаберите **Читање** > **Предложак Project Service Automation пројекта**.  

2.  Са листе изаберите предложак пројекта, а затим изаберите **Отвори**.  

    > [!NOTE]
    >  Подразумевано, задаци који су копирани из предлошка у пројекат су подешени као ручно заказани.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Додељивање [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] улога ресурсима пројекта  

1.  Отворите пројекат и изаберите траку **Задатак**.  

2. Изаберите мени **Гантов графикон**, а затим изаберите **Листа ресурса**.  

3. На листи ресурса изаберите падајући мени **Улога ресурса за Project Service** и одаберите улогу за Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>Обезбедите радну снагу за пројекат помоћу ресурса  

1.  На картици „Project Service“ изаберите ред, па изаберите **Пронађи ресурсе**.  

2.  На екрану **Резервација ресурса** изаберите ресурс који желите да користите за пројекат.  

3.  Изаберите **Резервиши**, а затим изаберите **У реду**.  

## <a name="publish-your-project"></a>Објавите ваш пројекат  
Када се планирање пројекта заврши, следећи корак је увоз и објављивање пројекта у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

Пројекат ће се увести у функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Примењују се процеси одређивања цена и генерисања тима. Отворите пројекат у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] да бисте видели да ли су тим, процене за пројекат и структурна анализа посла генерисани. У следећој табели је приказано где да пронађете резултате.


|              Microsoft Project                                                           |                      Project Service Automation                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Гантов графикон**   | Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Структурна анализа посла**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Листа ресурса** |   Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Чланови пројектног тима**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Користите употребу**    |    Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Процене пројекта**.     |

**Да бисте увозили и објављивали пројекте**  
1. На картици **Project Service** дођите до **Објави** > **Нови Project Service Automation пројекат**.  

2. У дијалогу **Објављивање у нови пројекат у програму Project Service** унесите **Име пројекта** и изаберите **Клијент**.  

3. Опционално изаберите **Повежи план пројекта са функцијом Project Service Automation** да бисте повезали датотеку пројекта плана са функцијом Project Service Automation.  

4. Изаберите **Објави**.  

   Повезивање датотеке пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] од датотеке пројекта прави главну датотеку и подешава структурну анализу посла у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на само за читање.  Да бисте унели измене у план пројекта, потребно је да их направите у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да их објавите као исправке за функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>Уредите пројекат који је увезен  
 Да бисте унели промене у план пројекта који је увезен у функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], имате две опције:  

- Отворите главну датотеку и измените је у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- Опозовите везу датотеке и уредите је директно у функцији Project Service. Подразумевано, пројекат који је био отпремљен из програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] је закључан и може се уређивати само у функцији Project. Да бисте уредили датотеку у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], потребно је опозвати везу датотеке.  

### <a name="edit-in-pn_microsoft_project"></a>Уредите у услузи [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. У главном менију идите на **Project Service** > **Пројекти**.  

2. Са листе пројеката отворите онај који сте креирали у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Изаберите **Отвори у програму MS Project** са траке. То ће отворити повезану главну датотеку у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Раскините везу датотеке и уредите је у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. У главном менију идите на **Project Service** > **Пројекти**.  

2. Са листе пројеката отворите онај који сте креирали у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Изаберите **Раскини везу са програмом MS Project** са траке.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>Отпремање датотеке пројекта у SharePoint или Office групе  
 Датотеку пројекта можете да отпремите у SharePoint и да је пронађете у оквиру опције „Повезани документи“ за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.  Администратор мора да конфигурише SharePoint управљање документима и да га укључите за ентитет Пројекат. 

 Можете и да отпремите датотеку пројекта у [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] ако имате подешену опцију Office групе.

### <a name="upload-a-file-for-sharepoint"></a>Отпремање датотеке за SharePoint  

1. У главном менију идите на **Project Service** > **Отпреми**.  

2. Изаберите **У документа пројекта Project Service Automation**.  

3. У дијалогу **Омогући отварање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изаберите **Да** или **Не**.  

   - Ако изаберете **Да**, моћи ћете да изаберете **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** у решењу Project Service Automation и да покренете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и учитате датотеку пројекта из SharePoint библиотеке докумената.  

   - Ако одаберете **Не**, веза **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** неће функционисати.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотеку можете да пронађете у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у оквиру опције **Документи** за одређени [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.  

### <a name="upload-a-file-for-office-groups"></a>Отпремање датотеке за Office групе  

1. У главном менију идите на **Project Service** > **Отпреми**.  

2. Изаберите **У документа пројекта Project Service Automation**.  

3. У дијалогу **Омогући отварање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изаберите **Да** или **Не**.  

   - Ако изаберете **Да**, моћи ћете да изаберете **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** у решењу Project Service Automation, покренете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и учитате датотеку пројекта из SharePoint библиотеке докумената.  

   - Ако одаберете **Не**, веза **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** неће функционисати.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотеку можете да пронађете у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у оквиру опције **Документи** за одређени [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.  

## <a name="publish--your-project-as-a-template"></a>Објавите своје пројекте као предложак  
 Можете да сачувате ваш пројекат и да га поново употребите тако што ћете га сачувати ка предложак пројекта у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Предлошци пројеката су планови пројекта који могу поново да се користе у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. За више информација погледајте [Креирање предлошка пројекта (Project Service Automation)](../psa/create-project-template.md). 

1. На картици **Project Service** дођите до **Објави** > **Нови Project Service Automation предложак**.  

2. У дијалогу **Објавњивање у нови пројекат у предлошку Project Service** унесите **Име предлошка пројекта**.  

3. Опционално изаберите **Повежи план пројекта са функцијом Project Service Automation** да бисте повезали датотеку пројекта функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. Изаберите **Објави**.  

Повезивање датотеке пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] од датотеке пројекта прави главну датотеку и подешава структурну анализу посла у предлошку за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на само за читање.  Да бисте унели измене у план пројекта, потребно је да их направите у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да их објавите као исправке за функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>Прочитајте распоред ког је учитао ресурс

Када читате пројекат из услуге Project Service Automation, календар ресурса није синхронизован са клијентом за рачунаре. Ако постоје разлике у трајању задатка, напору или завршетку, то је вероватно зато што ресурси и клијент рачунара немају исти календар предлошка радних сати примењен на пројекат.


## <a name="data-synchronization"></a>Синхронизација података
Табеле у овом одељку пружају информације о синхронизацији података ентитета између функције Project Service Automation и програмског додатка Microsoft Project за рачунаре.

### <a name="project-task-entity-table"></a>Табела ентитета пројектног задатка
Следећа табела описује како се подаци ентитета пројектног задатка синхронизују између услуге Project Service Automation и програмског додатка за рачунаре услуге Microsoft Project.

| **Ентитет** | **Поље** | **Microsoft Project са услугом Project Service Automation** | **Project Service Automation са услугом Microsoft Project** |
| --- | --- | --- | --- |
| Пројектни задатак | Крајњи рок | Synchronized | Није синхронизовано |
| Пројектни задатак | Процењено ангажовање | Synchronized | Није синхронизовано |
| Пројектни задатак | ID MS Project клијента | Synchronized | Није синхронизовано |
| Пројектни задатак | Надређени задатак | Synchronized | Није синхронизовано |
| Пројектни задатак | Project | Synchronized | Није синхронизовано |
| Пројектни задатак | Пројектни задатак | Synchronized | Није синхронизовано |
| Пројектни задатак | Име пројектног задатка | Synchronized | Није синхронизовано |
| Пројектни задатак | Јединица за одређивање ресурса (неодобрено у верзији 3.0) | Synchronized | Није синхронизовано |
| Пројектни задатак | Заказано трајање | Synchronized | Није синхронизовано |
| Пројектни задатак | Датум почетка | Synchronized | Није синхронизовано |
| Пројектни задатак | ID за САП | Synchronized | Није синхронизовано |

### <a name="team-member-entity-table"></a>Табела ентитета члана тима
Следећа табела описује како се подаци ентитета члана тима синхронизују између услуге Project Service Automation и Micros

| **Ентитет** | **Поље** | **Microsoft Project са услугом Project Service Automation** | **Project Service Automation са услугом Microsoft Project** |
| --- | --- | --- | --- |
| Члан тима | ID MS Project клијента | Synchronized | Није синхронизовано |
| Члан тима | Име положаја | Synchronized | Није синхронизовано |
| Члан тима | пројекат | Synchronized | Synchronized |
| Члан тима | Пројектни тим | Synchronized | Synchronized |
| Члан тима | Јединица за одређивање ресурса | Није синхронизовано | Synchronized |
| Члан тима | Улога | Није синхронизовано | Synchronized |
| Члан тима | Часови радног времена | Није синхронизовано | Није синхронизовано |

### <a name="resource-assignment-entity-table"></a>Табела ентитета доделе ресурса
Следећа табела описује како се подаци ентитета доделе ресурса синхронизују између услуге Project Service Automation и Micros

| **Ентитет** | **Поље** | **Microsoft Project са услугом Project Service Automation** | **Project Service Automation са услугом Microsoft Project** |
| --- | --- | --- | --- |
| Додела ресурса | Датум „Од“ | Synchronized | Није синхронизовано |
| Додела ресурса | Час(ов)а | Synchronized | Није синхронизовано |
| Додела ресурса | ID MS Project клијента | Synchronized | Није синхронизовано |
| Додела ресурса | Планирани рад | Synchronized | Није синхронизовано |
| Додела ресурса | Project | Synchronized | Није синхронизовано |
| Додела ресурса | Пројектни тим | Synchronized | Није синхронизовано |
| Додела ресурса | Додела ресурса | Synchronized | Није синхронизовано |
| Додела ресурса | Задатак | Synchronized | Није синхронизовано |
| Додела ресурса | Датум „До“ | Synchronized | Није синхронизовано |

### <a name="project-task-dependencies-entity-table"></a>Табела ентитета зависних елемената пројектног задатка
Следећа табела описује како се подаци ентитета зависних елемената пројектног задатка синхронизују између услуге Project Service Automation и Micros

| **Ентитет** | **Поље** | **Microsoft Project са услугом Project Service Automation** | **Project Service Automation са услугом Microsoft Project** |
| --- | --- | --- | --- |
| Зависности пројектних задатака | Зависност пројектног задатка | Synchronized | Није синхронизовано |
| Зависности пројектних задатака | Тип везе | Synchronized | Није синхронизовано |
| Зависности пројектних задатака | Претходни задатак | Synchronized | Није синхронизовано |
| Зависности пројектних задатака | Project | Synchronized | Није синхронизовано |
| Зависности пројектних задатака | Следећи задатак | Synchronized | Није синхронизовано |

### <a name="additional-resources"></a>Додатни ресурси
 [Водич за менаџера пројекта](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]