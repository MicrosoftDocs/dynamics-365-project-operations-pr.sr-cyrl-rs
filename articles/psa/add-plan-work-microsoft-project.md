---
title: Користите програмски додатак Project Service за планирање вашег рада у програму Microsoft Project | MicrosoftDocs
description: Ова тема пружа информације о додавању, конфигурисању и коришћењу програмског додатка Microsoft Project у програму Microsoft Project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: 6bc74442866caccc02e53afc913a55aab81f9629
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129696"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>Користите програмски додатак Project Service Automation за планирање вашег рада у програму Microsoft Project

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] вам олакшава да обављате планирање пројеката, укључујући процене. Можете да дефинишете рад тако да трошкови, ангажовање и продајна вредност буду јасни када коначан предлог буде прослеђен.  

 Сада можете да инсталирате систем [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] и да послове планирања обављате у познатом окружења програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. Користите робусне могућности планирања и управљања програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], а затим ажурирајте план пројекта у програму Project Service Automation.  

> [!IMPORTANT]
> - Да бисте користили SharePoint управљање документима за складиштење у вашим [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотекама за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекте, ваш [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] администратор ће морати да укључи управљање документима. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] је компатибилан само са [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional издањем.  

## <a name="download-and-install-the-add-in"></a>Преузмите и инсталирајте програмски додатак  
 Припремите ваше информације за пријављивање у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Те информације ће вам бити потребне да бисте се повезали са програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] на функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  Из центра за преузимање преузмите програмски додатак за подржану верзију услуге of Project Service, верзије [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) или [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  Кликните на везу за преузимање.  

3.  Након преузимања, кликните на **Да** да бисте инсталирали програмски додатак.  

## <a name="configure-the-add-in"></a>Конфигуришите програмски додатак  

1. Отворите [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и кликните на картицу **Project Service**.  

2. Кликните на дугме **Повежи**.  

3. Унесите своје информације за пријављивање и кликните на дугме **Пријави се**.  

   Сада можете почети са коришћењем програмског додатка.  

## <a name="read-from-a-template"></a>Читање из предлошка  
 Читајте из предлошка који сте креирали у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] и копирали у програм [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] да бисте започели планирање пројекта. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Креирање предлошка за пројекат (Project Service Automation)](../psa/create-project-template.md)  

1.  Са картице **Project Service** кликните на дугме **Читање** > **Предложак Project Service Automation пројекта**.  

2.  Са листе изаберите предложак пројекта и кликните на дугме **Отвори**.  

    > [!NOTE]
    >  Подразумевано, задаци који су копирани из предлошка у пројекат су подешени као ручно заказани.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Додељивање [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] улога ресурсима пројекта  

1.  Отворите пројекат и кликните на траку **Задатак**.  

2.  Кликните на мени **Гантов графикон**, а затим изаберите **Листа ресурса**.  

3.  На листу ресурса кликните на дугме у падајућем менију **Улога ресурса за Project Service** и одаберите улогу за Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>Обезбедите радну снагу за пројекат помоћу ресурса  

1.  На картици „Project Service“ изаберите ред и кликните на дугме **Пронађи ресурсе**.  

2.  На екрану **Резервација ресурса** изаберите ресурс који желите да користите за пројекат.  

3.  Кликните на дугме **Резервиши**, а затим на **У реду**.  

## <a name="publish-your-project"></a>Објавите ваш пројекат  
Када се планирање пројекта заврши, следећи корак је увоз и објављивање пројекта у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

Пројекат ће се увести у функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Примењују се процеси одређивања цена и генерисања тима. Отворите пројекат у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] да бисте видели да ли су тим, процене за пројекат и структурна анализа посла генерисани. У следећој табели је приказано где да пронађете резултате:


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Гантов графикон**   | Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Структурна анализа посла**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Листа ресурса** |   Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Чланови пројектног тима**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Користите употребу**    |    Увози у [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] екран **Процене пројекта**.     |

**Да бисте увозили и објављивали пројекте**  
1. Са картице **Project Service** кликните на **Објави** > **Нови Project Service Automation пројекат**.  

2. У дијалогу **Објави у нови пројекат у програму Project Service** унесите **Име пројекта** и изаберите **Клијент**.  

