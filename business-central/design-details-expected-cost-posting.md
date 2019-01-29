---
title: Design Details - Expected Cost Posting | Microsoft Docs
description: Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: ae88a455552c7194422d07e6e666bd81b7eab101
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "254210"
---
# <a name="design-details-expected-cost-posting"></a><span data-ttu-id="fcb74-103">Design Details: Expected Cost Posting</span><span class="sxs-lookup"><span data-stu-id="fcb74-103">Design Details: Expected Cost Posting</span></span>
<span data-ttu-id="fcb74-104">Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.</span><span class="sxs-lookup"><span data-stu-id="fcb74-104">Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.</span></span>  

 <span data-ttu-id="fcb74-105">You can post expected cost to inventory and to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="fcb74-105">You can post expected cost to inventory and to the general ledger.</span></span> <span data-ttu-id="fcb74-106">When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost.</span><span class="sxs-lookup"><span data-stu-id="fcb74-106">When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost.</span></span> <span data-ttu-id="fcb74-107">This expected cost affects the inventory value, but is not posted to the general ledger unless you set up the system up to do so.</span><span class="sxs-lookup"><span data-stu-id="fcb74-107">This expected cost affects the inventory value, but is not posted to the general ledger unless you set up the system up to do so.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fcb74-108">Expected costs are only managed for item transactions.</span><span class="sxs-lookup"><span data-stu-id="fcb74-108">Expected costs are only managed for item transactions.</span></span> <span data-ttu-id="fcb74-109">Expected costs are not for immaterial transaction nature codes, such as capacity and item charges.</span><span class="sxs-lookup"><span data-stu-id="fcb74-109">Expected costs are not for immaterial transaction types, such as capacity and item charges.</span></span>  

 <span data-ttu-id="fcb74-110">If only the quantity part of an inventory increase has been posted, then the inventory value in the general ledger does not change unless you have selected the **Expected Cost Posting to G/L** check box on the **Inventory Setup** page.</span><span class="sxs-lookup"><span data-stu-id="fcb74-110">If only the quantity part of an inventory increase has been posted, then the inventory value in the general ledger does not change unless you have selected the **Expected Cost Posting to G/L** check box on the **Inventory Setup** page.</span></span> <span data-ttu-id="fcb74-111">In that case, the expected cost is posted to interim accounts at the time of receipt.</span><span class="sxs-lookup"><span data-stu-id="fcb74-111">In that case, the expected cost is posted to interim accounts at the time of receipt.</span></span> <span data-ttu-id="fcb74-112">After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the inventory account.</span><span class="sxs-lookup"><span data-stu-id="fcb74-112">After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the inventory account.</span></span>  

 <span data-ttu-id="fcb74-113">To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.</span><span class="sxs-lookup"><span data-stu-id="fcb74-113">To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.</span></span>  

## <a name="example"></a><span data-ttu-id="fcb74-114">Example</span><span class="sxs-lookup"><span data-stu-id="fcb74-114">Example</span></span>  
 <span data-ttu-id="fcb74-115">The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G/L** check box are selected on the **Inventory Setup** page.</span><span class="sxs-lookup"><span data-stu-id="fcb74-115">The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G/L** check box are selected on the **Inventory Setup** page.</span></span>  

 <span data-ttu-id="fcb74-116">You post a purchase order as received.</span><span class="sxs-lookup"><span data-stu-id="fcb74-116">You post a purchase order as received.</span></span> <span data-ttu-id="fcb74-117">The expected cost is LCY 95.00.</span><span class="sxs-lookup"><span data-stu-id="fcb74-117">The expected cost is LCY 95.00.</span></span>  

 <span data-ttu-id="fcb74-118">**Value Entries**</span><span class="sxs-lookup"><span data-stu-id="fcb74-118">**Value Entries**</span></span>  

