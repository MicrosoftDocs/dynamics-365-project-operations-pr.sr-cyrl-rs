---
title: Промене ентитета, контрола и корисничког интерфејса (Project Service Automation 3.x)
description: Ова тема описује промене решења за Microsoft Dynamics Project Service Automation 3.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 2d93e5eaae7cff302be1cb2e96e3f45c24739b0c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084167"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>Промене ентитета, контрола и корисничког интерфејса (Project Service Automation 3.x)
Уз издање Microsoft Dynamics Project Service Automation (PSA) 3.x, извршене су многе промене у ентитетима, контролама, приказима и корисничком интерфејсу. Ова тема пружа информације о овим важним променама.

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>Односи надређених и подређених ентитета за документ продаје, ставку документа продаје, детаљи ставке документа продаје
У верзијама апликације Dynamics 365 Project Service Automation (PSA) које су објављене пре верзије 3.0, неки од односа између ентитета докумената продаје, ставки докумената продаје и детаља ставке докумената продаје имплементирани су кроз поља ниске која су евидентирала приказ ниске за of GUID повезаног ентитета. До овога је долазило због ограничења платформе која је захтевала значајни део прилагођеног кода на страни сервера, као и на страни клијента решења да би ти односи радили слично типичном односу између Dynamics CRM ентитета и да би се поља ниске понашала као поља за проналажење.

PSA 3.0 је ажуриран тако да користи нове односе између ентитета докумената продаје и ставке документа продаје.

С обзиром на то да поља за проналажење могу да се користе за означавање референци на ентитете, поља која су складиштила вредност ниске за GUID повезаног ентитета у претходним верзијама више нису потребна и зато су застарела. Прилагођени кôд на страни клијента и сервера који рукује односима дефинисаним у застарелим пољима ниске такође је застарео.

### <a name="entity-schema-changes"></a>Промене шема ентитета
Следећа табела пружа листу „један на један“ застарелих поља ниске и нових поља за проналажење ентитета. 

 Ентитет |   Застарело поље (ниска) | Ново поље (проналажење)
--- | --- | ---
invoicedetail (ставка фактуре) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (стварна вредност) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (Распоред фактурисања за предмет уговора за пројекат) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (Контролна тачка предмета уговора за пројекат) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (чињеница) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (Детаљ ставке фактуре) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (ставка у главној књизи) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (Категорија ресурса за предмет уговора за пројекат) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (Детаљ предмета уговора за пројекат) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (Категорија трансакције за предмет уговора за пројекат) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (Класификација трансакција за предмет уговора за пројекат) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (Распоред фактурисања ставки понуде) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (Категорија ресурса ставке понуде) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (Контролна тачка ставке понуде) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (Детаљ ставке понуде) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (Категорија трансакције ставке понуде) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (Класификација трансакције ставке понуде) |  msdyn_quoteline |   msdyn_quotelineid
Детаљ улазне поруџбине (ставка поруџбине) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>Застарели прилагођени прикази и контроле
Следећи прилагођени прикази и контроле и њихови повезани артефакти су застарели.

- Приказ наплативости.
- Прилагођене контроле мреже за приказивање детаља ставке понуде на страници са **информацијама о пројекту** за ставли понуде.
- Прилагођене контроле мреже за приказивање детаља предмета уговора о пројекту на страници са **информацијама о пројекту** за ставку улазне поруџбине.

> [!NOTE]
> За комплетну листу застарелих ресурса, погледајте [Застарели веб-ресурси у апликацији Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md)

## <a name="unified-client-interface-app-module"></a>Модул апликације за обједињени клијентски интерфејс
Уз увођење модула за апликације обједињеног клијентског интерфејса, PSA ставке мапа локација су уклоњене из система.  
Функционалност која се односи на пребацивање образаца за ентитете Могућност за пословање, Понуда, Поруџбина, Фактура је застарела пошто више није потребна, јер модул за апликацију обједињеног клијентског интерфејса укључује само PSA верзије образаца.  

Следећи веб-ресурси су застарели:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\Документ продаје\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> За комплетну листу застарелих ресурса, погледајте [Застарели веб-ресурси у апликацији Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md).

