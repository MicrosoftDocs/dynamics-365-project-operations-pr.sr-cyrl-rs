---
title: Управљање већим бројем клијената у предметима уговора заснованим на пројекту
description: Ова тема пружа информације о раду са предметима уговора и уговорима који садрже више клијената.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 71081775ab45167bc1bff1979f7856a2a2a91385
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181920"
---
# <a name="manage-multiple-customers-on-project-based-contract-lines"></a>Управљање већим бројем клијената у предметима уговора заснованим на пројекту

_**Односи се на:** Project Operations за сценарије засноване на ресурсима/без залиха, једноставна примена – од погодбе до профактуре_

Предмети уговора засновани на пројекту могу садржати листу клијената који су одговорни за плаћање. Ова листа клијената на предмету уговора заснованом на пројекту може бити иста као листа клијената на уговору, али то није обавезно. Када се добије понуда за пројекат и креира уговор за пројекат, листа клијената у ставки понуде се копира у одговарајући предмет уговора. Клијенти на понуди се копирају у уговор.

Када се фактурише уговор о пројекту, листа клијената на предмету уговора заснованом на пројекту има приоритет над листом клијената у уговору. Списак клијената на уговору о пројекту користи се само за доделу подразумеваних вредности новим предметима уговора.

Сви клијенти за уговор на картици **Клијенти** уговора о пројекту подразумевају се као клијенти предмета уговора на свим новим предметима уговора креираним за уговор о пројекту. Ниједан постојећи предмет уговора неће наследити нове записе клијената уговора креиране након њих.

## <a name="create-update-or-delete-a-contract-line-customer-record"></a>Креирање, ажурирање или брисање записа клијента из предмета уговора

Можете креирати, ажурирати или избрисати клијента предмета уговора са картице **Клијенти предмета уговора** на страници **Линија уговора заснована на пројекту**. Када се нови клијент дода у предмет уговора заснован на пројекту, он се такође додаје у целокупни уговор као клијент уговора са подразумеваним процентом поделе наплате од нула процената. Проценат поделе наплате у целокупном уговору копира се у нове предмете уговора и у евентуални уговор о пројекту. Међутим, приликом фактурисања из уговора користи се проценат поделе наплате на нивоу предмета уговора, а не проценат поделе наплате на укупном нивоу уговора. 

У наставку се налазе поља на запису клијента предмета уговора за предмет уговора заснован на пројекту како бисте имали на уму док радите са њим:

| Поље | Локација | Опис | Последични утицај |
| --- | --- | --- | --- |
| Налог | Мрежа која може да се уређује на картици **Клијенти предмета уговора**, главни образац и образац за брзо креирање клијента предмета уговора | Сви активни налози. Ово поље се закључава након креирања записа. Да бисте ажурирали поље, избришите запис и направите нови. Ако сте евидентирали било коју стварну вредност, не можете избрисати запис. Међутим, проценат поделе наплате можете означити као нула за тај налог. Када је запис означен као нула, то утиче на све будуће стварне вредности трошкова и прихода који се приписују или деле овом клијенту. | Када одаберете налог са главне листе налога да бисте га додали и сачували, клијент из предмета уговора се такође додаје као клијент за уговор. Клијенти предмета уговора се користе када се генеришу фактуре. |
| Проценат дељења наплате | Мрежа која може да се уређује на картици **Клијенти предмета уговора**, главни образац и образац за брзо креирање клијента предмета уговора | Ово поље представља проценат сваке ненаплаћене продајне трансакције која ће бити приписана овом клијенту предмета уговора. | Клијенти предмета уговора и проценти поделе наплате користе се када се стварне вредности креирају након одобрења и када се генерише фактура. |
| Ограничење које не сме да се прекорачи | Мрежа која може да се уређује на картици **Клијенти предмета уговора**, главни образац и образац за брзо креирање клијента предмета уговора | Означава да ли постоји договорено ограничење или горње ограничење укупног износа који ће се фактурисати овом клијенту за предмет уговора. | Ограничење непрекорачења за клијента предмета уговора користи се када се креирају стварне вредности и генеришу фактуре. |
| Предузеће-власник | Мрежа која може да се уређује на картици **Клијенти ставке понуде**, главни образац и образац за брзо креирање клијента ставке понуде | Правно лице у којем је овај клијент подешен. Ово поље је само за читање и постављено је на предузеће-власника понуде. Листа клијената које треба додати у поље **Пословни контакт** већ је филтрирана на листу из овог предузећа-власника. | Концепт предузећа-власника изједначава се са концептом правног лица. Сви трошкови и приходи који произлазе из овог пројекта евидентирани су у главној књизи предузећа-власника. |
| Да ли је заокруживање | Мрежа која може да се уређује на картици **Клијенти предмета уговора**, главни образац и образац за брзо креирање клијента предмета уговора | Ово поље означава да ли је овај клијент подразумевани клијент за заокруживање за овај предмет уговора заснован на пројекту. | Када генеришете стварну вредност у складу са процентом поделе наплате, могу постојати неке разлике у заокруживању. У том случају, разлике у заокруживању се приписују овом купцу. |

## <a name="edit-billing-split-percentages"></a>Уређивање процената поделе наплате

Проценти поделе наплате се могу уређивати у мрежи. Када проценти поделе наплате не буду износили 100 процената, јавиће се грешка. Када уредите проценте поделе наплате, освежите страницу да бисте уклонили грешку.

Такође можете покушати да изаберете **Равномерно распореди** на подформи клијента предмета уговора. Ова радња равномерно распоређује поделе наплате за све клијенте предмета уговора. Ако постоји било који фактор заокруживања, он ће се додати клијенту за заокруживање. Један клијент из предмета уговора увек је означен као клијент за **заокруживање**, чија заставица **Заокруживање** је постављена на **Да**.