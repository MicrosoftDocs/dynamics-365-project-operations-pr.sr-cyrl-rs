---
title: Управљање ресурсима
description: Ова тема пружа информације о томе како можете да управљате ресурсима.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
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
ms.openlocfilehash: 5b34ad66750dba9459d551a2527c13111196511e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: sr-Cyrl-RS
ms.lasthandoff: 10/16/2020
ms.locfileid: "4084173"
---
# <a name="manage-resources"></a><span data-ttu-id="56cc9-103">Управљање ресурсима</span><span class="sxs-lookup"><span data-stu-id="56cc9-103">Manage resources</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="56cc9-104">Dynamics 365 Project Service Automation укључује контролну таблу менаџера ресурса која пружа визуелни преглед потражње и укупне искоришћености ресурса у целој организацији.</span><span class="sxs-lookup"><span data-stu-id="56cc9-104">Dynamics 365 Project Service Automation includes a resource manager dashboard that provides a visual overview of resource demand and utilization throughout the organization.</span></span> <span data-ttu-id="56cc9-105">Можете користити графиконе на овој контролној табли да бисте визуализовали следеће информације:</span><span class="sxs-lookup"><span data-stu-id="56cc9-105">You can use the charts on this dashboard to visualize the following information:</span></span>

- <span data-ttu-id="56cc9-106">**Потражња за ресурсима** - Графикон **Активни захтеви за ресурсе** приказује ресурсе који су прослеђени.</span><span class="sxs-lookup"><span data-stu-id="56cc9-106">**Resource demand** – The **Active Resource Request** chart shows resources that have been submitted.</span></span> <span data-ttu-id="56cc9-107">Ресурси се обједињују по улози или пројекту.</span><span class="sxs-lookup"><span data-stu-id="56cc9-107">The resources are aggregated by either role or project.</span></span>
- <span data-ttu-id="56cc9-108">**Непрослеђена потражња за ресурсима** - Графикон **Недодељена потражња за ресурсима** приказује све потребе за ресурсима које нису прослеђене.</span><span class="sxs-lookup"><span data-stu-id="56cc9-108">**Unsubmitted resource demand** – The **Unassigned Resource Demand** chart shows all the resource requirements that haven't been submitted.</span></span> <span data-ttu-id="56cc9-109">То помаже менаџерима ресурса да погледају потражњу која није чврста и која може бити прослеђена путем захтева за ресурсе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-109">It helps resource managers view demand that isn't firm and might be submitted through a resource request.</span></span>
- <span data-ttu-id="56cc9-110">**Наплатива укупна искоришћеност током прошле седмице** - Графикон **Укупна искоришћеност према улози** приказује проценат стварне укупне искоришћености према улогама у организацији у односу на циљану наплативу укупну искоришћеност по улози.</span><span class="sxs-lookup"><span data-stu-id="56cc9-110">**Billable utilization for the past week** – The **Utilization by Role** chart shows the percentage of the organization's actual billable utilization by role against its target billable utilization by role.</span></span>

    > [!NOTE]
    > <span data-ttu-id="56cc9-111">Да би графикон **Укупна искоришћеност према улози** био доступан, креирајте посао који покреће ток посла UpdateRoleUtilization.</span><span class="sxs-lookup"><span data-stu-id="56cc9-111">To make the **Utilization by Role** chart available, create a job that runs the UpdateRoleUtilization workflow.</span></span> <span data-ttu-id="56cc9-112">Овај периодичан посао се покреће сваких седам дана како би се израчунала наплатива укупна искоришћеност за претходних седам дана.</span><span class="sxs-lookup"><span data-stu-id="56cc9-112">This recurring job runs every seven days to calculate billable utilization for the previous seven days.</span></span> <span data-ttu-id="56cc9-113">Резултати се обједињују по улогама.</span><span class="sxs-lookup"><span data-stu-id="56cc9-113">The results are aggregated by role.</span></span>

## <a name="manage-project-team-members"></a><span data-ttu-id="56cc9-114">Управљање члановима пројектног тима</span><span class="sxs-lookup"><span data-stu-id="56cc9-114">Manage project team members</span></span>

<span data-ttu-id="56cc9-115">Менаџери пројеката могу користити контролну таблу за управитеље ресурсима за управљање ресурсима на пројектима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-115">Project managers can use the resource manager dashboard to manage the resources on projects.</span></span> <span data-ttu-id="56cc9-116">На пример, могу да додају члана тима директно у пројекат и резервишу члана тима да испуне потребе за ресурсима које је евидентирао генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-116">For example, they can add a team member directly to a project and book a team member to fulfill the resource requirements that were captured by a generic resource.</span></span>

### <a name="add-a-team-member-directly-to-a-project"></a><span data-ttu-id="56cc9-117">Додавање члана тима директно у пројекат</span><span class="sxs-lookup"><span data-stu-id="56cc9-117">Add a team member directly to a project</span></span>

<span data-ttu-id="56cc9-118">Да бисте директно додали члана тима у пројекат, на страници **Пројекти** , на картици **Тим** одаберите **Нови**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-118">To add a team member directly to a project, on the **Projects** page, on the **Team** tab, select **New**.</span></span> <span data-ttu-id="56cc9-119">Појавиће се дијалог **Брзо креирање члана пројектног тима**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-119">The **Quick Create:Project Team Member** dialog box appears.</span></span> <span data-ttu-id="56cc9-120">У овом дијалогу можете извршити ове задатке:</span><span class="sxs-lookup"><span data-stu-id="56cc9-120">In this dialog box, you can perform these tasks:</span></span>

- <span data-ttu-id="56cc9-121">**Резервисање именованог ресурса** - У пољу **Ресурса који може да се резервише** одаберите име ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-121">**Book a named resource** – In the **Bookable Resource** field, select the name of the resource.</span></span> <span data-ttu-id="56cc9-122">Затим изаберите улогу, подесите период и изаберите начин додељивања.</span><span class="sxs-lookup"><span data-stu-id="56cc9-122">Then select the role, set the period, and select an allocation method.</span></span> <span data-ttu-id="56cc9-123">Именовани ресурс који сте одабрали додаје се пројекту употребом одабраног начина доделе и календара ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-123">The named resource that you selected is added to the project by using the selected allocation method and the resources calendar.</span></span>
- <span data-ttu-id="56cc9-124">**Додавање генеричког ресурса** - Оставите поље **Ресурс који може да се резервише** празно, а затим одаберите улогу, подесите период и изаберите жељени начин додељивања.</span><span class="sxs-lookup"><span data-stu-id="56cc9-124">**Add a generic resource** – Leave the **Bookable resource** field blank, and then select the role, set the period, and select the preferred allocation method.</span></span> <span data-ttu-id="56cc9-125">У тим се додаје генерички ресурс као чувар места који садржи образац потражње који се користи за резервисање именованих ресурса за тим.</span><span class="sxs-lookup"><span data-stu-id="56cc9-125">A generic resource is added to the team as a placeholder to hold the demand pattern that is used to book named resources on the team.</span></span> <span data-ttu-id="56cc9-126">Захтев се поставља према календару пројекта.</span><span class="sxs-lookup"><span data-stu-id="56cc9-126">The requirement is made according to the project calendar.</span></span>
- <span data-ttu-id="56cc9-127">**Додавање именованог ресурса у тим без трошења капацитета ресурса** - У пољу **Ресурс који може да се резервише** одаберите ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-127">**Add a named resource to the team without consuming resource capacity** – In the **Bookable Resource** field, select a resource.</span></span> <span data-ttu-id="56cc9-128">Затим изаберите период и изаберите **Ниједан** као начин додељивања.</span><span class="sxs-lookup"><span data-stu-id="56cc9-128">Then select the period, and select **None** as the allocation method.</span></span> <span data-ttu-id="56cc9-129">Ресурс се додаје у тим, али капацитет ресурса се не троши резервацијом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-129">The resource is added to the team, but the resource's capacity isn't consumed through a booking.</span></span>

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a><span data-ttu-id="56cc9-130">Резервисање члана тима ради испуњавања потребе за генеричким ресурсом</span><span class="sxs-lookup"><span data-stu-id="56cc9-130">Book a team member to fulfill resource requirements for a generic resource</span></span>

