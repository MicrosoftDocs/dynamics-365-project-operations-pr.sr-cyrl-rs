---
title: Преглед трошкова
description: Ова тема пружа информације о функционалности трошкова у услузи Project Operations.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 6da831fef5dba060b8019d7689645405c7ebdbed
ms.sourcegitcommit: 0874b3d89e1dc0e65a51cedb82bf8f80831ca0bb
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/06/2020
ms.locfileid: "3967384"
---
# <a name="expense-home-page"></a><span data-ttu-id="8881c-103">Почетна страница трошкова</span><span class="sxs-lookup"><span data-stu-id="8881c-103">Expense home page</span></span>

<span data-ttu-id="8881c-104">_**Односи се на:** Project Operations за ресурс/сценарије који нису засновани на залихама, лагану примену – од погодбе до профактуре_</span><span class="sxs-lookup"><span data-stu-id="8881c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="8881c-105">Dynamics 365 Project Operations подржава могућност обраде трошкова.</span><span class="sxs-lookup"><span data-stu-id="8881c-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="8881c-106">Обрада трошкова се одвија са пројектима или без њих коришћењем прилагодљивог тока посла смерница, категорија трансакција и одобрења.</span><span class="sxs-lookup"><span data-stu-id="8881c-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="8881c-107">У услузи Project Operations постоје два подржана модела примене за трошкове:</span><span class="sxs-lookup"><span data-stu-id="8881c-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="8881c-108">**Потпуно**: Потпуна примена је доступна за **Project Operations за сценарије засноване на ресурсима / без залиха** или **Project Operations за сценарије засноване на налогу за производњу**.</span><span class="sxs-lookup"><span data-stu-id="8881c-108">**Full**: Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order based scenarios**.</span></span>
- <span data-ttu-id="8881c-109">**Основно**: Основна примена је доступна за **Project Operations за сценарије засноване на ресурсима / без залиха** и **Једноставна примена – од погодбе до профактуре**.</span><span class="sxs-lookup"><span data-stu-id="8881c-109">**Basic**: Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="8881c-110">Пуно</span><span class="sxs-lookup"><span data-stu-id="8881c-110">Full</span></span> 
<span data-ttu-id="8881c-111">Потпуна примена трошкова обезбеђује потпуно спровођење смерница, што обухвата могућност креирања смерница, као што су:</span><span class="sxs-lookup"><span data-stu-id="8881c-111">Full Expense deployment provides a complete policy enforcement which includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="8881c-112">Ограничења категорија трошкова</span><span class="sxs-lookup"><span data-stu-id="8881c-112">Expense category limits</span></span>
  - <span data-ttu-id="8881c-113">Путовање</span><span class="sxs-lookup"><span data-stu-id="8881c-113">Travel</span></span>
  - <span data-ttu-id="8881c-114">Дневница</span><span class="sxs-lookup"><span data-stu-id="8881c-114">Per diem</span></span>
  - <span data-ttu-id="8881c-115">Увози кредитних картица</span><span class="sxs-lookup"><span data-stu-id="8881c-115">Credit card imports</span></span>
  - <span data-ttu-id="8881c-116">Оптичко препознавање знакова признанице</span><span class="sxs-lookup"><span data-stu-id="8881c-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="8881c-117">Основно</span><span class="sxs-lookup"><span data-stu-id="8881c-117">Basic</span></span> 
<span data-ttu-id="8881c-118">Сценариј примене основних трошкова вам омогућава само евидентирање основних трошкова у односу на пројекат.</span><span class="sxs-lookup"><span data-stu-id="8881c-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="8881c-119">За више информација, погледајте [Унос трошкова (једноставно)](basic-expense.md)</span><span class="sxs-lookup"><span data-stu-id="8881c-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="8881c-120">Одредите своју примену трошкова</span><span class="sxs-lookup"><span data-stu-id="8881c-120">Determine your Expense deployment</span></span>
<span data-ttu-id="8881c-121">Да бисте утврдили да ли покрећете примену управљања основним трошковима, проверите да ли се URL адреса завршава са **.crm.dynamics.com**.</span><span class="sxs-lookup"><span data-stu-id="8881c-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 
