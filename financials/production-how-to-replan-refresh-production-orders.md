---
title: How to Replan or Refresh Production Orders Directly| Microsoft Docs
description: The production order lines contain the items that are to be produced in the production order.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/06/2017
ms.author: sgroespe
ms.openlocfilehash: 1750aa3c51731a7f770f278e2f87feec2f938496
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "242347"
---
# <a name="replan-or-refresh-production-orders-directly"></a><span data-ttu-id="8ac8f-103">Replan or Refresh Production Orders Directly</span><span class="sxs-lookup"><span data-stu-id="8ac8f-103">Replan or Refresh Production Orders Directly</span></span>
<span data-ttu-id="8ac8f-104">The **Replan** function on production orders is typically used after you have added or changed components that constitute underlying production orders.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-104">The **Replan** function on production orders is typically used after you have added or changed components that constitute underlying production orders.</span></span> <span data-ttu-id="8ac8f-105">The function calculates changes made to components and routings lines, and it includes items on lower production BOM levels for which it may generate new production orders.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-105">The function calculates changes made to components and routings lines, and it includes items on lower production BOM levels for which it may generate new production orders.</span></span>  

<span data-ttu-id="8ac8f-106">Based on the changes you have made to the components and routing lines, the Replan function calculates and plans for any new demand for the production order.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-106">Based on the changes you have made to the components and routing lines, the Replan function calculates and plans for any new demand for the production order.</span></span>  

<span data-ttu-id="8ac8f-107">The **Refresh** function on production orders is typically used after you have done one of the following:</span><span class="sxs-lookup"><span data-stu-id="8ac8f-107">The **Refresh** function on production orders is typically used after you have done one of the following:</span></span>

- <span data-ttu-id="8ac8f-108">Created a production order header manually to calculate and create line data for the first time.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-108">Created a production order header manually to calculate and create line data for the first time.</span></span>
- <span data-ttu-id="8ac8f-109">Made changes to the production order header to recalculate all the line data.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-109">Made changes to the production order header to recalculate all the line data.</span></span>

<span data-ttu-id="8ac8f-110">The Refresh function calculates changes made to a production order header and does not involve production BOM levels.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-110">The Refresh function calculates changes made to a production order header and does not involve production BOM levels.</span></span> <span data-ttu-id="8ac8f-111">The function calculates and initiates the values of the component lines and routing lines based on the master data defined in the assigned production BOM and routing, according to the order quantity and due date on the production order’s header.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-111">The function calculates and initiates the values of the component lines and routing lines based on the master data defined in the assigned production BOM and routing, according to the order quantity and due date on the production order’s header.</span></span>

<span data-ttu-id="8ac8f-112">You can either insert the production order lines manually or use the function that calculates the production order lines from the header.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-112">You can either insert the production order lines manually or use the function that calculates the production order lines from the header.</span></span>  

> [!NOTE]
>  <span data-ttu-id="8ac8f-113">If you use the Refresh function to recalculate production order lines, the old production order lines are deleted and new lines are calculated.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-113">If you use the Refresh function to recalculate production order lines, the old production order lines are deleted and new lines are calculated.</span></span>  

## <a name="to-replan-a-production-order"></a><span data-ttu-id="8ac8f-114">To replan a production order</span><span class="sxs-lookup"><span data-stu-id="8ac8f-114">To replan a production order</span></span>  
1.  <span data-ttu-id="8ac8f-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8ac8f-116">Open the production order you want to replan.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-116">Open the production order you want to replan.</span></span>  
3.  <span data-ttu-id="8ac8f-117">On the **Lines** FastTab, choose the **Lines** action, and then choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-117">On the **Lines** FastTab, choose the **Lines** action, and then choose the **Components** action.</span></span>  
4.  <span data-ttu-id="8ac8f-118">Add a component, which is a produced item or subassembly.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-118">Add a component, which is a produced item or subassembly.</span></span>  
5.  <span data-ttu-id="8ac8f-119">From the production order, choose the **Replan** action.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-119">From the production order, choose the **Replan** action.</span></span>  

    <span data-ttu-id="8ac8f-120">In the **Replan Production Order** window, proceed to define how and what to replan.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-120">In the **Replan Production Order** window, proceed to define how and what to replan.</span></span>  