<span data-ttu-id="56cc9-131">У апликацији PSA можете да резервишете генерички ресурс за пројектни тим и можете да одредите улогу, потребни капацитет и како се тај капацитет дистрибуира.</span><span class="sxs-lookup"><span data-stu-id="56cc9-131">In PSA, you can book a generic resource on a project team, and can specify the role, the required capacity, and how that capacity is distributed.</span></span> <span data-ttu-id="56cc9-132">У оквиру потребе за ресурсом можете да наведете атрибуте који су повезани са генеричким ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-132">On the resource requirement, you can specify attributes that are associated with the generic resource.</span></span> <span data-ttu-id="56cc9-133">Ови атрибути укључују тражене вештине, жељену организациону јединицу и жељене ресурсе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-133">These attributes include required skills, the preferred organizational unit, and preferred resources.</span></span>

<span data-ttu-id="56cc9-134">Следите ове кораке да бисте навели потребне вештине генеричког ресурса за програмера.</span><span class="sxs-lookup"><span data-stu-id="56cc9-134">Follow these steps to specify required skills on a generic resource for a developer.</span></span>

1. <span data-ttu-id="56cc9-135">На страници **Пројекти** на картици **Тим** одаберите **Нови** да резервишете генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-135">On the **Projects** page, on the **Team** tab, select **New** to book a generic resource.</span></span>

    ![Генерички ресурс резервисан за тим](media/Resource-Management-image9.png)

2. <span data-ttu-id="56cc9-137">У приказу **Сви чланови тима** , у колони **Потреба за ресурсом** изаберите везу да додате потребне вештине за генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-137">In the **All Team Members** view, in the **Resource Requirement** column, select the link to add required skills for the generic resource.</span></span>

    ![Веза захтева](media/Resource-Management-image10.png)

3. <span data-ttu-id="56cc9-139">На страници **Потреба за ресурсом** која се појављује у мрежи **Вештине** одаберите три тачке ( **...** ), а затим изаберите **Додај нову карактеристику захтева** да додате потребне вештине за програмера.</span><span class="sxs-lookup"><span data-stu-id="56cc9-139">On the **Resource Requirement** page that appears, in the **Skills** grid, select the ellipsis ( **...** ) and then select **Add New Requirement Characteristic** to add the required skills for your developer.</span></span>

    ![Команда за додавање нове карактеристике захтева](media/Resource-Management-image11.png)

4. <span data-ttu-id="56cc9-141">У дијалогу **Брзо креирање карактеристике захтева** који се појављује, у пољу **Карактеристике** одаберите жељену вештину.</span><span class="sxs-lookup"><span data-stu-id="56cc9-141">In the **Quick Create: Requirement Characteristic** dialog box that appears, in the **Characteristic** field, select the required skill.</span></span> <span data-ttu-id="56cc9-142">Затим, у пољу **Вредност оцене** одаберите ниво стручности за ову вештину.</span><span class="sxs-lookup"><span data-stu-id="56cc9-142">Then, in the **Rating value** field, select the proficiency level for that skill.</span></span> <span data-ttu-id="56cc9-143">Коначно у пољу **Потреба за ресурсом** подесите потребу да бисте обезбедили ресурсе из организационих јединица или чак именованих ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-143">Finally, in the **Resource Requirement** field, set the requirement to source resources from organizational units or even named resources.</span></span> <span data-ttu-id="56cc9-144">Када завршите, изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-144">When you've finished, select **Save**.</span></span>

    ![Дијалог за брзо креирање карактеристика захтева](media/Resource-Management-image12.png)

5. <span data-ttu-id="56cc9-146">На страници **Потреба за ресурсом** изаберите **Резервиши** да бисте испунили потребу за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-146">On the **Resource Requirement** page, select **Book** to fulfill the resource requirement.</span></span>

    ![Дугме за резервисање на страници Потреба за ресурсом](media/Resource-Management-image13.png)

    <span data-ttu-id="56cc9-148">Такође можете одабрати генерички ресурс у мрежи **Сви чланови тима** , а затим изабрати **Резервиши**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-148">You can also select the generic resource in the **All Team Members** grid and then select **Book**.</span></span>

    ![Дугме за резервацију изнад мреже Сви чланови тима](media/Resource-Management-image14.png)

    > [!NOTE]
    > <span data-ttu-id="56cc9-150">У овом примеру, постоји 40 захтеваних сати, али нема стварно резервираних сати, јер генерички ресурси немају резервације.</span><span class="sxs-lookup"><span data-stu-id="56cc9-150">In this example, there are 40 required hours but no actual booked hours, because generic resources don't have bookings.</span></span> <span data-ttu-id="56cc9-151">Уз то, нема додељених сати, јер је генерички ресурс додат директно у тим.</span><span class="sxs-lookup"><span data-stu-id="56cc9-151">Additionally, there are no assigned hours, because the generic resource was added directly to the team.</span></span> <span data-ttu-id="56cc9-152">Није додат додељивањем задатка.</span><span class="sxs-lookup"><span data-stu-id="56cc9-152">It wasn't added by using task assignment.</span></span>

    <span data-ttu-id="56cc9-153">На страници **Помоћник за заказивање** можете филтрирати доступне ресурсе према потребама које су наведене у потреби за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-153">On the **Scheduling Assistant** page, you can filter available resources by the requirements that are specified on the resource requirement.</span></span> <span data-ttu-id="56cc9-154">Ресурси су сортирани према параметрима сортирања који су наведени на табели распореда.</span><span class="sxs-lookup"><span data-stu-id="56cc9-154">Resources are sorted according to the sorting parameters that are specified on the Schedule Board.</span></span>

    ![Страница Помоћник за заказивање](media/Resource-Management-image15.png)

    <span data-ttu-id="56cc9-156">Ево неколико филтера који се често користе:</span><span class="sxs-lookup"><span data-stu-id="56cc9-156">Here are some filters that are often used:</span></span>

    - <span data-ttu-id="56cc9-157">**Карактеристике уз оцену** - Филтрирајте по вештинама, цертификацијама и другим квалитетима ресурса, поред оцена стручности.</span><span class="sxs-lookup"><span data-stu-id="56cc9-157">**Characteristics along with a rating** – Filter by skills, certifications, and other resource qualities, in addition to ratings of proficiency.</span></span>
    - <span data-ttu-id="56cc9-158">**Улоге** - Филтрирајте према подразумеваним улогама које су додељене ресурсима који могу да се резервишу.</span><span class="sxs-lookup"><span data-stu-id="56cc9-158">**Roles** – Filter by the default roles that are assigned to bookable resources.</span></span>
    - <span data-ttu-id="56cc9-159">**Организационе јединице** - Филтрирајте ресурсе који могу да се резервишу према организационим јединицама којима су додељени.</span><span class="sxs-lookup"><span data-stu-id="56cc9-159">**Organizational units** – Filter bookable resources by the organizational units that they are assigned to.</span></span>

