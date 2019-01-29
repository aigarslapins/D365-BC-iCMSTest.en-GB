---
title: Design Details - Variance | Microsoft Docs
description: Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: e853659d40c03bd58240e1dd12e40a824632de31
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "220073"
---
# <a name="design-details-variance"></a><span data-ttu-id="b2a09-103">Design Details: Variance</span><span class="sxs-lookup"><span data-stu-id="b2a09-103">Design Details: Variance</span></span>
<span data-ttu-id="b2a09-104">Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.</span><span class="sxs-lookup"><span data-stu-id="b2a09-104">Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.</span></span>  

 <span data-ttu-id="b2a09-105">actual cost – standard cost = variance</span><span class="sxs-lookup"><span data-stu-id="b2a09-105">actual cost – standard cost = variance</span></span>  

 <span data-ttu-id="b2a09-106">If the actual cost changes, for example, because you post an item charge on a later date, then the variance is updated accordingly.</span><span class="sxs-lookup"><span data-stu-id="b2a09-106">If the actual cost changes, for example, because you post an item charge on a later date, then the variance is updated accordingly.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="b2a09-107">Revaluation does not affect the variance calculation, because revaluation only changes the inventory value.</span><span class="sxs-lookup"><span data-stu-id="b2a09-107">Revaluation does not affect the variance calculation, because revaluation only changes the inventory value.</span></span>  

## <a name="example"></a><span data-ttu-id="b2a09-108">Example</span><span class="sxs-lookup"><span data-stu-id="b2a09-108">Example</span></span>  
 <span data-ttu-id="b2a09-109">The following example illustrates how variance is calculated for purchased items.</span><span class="sxs-lookup"><span data-stu-id="b2a09-109">The following example illustrates how variance is calculated for purchased items.</span></span> <span data-ttu-id="b2a09-110">It is based on the following scenario:</span><span class="sxs-lookup"><span data-stu-id="b2a09-110">It is based on the following scenario:</span></span>  

1. <span data-ttu-id="b2a09-111">The user purchases an item at LCY 90.00, but the standard cost is LCY 100.00.</span><span class="sxs-lookup"><span data-stu-id="b2a09-111">The user purchases an item at LCY 90.00, but the standard cost is LCY 100.00.</span></span> <span data-ttu-id="b2a09-112">Accordingly, the purchase variance is LCY –10.00.</span><span class="sxs-lookup"><span data-stu-id="b2a09-112">Accordingly, the purchase variance is LCY –10.00.</span></span>  
2. <span data-ttu-id="b2a09-113">LCY 10.00 is credited to the purchase variance account.</span><span class="sxs-lookup"><span data-stu-id="b2a09-113">LCY 10.00 is credited to the purchase variance account.</span></span>  
3. <span data-ttu-id="b2a09-114">The user posts an item charge of LCY 20.00.</span><span class="sxs-lookup"><span data-stu-id="b2a09-114">The user posts an item charge of LCY 20.00.</span></span> <span data-ttu-id="b2a09-115">Accordingly, the actual cost is increased to LCY 110.00, and the value of the purchase variance becomes LCY 10.00.</span><span class="sxs-lookup"><span data-stu-id="b2a09-115">Accordingly, the actual cost is increased to LCY 110.00, and the value of the purchase variance becomes LCY 10.00.</span></span>  
4. <span data-ttu-id="b2a09-116">LCY 20.00 is debited to the purchase variance account.</span><span class="sxs-lookup"><span data-stu-id="b2a09-116">LCY 20.00 is debited to the purchase variance account.</span></span> <span data-ttu-id="b2a09-117">Accordingly, the net purchase variance becomes LCY 10.00.</span><span class="sxs-lookup"><span data-stu-id="b2a09-117">Accordingly, the net purchase variance becomes LCY 10.00.</span></span>  
5. <span data-ttu-id="b2a09-118">The user revalues the item from LCY 100.00 to LCY 70.00.</span><span class="sxs-lookup"><span data-stu-id="b2a09-118">The user revalues the item from LCY 100.00 to LCY 70.00.</span></span> <span data-ttu-id="b2a09-119">This does not affect the variance calculation, only the inventory value.</span><span class="sxs-lookup"><span data-stu-id="b2a09-119">This does not affect the variance calculation, only the inventory value.</span></span>  

   <span data-ttu-id="b2a09-120">The following table shows the resulting value entries.</span><span class="sxs-lookup"><span data-stu-id="b2a09-120">The following table shows the resulting value entries.</span></span>  

   <span data-ttu-id="b2a09-121">![Purchase variance calculation](media/design_details_inventory_costing_11_purchase_variance.png "design_details_inventory_costing_11_purchase_variance")</span><span class="sxs-lookup"><span data-stu-id="b2a09-121">![Purchase variance calculation](media/design_details_inventory_costing_11_purchase_variance.png "design_details_inventory_costing_11_purchase_variance")</span></span>  