3. Опционално означите **Повежи план пројекта са функцијом Project Service Automation** да бисте повезали датотеку пројекта плана са функцијом Project Service Automation.  

4. Изаберите дугме **Објави**  

   Повезивање датотеке пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] од датотеке пројекта прави главну датотеку и подешава структурну анализу посла у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на само за читање.  Да бисте унели измене у план пројекта, потребно је да их направите у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да их објавите као исправке за функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>Уредите пројекат који је увезен  
 Да бисте унели промене у план пројекта који је увезен у функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], имате две опције:  

- Отворите главну датотеку и измените је у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- Опозовите везу датотеке и уредите је директно у функцији Project Service. Подразумевано, пројекат који је био отпремљен из програма [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] је закључан и може се уређивати само у функцији Project. Да бисте уредили датотеку у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], потребно је опозвати везу датотеке.  

### <a name="edit-in-pn_microsoft_project"></a>Уређивање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. У главном менију кликните на **Project Service** > **Пројекти**.  

2. Са листе пројеката отворите онај који сте креирали у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Кликните на дугме **Отвори у програму MS Project** са траке. То ће отворити повезану главну датотеку у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Раскините везу датотеке и уредите је у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. У главном менију кликните на **Project Service** > **Пројекти**.  

2. Са листе пројеката отворите онај који сте креирали у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Кликните на дугме **Раскини везу са програмом MS Project** са траке.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>Отпремање датотеке пројекта у SharePoint или Office групе  
 Датотеку пројекта можете да отпремите у SharePoint и да је пронађете у оквиру опције „Повезани документи“ за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.  Администратор мора да конфигурише SharePoint управљање документима и да га укључите за ентитет Пројекат. 

 Можете и да отпремите датотеку пројекта у [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] ако имате подешену опцију Office групе.

### <a name="upload-a-file-for-sharepoint"></a>Отпремање датотеке за SharePoint  

1. У главном менију кликните на **Project Service** > **Отпреми**.  

2. Изаберите **У документа пројекта Project Service Automation**.  

3. У дијалогу **Омогући отварање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изаберите **Да** или **Не**.  

   - Ако кликнете на **Да**, моћи ћете да изаберете дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** у решењу Project Service Automation, да покренете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и учитате датотеку пројекта из SharePoint библиотеке докумената.  

   - Ако кликнете на **Не**, веза за дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** неће радити.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотеку можете да пронађете у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у оквиру опције **Документи** за одређени [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.  

### <a name="upload-a-file-for-office-groups"></a>Отпремање датотеке за Office групе  

1. У главном менију кликните на **Project Service** > **Отпреми**.  

2. Изаберите **У документа пројекта Project Service Automation**.  

3. У дијалогу **Омогући отварање у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изаберите **Да** или **Не**.  

   - Ако кликнете на **Да**, моћи ћете да изаберете дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** у решењу Project Service Automation, да покренете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и учитате датотеку пројекта из SharePoint библиотеке докумената.  

   - Ако кликнете на **Не**, веза за дугме **Отвори у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** неће радити.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] датотеку можете да пронађете у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] у оквиру опције **Документи** за одређени [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] пројекат.  

## <a name="publish--your-project-as-a-template"></a>Објавите своје пројекте као предложак  
 Можете да сачувате ваш пројекат и да га поново употребите тако што ћете га сачувати ка предложак пројекта у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  Предлошци пројеката су планови пројекта који могу поново да се користе у функцији [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Креирање предлошка за пројекат (Project Service Automation)](../psa/create-project-template.md)  

1. Са картице **Project Service** кликните на дугме **Објави** > **Нови Project Service Automation шаблон пројекта**.  

2. У дијалогу **Објави у нови пројекат у предлошку Project Service** унесите **Име предлошка пројекта**.  

3. Опционално означите **Повежи план пројекта са функцијом Project Service Automation** да бисте повезали датотеку пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. Изаберите дугме **Објави**  

Повезивање датотеке пројекта са функцијом [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] од датотеке пројекта прави главну датотеку и подешава структурну анализу посла у предлошку за [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на само за читање.  Да бисте унели измене у план пројекта, потребно је да их направите у програму [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да их објавите као исправке за функцију [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

### <a name="see-also"></a>Такође погледајте  
 [Водич за менаџера пројекта](../psa/project-manager-guide.md)