6. <span data-ttu-id="56cc9-160">Ако нисте задовољни резултатима иницијалне претраге захтева, можете променити критеријуме филтрирања.</span><span class="sxs-lookup"><span data-stu-id="56cc9-160">If you aren't satisfied with the results of the initial requirement search, you can change the filter criteria.</span></span> <span data-ttu-id="56cc9-161">Проширите окно **Приказ филтера** са леве стране, а затим изаберите **Претражи** да бисте пронашли додатне ресурсе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-161">Expand the **Filter View** pane on the left, and then select **Search** to find additional resources.</span></span>

    ![Окно са приказом филтера](media/Resource-Management-image16.png)

7. <span data-ttu-id="56cc9-163">Да бисте променили начин сортирања резултата, изаберите **Сортирај**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-163">To change how the results are sorted, select **Sort**.</span></span>

    ![Команда за сортирање](media/Resource-Management-image17.png)

8. <span data-ttu-id="56cc9-165">Одаберите ресурсе у складу са потражњом која је наведена у захтеву, као што је назначено у врху мреже.</span><span class="sxs-lookup"><span data-stu-id="56cc9-165">Select resources according to the demand that is specified on the requirement, as indicated at the top of the grid.</span></span> <span data-ttu-id="56cc9-166">Можете избрисати избор ћелија у мрежи и оставити отворен капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-166">You can clear the selection of cells in the grid and leave that resource capacity open.</span></span> <span data-ttu-id="56cc9-167">Само један ресурс може бити изабран као резервисан у одређеном тренутку.</span><span class="sxs-lookup"><span data-stu-id="56cc9-167">Only one resource at a time can be selected as booked.</span></span>

9. <span data-ttu-id="56cc9-168">Изаберите **Резервиши** да резервишете изабрани ресурс и оставите табелу распореда отворену, тако да можете да изаберете додатне ресурсе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-168">Select **Book** to book the selected resource and leave the Schedule Board open, so that you can select additional resources.</span></span> <span data-ttu-id="56cc9-169">Или одаберите **Резервиши и изађи** да резервишете изабрани ресурс и затворите табелу распореда.</span><span class="sxs-lookup"><span data-stu-id="56cc9-169">Alternatively, select **Book & Exit** to book the selected resource and close the Schedule Board.</span></span>

    ![Ресурс за резервацију](media/Resource-Management-image19.png)

    <span data-ttu-id="56cc9-171">Добијате обавештење о резервисаним сатима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-171">You receive a notification about booked hours.</span></span> <span data-ttu-id="56cc9-172">Показатељи потражње показују колико је захтев за резервацију испуњен и колико још остаје.</span><span class="sxs-lookup"><span data-stu-id="56cc9-172">The demand indicators show how much the booking requirement is satisfied and how much remains.</span></span> <span data-ttu-id="56cc9-173">Такође можете видети колико је потрошен капацитета одабраног ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-173">You can also see how much of the selected resource's capacity is consumed.</span></span> <span data-ttu-id="56cc9-174">Изаберите **Прошири** да бисте видели више детаља о резервацијама ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-174">Select **Expand** to view more details about resource bookings.</span></span>

9. <span data-ttu-id="56cc9-175">Вратите се на приказ **Сви чланови тима**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-175">Return to the **All Team Members** view.</span></span> <span data-ttu-id="56cc9-176">У мрежи можете да приметите да је генерички ресурс замењен именованим ресурсом и да је 40 сати наведено као резервирано за тај ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-176">In the grid, notice that the generic resource has been replaced by the named resource, and 40 hours are listed as booked for that resource.</span></span>

    ![Мрежа Ажурирани сви чланови тима](media/Resource-Management-image20.png)

    > [!NOTE]
    > <span data-ttu-id="56cc9-178">Нису приказани додељени сати јер су резервисани директно у тиму.</span><span class="sxs-lookup"><span data-stu-id="56cc9-178">No assigned hours are shown, because they were booked directly on the team.</span></span> <span data-ttu-id="56cc9-179">Нису резервисани коришћењем додела задатка.</span><span class="sxs-lookup"><span data-stu-id="56cc9-179">They weren't booked by using task assignment.</span></span>

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a><span data-ttu-id="56cc9-180">Додељивање генеричких ресурса задацима и генерисање потреба за ресурсима</span><span class="sxs-lookup"><span data-stu-id="56cc9-180">Assign generic resources to tasks and generate resource requirements</span></span>

<span data-ttu-id="56cc9-181">У апликацији PSA можете да креирате задатке и да им онда доделите генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-181">In PSA, you can create tasks and then assign generic resources to them.</span></span> <span data-ttu-id="56cc9-182">На овај начин, потражња за ресурсима може бити представљена чуварима места док процењује свој распоред и финансијске бројке.</span><span class="sxs-lookup"><span data-stu-id="56cc9-182">In this way, resource demand can be represented by placeholders while you estimate your schedule and financial numbers.</span></span> <span data-ttu-id="56cc9-183">Затим можете да генеришете потребе за генеричким ресурсима и испуните их.</span><span class="sxs-lookup"><span data-stu-id="56cc9-183">You can then generate resource requirements for the generic resources and fulfill them.</span></span>

1. <span data-ttu-id="56cc9-184">На страници **Пројекти** на картици **Распоред** одаберите **Додај** да креирате задатак.</span><span class="sxs-lookup"><span data-stu-id="56cc9-184">On the **Projects** page, on the **Schedule** tab, select **Add** to create a task.</span></span>

    ![Креиран је нови задатак](media/Resource-Management-image21.png)

2. <span data-ttu-id="56cc9-186">У пољу **Ресурси** изаберите симбол **бирача ресурса**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-186">In the **Resources** field, select the **Resource Picker** symbol.</span></span> <span data-ttu-id="56cc9-187">Појављује се бирач ресурса и показује постојеће чланове тима за пројекат.</span><span class="sxs-lookup"><span data-stu-id="56cc9-187">The Resource Picker appears and shows existing team members for the project.</span></span>

    ![Бирач ресурса](media/Resource-Management-image22.png)

3. <span data-ttu-id="56cc9-189">Унесите име новог генеричког ресурса, а затим изаберите **Креирај**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-189">Enter the name of the new generic resource, and then select **Create**.</span></span>

    ![Унето је име новог генеричког ресурса](media/Resource-Management-image23.png)