## <a name="determining-the-standard-cost"></a><span data-ttu-id="b2a09-122">Determining the Standard Cost</span><span class="sxs-lookup"><span data-stu-id="b2a09-122">Determining the Standard Cost</span></span>  
 <span data-ttu-id="b2a09-123">The standard cost is used when calculating variance and the amount to capitalise.</span><span class="sxs-lookup"><span data-stu-id="b2a09-123">The standard cost is used when calculating variance and the amount to capitalize.</span></span> <span data-ttu-id="b2a09-124">Since the standard cost can be changed over time because of manual update calculation, you need a point in time when the standard cost is fixed for variance calculation.</span><span class="sxs-lookup"><span data-stu-id="b2a09-124">Since the standard cost can be changed over time because of manual update calculation, you need a point in time when the standard cost is fixed for variance calculation.</span></span> <span data-ttu-id="b2a09-125">This point is when the inventory increase is invoiced.</span><span class="sxs-lookup"><span data-stu-id="b2a09-125">This point is when the inventory increase is invoiced.</span></span> <span data-ttu-id="b2a09-126">For produced or assembled items, the point when standard cost is determined is when the cost is adjusted.</span><span class="sxs-lookup"><span data-stu-id="b2a09-126">For produced or assembled items, the point when standard cost is determined is when the cost is adjusted.</span></span>  

 <span data-ttu-id="b2a09-127">The following table shows how different cost shares are calculated for produced and assembled items when you use the Calculate Standard Cost function.</span><span class="sxs-lookup"><span data-stu-id="b2a09-127">The following table shows how different cost shares are calculated for produced and assembled items when you use the Calculate Standard Cost function.</span></span>  