|<span data-ttu-id="fcb74-119">Posting Date</span><span class="sxs-lookup"><span data-stu-id="fcb74-119">Posting Date</span></span>|<span data-ttu-id="fcb74-120">Entry Type</span><span class="sxs-lookup"><span data-stu-id="fcb74-120">Entry Type</span></span>|<span data-ttu-id="fcb74-121">Cost Amount (Expected)</span><span class="sxs-lookup"><span data-stu-id="fcb74-121">Cost Amount (Expected)</span></span>|<span data-ttu-id="fcb74-122">Expected Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="fcb74-122">Expected Cost Posted to G/L</span></span>|<span data-ttu-id="fcb74-123">Expected Cost</span><span class="sxs-lookup"><span data-stu-id="fcb74-123">Expected Cost</span></span>|<span data-ttu-id="fcb74-124">Item Ledger Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-124">Item Ledger Entry No.</span></span>|<span data-ttu-id="fcb74-125">Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-125">Entry No.</span></span>|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="fcb74-126">01-01-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-126">01-01-20</span></span>|<span data-ttu-id="fcb74-127">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="fcb74-127">Direct Cost</span></span>|<span data-ttu-id="fcb74-128">95.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-128">95.00</span></span>|<span data-ttu-id="fcb74-129">95.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-129">95.00</span></span>|<span data-ttu-id="fcb74-130">Yes</span><span class="sxs-lookup"><span data-stu-id="fcb74-130">Yes</span></span>|<span data-ttu-id="fcb74-131">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-131">1</span></span>|<span data-ttu-id="fcb74-132">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-132">1</span></span>|  

 <span data-ttu-id="fcb74-133">**Relation Entries in the G/L – Item Ledger Relation Table**</span><span class="sxs-lookup"><span data-stu-id="fcb74-133">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="fcb74-134">G/L Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-134">G/L Entry No.</span></span>|<span data-ttu-id="fcb74-135">Value Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-135">Value Entry No.</span></span>|<span data-ttu-id="fcb74-136">G/L Register No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-136">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="fcb74-137">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-137">1</span></span>|<span data-ttu-id="fcb74-138">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-138">1</span></span>|<span data-ttu-id="fcb74-139">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-139">1</span></span>|  
|<span data-ttu-id="fcb74-140">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-140">2</span></span>|<span data-ttu-id="fcb74-141">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-141">1</span></span>|<span data-ttu-id="fcb74-142">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-142">1</span></span>|  

 <span data-ttu-id="fcb74-143">**General Ledger Entries**</span><span class="sxs-lookup"><span data-stu-id="fcb74-143">**General Ledger Entries**</span></span>  

|<span data-ttu-id="fcb74-144">Posting Date</span><span class="sxs-lookup"><span data-stu-id="fcb74-144">Posting Date</span></span>|<span data-ttu-id="fcb74-145">G/L Account</span><span class="sxs-lookup"><span data-stu-id="fcb74-145">G/L Account</span></span>|<span data-ttu-id="fcb74-146">Account No. (En-US Demo)</span><span class="sxs-lookup"><span data-stu-id="fcb74-146">Account No. (En-US Demo)</span></span>|<span data-ttu-id="fcb74-147">Amount</span><span class="sxs-lookup"><span data-stu-id="fcb74-147">Amount</span></span>|<span data-ttu-id="fcb74-148">Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-148">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="fcb74-149">01-01-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-149">01-01-20</span></span>|<span data-ttu-id="fcb74-150">Inventory Accrual Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="fcb74-150">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="fcb74-151">5530</span><span class="sxs-lookup"><span data-stu-id="fcb74-151">5530</span></span>|<span data-ttu-id="fcb74-152">-95.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-152">-95.00</span></span>|<span data-ttu-id="fcb74-153">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-153">2</span></span>|  
|<span data-ttu-id="fcb74-154">01-01-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-154">01-01-20</span></span>|<span data-ttu-id="fcb74-155">Inventory Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="fcb74-155">Inventory Account (Interim)</span></span>|<span data-ttu-id="fcb74-156">2131</span><span class="sxs-lookup"><span data-stu-id="fcb74-156">2131</span></span>|<span data-ttu-id="fcb74-157">95.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-157">95.00</span></span>|<span data-ttu-id="fcb74-158">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-158">1</span></span>|  

 <span data-ttu-id="fcb74-159">At a later date, you post the purchase order as invoiced.</span><span class="sxs-lookup"><span data-stu-id="fcb74-159">At a later date, you post the purchase order as invoiced.</span></span> <span data-ttu-id="fcb74-160">The invoiced cost is LCY 100.00.</span><span class="sxs-lookup"><span data-stu-id="fcb74-160">The invoiced cost is LCY 100.00.</span></span>  

 <span data-ttu-id="fcb74-161">**Value Entries**</span><span class="sxs-lookup"><span data-stu-id="fcb74-161">**Value Entries**</span></span>  