6.  <span data-ttu-id="8ac8f-121">In the **Scheduling Direction** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-121">In the **Scheduling Direction** field, select one of the following options.</span></span>  

    |<span data-ttu-id="8ac8f-122">Option</span><span class="sxs-lookup"><span data-stu-id="8ac8f-122">Option</span></span>|<span data-ttu-id="8ac8f-123">Description</span><span class="sxs-lookup"><span data-stu-id="8ac8f-123">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="8ac8f-124">**Back**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-124">**Back**</span></span>|<span data-ttu-id="8ac8f-125">Calculates the operation sequence backwards from the earliest possible ending date, defined by due date and/or other scheduled orders, to the latest possible starting date.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-125">Calculates the operation sequence backwards from the earliest possible ending date, defined by due date and/or other scheduled orders, to the latest possible starting date.</span></span> <span data-ttu-id="8ac8f-126">**Note:**  This default option is relevant in the majority of situations.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-126">**Note:**  This default option is relevant in the majority of situations.</span></span>|  
    |<span data-ttu-id="8ac8f-127">**Forward**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-127">**Forward**</span></span>|<span data-ttu-id="8ac8f-128">Calculates the operation sequence forward from the earliest latest possible starting date, defined by due date and/or other scheduled orders, to the earliest possible ending date.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-128">Calculates the operation sequence forward from the earliest latest possible starting date, defined by due date and/or other scheduled orders, to the earliest possible ending date.</span></span> <span data-ttu-id="8ac8f-129">**Note:**  This option is only relevant for expedite orders.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-129">**Note:**  This option is only relevant for expedite orders.</span></span>|  

7.  <span data-ttu-id="8ac8f-130">In the **Plan** field, select whether to calculate production requirements for produced items on the production BOM, as follows.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-130">In the **Plan** field, select whether to calculate production requirements for produced items on the production BOM, as follows.</span></span>  

    |<span data-ttu-id="8ac8f-131">Option</span><span class="sxs-lookup"><span data-stu-id="8ac8f-131">Option</span></span>|<span data-ttu-id="8ac8f-132">Description</span><span class="sxs-lookup"><span data-stu-id="8ac8f-132">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="8ac8f-133">**No Levels**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-133">**No Levels**</span></span>|<span data-ttu-id="8ac8f-134">Do not consider lower level production.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-134">Do not consider lower level production.</span></span> <span data-ttu-id="8ac8f-135">This only updates the item’s schedule, like refresh.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-135">This only updates the item’s schedule, like refresh.</span></span>|  
    |<span data-ttu-id="8ac8f-136">**One Level**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-136">**One Level**</span></span>|<span data-ttu-id="8ac8f-137">Plan for first-level production demand.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-137">Plan for first-level production demand.</span></span> <span data-ttu-id="8ac8f-138">First-level production orders may be created.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-138">First-level production orders may be created.</span></span>|  
    |<span data-ttu-id="8ac8f-139">**All Levels**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-139">**All Levels**</span></span>|<span data-ttu-id="8ac8f-140">Plan for all-level production demand.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-140">Plan for all-level production demand.</span></span> <span data-ttu-id="8ac8f-141">All-level production orders may be created.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-141">All-level production orders may be created.</span></span>|  

8.  <span data-ttu-id="8ac8f-142">Select **One Level**, and choose the **OK** button to replan the production order, and calculate and create a new underlying production order for the introduced subassembly, if it is not fully available.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-142">Select **One Level**, and choose the **OK** button to replan the production order, and calculate and create a new underlying production order for the introduced subassembly, if it is not fully available.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8ac8f-143">Changes implemented with the **Replan** function are very likely to change the capacity need of the production order and you may therefore have to reschedule operations afterwards.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-143">Changes implemented with the **Replan** function are very likely to change the capacity need of the production order and you may therefore have to reschedule operations afterwards.</span></span>  

