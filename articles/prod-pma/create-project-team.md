---
title: Креирање пројектног тима
description: Ова тема пружа информације о томе како да креирате и управљате пројектним тимовима.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kdwns
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a7eb9101352afd27b527bf6b8acc6f92198f44ea
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084137"
---
# <a name="create-a-project-team"></a>Креирање пројектног тима

[!include [banner](../includes/banner.md)]

Да би користио улоге које су претходно постављене у пројекту, менаџер пројекта мора повезати улоге са пројектом. За пројекат се може доделити више улога. Да би се спречила забуна, ове улоге се аутоматски означавају током резервације. На пример, ако менаџер пројекта захтева три софтверска инжењера, аутоматски се генеришу три улоге софтверског инжењера које имају ознаке **софтверски инжењер 1** , **софтверски инжењер 2** и **софтверски инжењер 3**. Ако су карактеристике улоге претходно постављене за улогу, оне се примењују као филтер током претраживања ресурса. Додатне карактеристике се могу додати по потреби за даље прецизирање претраге.

Поставке приказа такође се могу прилагодити како би се добио бољи приказ доступности ресурса. Постоје опције за приказивање расположивости по сатима, дневно, недељно, месечно, квартално и годишње. Такође постоји опција за приказ расположивог и преосталог капацитета ресурса. Ова опција је корисна за управљање временом када процењујете доступно време за активности или доступност ресурса.

Менаџер пројекта може одабрати улогу на страници, а затим, ако постоји доступан ресурс који одговара захтевима, изаберите да резервишете ресурс за попуњавање улоге. Имајте на уму да ресурси у овом тренутку не морају бити резервисани у фази планирања. Када креирате САП, можете заменити улоге ресурсима особља за пројекат. Ако се улоге замене ресурсима особља у САП-у, подешавање ресурса аутоматски ажурира списак и распоред пројектног тима.

[![Списак пројектног тима који укључује и улоге и стварне ресурсе](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg) 

Менаџер пројекта има разне могућности за резервацију ресурса за пројекат, као што су **Преостали капацитет** , **Пун капацитет** , **Проценат капацитета** и **Наведите радно време**. Ове опције резервације могу се отказати у било ком тренутку ако се промене додељивања ресурса. Подржане су две врсте резервација:

- **Фиксна резервација** – Резервација ресурса је одобрена и потврђена за рад на ангажовању током одређеног времена.
- **Условна резервација** – Резервације ресурса су условно подешене за рад на ангажовању током одређеног времена.

Следећа процедура објашњава како да креирате пројектни тим.

## <a name="create-a-project-team"></a>Креирање пројектног тима

1. На страници листе **Сви пројекти** изаберите пројекат, а затим изаберите **Уреди**.
2. На картици **Пројектни тим и распоређивање** , у поље **Датум завршетка распореда** унесите датум почетка распореда увећан за један месец. На пример, ако је датум почетка распореда 24. јун 2017. (24.6.2017), Унесите **24.07.2017**.
3. Изаберите **Додај**.
4. У окну **Додавање улога у пројекат** , у пољу **Улога** изаберите **Виши менаџер пројекта**.
5. Изаберите **Потребне компетенције**.
6. На страници **Одаберите карактеристике** , карактеристике које сте претходно поставили за улогу вишег менаџера пројекта су подразумевано изабране. Изаберите **У реду**.
7. На страници **Додавање улоге пројекту** , у пољу **Број ресурса** унесите **1**.
8. У пољу **Ресурс** , преглед приказује све ресурсе који имају потребне компетенције. Изаберите **Данијел Голдшмит** , а затим изаберите **Креирај**.
9. На страници **Пројекат** изаберите **Додај**.
10. У окну **Додавање улога у пројекат** , у пољу **Улога** изаберите **Члан тима**. У поље **Број ресурса** унесите **5**.
11. Изаберите **Креирај**.
12. На страници **Пројекти** , изаберите **Попуни ресурс**.

## <a name="monitor-project-teams"></a>Надгледајте пројектне тимове
1. На страници **Сви пројекти** , изаберите везу **ID пројекта** за пројекат **Надоградња XYZ фаза 2**.
2. На брзој картици **Пројектни тим и заказивање** , уверите се да су наведени ресурси пројекта тачни.