4. <span data-ttu-id="56cc9-191">У дијалогу **Брзо креирање члана пројектног тима** који се појављује, у пољу **Улога** одаберите улогу генеричког ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-191">In the **Quick Create: Project Team Member** dialog box that appears, in the **Role** field, select the role for the generic resource.</span></span> <span data-ttu-id="56cc9-192">У пољу **Јединица за обезбеђивање ресурса** изаберите организациону јединицу за генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-192">In the **Resourcing Unit** field, select the organizational unit for the generic resource.</span></span> <span data-ttu-id="56cc9-193">Затим изаберите **Сачувај**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-193">Then select **Save**.</span></span>

    ![Дијалог за брзо креирање члана пројектног тима](media/Resource-Management-image24.png)

    <span data-ttu-id="56cc9-195">Генерички члан тима је сада додељен задатку.</span><span class="sxs-lookup"><span data-stu-id="56cc9-195">The generic team member is now assigned to the task.</span></span>

    ![Генерички члан тима је додељен задатку](media/Resource-Management-image25.png)

    <span data-ttu-id="56cc9-197">На картици **Тим** видећете новог генеричког члана тима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-197">On the **Team** tab, you will see the new generic team member.</span></span> <span data-ttu-id="56cc9-198">Имајте на уму да има само додељене сате.</span><span class="sxs-lookup"><span data-stu-id="56cc9-198">Notice that it has only assigned hours.</span></span> <span data-ttu-id="56cc9-199">Ови часови су збир свих задатака који су додељени генеричком члану тима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-199">These hours are the sum of all tasks that are assigned to the generic team member.</span></span> <span data-ttu-id="56cc9-200">Генерички члан тима још увек нема захтеване сате нити потребу за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-200">The generic team member doesn't yet have required hours or a resource requirement.</span></span>

    ![Генерички члан тима на картици Тим](media/Resource-Management-image26.png)

5. <span data-ttu-id="56cc9-202">Сада можете доделити генеричког члана тима другим задацима помоћу бирача ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-202">You can now assign the generic team member to other tasks by using the Resource Picker.</span></span>

    ![Генерички члан тима у бирачу ресурса](media/Resource-Management-image27.png)

    <span data-ttu-id="56cc9-204">Када завршите са додељивањем генеричког ресурса задацима, можете да генеришете потребу за генеричким ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-204">When you've finished assigning the generic resource to tasks, you can generate a resource requirement for the generic resource.</span></span>

5. <span data-ttu-id="56cc9-205">На картици **Тим** изаберите генерички ресурс, а затим изаберите **Генериши захтев**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-205">On the **Team** tab, select the generic resource, and then select **Generate Requirement**.</span></span>

    ![Команда за генерисање захтева](media/Resource-Management-image28.png)

    <span data-ttu-id="56cc9-207">Када се захтев генерише, члан генеричког тима ће имати захтеване сате и везу ка потреби за ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-207">When the requirement is generated, the generic team member will have required hours and a link for the resource requirement.</span></span>

    ![Веза ка потреби за ресурсом](media/Resource-Management-image29.png)

    <span data-ttu-id="56cc9-209">Када резервишете именовани ресурс, генерички ресурс се уклања из тима и замењује именованим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-209">After you book a named resource, the generic resource is removed from the team and replaced by the named resource.</span></span>

    ![Генерички ресурс је замењен именованим ресурсом](media/Resource-Management-image30.png)

    <span data-ttu-id="56cc9-211">На картици **Распоред** се доделе генеричким ресурсима уклањају и замењују именованим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-211">On the **Schedule** tab, the generic resource assignments are removed and replaced by the named resource.</span></span>

    ![Доделе генеричким ресурсима су замењене именованим ресурсом на картици Распоред](media/Resource-Management-image31.png)

    > [!NOTE]
    > <span data-ttu-id="56cc9-213">Ово понашање се дешава само када је именовани ресурс у потпуности резервисан за потребу за генеричким ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-213">This behavior occurs only when a named resource is fully booked for the generic resource requirement.</span></span> <span data-ttu-id="56cc9-214">Када именовани ресурс делимично замењује потребу за генеричким ресурсом или више именованих ресурса замењује потребу за генеричким ресурсима, генерички ресурс остаје додељен задатку.</span><span class="sxs-lookup"><span data-stu-id="56cc9-214">When either a named resource partially replaces the generic resource requirement or multiple named resources replace the generic resource requirement, the generic resource remains assigned to the task.</span></span>

    <span data-ttu-id="56cc9-215">На следећој илустрацији, задатак од 80 сати је планиран за период од пет дана (16 сати дневно током пет дана) и додељен је генеричком ресурсу који се зове **Функционални**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-215">In the following illustration, an 80-hour task has been planned for a five-day duration (16 hours per day over five days) and assigned to the generic resource that is named **Functional**.</span></span>

    ![Осамдесетчасовни задатак за пет дана је додељен функционалном генеричком извору](media/Resource-Management-image32.png)

    <span data-ttu-id="56cc9-217">Када генеришете захтев, он је за 80 сати током петодневног периода.</span><span class="sxs-lookup"><span data-stu-id="56cc9-217">When you generate the requirement, it's for 80 hours over five days.</span></span>

    ![Захтев је генерисан за 80 сати током пет дана](media/Resource-Management-image33.png)

    <span data-ttu-id="56cc9-219">Будући да доступни ресурси раде само осам сати дневно, потребна су два ресурса да би се испунио захтев.</span><span class="sxs-lookup"><span data-stu-id="56cc9-219">Because available resources work only eight hours per day, two resources are needed to fulfill the requirement.</span></span>

    ![Други ресурс](media/Resource-Management-image35.png)

    <span data-ttu-id="56cc9-221">На картици **Тим** сада можете видети да генерички ресурс нема захтеване сате, али додељени сати се и даље појављују заједно са два именована ресурса која чине испуњење.</span><span class="sxs-lookup"><span data-stu-id="56cc9-221">On the **Team** tab, you can now see that the generic resource has no required hours, but the assigned hours still appear together with the two named resources that make up the fulfillment.</span></span>

    ![Два именована ресурса на картици Тим](media/Resource-Management-image36.png)

    <span data-ttu-id="56cc9-223">На картици **Распоред** генерички ресурс остаје додељен задатку.</span><span class="sxs-lookup"><span data-stu-id="56cc9-223">On the **Schedule** tab, the generic resource remains assigned to the task.</span></span>

    ![Генерички ресурси на картици Распоред](media/Resource-Management-image37.png)

<span data-ttu-id="56cc9-225">PSA не додељује оба ресурса задатку, јер би таквим понашањем настао мање предвидљив распоред.</span><span class="sxs-lookup"><span data-stu-id="56cc9-225">PSA doesn't assign both resources to the task, because that behavior would produce a less predictable schedule.</span></span> <span data-ttu-id="56cc9-226">У овом једноставном примеру лако је подједнако поделити сате на два ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-226">In this simple example, it's easy to divide the hours equally between two resources.</span></span> <span data-ttu-id="56cc9-227">Међутим, у сложенијим сценаријима који укључују више задатака и више ресурса, PSA би морао да претпостави како треба да распореди резервације које су примљене за више ресурса у више задатака.</span><span class="sxs-lookup"><span data-stu-id="56cc9-227">However, in more complex scenarios that involve multiple tasks and multiple resources, PSA would have to make assumptions about how it should allocate the bookings that are received for multiple resources across multiple tasks.</span></span>

<span data-ttu-id="56cc9-228">Стога је у тим сценаријима руководилац пројекта одговоран за рашчлањивање више резервација и њихово додељивање према потреби.</span><span class="sxs-lookup"><span data-stu-id="56cc9-228">Therefore, in these scenarios, the project manager is responsible for parsing the multiple bookings and assigning them as needed.</span></span> <span data-ttu-id="56cc9-229">Да би доделио резервације, менаџер пројекта додељује задатке из генеричких ресурса именованим ресурсима и затим користи приказ **Усаглашеност** да би осигурао да додела функционише са резервацијама.</span><span class="sxs-lookup"><span data-stu-id="56cc9-229">To allocate the bookings, the project manager assigns the tasks from the generic resources to the named resources and then uses the **Reconciliation** view to make sure that the allocation works with the bookings.</span></span>

