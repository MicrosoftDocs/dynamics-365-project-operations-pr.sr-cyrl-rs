---
title: Конфигуришите материјале који нису на залихама и фактуре добављача на чекању
description: Ова тема објашњава како да омогућите материјале који нису на залихама и фактуре добављача на чекању.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 24418f3aad8356bd209eef7487a47a3870bce10f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993929"
---
# <a name="configure-non-stocked-materials-and-pending-vendor-invoices"></a><span data-ttu-id="22e6d-103">Конфигуришите материјале који нису на залихама и фактуре добављача на чекању</span><span class="sxs-lookup"><span data-stu-id="22e6d-103">Configure non-stocked materials and pending vendor invoices</span></span>

<span data-ttu-id="22e6d-104">_**Односи се на:** Project Operations за сценарије засноване на ресурсима / без залиха_</span><span class="sxs-lookup"><span data-stu-id="22e6d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="minimum-version-requirement"></a><span data-ttu-id="22e6d-105">Минималан захтев верзије</span><span class="sxs-lookup"><span data-stu-id="22e6d-105">Minimum version requirement</span></span>

<span data-ttu-id="22e6d-106">Коришћење материјала који нису на залихама и фактура добављача на чекању за Dynamics 365 Project Operations сценарије без залиха/на основу ресурса захтевају следеће верзије:</span><span class="sxs-lookup"><span data-stu-id="22e6d-106">Using non-stocked materials and pending vendor invoices for Dynamics 365 Project Operations non-stocked/resource based scenarios requires the following versions:</span></span>

<span data-ttu-id="22e6d-107">Dynamics 365 Dataverse решења:</span><span class="sxs-lookup"><span data-stu-id="22e6d-107">Dynamics 365 Dataverse solutions:</span></span>

- <span data-ttu-id="22e6d-108">Project Operations – 4.9.0.221 или новији</span><span class="sxs-lookup"><span data-stu-id="22e6d-108">Project Operations – 4.9.0.221 or higher</span></span>
- <span data-ttu-id="22e6d-109">Решење за оркестрацију двоструког писања – 2.2.2.23 или новије</span><span class="sxs-lookup"><span data-stu-id="22e6d-109">Dual-write application orchestration solution - 2.2.2.23 or higher</span></span>

<span data-ttu-id="22e6d-110">Dynamics 365 Finance:</span><span class="sxs-lookup"><span data-stu-id="22e6d-110">Dynamics 365 Finance:</span></span>
- <span data-ttu-id="22e6d-111">10.0.18 (10.0.793.52) или новији.</span><span class="sxs-lookup"><span data-stu-id="22e6d-111">10.0.18 (10.0.793.52) or higher.</span></span> <span data-ttu-id="22e6d-112">Уверите се да је ваше Finance окружење актуелно и да се примењују сва ажурирања квалитета како би се испунили минимални захтеви за верзију.</span><span class="sxs-lookup"><span data-stu-id="22e6d-112">Make sure that your Finance environment is current and all quality updates are applied to meet the minimum version requirements.</span></span>

## <a name="run-dual-write-maps-for-non-stocked-materials-and-vendor-invoice-integration"></a><span data-ttu-id="22e6d-113">Покрените мапе двоструког писања за нескладиштене материјале и интеграцију рачуна добављача</span><span class="sxs-lookup"><span data-stu-id="22e6d-113">Run Dual-write maps for non-stocked materials and vendor invoice integration</span></span>

