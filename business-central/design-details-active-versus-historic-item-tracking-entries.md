---
title: Design Details - Active versus Historic Item Tracking Entries | Microsoft Docs
description: When parts of a document line quantity are posted, only that particular quantity is transferred to the item ledger entries and its item tracking numbers. However, you will want to access all relevant item tracking information directly from the active document line. That is, not only will you want to see the entries that are related to the remaining quantity, you will also want information about the units that have been posted. When you view or modify the **Item Tracking Lines** page, the collective contents of the **Tracking Specification** table (T336) and **Reservation Entry** table (T337) are presented in a temporary version of T336. This ensures that historic and active item tracking data is accessed as one.
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
ms.openlocfilehash: 30a15b664c46729b8e3901bc49982eefc21f1c2a
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "269931"
---
# <a name="design-details-active-versus-historic-item-tracking-entries"></a><span data-ttu-id="2acc5-107">Design Details: Active versus Historic Item Tracking Entries</span><span class="sxs-lookup"><span data-stu-id="2acc5-107">Design Details: Active versus Historic Item Tracking Entries</span></span>
<span data-ttu-id="2acc5-108">When parts of a document line quantity are posted, only that particular quantity is transferred to the item ledger entries and its item tracking numbers.</span><span class="sxs-lookup"><span data-stu-id="2acc5-108">When parts of a document line quantity are posted, only that particular quantity is transferred to the item ledger entries and its item tracking numbers.</span></span> <span data-ttu-id="2acc5-109">However, you will want to access all relevant item tracking information directly from the active document line.</span><span class="sxs-lookup"><span data-stu-id="2acc5-109">However, you will want to access all relevant item tracking information directly from the active document line.</span></span> <span data-ttu-id="2acc5-110">That is, not only will you want to see the entries that are related to the remaining quantity, you will also want information about the units that have been posted.</span><span class="sxs-lookup"><span data-stu-id="2acc5-110">That is, not only will you want to see the entries that are related to the remaining quantity, you will also want information about the units that have been posted.</span></span> <span data-ttu-id="2acc5-111">When you view or modify the **Item Tracking Lines** page, the collective contents of the **Tracking Specification** table (T336) and **Reservation Entry** table (T337) are presented in a temporary version of T336.</span><span class="sxs-lookup"><span data-stu-id="2acc5-111">When you view or modify the **Item Tracking Lines** page, the collective contents of the **Tracking Specification** table (T336) and **Reservation Entry** table (T337) are presented in a temporary version of T336.</span></span> <span data-ttu-id="2acc5-112">This ensures that historic and active item tracking data is accessed as one.</span><span class="sxs-lookup"><span data-stu-id="2acc5-112">This ensures that historic and active item tracking data is accessed as one.</span></span>  

 <span data-ttu-id="2acc5-113">The following table shows how T336 and T337 are used in a purchase scenario.</span><span class="sxs-lookup"><span data-stu-id="2acc5-113">The following table shows how T336 and T337 are used in a purchase scenario.</span></span> <span data-ttu-id="2acc5-114">The bold figures represent values that the user manually enters on the **Item Tracking Lines** page.</span><span class="sxs-lookup"><span data-stu-id="2acc5-114">The bold figures represent values that the user manually enters on the **Item Tracking Lines** page.</span></span>  

 <span data-ttu-id="2acc5-115">Step 1: Create a purchase order line of seven pieces with item tracking numbers.</span><span class="sxs-lookup"><span data-stu-id="2acc5-115">Step 1: Create a purchase order line of seven pieces with item tracking numbers.</span></span>  

