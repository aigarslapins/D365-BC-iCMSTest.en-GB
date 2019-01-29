---
title: Set Up Opportunity Sales Cycles and Cycle Stages| Microsoft Docs
description: Describes how to define sales stages, from initial contact to closing, to create a sales cycle and assign it to opportunities in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
ms.openlocfilehash: 319a59c865b7883cf7de5c35d9ebce5c30de0f76
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "270122"
---
# <a name="set-up-opportunity-sales-cycles-and-cycle-stages"></a><span data-ttu-id="d2a8f-103">Set Up Opportunity Sales Cycles and Cycle Stages</span><span class="sxs-lookup"><span data-stu-id="d2a8f-103">Set Up Opportunity Sales Cycles and Cycle Stages</span></span>
<span data-ttu-id="d2a8f-104">Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-104">Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages.</span></span> <span data-ttu-id="d2a8f-105">A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-105">A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale.</span></span> <span data-ttu-id="d2a8f-106">Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-106">Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage.</span></span> <span data-ttu-id="d2a8f-107">You can also specify whether a stage can be skipped.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-107">You can also specify whether a stage can be skipped.</span></span> <span data-ttu-id="d2a8f-108">You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-108">You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.</span></span>

<span data-ttu-id="d2a8f-109">Implementing opportunity sales cycles involves setting up the sales cycle, defining the different stages of the cycle, and then assigning the cycle to opportunities.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-109">Implementing opportunity sales cycles involves setting up the sales cycle, defining the different stages of the cycle, and then assigning the cycle to opportunities.</span></span> <span data-ttu-id="d2a8f-110">Assigning the relevant activity or tasks to the opportunity may also be part of setting up a sales cycle.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-110">Assigning the relevant activity or tasks to the opportunity may also be part of setting up a sales cycle.</span></span>

<span data-ttu-id="d2a8f-111">This topic also describes how to set up tasks and activities, and how to assign tasks to activities.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-111">This topic also describes how to set up tasks and activities, and how to assign tasks to activities.</span></span> <span data-ttu-id="d2a8f-112">For more information, see the "To set up activities with tasks" section.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-112">For more information, see the "To set up activities with tasks" section.</span></span>

## <a name="to-set-up-opportunity-sales-cycle-codes"></a><span data-ttu-id="d2a8f-113">To set up opportunity sales cycle codes</span><span class="sxs-lookup"><span data-stu-id="d2a8f-113">To set up opportunity sales cycle codes</span></span>
1. <span data-ttu-id="d2a8f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Cycles**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Cycles**, and then choose the related link.</span></span> <span data-ttu-id="d2a8f-115">The **Sales Cycles** page opens, and lists all the existing sales cycles.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-115">The **Sales Cycles** page opens, and lists all the existing sales cycles.</span></span>
2. <span data-ttu-id="d2a8f-116">Choose the **New** action, and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-116">Choose the **New** action, and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="d2a8f-117">Repeat these steps to set up as many sales cycles as you want.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-117">Repeat these steps to set up as many sales cycles as you want.</span></span> <span data-ttu-id="d2a8f-118">After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-118">After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.</span></span>

## <a name="to-define-opportunity-sales-cycle-stages"></a><span data-ttu-id="d2a8f-119">To define opportunity sales cycle stages</span><span class="sxs-lookup"><span data-stu-id="d2a8f-119">To define opportunity sales cycle stages</span></span>
1. <span data-ttu-id="d2a8f-120">On the **Sales Cycles** page, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-120">On the **Sales Cycles** page, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action.</span></span> <span data-ttu-id="d2a8f-121">The **Sales Cycle Stages** page opens.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-121">The **Sales Cycle Stages** page opens.</span></span>
2. <span data-ttu-id="d2a8f-122">Choose the **New** action to enter a new stage in the sales cycle.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-122">Choose the **New** action to enter a new stage in the sales cycle.</span></span>

<span data-ttu-id="d2a8f-123">Repeat these steps to set up as many stages as you want within the sales cycle.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-123">Repeat these steps to set up as many stages as you want within the sales cycle.</span></span>

## <a name="to-assign-stage-cycles-to-opportunities"></a><span data-ttu-id="d2a8f-124">To assign stage cycles to opportunities</span><span class="sxs-lookup"><span data-stu-id="d2a8f-124">To assign stage cycles to opportunities</span></span>
<span data-ttu-id="d2a8f-125">After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-125">After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field.</span></span> <span data-ttu-id="d2a8f-126">For more information, see [Create Sales Opportunities](marketing-how-create-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="d2a8f-126">For more information, see [Create Sales Opportunities](marketing-how-create-opportunities.md).</span></span>