### <a name="edit-a-resource-requirement"></a><span data-ttu-id="56cc9-230">Уређивање потребе за ресурсом</span><span class="sxs-lookup"><span data-stu-id="56cc9-230">Edit a resource requirement</span></span>

<span data-ttu-id="56cc9-231">Након што креира потребу за ресурсом, менаџер пројекта или менаџер ресурса можда ће желети да измени детаље како би прецизирао критеријуме за претрагу када се користи табела распореда.</span><span class="sxs-lookup"><span data-stu-id="56cc9-231">After a resource requirement has been created, a project manager or resource manager might want to edit the details to refine the search criteria when the Schedule Board is used.</span></span> <span data-ttu-id="56cc9-232">Да бисте уредили потребу за ресурсом, следите ове кораке.</span><span class="sxs-lookup"><span data-stu-id="56cc9-232">To edit the resource requirement, follow these steps.</span></span>

1. <span data-ttu-id="56cc9-233">На страници **Пројекти** на картици **Тим** одаберите везу ка било ком захтеву за генерички ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-233">On the **Projects** page, on the **Team** tab, select the link to any requirement on a generic resource.</span></span>
2. <span data-ttu-id="56cc9-234">На страници **Потреба за ресурсом** која се појављује можете ажурирати неколико атрибута.</span><span class="sxs-lookup"><span data-stu-id="56cc9-234">On the **Resource Requirement** page that appears, you can update several attributes.</span></span> <span data-ttu-id="56cc9-235">У наставку су наведени неки примери:</span><span class="sxs-lookup"><span data-stu-id="56cc9-235">Here are some examples:</span></span>

    - <span data-ttu-id="56cc9-236">Име</span><span class="sxs-lookup"><span data-stu-id="56cc9-236">Name</span></span>
    - <span data-ttu-id="56cc9-237">Од датума</span><span class="sxs-lookup"><span data-stu-id="56cc9-237">From Date</span></span>
    - <span data-ttu-id="56cc9-238">До датума</span><span class="sxs-lookup"><span data-stu-id="56cc9-238">To Date</span></span>
    - <span data-ttu-id="56cc9-239">Трајање</span><span class="sxs-lookup"><span data-stu-id="56cc9-239">Duration</span></span>
    - <span data-ttu-id="56cc9-240">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="56cc9-240">Resource Type</span></span>

<span data-ttu-id="56cc9-241">На страници **Потреба за ресурсом** менаџер пројекта или менаџер ресурса такође може дефинисати следеће информације:</span><span class="sxs-lookup"><span data-stu-id="56cc9-241">On the **Resource Requirement** page, the project manager or resource manager can also define the following information:</span></span>

- <span data-ttu-id="56cc9-242">Вештине</span><span class="sxs-lookup"><span data-stu-id="56cc9-242">Skills</span></span>
- <span data-ttu-id="56cc9-243">Улоге</span><span class="sxs-lookup"><span data-stu-id="56cc9-243">Roles</span></span>
- <span data-ttu-id="56cc9-244">Жељене поставке ресурса</span><span class="sxs-lookup"><span data-stu-id="56cc9-244">Resource preferences</span></span>
- <span data-ttu-id="56cc9-245">Жељену организациону јединицу</span><span class="sxs-lookup"><span data-stu-id="56cc9-245">Preferred organizational unit</span></span>

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a><span data-ttu-id="56cc9-246">Ажурирање резервација ресурса након њиховог резервисања за пројекат</span><span class="sxs-lookup"><span data-stu-id="56cc9-246">Update resource bookings after they are booked on a project</span></span>

<span data-ttu-id="56cc9-247">Након што додате генерички или именовани ресурс у пројектни тим, можете променити резервације ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-247">After you've added a generic or named resource to a project team, you can change the resource's bookings.</span></span>

1. <span data-ttu-id="56cc9-248">На страници **Пројекти** на картици **Тим** одаберите члана тима, а затим изаберите **Одржавање резервација**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-248">On the **Projects** page, on the **Team** tab, select a team member, and then select **Maintain Bookings**.</span></span>

    ![Табела распореда се отвара за изабраног члана тима](media/Resource-Management-image40.png)

    <span data-ttu-id="56cc9-250">Појављује се табела распореда и приказује резервације члана пројектног тима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-250">The Schedule Board appears and shows the project team member's bookings.</span></span> <span data-ttu-id="56cc9-251">Проширите евиденцију члана тима да бисте видели сате који су резервисани за овај пројекат и друге пројекте који троше капацитет члана тима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-251">Expand the team member's record to view the hours that have been booked against this project and other projects that are consuming the team member's capacity.</span></span>

2. <span data-ttu-id="56cc9-252">Изаберите и превуците резервацију да бисте је проширили или скратили.</span><span class="sxs-lookup"><span data-stu-id="56cc9-252">Select and drag the booking to extend or shorten it.</span></span> <span data-ttu-id="56cc9-253">Појавиће се дијалог **Креирање резервације ресурса** који вам омогућава да подесите резервацију.</span><span class="sxs-lookup"><span data-stu-id="56cc9-253">A **Create Resource Booking** dialog box appears that lets you adjust the booking.</span></span>

    ![Дијалог за креирање резервације ресурса](media/Resource-Management-image41.png)

3. <span data-ttu-id="56cc9-255">Кликните десним тастером миша на резервацију.</span><span class="sxs-lookup"><span data-stu-id="56cc9-255">Right-click the booking.</span></span> <span data-ttu-id="56cc9-256">Затим можете да користите мени са пречицама да бисте довршили следеће радње:</span><span class="sxs-lookup"><span data-stu-id="56cc9-256">You can then use the shortcut menu to complete the following actions:</span></span>

    - <span data-ttu-id="56cc9-257">Промените статус резервације.</span><span class="sxs-lookup"><span data-stu-id="56cc9-257">Change the booking status.</span></span>
    - <span data-ttu-id="56cc9-258">Уредите резервацију.</span><span class="sxs-lookup"><span data-stu-id="56cc9-258">Edit the booking.</span></span>
    - <span data-ttu-id="56cc9-259">Замените ресурс у пројектном тиму.</span><span class="sxs-lookup"><span data-stu-id="56cc9-259">Substitute a resource on the project team.</span></span>

### <a name="change-the-booking-status"></a><span data-ttu-id="56cc9-260">Промена статуса резервације</span><span class="sxs-lookup"><span data-stu-id="56cc9-260">Change the booking status</span></span>

<span data-ttu-id="56cc9-261">Можете променити било који подразумевани или прилагођени статус резервације.</span><span class="sxs-lookup"><span data-stu-id="56cc9-261">You can change any default or custom booking status.</span></span>

![Команда за промену статуса](media/Resource-Management-image42.png)

<span data-ttu-id="56cc9-263">Следећи статуси су уврштени у PSA:</span><span class="sxs-lookup"><span data-stu-id="56cc9-263">The following statuses are included in PSA:</span></span>