|<span data-ttu-id="fcb74-162">Posting Date</span><span class="sxs-lookup"><span data-stu-id="fcb74-162">Posting Date</span></span>|<span data-ttu-id="fcb74-163">Cost Amount (Actual)</span><span class="sxs-lookup"><span data-stu-id="fcb74-163">Cost Amount (Actual)</span></span>|<span data-ttu-id="fcb74-164">Cost Amount (Expected)</span><span class="sxs-lookup"><span data-stu-id="fcb74-164">Cost Amount (Expected)</span></span>|<span data-ttu-id="fcb74-165">Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="fcb74-165">Cost Posted to G/L</span></span>|<span data-ttu-id="fcb74-166">Expected Cost</span><span class="sxs-lookup"><span data-stu-id="fcb74-166">Expected Cost</span></span>|<span data-ttu-id="fcb74-167">Item Ledger Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-167">Item Ledger Entry No.</span></span>|<span data-ttu-id="fcb74-168">Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-168">Entry No.</span></span>|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="fcb74-169">01-15-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-169">01-15-20</span></span>|<span data-ttu-id="fcb74-170">100.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-170">100.00</span></span>|<span data-ttu-id="fcb74-171">-95.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-171">-95.00</span></span>|<span data-ttu-id="fcb74-172">100.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-172">100.00</span></span>|<span data-ttu-id="fcb74-173">No</span><span class="sxs-lookup"><span data-stu-id="fcb74-173">No</span></span>|<span data-ttu-id="fcb74-174">1</span><span class="sxs-lookup"><span data-stu-id="fcb74-174">1</span></span>|<span data-ttu-id="fcb74-175">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-175">2</span></span>|  

 <span data-ttu-id="fcb74-176">**Relation Entries in the G/L – Item Ledger Relation Table**</span><span class="sxs-lookup"><span data-stu-id="fcb74-176">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="fcb74-177">G/L Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-177">G/L Entry No.</span></span>|<span data-ttu-id="fcb74-178">Value Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-178">Value Entry No.</span></span>|<span data-ttu-id="fcb74-179">G/L Register No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-179">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="fcb74-180">3</span><span class="sxs-lookup"><span data-stu-id="fcb74-180">3</span></span>|<span data-ttu-id="fcb74-181">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-181">2</span></span>|<span data-ttu-id="fcb74-182">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-182">2</span></span>|  
|<span data-ttu-id="fcb74-183">4</span><span class="sxs-lookup"><span data-stu-id="fcb74-183">4</span></span>|<span data-ttu-id="fcb74-184">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-184">2</span></span>|<span data-ttu-id="fcb74-185">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-185">2</span></span>|  
|<span data-ttu-id="fcb74-186">5</span><span class="sxs-lookup"><span data-stu-id="fcb74-186">5</span></span>|<span data-ttu-id="fcb74-187">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-187">2</span></span>|<span data-ttu-id="fcb74-188">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-188">2</span></span>|  
|<span data-ttu-id="fcb74-189">6</span><span class="sxs-lookup"><span data-stu-id="fcb74-189">6</span></span>|<span data-ttu-id="fcb74-190">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-190">2</span></span>|<span data-ttu-id="fcb74-191">2</span><span class="sxs-lookup"><span data-stu-id="fcb74-191">2</span></span>|  

 <span data-ttu-id="fcb74-192">**General Ledger Entries**</span><span class="sxs-lookup"><span data-stu-id="fcb74-192">**General Ledger Entries**</span></span>  

