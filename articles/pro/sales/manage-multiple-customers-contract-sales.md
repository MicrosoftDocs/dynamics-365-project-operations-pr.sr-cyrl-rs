---
title: Управљање са више клијената на уговорима за пројекат – једноставно
description: Ова тема пружа информације о управљању већим бројем клијената на уговорима заснованим на пројекту.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b248dabdbd5239b140da7c99d3f38609facfe75e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181335"
---
# <a name="manage-multiple-customers-on-project-contracts---lite"></a>Управљање са више клијената на уговорима за пројекат – једноставно

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Уговори за пројекат у услузи Dynamics 365 Project Operations подржавају сценарио када уговор обухвата више клијената који финансирају погодбу. Картица **Резиме** на страници **Уговор о пројекту** укључује поље **Клијент**. Ово поље идентификује примарног клијента погодбе. Други клијенти за погодбу могу се подесити на картици **Клијенти** на страници **Уговор о пројекту**.

Сви клијенти за уговор наведени у уговору за пројекат подразумевају се као клијенти предмета уговора на свим новим предметима уговора заснованим на пројекту који су креирани за уговор о пројекту. Постојећи предмети уговора засновани на пројекту не наслеђују нове клијенте за уговор док се креирају нови записи.

Предмети уговора засновани на производу аутоматски се повезују са примарним клијентом.

Клијенти уговора и клијенти предмета уговора могу се додати, ажурирати или избрисати у било ком тренутку пре добијања уговора.

## <a name="primary-customer"></a>Примарни клијент

Клијент наведен на картици **Резиме** уговора за пројекат као потенцијални клијент је примарни клијент уговора. Када покушате да избришете примарног клијента са листе клијената на уговору, добићете поруку о грешци да запис примарног клијента на уговору не можете избрисати.

Примарни клијент се не може ажурирати са листе клијената за уговор. Уместо тога, промените потенцијалног клијента на картици **Резиме** уговора. Када се ово поље ажурира на страници **Резиме уговора**, нови клијент се додаје као нови клијент за уговор са подешеном заставицом **Примарни**. Претходни примарни клијент ће и даље ће бити клијент за уговор.

## <a name="create-update-or-delete-a-contract-customer-record"></a>Креирање, ажурирање или брисање записа клијента за уговор

Клијент за уговор може бити креиран, ажуриран или избрисан из картице **Клијенти** на страници **Уговор о пројекту**. Поља у следећој табели налазе се у запису клијента за уговор на уговору за пројекат и то треба да имате на уму док радите са уговором.

| Поље | Локација | Опис | Последични утицај |
| --- | --- | --- | --- |
| **Налог** | Мрежа која може да се уређује на картици **Клијенти уговора**, **главни образац** и **образац за брзо креирање** за клијента за уговор. | Наводи све активне налоге. Ово поље се закључава након креирања записа. Да бисте ажурирали пословни контакт, избришите запис и направите нови. Ако сте евидентирали било које стварне податке или ако је запис клијента за уговор примарни клијент, не можете избрисати запис. | Клијенти за уговор се копирају као клијенти из предмета уговора када се креира предмет уговора. |
| **Проценат дељења наплате** | Мрежа која може да се уређује на картици **Клијенти уговора**, **главни образац** и **образац за брзо креирање** за клијента за уговор. | Представља проценат сваке ненаплаћене продајне трансакције која ће бити приписана овом клијенту предмета уговора. | Прекопирано на нове предмете уговора и на клијенте предмета уговора за пројекат на новим предметима уговора за пројекат. |
| **Име уговора за фактурисање** | Мрежа која може да се уређује на картици **Клијенти уговора**, **главни образац** и **образац за брзо креирање** за клијента за уговор. | Ово текстуално поље треба да се користи за идентификацију особе за контакт на фактури за овог клијента. Ово поље добија подразумевану вредност из одговарајућег записа пословног контакта. | Прекопирано у поље **Име контакта за фактурисање** на фактури који се генерише за овог клијента. |
| **Име фактурисања** | Мрежа која може да се уређује на картици **Клијенти уговора**, **главни образац** и **образац за брзо креирање** за клијента за уговор | Ово текстуално поље треба да се користи за идентификацију особе за контакт на фактури за овог клијента. Ово поље добија подразумевану вредност из одговарајућег записа пословног контакта. | Прекопирано у поље **Име контакта за фактурисање** на фактури који се генерише за овог клијента. |
| **Услови плаћања** | Мрежа која може да се уређује на картици **Клијенти уговора**, **главни образац** и **образац за брзо креирање** за клијента за уговор. | Вредности се подразумевано добијају из одговарајућег записа пословног контакта. | Прекопирано у поље **Име контакта за фактурисање** на фактури који се генерише за овог клијента. |
| **Да ли је заокруживање** | Мрежа која може да се уређује на картици **Клијенти уговора**, **главни образац** и **образац за брзо креирање** за клијента за уговор. | Означава да ли је овај клијент подразумевани клијент за заокруживање за ову погодбу. На уговору за пројекат може бити само један клијент за заокруживање. | Када дељење трошкова и ненаплаћене количине доведе до разлике у заокруживању, та разлика се примењује на стварну вредност која се мапира на овог клијента. |
| **Ограничење које не сме да се прекорачи** | Мрежа која може да се уређује на картици **Клијенти уговора**, **главни образац** и **образац за брзо креирање** за клијента за уговор | Означава да ли постоји договорено ограничење или горње ограничење укупног износа који ће се фактурисати овом клијенту за ово ангажовање. | Подешавање **Ограничење које не сме да се прекорачи** на нивоу клијента за уговор оцењиваће се у **стварним вредностима ненаплаћене продаје** који упућују на овог клијента за уговор. |

## <a name="edit-billing-split-percentages"></a>Уређивање процената поделе наплате

Проценти поделе наплате се могу уређивати помоћу искуства директног уређивања у мрежи. Када проценти поделе наплате не буду износили 100 процената, добићете грешку. Када уредите проценте поделе наплате, освежите страницу да бисте одбацили грешку.

Такође можете изабрати **Равномерно распоређивање** на подформи **Клијенти за уговор** да бисте равномерно распоредили поделу наплате на све клијенте за уговор. Ако постоји фактор заокруживања, он ће се додати клијенту за заокруживање. Један од клијената за уговор је увек означен као клијент за **заокруживање**, што значи да је у запису клијента за уговор заставица заокруживања постављена на **Да**. То је обично примарни клијент за уговор, али то се може променити.