- <span data-ttu-id="56cc9-264">**Отказан** - Овај статус отказује резервацију ресурса и ослобађа капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-264">**Canceled** – This status cancels a resource's booking and frees up the resource's capacity.</span></span>
- <span data-ttu-id="56cc9-265">**Фиксна резервација** - Овај статус троши капацитет ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-265">**Hard Book** – This status consumes a resource's capacity.</span></span> <span data-ttu-id="56cc9-266">Резервација обично има овај статус када се отворите **Одржавање резервација** на мрежи **Сви чланови тима** на страници **Пројекти**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-266">A booking typically has this status when you open **Maintain Bookings** from the **All Team Members** grid on the **Projects** page.</span></span>
- <span data-ttu-id="56cc9-267">**Условна резервација** - Овај статус додаје ресурс у тим, али не троши његов капацитет.</span><span class="sxs-lookup"><span data-stu-id="56cc9-267">**Soft Book** – This status adds a resource to a team but doesn't consume the resource's capacity.</span></span> <span data-ttu-id="56cc9-268">Указује да је ресурс резервисан за потенцијални рад, али још увек има капацитет ако је потребан на другим пословима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-268">It indicates that the resource has been reserved for potential work but still has capacity if it's needed on other jobs.</span></span> <span data-ttu-id="56cc9-269">С обзиром на укупну доступност ресурса, условне резервације имају другачији статус од фиксних резервација.</span><span class="sxs-lookup"><span data-stu-id="56cc9-269">In the view of overall resource availability, soft bookings have a different status than hard bookings.</span></span>
- <span data-ttu-id="56cc9-270">**Предложен** - Овај статус представља предлог менаџера ресурса или менаџера пројеката за ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-270">**Proposed** – This status represents a resource manager's or project manager's proposal for a resource.</span></span> <span data-ttu-id="56cc9-271">Предлози не троше капацитет ресурса и ресурс се не додаје пројектном тиму.</span><span class="sxs-lookup"><span data-stu-id="56cc9-271">Proposals don't consume the capacity of a resource, and the resource isn't added to the project team.</span></span> <span data-ttu-id="56cc9-272">Да би резервација ресурса за тим била фиксна, менаџер пројекта мора прихватити предлог.</span><span class="sxs-lookup"><span data-stu-id="56cc9-272">To hard-book the resource on the team, the project manager must accept the proposal.</span></span>

### <a name="submit-resource-requests"></a><span data-ttu-id="56cc9-273">Проследите захтеве за ресурсе</span><span class="sxs-lookup"><span data-stu-id="56cc9-273">Submit resource requests</span></span>

<span data-ttu-id="56cc9-274">Захтеви за ресурсе користе се да пренесу потражњу (потребе за ресурсима) која мора бити испуњена од стране менаџера ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-274">Resource requests are used to carry the demand (resource requirement) that must be fulfilled by a resource manager.</span></span> <span data-ttu-id="56cc9-275">За генерички ресурс који је већ у тиму можете директно да проследите захтев за ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-275">For a generic resource that is already on the team, you can submit a resource request directly.</span></span> <span data-ttu-id="56cc9-276">Захтев за ресурс може се испунити на два начина:</span><span class="sxs-lookup"><span data-stu-id="56cc9-276">A resource request can be fulfilled in two ways:</span></span>

- <span data-ttu-id="56cc9-277">Менаџер ресурса директно испуњава захтев.</span><span class="sxs-lookup"><span data-stu-id="56cc9-277">The resource manager directly fulfills the request.</span></span> <span data-ttu-id="56cc9-278">У овом случају, генерички ресурс замењује фиксна резервација која има именовани ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-278">In this case, the generic resource is replaced by a hard booking that has a named resource.</span></span>
- <span data-ttu-id="56cc9-279">Менаџер ресурса предлаже ресурс менаџеру пројеката, а менаџер пројекта одобрава или одбацује предложени ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-279">The resource manager proposes a resource to the project manager, and the project manager approves or rejects the proposed resource.</span></span>

#### <a name="direct-fulfillment-of-resource-requests"></a><span data-ttu-id="56cc9-280">Директно испуњавање захтева за ресурсе</span><span class="sxs-lookup"><span data-stu-id="56cc9-280">Direct fulfillment of resource requests</span></span>

<span data-ttu-id="56cc9-281">Када се генерише потреба за ресурсом, пројектни менаџер може да проследи захтев за генерички ресурс ако изабере ресурс, а затим опцију **Проследи захтев**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-281">When a resource requirement is generated, a project manager can submit a resource request for a generic resource by selecting the resource and then selecting **Submit Request**.</span></span>

![Дугме Проследи захтев](media/Resource-Management-image45.png)

<span data-ttu-id="56cc9-283">Коментари о ресурсу могу се доставити менаџеру ресурса који испуњава захтев.</span><span class="sxs-lookup"><span data-stu-id="56cc9-283">Comments about the resource can be provided to the resource manager who is fulfilling the request.</span></span> <span data-ttu-id="56cc9-284">Након прослеђивања захтева, поље **Статус** за члана тима се мења у **Прослеђен**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-284">After the request is submitted, the **Status** field for the team member is changed to **Submitted**.</span></span>

![Уношење опционалних коментара](media/Resource-Management-image46.png)

<span data-ttu-id="56cc9-286">Када менаџер ресурса испуни захтев, генеричког члана тима замењује именовани ресурс у мрежи **Сви чланови тима**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-286">When the resource manager fulfills the request, the generic team member is replaced by the named resource in the **All Team Members** grid.</span></span>

