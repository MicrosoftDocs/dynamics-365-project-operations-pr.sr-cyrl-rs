---
title: Предмети могућности за пословање засновани на пројекту (Pro)
description: Ова тема пружа информације о предметима могућности за пословање заснованим на пројекту. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a688b9bed5a38e7b5947cbcee1e3cb8ab211e98
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896389"
---
# <a name="project-based-opportunity-lines-pro"></a>Предмети могућности за пословање засновани на пројекту (Pro)

_**Односи се на:** Једноставна примена – од погодбе до профактуре_

Предмети могућности за пословање засновани на пројекту доступни су само у оквиру могућности за пословање заснованих на пројекту. Записи могућности за пословање засновани на пројекту имају поље **Тип** постављено на **Засновано на послу**.

Предмети могућности за пословање засновани на пројекту су ставке које ће бити испоручене клијенту коришћењем пројекта. Међутим, пројекат не може бити везан за предмет могућности за пословање заснован на пројекту. Пројекти се могу везати за ставке из фазе **понуде** и касније, јер могућност за пословање је обично у раној фази животног циклуса погодбе. Одређивање броја пројеката који ће се користити за испоруку посла клијенту је одлука која се доноси касније у фази продаје. Фазу могућности за пословање можете користити за идентификовање дискретних компоненти испоруке за клијента. Одлуке у вези са стварним бројем пројеката који се користе за испоруку ових компоненти могу се одбацити док се не сазна више информација о самом раду.

Испод су поља у предмету могућности за пословање заснованом на пројекту:

| **Поље** | **Локација** | **Релевантност, сврха и смернице** | **Последични утицај** |
| --- | --- | --- | --- |
| Тип производа | Картица Општи подаци (скривена) | Можете да изаберите неку од следећих опција:</br>- Услуга заснована на пројекту (доступна само када је инсталирана услуга Dynamics 365 Project Operations)</br>- Производ (доступан само када су инсталиране услуге Project Operations и Dynamics 365 Sales) | Вредност овог поља је постављена на **Услуга заснована на пројекту** када креирате ставку могућности за пословање засновану на пројекту из мреже ставки заснованих на пројекту у могућности за пословање. <br> Ако промените или замените ову вредност, функционалност пројекта неће бити омогућена на ставкама заснованим на пројекту. |
| Могућност за пословање | Картица Општи подаци | Ово поље је само за читање и односи се на надређени запис могућности за пословање којем припада ова ставка. | Нема последичног утицаја из овог поља. |
| Име | Картица Општи подаци | Ово текстуално поље подложно уређивању може се користити за давање кратког идентитета ставци. | Ова вредност се преноси на ставку понуде када креирате понуду из ове могућности за пословање. |
| Буџет клијента | Картица Општи подаци | Ово поље валуте за уређивање може се користити за праћење износа који је клијент спреман да потроши за ову ставку. | Ова вредност се преноси на одговарајуће поље ставке понуде када понуду креирате из ове могућности за пословање. |
| Начин наплате | Картица Општи подаци | Ово поље подложно уређивању има следеће вредности:</br>- Време и материјал</br>- Фиксна цена | Ова вредност се преноси на одговарајуће поље ставке понуде када понуду креирате из ове могућности за пословање. Када креирате ставку понуде, поље је закључано и не може се променити. Доделите вредност овог поља што је тачније могуће. Ако је потребно да промените вредност овог поља у ставци понуде, избришите и поново креирајте ставку понуде. |