|<span data-ttu-id="fcb74-193">Posting Date</span><span class="sxs-lookup"><span data-stu-id="fcb74-193">Posting Date</span></span>|<span data-ttu-id="fcb74-194">G/L Account</span><span class="sxs-lookup"><span data-stu-id="fcb74-194">G/L Account</span></span>|<span data-ttu-id="fcb74-195">Account No. (En-US Demo)</span><span class="sxs-lookup"><span data-stu-id="fcb74-195">Account No. (En-US Demo)</span></span>|<span data-ttu-id="fcb74-196">Amount</span><span class="sxs-lookup"><span data-stu-id="fcb74-196">Amount</span></span>|<span data-ttu-id="fcb74-197">Entry No.</span><span class="sxs-lookup"><span data-stu-id="fcb74-197">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="fcb74-198">01-15-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-198">01-15-20</span></span>|<span data-ttu-id="fcb74-199">Inventory Accrual Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="fcb74-199">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="fcb74-200">5530</span><span class="sxs-lookup"><span data-stu-id="fcb74-200">5530</span></span>|<span data-ttu-id="fcb74-201">95.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-201">95.00</span></span>|<span data-ttu-id="fcb74-202">4</span><span class="sxs-lookup"><span data-stu-id="fcb74-202">4</span></span>|  
|<span data-ttu-id="fcb74-203">01-15-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-203">01-15-20</span></span>|<span data-ttu-id="fcb74-204">Inventory Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="fcb74-204">Inventory Account (Interim)</span></span>|<span data-ttu-id="fcb74-205">2131</span><span class="sxs-lookup"><span data-stu-id="fcb74-205">2131</span></span>|<span data-ttu-id="fcb74-206">-95.00</span><span class="sxs-lookup"><span data-stu-id="fcb74-206">-95.00</span></span>|<span data-ttu-id="fcb74-207">3</span><span class="sxs-lookup"><span data-stu-id="fcb74-207">3</span></span>|  
|<span data-ttu-id="fcb74-208">01-15-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-208">01-15-20</span></span>|<span data-ttu-id="fcb74-209">Direct Cost Applied Account</span><span class="sxs-lookup"><span data-stu-id="fcb74-209">Direct Cost Applied Account</span></span>|<span data-ttu-id="fcb74-210">7291</span><span class="sxs-lookup"><span data-stu-id="fcb74-210">7291</span></span>|<span data-ttu-id="fcb74-211">-100</span><span class="sxs-lookup"><span data-stu-id="fcb74-211">-100</span></span>|<span data-ttu-id="fcb74-212">6</span><span class="sxs-lookup"><span data-stu-id="fcb74-212">6</span></span>|  
|<span data-ttu-id="fcb74-213">01-15-20</span><span class="sxs-lookup"><span data-stu-id="fcb74-213">01-15-20</span></span>|<span data-ttu-id="fcb74-214">Inventory Account</span><span class="sxs-lookup"><span data-stu-id="fcb74-214">Inventory Account</span></span>|<span data-ttu-id="fcb74-215">2130</span><span class="sxs-lookup"><span data-stu-id="fcb74-215">2130</span></span>|<span data-ttu-id="fcb74-216">100</span><span class="sxs-lookup"><span data-stu-id="fcb74-216">100</span></span>|<span data-ttu-id="fcb74-217">5</span><span class="sxs-lookup"><span data-stu-id="fcb74-217">5</span></span>|  

## <a name="see-also"></a><span data-ttu-id="fcb74-218">See Also</span><span class="sxs-lookup"><span data-stu-id="fcb74-218">See Also</span></span>
 <span data-ttu-id="fcb74-219">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="fcb74-219">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="fcb74-220">[Design Details: Cost Adjustment](design-details-cost-adjustment.md) </span><span class="sxs-lookup"><span data-stu-id="fcb74-220">[Design Details: Cost Adjustment](design-details-cost-adjustment.md) </span></span>  
 <span data-ttu-id="fcb74-221">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span><span class="sxs-lookup"><span data-stu-id="fcb74-221">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span></span>  
 <span data-ttu-id="fcb74-222">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span><span class="sxs-lookup"><span data-stu-id="fcb74-222">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span></span>  
 [<span data-ttu-id="fcb74-223">Design Details: Variance</span><span class="sxs-lookup"><span data-stu-id="fcb74-223">Design Details: Variance</span></span>](design-details-variance.md)  
 [<span data-ttu-id="fcb74-224">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="fcb74-224">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
 [<span data-ttu-id="fcb74-225">Finance</span><span class="sxs-lookup"><span data-stu-id="fcb74-225">Finance</span></span>](finance.md)  
 <span data-ttu-id="fcb74-226">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fcb74-226">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>