## <a name="to-refresh-a-production-order"></a><span data-ttu-id="8ac8f-144">To refresh a production order</span><span class="sxs-lookup"><span data-stu-id="8ac8f-144">To refresh a production order</span></span>  
<span data-ttu-id="8ac8f-145">If you have amended production order lines, components, or routing lines, you must also refresh the information on the production order.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-145">If you have amended production order lines, components, or routing lines, you must also refresh the information on the production order.</span></span> <span data-ttu-id="8ac8f-146">In the following procedure, the components are calculated for a firm planned production order.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-146">In the following procedure, the components are calculated for a firm planned production order.</span></span> <span data-ttu-id="8ac8f-147">The steps are similar for routing lines.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-147">The steps are similar for routing lines.</span></span>

1. <span data-ttu-id="8ac8f-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8ac8f-149">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-149">Choose the **New** action.</span></span> <span data-ttu-id="8ac8f-150">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="8ac8f-150">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span></span>  
3. <span data-ttu-id="8ac8f-151">Choose the **Refresh** action.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-151">Choose the **Refresh** action.</span></span>
4. <span data-ttu-id="8ac8f-152">In the **Refresh Production Order** window, select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="8ac8f-152">In the **Refresh Production Order** window, select one of the following options:</span></span>


   |          <span data-ttu-id="8ac8f-153">Option</span><span class="sxs-lookup"><span data-stu-id="8ac8f-153">Option</span></span>          |        <span data-ttu-id="8ac8f-154">Description</span><span class="sxs-lookup"><span data-stu-id="8ac8f-154">Description</span></span>         |
   |--------------------------|----------------------------|
   | <span data-ttu-id="8ac8f-155">**Scheduling Direction**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-155">**Scheduling Direction**</span></span> |        <span data-ttu-id="8ac8f-156">**Forward**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-156">**Forward**</span></span>         |
   |                          |        <span data-ttu-id="8ac8f-157">**Backward**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-157">**Backward**</span></span>        |
   |      <span data-ttu-id="8ac8f-158">**Calculate**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-158">**Calculate**</span></span>       |         <span data-ttu-id="8ac8f-159">**Lines**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-159">**Lines**</span></span>          |
   |                          |        <span data-ttu-id="8ac8f-160">**Routings**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-160">**Routings**</span></span>        |
   |                          |     <span data-ttu-id="8ac8f-161">**Component Need**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-161">**Component Need**</span></span>     |
   |      <span data-ttu-id="8ac8f-162">**Warehouse**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-162">**Warehouse**</span></span>       | <span data-ttu-id="8ac8f-163">**Create Inbound Request**</span><span class="sxs-lookup"><span data-stu-id="8ac8f-163">**Create Inbound Request**</span></span> |


5. <span data-ttu-id="8ac8f-164">Choose the **OK** button to confirm your selection.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-164">Choose the **OK** button to confirm your selection.</span></span> <span data-ttu-id="8ac8f-165">Now the production order lines are calculated.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-165">Now the production order lines are calculated.</span></span>

> [!NOTE]  
>  <span data-ttu-id="8ac8f-166">Calculating production order components deletes previous changes in the components.</span><span class="sxs-lookup"><span data-stu-id="8ac8f-166">Calculating production order components deletes previous changes in the components.</span></span>

## <a name="see-also"></a><span data-ttu-id="8ac8f-167">See Also</span><span class="sxs-lookup"><span data-stu-id="8ac8f-167">See Also</span></span>  
[<span data-ttu-id="8ac8f-168">Planning</span><span class="sxs-lookup"><span data-stu-id="8ac8f-168">Planning</span></span>](production-planning.md)  
[<span data-ttu-id="8ac8f-169">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="8ac8f-169">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="8ac8f-170">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="8ac8f-170">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="8ac8f-171">Inventory</span><span class="sxs-lookup"><span data-stu-id="8ac8f-171">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="8ac8f-172">Purchasing</span><span class="sxs-lookup"><span data-stu-id="8ac8f-172">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="8ac8f-173">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="8ac8f-173">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="8ac8f-174">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="8ac8f-174">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="8ac8f-175">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8ac8f-175">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