|<span data-ttu-id="b2a09-128">Cost Share</span><span class="sxs-lookup"><span data-stu-id="b2a09-128">Cost Share</span></span>|<span data-ttu-id="b2a09-129">Purchased Item</span><span class="sxs-lookup"><span data-stu-id="b2a09-129">Purchased Item</span></span>|<span data-ttu-id="b2a09-130">Produced/Assembled Item</span><span class="sxs-lookup"><span data-stu-id="b2a09-130">Produced/Assembled Item</span></span>|  
|----------------|--------------------|------------------------------|  
|<span data-ttu-id="b2a09-131">**Standard Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-131">**Standard Cost**</span></span>||<span data-ttu-id="b2a09-132">Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost + Single-Level Cap. Ovhd. Cost + Single-Level Mfg. Ovhd. Cost</span><span class="sxs-lookup"><span data-stu-id="b2a09-132">Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost + Single-Level Cap. Ovhd. Cost + Single-Level Mfg. Ovhd. Cost</span></span>|  
|<span data-ttu-id="b2a09-133">**Single-Level Material Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-133">**Single-Level Material Cost**</span></span>|<span data-ttu-id="b2a09-134">Unit Cost</span><span class="sxs-lookup"><span data-stu-id="b2a09-134">Unit Cost</span></span>|<span data-ttu-id="b2a09-135">![Equation 1](media/design_details_inventory_costing_11_equation_1.png "design_details_inventory_costing_11_equation_1")</span><span class="sxs-lookup"><span data-stu-id="b2a09-135">![Equation 1](media/design_details_inventory_costing_11_equation_1.png "design_details_inventory_costing_11_equation_1")</span></span>|  
|<span data-ttu-id="b2a09-136">**Single-Level Capacity Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-136">**Single-Level Capacity Cost**</span></span>|<span data-ttu-id="b2a09-137">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-137">Not applicable</span></span>|<span data-ttu-id="b2a09-138">![Equation 2](media/design_details_inventory_costing_11_equation_2.png "design_details_inventory_costing_11_equation_2")</span><span class="sxs-lookup"><span data-stu-id="b2a09-138">![Equation 2](media/design_details_inventory_costing_11_equation_2.png "design_details_inventory_costing_11_equation_2")</span></span>|  
|<span data-ttu-id="b2a09-139">**Single-Level Subcontrd. Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-139">**Single-Level Subcontrd. Cost**</span></span>|<span data-ttu-id="b2a09-140">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-140">Not applicable</span></span>|<span data-ttu-id="b2a09-141">![Equation 3](media/design_details_inventory_costing_11_equation_3.png "design_details_inventory_costing_11_equation_3")</span><span class="sxs-lookup"><span data-stu-id="b2a09-141">![Equation 3](media/design_details_inventory_costing_11_equation_3.png "design_details_inventory_costing_11_equation_3")</span></span>|  
|<span data-ttu-id="b2a09-142">**Single-Level Cap. Ovhd Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-142">**Single-Level Cap. Ovhd Cost**</span></span>|<span data-ttu-id="b2a09-143">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-143">Not applicable</span></span>|<span data-ttu-id="b2a09-144">![Equation 4](media/design_details_inventory_costing_11_equation_4.png "design_details_inventory_costing_11_equation_4")</span><span class="sxs-lookup"><span data-stu-id="b2a09-144">![Equation 4](media/design_details_inventory_costing_11_equation_4.png "design_details_inventory_costing_11_equation_4")</span></span>|  
|<span data-ttu-id="b2a09-145">**Single-Level Mfg. Ovhd Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-145">**Single-Level Mfg. Ovhd Cost**</span></span>|<span data-ttu-id="b2a09-146">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-146">Not applicable</span></span>|<span data-ttu-id="b2a09-147">(Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost) \* Indirect Cost % / 100 + Overhead Rate</span><span class="sxs-lookup"><span data-stu-id="b2a09-147">(Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost) \* Indirect Cost % / 100 + Overhead Rate</span></span>|  
|<span data-ttu-id="b2a09-148">**Rolled-up Material Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-148">**Rolled-up Material Cost**</span></span>|<span data-ttu-id="b2a09-149">Unit Cost</span><span class="sxs-lookup"><span data-stu-id="b2a09-149">Unit Cost</span></span>|<span data-ttu-id="b2a09-150">![Equation 5](media/design_details_inventory_costing_11_equation_5.png "design_details_inventory_costing_11_equation_5")</span><span class="sxs-lookup"><span data-stu-id="b2a09-150">![Equation 5](media/design_details_inventory_costing_11_equation_5.png "design_details_inventory_costing_11_equation_5")</span></span>|  
|<span data-ttu-id="b2a09-151">**Rolled-up Capacity Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-151">**Rolled-up Capacity Cost**</span></span>|<span data-ttu-id="b2a09-152">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-152">Not applicable</span></span>|<span data-ttu-id="b2a09-153">![Equation 6](media/design_details_inventory_costing_11_equation_6.png "design_details_inventory_costing_11_equation_6")</span><span class="sxs-lookup"><span data-stu-id="b2a09-153">![Equation 6](media/design_details_inventory_costing_11_equation_6.png "design_details_inventory_costing_11_equation_6")</span></span>|  
|<span data-ttu-id="b2a09-154">**Rolled-Up Subcontracted Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-154">**Rolled-Up Subcontracted Cost**</span></span>|<span data-ttu-id="b2a09-155">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-155">Not applicable</span></span>|<span data-ttu-id="b2a09-156">![Equation 7](media/design_details_inventory_costing_11_equation_7.png "design_details_inventory_costing_11_equation_7")</span><span class="sxs-lookup"><span data-stu-id="b2a09-156">![Equation 7](media/design_details_inventory_costing_11_equation_7.png "design_details_inventory_costing_11_equation_7")</span></span>|  
|<span data-ttu-id="b2a09-157">**Rolled-up Capacity Ovhd. Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-157">**Rolled-up Capacity Ovhd. Cost**</span></span>|<span data-ttu-id="b2a09-158">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-158">Not applicable</span></span>|<span data-ttu-id="b2a09-159">![Equation 8](media/design_details_inventory_costing_11_equation_8.png "design_details_inventory_costing_11_equation_8")</span><span class="sxs-lookup"><span data-stu-id="b2a09-159">![Equation 8](media/design_details_inventory_costing_11_equation_8.png "design_details_inventory_costing_11_equation_8")</span></span>|  
|<span data-ttu-id="b2a09-160">**Rolled-up Mfg. Ovhd. Cost**</span><span class="sxs-lookup"><span data-stu-id="b2a09-160">**Rolled-up Mfg. Ovhd. Cost**</span></span>|<span data-ttu-id="b2a09-161">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b2a09-161">Not applicable</span></span>|<span data-ttu-id="b2a09-162">![Equation 9](media/design_details_inventory_costing_11_equation_9.png "design_details_inventory_costing_11_equation_9")</span><span class="sxs-lookup"><span data-stu-id="b2a09-162">![Equation 9](media/design_details_inventory_costing_11_equation_9.png "design_details_inventory_costing_11_equation_9")</span></span>|  

## <a name="see-also"></a><span data-ttu-id="b2a09-163">See Also</span><span class="sxs-lookup"><span data-stu-id="b2a09-163">See Also</span></span>  
 <span data-ttu-id="b2a09-164">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="b2a09-164">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="b2a09-165">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span><span class="sxs-lookup"><span data-stu-id="b2a09-165">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span></span>  
 [<span data-ttu-id="b2a09-166">Finance</span><span class="sxs-lookup"><span data-stu-id="b2a09-166">Finance</span></span>](finance.md)  
 <span data-ttu-id="b2a09-167">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b2a09-167">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>