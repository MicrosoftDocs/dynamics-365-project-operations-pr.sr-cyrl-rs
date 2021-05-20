---
title: Шта је ново или промењено у издању 13 исправке Project Service Automation верзије 3
description: У овој теми дате су информације о томе шта је ново у издању исправке 13 за Project Service Automation у верзији 3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: a4ebc2e6ca3f6be0a05a7240d762d7a8cf92d81b
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949472"
---
# <a name="project-service-automation-update-release-13-v3"></a>Project Service Automation издање исправке 13, у верзији 3

[!include [banner](../includes/psa-now-project-operations.md)]

Са задовољство најављујемо најновију исправку за апликацију Dynamics 365 Project Service Automation (PSA). Ово издање укључује нека важна побољшања у квалитету, перформансама и употребљивости. Ово издање је компатибилно са услугом Dynamics 365 9.x. Да бисте ажурирали ово издање, посетите центар за администрацију за Dynamics 365 online и идите до странице са решењима како бисте инсталирали исправку. За још информација погледајте чланак [Инсталирање, исправка или уклањање жељеног решења](/power-platform/admin/install-remove-preferred-solution).

У овој теми дате су функције које су нове или су промењене у решењу Project Service Automation у верзији 3, издање исправке 13. Ова верзија има број верзије V3.10.3.18 и доступна је према следећем плану:

- **Општа доступност (само-исправка):** новембар 2019. године
- **аутоматска исправка:** децембар 2019. године


## <a name="update-release-13"></a>Издање исправке 13 

### <a name="bug-fixes"></a>Исправке грешака

- Време и трошак

     - Исправљено: функција претраге на страници **Одобрење трошкова** не ради приликом претраживања према сврси трошкова.

- Управљање ресурсима

     - Исправљено: бројеви у сравњењу су исправљени како би били поравнати удесно.
     - Исправљено: није могуће доделити именоване ресурсе задацима путем картице **Распоред**.

- Управљање пројектима

     - Исправљено: Изузетак за референцу на вредност које нема приликом додељивања члана тима када за **TransactionType** недостају информације о подешавању за ентитете **Unit** и **DefaultGroup**.

- Sales

     - Исправљено: дуплирани записи типа трансакције враћају грешку када се креирају записи цене улоге.
     - Исправљено: Додатна дугмад за ставке **Нова могућност за пословање**, **Понуда**, **Ставка поруџбине** и **Додавање производа** су видљива у командама за могућности за пословање, понуде, наручивање производа и подформе за ставке засноване на пројекту.




[!INCLUDE[footer-include](../includes/footer-banner.md)]