## <a name="to-set-up-activities-with-tasks"></a><span data-ttu-id="d2a8f-127">To set up activities with tasks</span><span class="sxs-lookup"><span data-stu-id="d2a8f-127">To set up activities with tasks</span></span>
<span data-ttu-id="d2a8f-128">You can combine multiple task, for example tasks that each represent a step, in activities.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-128">You can combine multiple task, for example tasks that each represent a step, in activities.</span></span> <span data-ttu-id="d2a8f-129">Activity tasks are related to each other by a date formula.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-129">Activity tasks are related to each other by a date formula.</span></span> <span data-ttu-id="d2a8f-130">You can assign activities to opportunities, salespeople, or contacts.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-130">You can assign activities to opportunities, salespeople, or contacts.</span></span>

1. <span data-ttu-id="d2a8f-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Activities**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Activities**, and then choose the related link.</span></span>
2. <span data-ttu-id="d2a8f-132">Choose the **New** action, and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-132">Choose the **New** action, and fill in the fields as necessary.</span></span>
3. <span data-ttu-id="d2a8f-133">On the **Lines** FastTab, fill in the fields as necessary to define one or more tasks in the activity.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-133">On the **Lines** FastTab, fill in the fields as necessary to define one or more tasks in the activity.</span></span>

## <a name="to-assign-tasks-or-activities-of-tasks-to-opportunities"></a><span data-ttu-id="d2a8f-134">To assign tasks or activities of tasks to opportunities</span><span class="sxs-lookup"><span data-stu-id="d2a8f-134">To assign tasks or activities of tasks to opportunities</span></span>
<span data-ttu-id="d2a8f-135">When you have set up a task, you can assign it to a sales opportunity and thereby assign the activity that the task belongs to.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-135">When you have set up a task, you can assign it to a sales opportunity and thereby assign the activity that the task belongs to.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d2a8f-136">This procedure describes how to assign activity tasks to opportunities.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-136">This procedure describes how to assign activity tasks to opportunities.</span></span> <span data-ttu-id="d2a8f-137">the steps are similar when you assign tasks to salespeople and contacts.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-137">the steps are similar when you assign tasks to salespeople and contacts.</span></span>

1. <span data-ttu-id="d2a8f-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Opportunities**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Opportunities**, and then choose the related link.</span></span>
2. <span data-ttu-id="d2a8f-139">Select an opportunity, and then choose the **Tasks** action.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-139">Select an opportunity, and then choose the **Tasks** action.</span></span>
3. <span data-ttu-id="d2a8f-140">On the **Task List** page, choose the **Create Task** action.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-140">On the **Task List** page, choose the **Create Task** action.</span></span>
4.  <span data-ttu-id="d2a8f-141">The **Create Task** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-141">The **Create Task** page, fill in the fields as necessary.</span></span>

    <span data-ttu-id="d2a8f-142">Notice in the **Opportunity** field, that it is automatically assigned to the opportunity in question.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-142">Notice in the **Opportunity** field, that it is automatically assigned to the opportunity in question.</span></span>
5. <span data-ttu-id="d2a8f-143">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-143">Choose the **OK** button.</span></span>
6. <span data-ttu-id="d2a8f-144">On the **Task List** page, select the new task, and then choose the **Assign Activities** action.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-144">On the **Task List** page, select the new task, and then choose the **Assign Activities** action.</span></span>
7. <span data-ttu-id="d2a8f-145">On the **Assign Activity** page, fill in the fields as necessary, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-145">On the **Assign Activity** page, fill in the fields as necessary, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="d2a8f-146">See Also</span><span class="sxs-lookup"><span data-stu-id="d2a8f-146">See Also</span></span>
[<span data-ttu-id="d2a8f-147">Processing Sales Opportunities</span><span class="sxs-lookup"><span data-stu-id="d2a8f-147">Processing Sales Opportunities</span></span>](marketing-processing-sales-opportunities.md)  
[<span data-ttu-id="d2a8f-148">Sales</span><span class="sxs-lookup"><span data-stu-id="d2a8f-148">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="d2a8f-149">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d2a8f-149">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>