<span data-ttu-id="22e6d-114">Овај одељак пружа информације о одређеним мапама потребним за материјал који није на залихама и фактуре добављача.</span><span class="sxs-lookup"><span data-stu-id="22e6d-114">This section provides information about specific the maps required for non-stocked materials and vendor invoices.</span></span> <span data-ttu-id="22e6d-115">Проверите да ли су неопходне мапе наведене у теми [Обезбедите ново окружење](../environment/resource-provision-new-environment.md#run-project-operations-dual-write-maps) покренуте у вашем окружењу.</span><span class="sxs-lookup"><span data-stu-id="22e6d-115">Verify that the prerequisite maps listed in the [Provision a new environment](../environment/resource-provision-new-environment.md#run-project-operations-dual-write-maps) topic are running on your environment.</span></span>

1. <span data-ttu-id="22e6d-116">Идите на Lifecycle Services (LCS), дођите до LCS пројекта и идите на страницу **Детаљи окружења**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-116">Go to Lifecycle Services (LCS), navigate to your LCS project, and go to the **Environment details** page.</span></span>
2. <span data-ttu-id="22e6d-117">У одељку Информације о **Common Data Service окружењу**, изаберите **Веза до услуге CDS за апликације**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-117">In the **Common Data Service Environment Information** section, select **Link to CDS for Apps**.</span></span> <span data-ttu-id="22e6d-118">Када изаберете везу, бићете преусмерени на листу ентитета у мапирањима.</span><span class="sxs-lookup"><span data-stu-id="22e6d-118">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="22e6d-119">Обавезно покрените следеће мапе.</span><span class="sxs-lookup"><span data-stu-id="22e6d-119">Make sure the following maps are running.</span></span> <span data-ttu-id="22e6d-120">Ако се не покрећу, покрените их и побрините се да укључите све повезане мапе табела.</span><span class="sxs-lookup"><span data-stu-id="22e6d-120">If they aren't running, start them and make sure to include all related table maps.</span></span>

    - <span data-ttu-id="22e6d-121">CDS је објавио различите производе (производи)</span><span class="sxs-lookup"><span data-stu-id="22e6d-121">CDS released distinct products (products)</span></span>
    - <span data-ttu-id="22e6d-122">Продавци v2 (msdyn_vendors)</span><span class="sxs-lookup"><span data-stu-id="22e6d-122">Vendors v2 (msdyn_vendors)</span></span>
    - <span data-ttu-id="22e6d-123">Project Operations табела за процене материјала (msdyn_estimatelines)</span><span class="sxs-lookup"><span data-stu-id="22e6d-123">Project Operations table for material estimates (msdyn_estimatelines)</span></span>
    - <span data-ttu-id="22e6d-124">Project Operations ентитет извоза фактуре продавца (msdyn_projectvendorinvoices)</span><span class="sxs-lookup"><span data-stu-id="22e6d-124">Project Operations integration project vendor invoice export entity (msdyn_projectvendorinvoices)</span></span>
    - <span data-ttu-id="22e6d-125">Project Operations ентитет извоза реда фактуре продавца (msdyn_projectvendorinvoicelines)</span><span class="sxs-lookup"><span data-stu-id="22e6d-125">Project Operations integration project vendor invoice line export entity (msdyn_projectvendorinvoicelines)</span></span>
    - <span data-ttu-id="22e6d-126">Project Operations стварне вредности интеграције (msdyn_actuals).</span><span class="sxs-lookup"><span data-stu-id="22e6d-126">Project Operations integration actuals (msdyn_actuals).</span></span> <span data-ttu-id="22e6d-127">Обавезно покрените верзију мапе 1.0.0.14 или новију.</span><span class="sxs-lookup"><span data-stu-id="22e6d-127">Make sure you are running map version 1.0.0.14 or higher.</span></span> <span data-ttu-id="22e6d-128">Активну верзију мапе можете видети у колони **Верзија** на страници **Двоструко уписивање**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-128">You can see the active version of the map in the **Version** column on the **Dual Write** page.</span></span> <span data-ttu-id="22e6d-129">Можете активирати нову верзију мапе ако изаберете **Верзија табеле мапе**, а затим сачувајте изабрану верзију.</span><span class="sxs-lookup"><span data-stu-id="22e6d-129">You can activate a new version of the map by selecting **Table map version** and then saving the selected version.</span></span>

<span data-ttu-id="22e6d-130">Ако користите стандардне демо податке, можда ћете такође морати да зауставите и поново покренете следеће мапе ентитета са почетном синхронизацијом:</span><span class="sxs-lookup"><span data-stu-id="22e6d-130">If you are using standard demo data, you might also need to stop and restart the following entity maps with initial sync:</span></span>
  - <span data-ttu-id="22e6d-131">Дани плаћања CDS V2 (msdyn_paymentdays)</span><span class="sxs-lookup"><span data-stu-id="22e6d-131">Payment days CDS V2 (msdyn_paymentdays)</span></span>
  - <span data-ttu-id="22e6d-132">Распоред плаћања (msdyn_paymentschedules)</span><span class="sxs-lookup"><span data-stu-id="22e6d-132">Payment schedule (msdyn_paymentschedules)</span></span>
  - <span data-ttu-id="22e6d-133">Услови плаћања (msdyn_paymentterms)</span><span class="sxs-lookup"><span data-stu-id="22e6d-133">Terms of payment (msdyn_paymentterms)</span></span>
  - <span data-ttu-id="22e6d-134">Групе добављача (msdyn_vendorgroups)</span><span class="sxs-lookup"><span data-stu-id="22e6d-134">Vendor groups (msdyn_vendorgroups)</span></span>
  - <span data-ttu-id="22e6d-135">Јединице (uom)</span><span class="sxs-lookup"><span data-stu-id="22e6d-135">Units (uom)</span></span>

> [!NOTE]
> <span data-ttu-id="22e6d-136">Почетна синхронизација за групе добављача и јединице можда неће успети за неколико записа у постојећем демо скупу података.</span><span class="sxs-lookup"><span data-stu-id="22e6d-136">The initial sync for vendor groups and units might fail for a few records in the existing demo data set.</span></span> <span data-ttu-id="22e6d-137">Грешке можете занемарити јер вас оне неће спречити да користите демо податке са Project Operations.</span><span class="sxs-lookup"><span data-stu-id="22e6d-137">You can ignore the failures as they won't prevent you from using demo data with Project Operations.</span></span>

## <a name="configure-prerequisites-in-dataverse"></a><span data-ttu-id="22e6d-138">Конфигуришите предуслове у Dataverse</span><span class="sxs-lookup"><span data-stu-id="22e6d-138">Configure prerequisites in Dataverse</span></span>

### <a name="activate-workflow-to-create-accounts-based-on-vendor-entity"></a><span data-ttu-id="22e6d-139">Активирајте ток посла да бисте креирали налоге на основу ентитета добављача</span><span class="sxs-lookup"><span data-stu-id="22e6d-139">Activate workflow to create accounts based on vendor entity</span></span>

<span data-ttu-id="22e6d-140">Решење за оркестрацију двоструког уписивања пружа [добављачима главну интеграцију](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-mapping.md).</span><span class="sxs-lookup"><span data-stu-id="22e6d-140">The Dual Write Orchestration solution provides [Vendors master integration](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-mapping.md).</span></span> <span data-ttu-id="22e6d-141">Као предуслов за ову функцију, подаци добављача морају се креирати у ентитету **Налози**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-141">As a prerequisite for this feature, vendor data must be created in the **Accounts** entity.</span></span> <span data-ttu-id="22e6d-142">Активирајте процес тока посла шаблона да бисте креирали добављаче у табели **Налози** како је описано у [Пребацујте се између дизајна добављача](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-switch.md#use-the-extended-vendor-design-for-vendors-of-the-organization-type).</span><span class="sxs-lookup"><span data-stu-id="22e6d-142">Activate a template workflow process to create vendors in the **Accounts** table as described in [Switch between vendor designs](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-switch.md#use-the-extended-vendor-design-for-vendors-of-the-organization-type).</span></span>

### <a name="set-products-to-be-created-as-active"></a><span data-ttu-id="22e6d-143">Подесите производе који ће се креирати као активни</span><span class="sxs-lookup"><span data-stu-id="22e6d-143">Set products to be created as active</span></span>

<span data-ttu-id="22e6d-144">Материјали ван залиха морају бити конфигурисани као **Објављени производи** у Finance.</span><span class="sxs-lookup"><span data-stu-id="22e6d-144">Non-stocked materials must be configured as **Released products** in Finance.</span></span> <span data-ttu-id="22e6d-145">Решење за оркестрацију двоструког уписивања пружа готову [Каталог производа интеграција објављених производа у Dataverse](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/product-mapping.md).</span><span class="sxs-lookup"><span data-stu-id="22e6d-145">The Dual Write Orchestration solution provides an out-of-the-box [Released products integration to Dataverse Product catalog](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/product-mapping.md).</span></span> <span data-ttu-id="22e6d-146">Подразумевано се производи из Finance синхронизују са Dataverse у статусу радне верзије.</span><span class="sxs-lookup"><span data-stu-id="22e6d-146">By default, products from Finance are synchronized to Dataverse in a draft state.</span></span> <span data-ttu-id="22e6d-147">Да бисте синхронизовали производ у активно стање, тако да се може директно користити у документима о употреби материјала или на фактурама добављача на чекању, идите на **Систем** > **Администрација** > **Администрација система** > **Подешавања система** и на картици **Продаја** подесите **Креирајте производе у активном стању** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-147">To synchronize the product to an active state so that it can be directly used in material usage documents or pending vendor invoices, go to **System** > **Administration** > **System administration** > **System settings**, and on the **Sales** tab, set **Create products in active state** to **Yes**.</span></span>

## <a name="configure-prerequisites-in-finance"></a><span data-ttu-id="22e6d-148">Конфигуришите предуслове у Finance</span><span class="sxs-lookup"><span data-stu-id="22e6d-148">Configure prerequisites in Finance</span></span>

### <a name="enable-the-feature-key-for-pending-vendor-invoices"></a><span data-ttu-id="22e6d-149">Омогућите тастер функције за фактуре добављача на чекању</span><span class="sxs-lookup"><span data-stu-id="22e6d-149">Enable the feature key for pending vendor invoices</span></span>

<span data-ttu-id="22e6d-150">Довршите следеће кораке да бисте омогућили функционалност за додавање детаља о пројекту у редове фактура добављача на чекању.</span><span class="sxs-lookup"><span data-stu-id="22e6d-150">Complete the following steps to enable functionality to add project details on pending vendor invoice lines.</span></span>

1. <span data-ttu-id="22e6d-151">У Finance идите у радни простор **Управљање функцијама**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-151">In Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="22e6d-152">На листи функција пронађите функцију **Омогућите фактуре добављача на чекању у Project Operations за ресурс/сценарије који нису засновани на залихама** и изаберите **Омогући**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-152">In the feature list, find **Enable pending vendor invoices on Project Operations for resource based/non-stocked scenarios** feature and select **Enable**.</span></span>

### <a name="define-category-groups-and-project-categories-for-items"></a><span data-ttu-id="22e6d-153">Дефинишите групе категорија и категорије пројеката за ставке</span><span class="sxs-lookup"><span data-stu-id="22e6d-153">Define category groups and project categories for items</span></span>

<span data-ttu-id="22e6d-154">Конфигуришите најмање једну групу категорија за тип трансакције **Ставка** и најмање једну категорију пројекта која користи ову групу.</span><span class="sxs-lookup"><span data-stu-id="22e6d-154">Configure at least one category group for the **Item** transaction type , and at least one project category using this group.</span></span> <span data-ttu-id="22e6d-155">За више информација, погледајте одељак [Конфигурисање категорија пројеката](../project-accounting/configure-project-categories.md#category-groups).</span><span class="sxs-lookup"><span data-stu-id="22e6d-155">For more information, see [Configure project categories](../project-accounting/configure-project-categories.md#category-groups).</span></span>

<span data-ttu-id="22e6d-156">Прегледајте профиле трошкова и прихода пројекта и конфигуришите подешавање главне књиге за трансакције ставки.</span><span class="sxs-lookup"><span data-stu-id="22e6d-156">Review the project cost and revenue profiles, and configure ledger posting setup for item transactions.</span></span> <span data-ttu-id="22e6d-157">За више информација погледајте [Конфигуришите рачуноводство за пројекте које треба наплатити](../project-accounting/configure-accounting-billable-projects.md).</span><span class="sxs-lookup"><span data-stu-id="22e6d-157">For more information, see [Configure accounting for billable projects](../project-accounting/configure-accounting-billable-projects.md).</span></span>

### <a name="set-up-a-write-in-product"></a><span data-ttu-id="22e6d-158">Подесите ручно додат производ</span><span class="sxs-lookup"><span data-stu-id="22e6d-158">Set up a write-in product</span></span>

<span data-ttu-id="22e6d-159">У Project Operations можете да забележите процене и употребу материјала за каталошке производе који су конфигурисани у издатом каталогу производа и за ручно додате производе.</span><span class="sxs-lookup"><span data-stu-id="22e6d-159">In Project Operations, you can record material estimates and usage for catalog products that are configured in the released product catalog and for write-in products.</span></span> <span data-ttu-id="22e6d-160">Коришћење ручно додатих производа захтева један објављен производ који је у ту сврху конфигурисан у Finance.</span><span class="sxs-lookup"><span data-stu-id="22e6d-160">Using write-in products requires a single released product that's configured in Finance for this purpose.</span></span> <span data-ttu-id="22e6d-161">Довршите следеће кораке за конфигурисање ручно додатог производа.</span><span class="sxs-lookup"><span data-stu-id="22e6d-161">Complete the following steps to configure a write-in product.</span></span> <span data-ttu-id="22e6d-162">Поновите ове кораке у сваком правном лицу које користи Project Operations за сценарије са ресурсима/материјалима који нису на залихама.</span><span class="sxs-lookup"><span data-stu-id="22e6d-162">Repeat these steps in each legal entity that is using Project Operations for resource/non-stocked scenarios.</span></span>

1. <span data-ttu-id="22e6d-163">У Finance идите на **Управљање информацијама о производу** > **Производи** > **Објављени производи** и изаберите **Ново**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-163">In Finance, go to **Product Information Management** > **Products** > **Released products**, and select **New**.</span></span>
2. <span data-ttu-id="22e6d-164">У пољу **Врста производа** изаберите **Ставка** и у пољу **Подтип производа** изаберите **Производ**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-164">In the **Product type** field, select **Item** and in the **Product subtype** field, select **Product**.</span></span>
3. <span data-ttu-id="22e6d-165">Унесите број производа (WRITEIN) и назив производа (ручно додат производ).</span><span class="sxs-lookup"><span data-stu-id="22e6d-165">Enter the product number (WRITEIN) and the product name (Write-in Product).</span></span>
4. <span data-ttu-id="22e6d-166">Изаберите групу модела ставки.</span><span class="sxs-lookup"><span data-stu-id="22e6d-166">Select  the item model group.</span></span> <span data-ttu-id="22e6d-167">Уверите се да изабрана група модела ставки има поље **Политика залиха Производ на залихама** постављено на **Нетачно**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-167">Make sure that the item model group you select has the **Inventory policy Stocked product** field set to **False**.</span></span>
5. <span data-ttu-id="22e6d-168">Изаберите вредности у пољима **Група предмета**, **Група димензија складишта** и **Група димензија праћења**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-168">Select values in the **Item group**, **Storage dimension group**, and **Tracking dimension group** fields.</span></span> <span data-ttu-id="22e6d-169">Користите **Димензија складишта** само за **Локација** и не постављајте никакве димензије праћења.</span><span class="sxs-lookup"><span data-stu-id="22e6d-169">Use the **Storage dimension** for **Site** only, and do not set any tracking dimensions.</span></span>
6. <span data-ttu-id="22e6d-170">Изаберите вредности у пољима **Јединица залиха**, **Јединица куповине** и **Јединица продаје**, а затим сачувајте промене.</span><span class="sxs-lookup"><span data-stu-id="22e6d-170">Select values in the **Inventory unit**, **Purchase unit**, and **Sales unit** field, and then save your changes.</span></span>
7. <span data-ttu-id="22e6d-171">На картици **План**, поставите подразумеване поставке редоследа и на картици **Инвентар** поставите подразумевану локацију и складиште.</span><span class="sxs-lookup"><span data-stu-id="22e6d-171">In the **Plan** tab, set the default order settings, and on the **Inventory** tab, set the default site and warehouse.</span></span>
8. <span data-ttu-id="22e6d-172">Идите у **Управљање пројектима и рачуноводство** > **Подешавање** > **Параметри управљања пројектом и рачуноводствени параметри** и отворите **Project Operations у услузи Dynamics 365 Dataverse**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-172">Go to **Project management and accounting** > **Setup** > **Project management and accounting parameters** and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
9. <span data-ttu-id="22e6d-173">На картици **Материјали** у пољу **Ручно додат производ** изаберите производ који сте креирали.</span><span class="sxs-lookup"><span data-stu-id="22e6d-173">On the **Materials** tab, in the **Write-in product** field, select the product you created.</span></span>
10. <span data-ttu-id="22e6d-174">У вашем Dataverse окружењу, на мапи локације отворите ентитет **Производи** и пронађите запис ручно додатог производа.</span><span class="sxs-lookup"><span data-stu-id="22e6d-174">In your Dataverse environment, in the site map, open the **Products** entity and find the write-in product record.</span></span> 
11. <span data-ttu-id="22e6d-175">Отворите детаље о запису и подесите статус производа на **Повучен**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-175">Open the record details and set product state to **Retired**.</span></span> <span data-ttu-id="22e6d-176">Овај статус производа спречава било кога да случајно користи овај запис директно у проценама материјала и документима о употреби.</span><span class="sxs-lookup"><span data-stu-id="22e6d-176">This product state prevents anyone from accidentally using this record directly in material estimates and usage documents.</span></span>

### <a name="set-up-a-procurement-integration-account"></a><span data-ttu-id="22e6d-177">Подесите налог за интеграцију набавки</span><span class="sxs-lookup"><span data-stu-id="22e6d-177">Set up a procurement integration account</span></span>

<span data-ttu-id="22e6d-178">Налог за интеграцију набавке користи се као налог за обрачун приликом књижења фактуре добављача на чекању са редовима додељеним пројекту.</span><span class="sxs-lookup"><span data-stu-id="22e6d-178">The procurement integration account is used as a clearing account when posting a pending vendor invoice with lines attributed to a project.</span></span>

<span data-ttu-id="22e6d-179">Када систем књижи фактуру добављача на чекању, овај налог се користи за износ трошкова пројекта.</span><span class="sxs-lookup"><span data-stu-id="22e6d-179">When the system posts a pending vendor invoice, this account is used for the project cost amount.</span></span> <span data-ttu-id="22e6d-180">Подаци о фактури добављача се обрађују у Dataverse и креира се одговарајући стварни пројекат.</span><span class="sxs-lookup"><span data-stu-id="22e6d-180">The vendor invoice details are processed in Dataverse, and a corresponding project actual is created.</span></span> <span data-ttu-id="22e6d-181">Информације из стварног пројекта додају се у дневник Project Operations интеграције.</span><span class="sxs-lookup"><span data-stu-id="22e6d-181">The information from the project actual is added to the Project Operations Integration journal.</span></span> <span data-ttu-id="22e6d-182">Када објавите дневник интеграције, износ се брише са налога интеграције набавки и евидентира на трошку пројекта.</span><span class="sxs-lookup"><span data-stu-id="22e6d-182">When you post the integration journal, the amount is cleared from the procurement integration account and recorded to the project cost.</span></span>

1. <span data-ttu-id="22e6d-183">Да бисте подесили налог интеграције набавке, идите у **Управљање пројектима и рачуноводство** > **Подешавање** > **Параметри управљања пројектом и рачуноводствени параметри** и отворите **Project Operations у услузи Dynamics 365 Dataverse**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-183">To set up the procurement integration account, go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**, and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
2. <span data-ttu-id="22e6d-184">Изаберите картицу **Материјали** и изаберите вредност у пољу **Налог за интеграцију набавки**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-184">Select the **Materials** tab, and select a value in the **Procurement integration account** field.</span></span>

#### <a name="set-up-project-category-defaults-for-an-item"></a><span data-ttu-id="22e6d-185">Подесите подразумеване категорије пројекта за ставку</span><span class="sxs-lookup"><span data-stu-id="22e6d-185">Set up project category defaults for an item</span></span>

1. <span data-ttu-id="22e6d-186">У Finance, идите у **Управљање пројектима и рачуноводство** > **Подешавање** > **Параметри управљања пројектом и рачуноводствени параметри** и отворите **Project Operations у услузи Dynamics 365 Dataverse**.</span><span class="sxs-lookup"><span data-stu-id="22e6d-186">In Finance, go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**, and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
2. <span data-ttu-id="22e6d-187">На картици **Подразумеване категорије пројеката** у пољу **Ставка** изаберите вредност.</span><span class="sxs-lookup"><span data-stu-id="22e6d-187">On the **Project category defaults** tab, in the **Item** field, select a value.</span></span> <span data-ttu-id="22e6d-188">Ова категорија пројекта користи се за материјалне трансакције ако категорија пројекта није постављена у евиденцији стварних података о пројекту.</span><span class="sxs-lookup"><span data-stu-id="22e6d-188">This project category is used for material transactions if the project category wasn't set on the project actuals record.</span></span>