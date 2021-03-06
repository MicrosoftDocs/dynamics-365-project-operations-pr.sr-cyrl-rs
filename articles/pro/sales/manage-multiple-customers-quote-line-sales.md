---
title: Управљање са више клијената у ставкама понуда заснованим на пројекту
description: Ова тема описује како се управља са више клијената у ставкама понуда заснованим на пројекту.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6a509fcf8d1fa11b4ce1ba1493d9c3cc64b4f22f
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965884"
---
# <a name="managing-multiple-customers-on-project-based-quote-lines"></a>Управљање са више клијената у ставкама понуда заснованим на пројекту

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Ставке понуде засноване на пројекту подржавају сценарије где свака ставка понуде има листу клијената који је плаћају. Ова листа клијената на ставци понуде засноване на пројекту може бити иста као листа клијената на понуди. Можете и да промените листу клијената да буде другачија. Када се оствари понуда за пројекат, листа клијената на ставци понуде засноване на пројекту се копира у одговарајући предмет уговора заснован на пројекту да би се креирао евентуални уговор о пројекту. Клијенти на основу понуде засноване на пројекту копирају се у уговор за пројекат.

Када фактуришете евентуални уговор за пројекат, листа клијената у предмету уговора заснованог на пројекту има приоритет над листом у уговору за пројекат. Листа клијената на пројектном уговору користи се само за подразумевана подешавања на новим предметима уговора о пројекту.

Сви клијенти понуде на картици **Клијенти** понуде за пројекат подразумевано су клијенти ставке понуде у свакој новој ставци понуде засноване на пројекту креираној за понуду за пројекат. Све постојеће ставке понуде засноване на пројекту не наслеђују нове записе клијената понуде креиране након њих.

## <a name="create-update-or-delete-a-quote-line-customer-record"></a>Креирање, ажурирање или брисање записа клијента ставке понуде

Можете да креирате, ажурирате или избришете клијента ставке понуде на картици **Клијенти ставке понуде** на страници **Ставка понуде заснована на пројекту**. Када додате новог клијента на ставци понуде засноване на пројекту, клијент се такође додаје у укупну понуду као клијент понуде, са подразумеваним процентом поделе наплате на укупној понуди од 0%. Проценат поделе наплате на целокупној понуди копира се у нове редове понуда и на евентуални уговор за пројекат. Међутим, приликом фактурисања из уговора користи се проценат поделе наплате на нивоу ставке понуде, а не проценат поделе наплате на укупном нивоу уговора. 

Следећа табела приказује поља у запису клијента ставке понуде у ставци понуде засноване на пројекту.

| Поље | Локација | Опис и смернице | Последични утицај |
| --- | --- | --- | --- |
| **Налог** | Мрежа за уређивање на картици **Клијенти ставке понуде**, главни образац и обрасци за брзо креирање за клијента на ставци понуде. | Наводи све активне налоге. Ово поље се закључава након креирања записа. Ако треба да ажурирате поље, избришите и поново направите запис. Ако сте евидентирали било коју стварну вредност, не можете избрисати запис. | Када одаберете пословни контакт са главне листе пословних контаката који желите да додате, клијент на ставци понуде се такође додаје као клијент на понуди када га сачувате. Када се понуда оствари, клијенти на ставкама понуде копирају се у клијенте на предметима уговора. |
| **Проценат дељења наплате** | Мрежа за уређивање на картици **Клијенти ставке понуде**, главни образац и обрасци за брзо креирање за клијента на ставци понуде. | Представља проценат сваке ненаплаћене продајне трансакције која ће бити приписана овом клијенту ставке понуде. | Копира се у клијенте предмета уговора за пројекат. |
| **Ограничење које не сме да се прекорачи** | Мрежа за уређивање на картици **Клијенти ставке понуде**, главни образац и обрасци за брзо креирање за клијента на ставци понуде. | Означава да ли постоји уговорено ограничење или горње ограничење укупног износа који ће се фактурисати овом клијенту за ову ставку понуде. | Копира се у клијенте предмета уговора о пројекту када се понуда оствари. |
| **Да ли се заокружује** | Мрежа за уређивање на картици **Клијенти ставке понуде**, главни образац и обрасци за брзо креирање за клијента на ставци понуде. | Означава да ли је овај клијент подразумевани клијент за заокруживање за ову ставку понуде засноване на пројекту. | Копира се у клијенте уговора о пројекту када се понуда оствари. |

## <a name="edit-billing-split-percentages"></a>Уређивање процената поделе наплате

Проценте поделе наплате можете уредити изнутра. Када проценти поделе наплате не износе 100%, долази до грешке. Када уређујете проценте поделе наплате, освежите страницу ставке понуде да бисте уклонили грешку.

Користите радњу равномерне расподеле на подформи клијената ставке понуде да бисте доделили поделе наплате свим клијентима ставке понуде. Ако постоји фактор заокруживања, то ће се додати клијенту за заокруживање. Један од клијената ставке понуде увек је означен као клијент за заокруживање, што значи да је у запису клијента ставке понуде заставица за заокруживање подешена на **Да**. 