![Генерички члан тима замењен је именованим ресурсом у мрежи Сви чланови тима](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a><span data-ttu-id="56cc9-288">Коришћење предлога ресурса за захтеве за ресурсе</span><span class="sxs-lookup"><span data-stu-id="56cc9-288">Use a resource proposal for resource requests</span></span>

<span data-ttu-id="56cc9-289">Уместо да директно резервише ресурс у захтеву за ресурсе, менаџер ресурса може да предложи ресурс менаџеру пројеката.</span><span class="sxs-lookup"><span data-stu-id="56cc9-289">Instead of directly booking a resource on a resource request, a resource manager can propose a resource to the project manager.</span></span> <span data-ttu-id="56cc9-290">Менаџер ресурса могао би користити ову опцију када није доступно тачно подударање са потребама.</span><span class="sxs-lookup"><span data-stu-id="56cc9-290">A resource manager might use this option when an exact match for the requirements isn't available.</span></span> <span data-ttu-id="56cc9-291">Када менаџер ресурса предложи ресурс, менаџер пројеката види да је поље **Статус** за генеричког члана тима промењено у **Захтева преглед**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-291">When a resource manager proposes a resource, the project manager sees that the **Status** field for the generic team member is changed to **Needs Review**.</span></span>

![Статус генеричког члана тима промењен је у Захтева преглед](media/Resource-Management-image48.png)

<span data-ttu-id="56cc9-293">Да бисте прегледали предложени ресурс заједно са визуелизацијом ефекта резервације предлога, двапут кликните на члана тима који има статус **Захтева преглед**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-293">To view the proposed resource together with a visualization of the effect of the proposal's booking, double-click the team member that has a status of **Needs Review**.</span></span> <span data-ttu-id="56cc9-294">Затим изаберите картицу **Предложени ресурси**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-294">Then select the **Proposed Resources** tab.</span></span>

![Картица Предложени ресурси](media/Resource-Management-image49.png)

<span data-ttu-id="56cc9-296">Изаберите **Прихвати све предлоге** да прихвате све предложене ресурсе или **Одбаците све предлоге** да их одбаците.</span><span class="sxs-lookup"><span data-stu-id="56cc9-296">Select **Accept All Proposals** to accept all proposed resources or **Reject All Proposals** to reject them.</span></span> <span data-ttu-id="56cc9-297">Ако прихватите предложене ресурсе, они се фиксно резервишу за пројекат као чланови тима и замењују генеричке ресурсе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-297">If you accept the proposed resources, they are hard-booked on the project as team members and replace the generic resources.</span></span>

> [!NOTE]
> <span data-ttu-id="56cc9-298">Морате или прихватити или одбацити све предложене ресурсе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-298">You must either accept or reject all proposed resources.</span></span> <span data-ttu-id="56cc9-299">Не можете их делимично прихватити ни одбацити.</span><span class="sxs-lookup"><span data-stu-id="56cc9-299">You can't partially accept or reject them.</span></span>

### <a name="substitute-a-resource-on-the-project-team"></a><span data-ttu-id="56cc9-300">Замена ресурса у пројектном тиму</span><span class="sxs-lookup"><span data-stu-id="56cc9-300">Substitute a resource on the project team</span></span>

<span data-ttu-id="56cc9-301">Понекад менаџер пројекта мора заменити резервисаног члана тима за пројекат.</span><span class="sxs-lookup"><span data-stu-id="56cc9-301">Sometimes, a project manager must substitute a booked team member on a project.</span></span>

1. <span data-ttu-id="56cc9-302">На страници **Пројекти** на картици **Тим** одаберите ресурс коме је потребна замена, а затим изаберите **Одржавање резервација**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-302">On the **Projects** page, on the **Team** tab, select the resource that needs a substitute, and then select **Maintain Bookings**.</span></span>
2. <span data-ttu-id="56cc9-303">Проширите ресурс за преглед пројеката којима је додељен.</span><span class="sxs-lookup"><span data-stu-id="56cc9-303">Expand the resource to view the projects that it's assigned to.</span></span>

    ![Ресурс је проширен ради приказа додељених пројеката](media/Resource-Management-image50.png)

3. <span data-ttu-id="56cc9-305">Кликните десним тастером миша на пројекат, а затим изаберите **Замена ресурса**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-305">Right-click the project, and then select **Substitute Resource**.</span></span>
4. <span data-ttu-id="56cc9-306">Ако знате ресурс који желите заменити тренутним ресурсом, одаберите или унесите име, а затим изаберите **Поново додели**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-306">If you know the resource that you want to substitute for the current resource, select or type the name, and then select **Re-assign**.</span></span>

    ![Одређивање заменског ресурса](media/Resource-Management-image51.png)

    <span data-ttu-id="56cc9-308">Алтернативно, следите ове кораке да бисте потражили ресурс:</span><span class="sxs-lookup"><span data-stu-id="56cc9-308">Alternatively, follow these steps to search for a resource:</span></span>

    1. <span data-ttu-id="56cc9-309">Изаберите **Проналажење замене**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-309">Select **Find Substitution**.</span></span>

        ![Тражење заменског ресурса](media/Resource-Management-image52.png)

        <span data-ttu-id="56cc9-311">Помоћник за заказивање приказује листу доступних замена.</span><span class="sxs-lookup"><span data-stu-id="56cc9-311">The Schedule Assistant returns a list of available substitutes.</span></span> <span data-ttu-id="56cc9-312">У помоћнику за заказивање можете додатно филтрирати доступне ресурсе да бисте пронашли одговарајућу замену.</span><span class="sxs-lookup"><span data-stu-id="56cc9-312">In the Schedule Assistant, you can further filter the available resources to find a suitable substitute.</span></span>

        ![Листа доступних замена](media/Resource-Management-image53.png)

    2. <span data-ttu-id="56cc9-314">Да бисте заменили ресурс, одаберите ресурс који желите, а затим изаберите **Замени**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-314">To substitute the resource, select the resource that you want, and then select **Substitute**.</span></span>

        ![Изабран је заменски ресурс](media/Resource-Management-image54.png)

    <span data-ttu-id="56cc9-316">Резервације и доделе замењују се новим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="56cc9-316">The bookings and assignments are substituted with the new resource.</span></span>

    ![Резервације и доделе замењују се новим ресурсом](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a><span data-ttu-id="56cc9-318">Усаглашавање резервација и додела чланова тима</span><span class="sxs-lookup"><span data-stu-id="56cc9-318">Reconcile team member bookings and assignments</span></span>

<span data-ttu-id="56cc9-319">За чланове тима, резервације и доделе су лабаво повезани.</span><span class="sxs-lookup"><span data-stu-id="56cc9-319">For team members, bookings and assignments are loosely coupled.</span></span> <span data-ttu-id="56cc9-320">Другим речима, ресурси могу имати доделе, али не и резервације или могу имати резервације, али не и доделе.</span><span class="sxs-lookup"><span data-stu-id="56cc9-320">In other words, resources can have assignments but no bookings, or they can have bookings but no assignments.</span></span> <span data-ttu-id="56cc9-321">У идеалном случају, резервације и доделе треба да се ускладе тако да ресурси имају потребан капацитет да изврше додељене задатке.</span><span class="sxs-lookup"><span data-stu-id="56cc9-321">Ideally, bookings and assignments should be aligned, so that resources have committed capacity to perform the task assignments.</span></span> <span data-ttu-id="56cc9-322">Међутим, резервације се могу заснивати на доступности, а временски распоред задатака може се мењати током пројекта.</span><span class="sxs-lookup"><span data-stu-id="56cc9-322">However, the bookings might be based on availability, and task timings might change as the project continues.</span></span> <span data-ttu-id="56cc9-323">Стога, лабава повезаност резервација и додела пружа флексибилност.</span><span class="sxs-lookup"><span data-stu-id="56cc9-323">Therefore, the loose coupling of bookings and assignments provides flexibility.</span></span>

<span data-ttu-id="56cc9-324">PSA има картицу **Усаглашеност** која омогућава менаџерима пројеката да усагласе резервације чланова тима и њихове доделе за пројектне тимове.</span><span class="sxs-lookup"><span data-stu-id="56cc9-324">PSA has a **Reconciliation** tab that lets project managers reconcile team members' bookings and their assignments for project teams.</span></span>

![Картица Усаглашеност](media/Resource-Management-image56.png)

<span data-ttu-id="56cc9-326">Картица **Усаглашеност** приказује резервације и доделе све до нивоа доделе појединачног задатка за сваког члана тима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-326">The **Reconciliation** tab shows bookings and assignments down to the level of the individual task assignment for each team member.</span></span> <span data-ttu-id="56cc9-327">Приказује сате у ћелијама који представљају временске периоде, од месеци, па све до дана.</span><span class="sxs-lookup"><span data-stu-id="56cc9-327">It shows hours in cells that represent time periods from months down to days.</span></span>

<span data-ttu-id="56cc9-328">Картица такође приказује укупни нето износ пројекта, заједно са колоном за укупну вредност.</span><span class="sxs-lookup"><span data-stu-id="56cc9-328">The tab also shows an overall net total for the project, together with a total column.</span></span>

<span data-ttu-id="56cc9-329">Картица за сваки ресурс израчунава разлику између резервација члана тима и укупног броја додељених задатака члана тима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-329">For each resource, the tab calculates the difference between the team member's bookings and a rollup of the team member's task assignments.</span></span> <span data-ttu-id="56cc9-330">У идеалном случају, та разлика би требало да буде 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="56cc9-330">Ideally, this difference should be 0 (zero).</span></span> <span data-ttu-id="56cc9-331">Другим речима, не би требало да постоји разлика између резервација и додела.</span><span class="sxs-lookup"><span data-stu-id="56cc9-331">In other words, there should be no difference between bookings and assignments.</span></span> <span data-ttu-id="56cc9-332">Разлике су обојене и засенчене како би се скренула пажња на две појаве:</span><span class="sxs-lookup"><span data-stu-id="56cc9-332">Differences are colored and shaded to draw attention to two conditions:</span></span>

- <span data-ttu-id="56cc9-333">**Недостатак резервација** - Недостатак резервација настаје када ресурс има више додела него резервација.</span><span class="sxs-lookup"><span data-stu-id="56cc9-333">**Booking shortage** – A booking shortage occurs when a resource has more assignments than bookings.</span></span> <span data-ttu-id="56cc9-334">Будући да овај капацитет није резервисан, менаџер пројекта може да коригује ту појаву проширивањем резервација ресурса како би покрио дефицит.</span><span class="sxs-lookup"><span data-stu-id="56cc9-334">Because this capacity hasn't been reserved, a project manager might want to correct this condition by extending the resource's bookings to cover the deficit.</span></span>
- <span data-ttu-id="56cc9-335">**Прекомерне резервације** – Прекомерна резервација настаје када је ресурс резервисан за пројекат, али није додељен задацима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-335">**Excess bookings** – Excess bookings occur when a resource has been booked to the project but hasn't been assigned to tasks.</span></span> <span data-ttu-id="56cc9-336">Та појава може бити прихватљива у случајевима када је ресурс резервисан за пројекат пре доделе задатка.</span><span class="sxs-lookup"><span data-stu-id="56cc9-336">This condition might be acceptable in the cases where the resource was booked to the project before task assignment occurred.</span></span> <span data-ttu-id="56cc9-337">Међутим, у другим случајевима се не планира додељивање ресурса задацима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-337">However, in other cases, the resource isn't planned to be assigned to tasks.</span></span> <span data-ttu-id="56cc9-338">У тим случајевима, менаџер пројекта треба да размотрити отказивање резервација ресурса, тако да се капацитет може користити за други пројекат.</span><span class="sxs-lookup"><span data-stu-id="56cc9-338">In these cases, the project manager should consider canceling the resource's bookings, so that the capacity can be used for another project.</span></span>

<span data-ttu-id="56cc9-339">У неким случајевима, када прегледате време на вишем нивоу од нивоа дана (на пример, на месечном нивоу), можда ћете видети укупну разлику која је нула за неки ресурс (другим речима, резервације = доделе).</span><span class="sxs-lookup"><span data-stu-id="56cc9-339">In some cases, when you view time at a higher level than the day level (for example, the month level), you might see a net difference of zero for a resource (in other words, bookings = assignments).</span></span> <span data-ttu-id="56cc9-340">Међутим, ако прегледате време на нивоу недеље, можда ћете видети да постоје доделе од нула сати и резервације од 40 сати у првој недељи, али доделе од 40 сати и резервације од нула сати у другој недељи.</span><span class="sxs-lookup"><span data-stu-id="56cc9-340">However, if you view time at the week level, you might see that there are assignments of zero hours and bookings of 40 hours in the first week, but assignments of 40 hours and bookings of zero hours in the second week.</span></span> <span data-ttu-id="56cc9-341">Све у свему, резервације и доделе се усклађују, али се разликују од једне до друге недеље.</span><span class="sxs-lookup"><span data-stu-id="56cc9-341">Overall, the bookings and assignments are reconciled, but they differ from one week to the next.</span></span>

<span data-ttu-id="56cc9-342">Када прегледате време на вишим нивоима, ћелије на картици **Усаглашеност** имају индикатор који ће вас обавестити да постоје разлике на нижим нивоима.</span><span class="sxs-lookup"><span data-stu-id="56cc9-342">When you view time at higher levels, cells in the **Reconciliation** tab have an indicator to inform you that there are differences at lower levels.</span></span> <span data-ttu-id="56cc9-343">Дуплим кликом на ћелију можете да је повећате како бисте видели разлику.</span><span class="sxs-lookup"><span data-stu-id="56cc9-343">By double-clicking in a cell, you can zoom in to view the difference.</span></span> <span data-ttu-id="56cc9-344">Затим можете да кликните десним тастером миша да бисте је умањили. Ако одаберете ресурс, а затим користите контролу **Следећа разлика** на траци са алаткама мреже, можете прећи на следећу разлику између резервација и додела за тај ресурс.</span><span class="sxs-lookup"><span data-stu-id="56cc9-344">You can then right-click to zoom out. By selecting a resource and then using the **Next difference** control on the grid toolbar, you can go to the next difference between bookings and assignments for that resource.</span></span> <span data-ttu-id="56cc9-345">Затим можете да користите контролу **Претходна разлика** за повратак.</span><span class="sxs-lookup"><span data-stu-id="56cc9-345">You can then use the **Previous difference** control to go back.</span></span> <span data-ttu-id="56cc9-346">Такође можете искључити индикатор разлике и понашање у навигацији у делу **Подешавања**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-346">You can also turn off the difference indicator and navigation behavior under **Settings**.</span></span>

![Индикатор разлике](media/Resource-Management-image57.png)

<span data-ttu-id="56cc9-348">Ако имате доделе задатака за ресурс, али нема резервација, на страници **Пројекти** на картици **Усаглашеност** изаберите недостатак резервација, а затим **Продужи резервацију**.</span><span class="sxs-lookup"><span data-stu-id="56cc9-348">If you have task assignments for a resource but no bookings, on the **Projects** page, on the **Reconciliation** tab, select the booking shortage, and then select **Extend Booking**.</span></span> <span data-ttu-id="56cc9-349">Појављује се дијалог **Продужење резервације** и приказује резервацију која је потребна да се реши проблем са недостатком ресурса.</span><span class="sxs-lookup"><span data-stu-id="56cc9-349">The **Extend Booking** dialog box appears and shows the booking that is needed to address the resource's shortage.</span></span> <span data-ttu-id="56cc9-350">Такође показује постојеће резервације ресурса за све пројекте или друге ентитете који се могу заказивати.</span><span class="sxs-lookup"><span data-stu-id="56cc9-350">It also shows the resource's existing bookings across all projects or other schedulable entities.</span></span> <span data-ttu-id="56cc9-351">Ако изаберете **У реду** да бисте креирали резервацију за ресурс, без обзира на доступност тог ресурса, можете проузроковати прекомерну резервацију.</span><span class="sxs-lookup"><span data-stu-id="56cc9-351">If you select **OK** to create the booking for the resource, regardless of that resource's availability, you might cause overbooking.</span></span>

![Дијалог Продужење резервације](media/Resource-Management-image58.png)

<span data-ttu-id="56cc9-353">Менаџер пројекта или менаџер ресурса тада може да користи табелу распореда како би управљао било којом ситуацијом у којој је ресурс прекомерно резервисан у односу на његов капацитет.</span><span class="sxs-lookup"><span data-stu-id="56cc9-353">The project manager or resource manager can then use the Schedule Board to manage any situations where a resource is overbooked beyond its capacity.</span></span>
