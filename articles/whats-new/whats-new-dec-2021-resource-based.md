---
title: Шта је ново децембра 2021. – Project Operations за сценарије засноване на ресурсима/без залиха
description: Ова тема пружа информације о квалитетним исправкама које су доступне у издању пројектних операција у децембру 2021.
author: sigitac
ms.date: 12/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c4869f3ab06ec80d620ec51bb4f0429412cd4d00
ms.sourcegitcommit: 9d20e7738cce195d344f5925a115741a1ce3ca36
ms.translationtype: MT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 12/21/2021
ms.locfileid: "7943041"
---
# <a name="whats-new-december-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>Шта је ново децембра 2021. – Project Operations за сценарије засноване на ресурсима/без залиха

*Односи се на: Project Operations за сценарије засноване на ресурсима / без залиха*

Ова тема се односи на следеће компоненте и верзије корпорације Dynamics 365 Project Operations Мицрософт:

- Операције пројекта у Dataverse верзији окружења 4.27.0.195, 4.27.0.242
- Управљање пројектима и рачуноводство Dynamics 365 Finance у окружењу верзија 10.0.23

## <a name="features-included-in-this-release"></a>Функције укључене у овом издању

- Побољшано решавање проблема за администраторе система. Када корисник не може да отвори пројекат, администратор може да прегледа грешке које нису повезане са лиценцом, а које се генеришу из пројекта за Веб [у евиденцијама заказивања пројекта](../project-management/schedule-api-logs.md).
- [Користите листе за проверу задатака у програму Мицрософт Пројецт за Веб](https://support.microsoft.com/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c). У програму Мицрософт Пројецт за Wеб можете да додате листу за проверу задатку да бисте пратили одређене ставке.

## <a name="project-operations-dual-write-maps-updates"></a>Ажурирања мапа двоструког уписивања за Project Operations

У овом издању нема исправки за Project Operations мапе двоструког уписивања. За тренутну листу и верзије Project Operations мапа двоструког уписивања, погледајте [Верзије Project Operations мапа двоструког уписивања](../environment/resource-dual-write-maps.md).

Увек покрените најновију верзију мапе у окружењу и омогућите све повезане мапе табела док ажурирате решење за пројектне Dataverse операције и верзију финансијског решења. Неке функције и могућности можда неће исправно функционисати ако најновија верзија мапе није активирана. Активну верзију мапе можете видети у колони **Верзија** на страници **Двоструко уписивање**. Да бисте активирали нову верзију мапе, изаберите **Верзије табеле мапе**, изаберите најновију верзију, а затим сачувајте изабрану верзију. Ако сте прилагодили мапу табеле без оквира, поново примените промене. За још информација погледајте [Управљање животним циклусом апликације](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Ако наиђете на проблем приликом почетка мапе, следите упутства у проблему са колонама табеле које недостају [у](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) одељку мапе водича за решавање проблема са двоструким уписивања.

## <a name="quality-updates"></a>Исправке квалитета

### <a name="project-operations-on-dataverse"></a>Project Operations у услузи Dataverse

| **Област функција** | **Референтни број** | **Исправка квалитета** |
| --- | --- | --- |
| Планирање и праћење | 2392596 | Планирајте да АПИ сада дозволи ажурирање **преосталих напора**, **довршеног напора** и **%Цомплете** поља. |
| Планирање и праћење | 2478497 | Поља **"Број** активности" **и "ИД** задатка" за АПИ распореда могу бити празна на улазу јер ће их систем попунити коришћењем аутоматизованог нумерисања.|
| Време и трошак | 2468135 | Број поновних одобрења се смањује са пет на три. |
| Време и трошак | 2468188 | Отклоњен је проблем са лог текстом који премашује **максималну дужину у** атрибуту **нотетеxт ентитета** белешке. |
| Наплата и одређивање цена | 2488698 | Ажурирана порука о грешци до које долази када у подешавању окружења недостају записи ентитета књиге који су попуњени из "Финансије". |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Управљање пројектима и рачуноводство у услузи Dynamics 365 Finance

| **Област функција** | **Референтни број** | **Исправка квалитета** |
| --- | --- | --- |
| Управљање пројектима и рачуноводство | [587187](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D587187&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225501421%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=qpKECMgKZe9sHGVZUhBxs%2F4ou3fXIiFFg2amMTJ6t9U%3D&amp;reserved=0) | Конто међукомпанијског прихода разматра само **"Све" - све реда без** укључене групе пореза на промет. |
| Управљање пројектима и рачуноводство | [599568](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D599568&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225600986%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=IudfEjWmkNeiTsWmR%2Fu2oR0CnnCkffAshvqZJuF76q8%3D&amp;reserved=0) | Процене праве линије се неправилно израчунавају. |
| Управљање пројектима и рачуноводство | [602728](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D602728&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227094434%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=Q2%2BveFHlGrzg4QHtqcgeqjyZSQkmpr%2Fku7oObKHMB9g%3D&amp;reserved=0) | Проблем књижења за фактурисани приход пројекта у примењеним предметима за задржавање резултира трансакцијама на ваучеру који није избалансиран. |
| Управљање пројектима и рачуноводство | [610906](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D610906&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227134259%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=xDBnz10T71GmOZt78ooFK3SYvmTLoC5fj1OftYNYDpY%3D&amp;reserved=0) | Побољшања перформанси за интеграцију са стварним операцијама пројекта. |
| Управљање пројектима и рачуноводство | [618670](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D618670&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227203949%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=PqvHsTGLcQ3bYbUlzYABYhl7J9v2zbnjcOgm%2FTvXB20%3D&amp;reserved=0) | Корисници не могу да фактуришу ако су трансакције трошка часова прокњижене са **ставком** "Никад" или **"Без".** |
| Управљање пројектима и рачуноводство | [623818](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D623818&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227303517%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=LAfdEiuKG8DoGk8O48MRLuaKYDINhCyMAtrlpGvVAw0%3D&amp;reserved=0) | Групне обраде не успевају ако неко од књижења налога не успе, а преостали налози се не обраде.  |
| Путовање и трошак | [575378](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D575378&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225451644%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=3tW0ngQqcz8pdNFY8FVuFlsgv3l73HMgeQTLbzIAAOg%3D&amp;reserved=0) | Статус одобравања за недодирљиве трошкове може да се промени. |
| Путовање и трошак | [592997](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D592997&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225521336%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=0leQsokHcl2NLqePFXC6%2BuH1V5UNRWUIPx0wTUaB4vg%3D&amp;reserved=0) | Извештај о трошковима који је прослеђен току посла вам омогућава да креирате нове редове трошкова. |
| Путовање и трошак | [594853](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D594853&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225541248%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=5PINC45EBeV8PC0Cvtt0QPPJn0VYQ%2FRCjBmlEsZJCq4%3D&amp;reserved=0) | У извештају о трошковима можете успоставити почетне вредности непрокњижених редова трошкова. |
| Путовање и трошак | [599821](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D599821&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225610944%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=eb2CAb8L9IUDxDoukDcZQxNyI3TNQtFO%2FcjycucNj44%3D&amp;reserved=0) | Ако постоје недодирљиви трошкови у којима је власник трошкова запослени, не можете да омогућите функцију аванса за готовину трошкова. |
| Путовање и трошак | [601446](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D601446&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225650767%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=Z4CBMqrmYtlIEBWxzMEBf%2BXu5dlst7NnKcQ62yoV%2BWM%3D&amp;reserved=0) | Ако је захтев за путовање постављен на вредност "Нулл", **у заглављу** трошкова не би требало да буде омогућено испревлачење. |
| Путовање и трошак | [601753](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D601753&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225660718%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=PVwbDhH5uqGJJZTNLddsHYlHsCknK%2FC%2FY%2Btg6fu8heo%3D&amp;reserved=0) | Поље **"Наплата"** у **управљању** трошковима се чисти када се трошкови уштеде. |
| Путовање и трошак | [602009](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D602009&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225680636%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=t3m29Vkxx8g96CvaDz%2FRzuciP2doP2xejomPl440wNs%3D&amp;reserved=0) | Када избришете ставку која има поткатегорију са изабраним опцијом "Искључи из опорезивања", укључио **је** клизач **·** **"Не" за извештај о** трошковима. |
| Путовање и трошак | [607516](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D607516&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919225849894%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=%2BceTskfUl1kTe2XHk6QSYu9UN%2FE%2F9nP2gv20kVweURA%3D&amp;reserved=0) |Књиговодствени догађај је празан и статус рачуноводства је нетачан. |
| Путовање и трошак | [617801](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D617801&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919226337756%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=L69x65xY6LQDS1u2sUbVX5QKEYgbDh6lld2Pm%2BSsUyI%3D&amp;reserved=0) | Ток посла не оцењује правилно извештај о трошковима када је трошак подељен на трансакцију кредитном картицом. |
| Путовање и трошак | [575295](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D575295&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227074518%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=FyrzO1Yx%2BWLfw5arIrFiW07QZC%2F%2BpUk3ekx3g66X8bE%3D&amp;reserved=0) | Нетачан износ валуте за извештавање о банковним трансакцијама добављача се књижи у затвореном периоду из извештаја о трошковима. |
| Путовање и трошак | [610910](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D610910&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227134259%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=P6wVchjx9GcH7nZ07yg3%2FuEFht6Df7Ew5Z4hSL%2BQ8oY%3D&amp;reserved=0) | У функцији "Редизајнираног извештаја о трошковима", подразумевани начин плаћања се попуњава за ред трошкова чак и ако се начин плаћања промени приликом креирања трошкова. |
| Путовање и трошак | [617146](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D617146&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227193996%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=134C%2BXGuzA8GmM7ZjWYaiYQfNqnV9a1mEKuzrh0hzpw%3D&amp;reserved=0) | Извештај о трошковима не можете проследити ако су смернице за пријем омогућене. |
| Путовање и трошак | [619783](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D619783&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227243778%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=pV1rLgOniDy3hXMHAtXeD9o4ZPTmyhZHd7O7zCUpLLs%3D&amp;reserved=0) | До следеће грешке долази када проследите извештај о **трошковима Стацк Траце: Предузеће не постоји**. |
| Путовање и трошак | [620773](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D620773&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227253737%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=%2B5ZZAsXV%2FM29%2Byg6JoGzwJFRa1Fi4NDj4BB38ZeYTH0%3D&amp;reserved=0) | Са редовима међукомпанијских трошкова, расподела не ажурира правно лице када се неоштећена трансакција поново дода извештају о трошковима. |
| Путовање и трошак | [621967](https://nam06.safelinks.protection.outlook.com/?url=https:%2F%2Ffix.lcs.dynamics.com%2FIssue%2FDetails%2F?bugId%3D621967&amp;data=04%7C01%7Cjespers%40microsoft.com%7Cc1d2484c411149f3a93708d9a8583e14%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637725919227273644%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000&amp;sdata=RdiupzmL8Dp8nqQIHu9rGMTdJ%2FVVhqN5EIP5uFYS2W4%3D&amp;reserved=0) | Продајна цена и износ у валути за извештавање у оквиру трансакција добављача неправилно се израчунавају у извештајима о трошковима који су повезани са пројектом и креирају се у страној валути коришћењем трансакција увезеним кредитним картицама. |