||<span data-ttu-id="2acc5-116">**Quantity (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-116">**Quantity (Base)**</span></span>|<span data-ttu-id="2acc5-117">**Qty. to Handle**</span><span class="sxs-lookup"><span data-stu-id="2acc5-117">**Qty. to Handle**</span></span>|<span data-ttu-id="2acc5-118">**Qty. to Invoice (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-118">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="2acc5-119">**Quantity Handled (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-119">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="2acc5-120">**Quantity Invoiced (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-120">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="2acc5-121">**T337**</span><span class="sxs-lookup"><span data-stu-id="2acc5-121">**T337**</span></span>|<span data-ttu-id="2acc5-122">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-122">7</span></span>|<span data-ttu-id="2acc5-123">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-123">0</span></span>|<span data-ttu-id="2acc5-124">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-124">0</span></span>|<span data-ttu-id="2acc5-125">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-125">0</span></span>|<span data-ttu-id="2acc5-126">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-126">0</span></span>|  
|<span data-ttu-id="2acc5-127">**T336**</span><span class="sxs-lookup"><span data-stu-id="2acc5-127">**T336**</span></span>|<span data-ttu-id="2acc5-128">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-128">0</span></span>|<span data-ttu-id="2acc5-129">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-129">0</span></span>|<span data-ttu-id="2acc5-130">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-130">0</span></span>|<span data-ttu-id="2acc5-131">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-131">0</span></span>|<span data-ttu-id="2acc5-132">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-132">0</span></span>|  

 <span data-ttu-id="2acc5-133">Step 2: Receive four pieces.</span><span class="sxs-lookup"><span data-stu-id="2acc5-133">Step 2: Receive four pieces.</span></span>  

||<span data-ttu-id="2acc5-134">**Quantity (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-134">**Quantity (Base)**</span></span>|<span data-ttu-id="2acc5-135">**Qty. to Handle**</span><span class="sxs-lookup"><span data-stu-id="2acc5-135">**Qty. to Handle**</span></span>|<span data-ttu-id="2acc5-136">**Qty. to Invoice (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-136">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="2acc5-137">**Quantity Handled (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-137">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="2acc5-138">**Quantity Invoiced (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-138">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="2acc5-139">**Item Tracking Lines** page</span><span class="sxs-lookup"><span data-stu-id="2acc5-139">**Item Tracking Lines** page</span></span>|<span data-ttu-id="2acc5-140">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-140">7</span></span>|<span data-ttu-id="2acc5-141">**4**</span><span class="sxs-lookup"><span data-stu-id="2acc5-141">**4**</span></span>|<span data-ttu-id="2acc5-142">**0**</span><span class="sxs-lookup"><span data-stu-id="2acc5-142">**0**</span></span>|<span data-ttu-id="2acc5-143">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-143">0</span></span>|<span data-ttu-id="2acc5-144">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-144">0</span></span>|  
|<span data-ttu-id="2acc5-145">**T337**</span><span class="sxs-lookup"><span data-stu-id="2acc5-145">**T337**</span></span>|<span data-ttu-id="2acc5-146">3</span><span class="sxs-lookup"><span data-stu-id="2acc5-146">3</span></span>|<span data-ttu-id="2acc5-147">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-147">0</span></span>|<span data-ttu-id="2acc5-148">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-148">0</span></span>|<span data-ttu-id="2acc5-149">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-149">0</span></span>|<span data-ttu-id="2acc5-150">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-150">0</span></span>|  
|<span data-ttu-id="2acc5-151">**T336**</span><span class="sxs-lookup"><span data-stu-id="2acc5-151">**T336**</span></span>|<span data-ttu-id="2acc5-152">4</span><span class="sxs-lookup"><span data-stu-id="2acc5-152">4</span></span>|<span data-ttu-id="2acc5-153">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-153">0</span></span>|<span data-ttu-id="2acc5-154">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-154">0</span></span>|<span data-ttu-id="2acc5-155">4</span><span class="sxs-lookup"><span data-stu-id="2acc5-155">4</span></span>|<span data-ttu-id="2acc5-156">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-156">0</span></span>|  

 <span data-ttu-id="2acc5-157">Step 3: Receive two pieces and invoice two pieces.</span><span class="sxs-lookup"><span data-stu-id="2acc5-157">Step 3: Receive two pieces and invoice two pieces.</span></span>  

||<span data-ttu-id="2acc5-158">**Quantity (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-158">**Quantity (Base)**</span></span>|<span data-ttu-id="2acc5-159">**Qty. to Handle**</span><span class="sxs-lookup"><span data-stu-id="2acc5-159">**Qty. to Handle**</span></span>|<span data-ttu-id="2acc5-160">**Qty. to Invoice (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-160">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="2acc5-161">**Quantity Handled (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-161">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="2acc5-162">**Quantity Invoiced (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-162">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="2acc5-163">**Item Tracking Lines** page</span><span class="sxs-lookup"><span data-stu-id="2acc5-163">**Item Tracking Lines** page</span></span>|<span data-ttu-id="2acc5-164">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-164">7</span></span>|<span data-ttu-id="2acc5-165">**2**</span><span class="sxs-lookup"><span data-stu-id="2acc5-165">**2**</span></span>|<span data-ttu-id="2acc5-166">**2**</span><span class="sxs-lookup"><span data-stu-id="2acc5-166">**2**</span></span>|<span data-ttu-id="2acc5-167">4</span><span class="sxs-lookup"><span data-stu-id="2acc5-167">4</span></span>|<span data-ttu-id="2acc5-168">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-168">0</span></span>|  
|<span data-ttu-id="2acc5-169">**T337**</span><span class="sxs-lookup"><span data-stu-id="2acc5-169">**T337**</span></span>|<span data-ttu-id="2acc5-170">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-170">1</span></span>|<span data-ttu-id="2acc5-171">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-171">0</span></span>|<span data-ttu-id="2acc5-172">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-172">0</span></span>|<span data-ttu-id="2acc5-173">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-173">0</span></span>|<span data-ttu-id="2acc5-174">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-174">0</span></span>|  
|<span data-ttu-id="2acc5-175">**T336**</span><span class="sxs-lookup"><span data-stu-id="2acc5-175">**T336**</span></span>|<span data-ttu-id="2acc5-176">6</span><span class="sxs-lookup"><span data-stu-id="2acc5-176">6</span></span>|<span data-ttu-id="2acc5-177">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-177">0</span></span>|<span data-ttu-id="2acc5-178">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-178">0</span></span>|<span data-ttu-id="2acc5-179">6</span><span class="sxs-lookup"><span data-stu-id="2acc5-179">6</span></span>|<span data-ttu-id="2acc5-180">2</span><span class="sxs-lookup"><span data-stu-id="2acc5-180">2</span></span>|  

 <span data-ttu-id="2acc5-181">Step 4: Receive one piece.</span><span class="sxs-lookup"><span data-stu-id="2acc5-181">Step 4: Receive one piece.</span></span>  

||<span data-ttu-id="2acc5-182">**Quantity (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-182">**Quantity (Base)**</span></span>|<span data-ttu-id="2acc5-183">**Qty. to Handle**</span><span class="sxs-lookup"><span data-stu-id="2acc5-183">**Qty. to Handle**</span></span>|<span data-ttu-id="2acc5-184">**Qty. to Invoice (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-184">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="2acc5-185">**Quantity Handled (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-185">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="2acc5-186">**Quantity Invoiced (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-186">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="2acc5-187">**Item Tracking Lines** page</span><span class="sxs-lookup"><span data-stu-id="2acc5-187">**Item Tracking Lines** page</span></span>|<span data-ttu-id="2acc5-188">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-188">7</span></span>|<span data-ttu-id="2acc5-189">**1**</span><span class="sxs-lookup"><span data-stu-id="2acc5-189">**1**</span></span>|<span data-ttu-id="2acc5-190">**0**</span><span class="sxs-lookup"><span data-stu-id="2acc5-190">**0**</span></span>|<span data-ttu-id="2acc5-191">6</span><span class="sxs-lookup"><span data-stu-id="2acc5-191">6</span></span>|<span data-ttu-id="2acc5-192">2</span><span class="sxs-lookup"><span data-stu-id="2acc5-192">2</span></span>|  
|<span data-ttu-id="2acc5-193">**T336**</span><span class="sxs-lookup"><span data-stu-id="2acc5-193">**T336**</span></span>|<span data-ttu-id="2acc5-194">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-194">7</span></span>|<span data-ttu-id="2acc5-195">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-195">0</span></span>|<span data-ttu-id="2acc5-196">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-196">0</span></span>|<span data-ttu-id="2acc5-197">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-197">7</span></span>|<span data-ttu-id="2acc5-198">2</span><span class="sxs-lookup"><span data-stu-id="2acc5-198">2</span></span>|  

 <span data-ttu-id="2acc5-199">Invoice 5 pieces.</span><span class="sxs-lookup"><span data-stu-id="2acc5-199">Invoice 5 pieces.</span></span>  

||<span data-ttu-id="2acc5-200">**Quantity (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-200">**Quantity (Base)**</span></span>|<span data-ttu-id="2acc5-201">**Qty. to Handle**</span><span class="sxs-lookup"><span data-stu-id="2acc5-201">**Qty. to Handle**</span></span>|<span data-ttu-id="2acc5-202">**Qty. to Invoice (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-202">**Qty. to Invoice (Base)**</span></span>|<span data-ttu-id="2acc5-203">**Quantity Handled (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-203">**Quantity Handled (Base)**</span></span>|<span data-ttu-id="2acc5-204">**Quantity Invoiced (Base)**</span><span class="sxs-lookup"><span data-stu-id="2acc5-204">**Quantity Invoiced (Base)**</span></span>|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|<span data-ttu-id="2acc5-205">**Item Tracking Lines** page</span><span class="sxs-lookup"><span data-stu-id="2acc5-205">**Item Tracking Lines** page</span></span>|<span data-ttu-id="2acc5-206">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-206">7</span></span>|<span data-ttu-id="2acc5-207">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-207">0</span></span>|<span data-ttu-id="2acc5-208">**5**</span><span class="sxs-lookup"><span data-stu-id="2acc5-208">**5**</span></span>|<span data-ttu-id="2acc5-209">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-209">7</span></span>|<span data-ttu-id="2acc5-210">2</span><span class="sxs-lookup"><span data-stu-id="2acc5-210">2</span></span>|  
|<span data-ttu-id="2acc5-211">**T336**</span><span class="sxs-lookup"><span data-stu-id="2acc5-211">**T336**</span></span>|<span data-ttu-id="2acc5-212">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-212">7</span></span>|<span data-ttu-id="2acc5-213">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-213">0</span></span>|<span data-ttu-id="2acc5-214">0</span><span class="sxs-lookup"><span data-stu-id="2acc5-214">0</span></span>|<span data-ttu-id="2acc5-215">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-215">7</span></span>|<span data-ttu-id="2acc5-216">7</span><span class="sxs-lookup"><span data-stu-id="2acc5-216">7</span></span>|  

## <a name="see-also"></a><span data-ttu-id="2acc5-217">See Also</span><span class="sxs-lookup"><span data-stu-id="2acc5-217">See Also</span></span>  
 <span data-ttu-id="2acc5-218">[Design Details: Item Tracking](design-details-item-tracking.md) </span><span class="sxs-lookup"><span data-stu-id="2acc5-218">[Design Details: Item Tracking](design-details-item-tracking.md) </span></span>  
 [<span data-ttu-id="2acc5-219">Design Details: Item Tracking Lines Page</span><span class="sxs-lookup"><span data-stu-id="2acc5-219">Design Details: Item Tracking Lines Page</span></span>](design-details-item-tracking-lines-window.md)