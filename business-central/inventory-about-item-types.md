---
title: Understanding Item Types| Microsoft Docs
description: You can adjust the inventory valuation of an item using the FIFO or Average costing methods, for example, when item costs change for reasons other than transactions.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/18/2018
ms.author: sgroespe
ms.openlocfilehash: 2240840e977bcd1186c74972ce0457deb03058a0
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "257208"
---
# <a name="about-item-types"></a><span data-ttu-id="30a15-103">About Item Types</span><span class="sxs-lookup"><span data-stu-id="30a15-103">About Item Types</span></span>
<span data-ttu-id="30a15-104">In the **Type** field on the **Item Card** page, you can select what the item is used for in your business and therefore how it is managed in the system.</span><span class="sxs-lookup"><span data-stu-id="30a15-104">In the **Type** field on the **Item Card** page, you can select what the item is used for in your business and therefore how it is managed in the system.</span></span> <span data-ttu-id="30a15-105">Three options exist:</span><span class="sxs-lookup"><span data-stu-id="30a15-105">Three options exist:</span></span>

|<span data-ttu-id="30a15-106">Option</span><span class="sxs-lookup"><span data-stu-id="30a15-106">Option</span></span>|<span data-ttu-id="30a15-107">Typical Purpose</span><span class="sxs-lookup"><span data-stu-id="30a15-107">Typical Purpose</span></span>|
|------|-----------|
|<span data-ttu-id="30a15-108">Inventory</span><span class="sxs-lookup"><span data-stu-id="30a15-108">Inventory</span></span>|<span data-ttu-id="30a15-109">A physical unit, such as a bicycle, for full business support.</span><span class="sxs-lookup"><span data-stu-id="30a15-109">A physical unit, such as a bicycle, for full business support.</span></span>|
|<span data-ttu-id="30a15-110">Non-Inventory</span><span class="sxs-lookup"><span data-stu-id="30a15-110">Non-Inventory</span></span>|<span data-ttu-id="30a15-111">A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.</span><span class="sxs-lookup"><span data-stu-id="30a15-111">A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.</span></span>|
|<span data-ttu-id="30a15-112">Service</span><span class="sxs-lookup"><span data-stu-id="30a15-112">Service</span></span>|<span data-ttu-id="30a15-113">A labour time unit, such as a consultancy hour, for limited business support.</span><span class="sxs-lookup"><span data-stu-id="30a15-113">A labor time unit, such as a consultancy hour, for limited business support.</span></span>|

<span data-ttu-id="30a15-114">The **Inventory** type involves full tracking of inventory quantity and value.</span><span class="sxs-lookup"><span data-stu-id="30a15-114">The **Inventory** type involves full tracking of inventory quantity and value.</span></span> <span data-ttu-id="30a15-115">Therefore, all item transaction nature codes are supported, and items of type Inventory can be used with all item-handling features.</span><span class="sxs-lookup"><span data-stu-id="30a15-115">Therefore, all item transaction types are supported, and items of type Inventory can be used with all item-handling features.</span></span>

<span data-ttu-id="30a15-116">The **Service** and **Non-Inventory** types do not involve tracking of inventory quantity and value.</span><span class="sxs-lookup"><span data-stu-id="30a15-116">The **Service** and **Non-Inventory** types do not involve tracking of inventory quantity and value.</span></span> <span data-ttu-id="30a15-117">Therefore, only selected item transaction nature codes and features are supported.</span><span class="sxs-lookup"><span data-stu-id="30a15-117">Therefore, only selected item transaction types and features are supported.</span></span>

<span data-ttu-id="30a15-118">The three item types support the following features respectively.</span><span class="sxs-lookup"><span data-stu-id="30a15-118">The three item types support the following features respectively.</span></span>

|<span data-ttu-id="30a15-119">Item Type</span><span class="sxs-lookup"><span data-stu-id="30a15-119">Item Type</span></span>|<span data-ttu-id="30a15-120">Sales</span><span class="sxs-lookup"><span data-stu-id="30a15-120">Sales</span></span>|<span data-ttu-id="30a15-121">Purchasing</span><span class="sxs-lookup"><span data-stu-id="30a15-121">Purchasing</span></span>|<span data-ttu-id="30a15-122">Job Consumption</span><span class="sxs-lookup"><span data-stu-id="30a15-122">Job Consumption</span></span>|<span data-ttu-id="30a15-123">Service Consumption</span><span class="sxs-lookup"><span data-stu-id="30a15-123">Service Consumption</span></span>|<span data-ttu-id="30a15-124">Assembly Consumption</span><span class="sxs-lookup"><span data-stu-id="30a15-124">Assembly Consumption</span></span>|<span data-ttu-id="30a15-125">Production Consumption</span><span class="sxs-lookup"><span data-stu-id="30a15-125">Production Consumption</span></span>|<span data-ttu-id="30a15-126">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="30a15-126">Assembly Output</span></span>|<span data-ttu-id="30a15-127">Production Output</span><span class="sxs-lookup"><span data-stu-id="30a15-127">Production Output</span></span>|<span data-ttu-id="30a15-128">Location Transfer</span><span class="sxs-lookup"><span data-stu-id="30a15-128">Location Transfer</span></span>|<span data-ttu-id="30a15-129">Physical Counting</span><span class="sxs-lookup"><span data-stu-id="30a15-129">Physical Counting</span></span>|<span data-ttu-id="30a15-130">Inventory Revaluation</span><span class="sxs-lookup"><span data-stu-id="30a15-130">Inventory Revaluation</span></span>|<span data-ttu-id="30a15-131">Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="30a15-131">Inventory Costing</span></span>|<span data-ttu-id="30a15-132">Item Tracking</span><span class="sxs-lookup"><span data-stu-id="30a15-132">Item Tracking</span></span>|<span data-ttu-id="30a15-133">Reservation</span><span class="sxs-lookup"><span data-stu-id="30a15-133">Reservation</span></span>|<span data-ttu-id="30a15-134">Warehousing</span><span class="sxs-lookup"><span data-stu-id="30a15-134">Warehousing</span></span>|<span data-ttu-id="30a15-135">Planning</span><span class="sxs-lookup"><span data-stu-id="30a15-135">Planning</span></span>|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|<span data-ttu-id="30a15-136">Inventory</span><span class="sxs-lookup"><span data-stu-id="30a15-136">Inventory</span></span>|<span data-ttu-id="30a15-137">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-137">Yes</span></span>|<span data-ttu-id="30a15-138">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-138">Yes</span></span>|<span data-ttu-id="30a15-139">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-139">Yes</span></span>|<span data-ttu-id="30a15-140">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-140">Yes</span></span>|<span data-ttu-id="30a15-141">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-141">Yes</span></span>|<span data-ttu-id="30a15-142">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-142">Yes</span></span>|<span data-ttu-id="30a15-143">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-143">Yes</span></span>|<span data-ttu-id="30a15-144">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-144">Yes</span></span>|<span data-ttu-id="30a15-145">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-145">Yes</span></span>|<span data-ttu-id="30a15-146">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-146">Yes</span></span>|<span data-ttu-id="30a15-147">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-147">Yes</span></span>|<span data-ttu-id="30a15-148">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-148">Yes</span></span>|<span data-ttu-id="30a15-149">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-149">Yes</span></span>|<span data-ttu-id="30a15-150">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-150">Yes</span></span>|<span data-ttu-id="30a15-151">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-151">Yes</span></span>|<span data-ttu-id="30a15-152">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-152">Yes</span></span>|
|<span data-ttu-id="30a15-153">Non-Inventory</span><span class="sxs-lookup"><span data-stu-id="30a15-153">Non-Inventory</span></span>|<span data-ttu-id="30a15-154">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-154">Yes</span></span>|<span data-ttu-id="30a15-155">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-155">Yes</span></span>|<span data-ttu-id="30a15-156">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-156">Yes</span></span>|<span data-ttu-id="30a15-157">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-157">Yes</span></span>|<span data-ttu-id="30a15-158">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-158">Yes</span></span>|<span data-ttu-id="30a15-159">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-159">Yes</span></span>|<span data-ttu-id="30a15-160">No</span><span class="sxs-lookup"><span data-stu-id="30a15-160">No</span></span>|<span data-ttu-id="30a15-161">No</span><span class="sxs-lookup"><span data-stu-id="30a15-161">No</span></span>|<span data-ttu-id="30a15-162">No</span><span class="sxs-lookup"><span data-stu-id="30a15-162">No</span></span>|<span data-ttu-id="30a15-163">No</span><span class="sxs-lookup"><span data-stu-id="30a15-163">No</span></span>|<span data-ttu-id="30a15-164">No</span><span class="sxs-lookup"><span data-stu-id="30a15-164">No</span></span>|<span data-ttu-id="30a15-165">No</span><span class="sxs-lookup"><span data-stu-id="30a15-165">No</span></span>|<span data-ttu-id="30a15-166">No</span><span class="sxs-lookup"><span data-stu-id="30a15-166">No</span></span>|<span data-ttu-id="30a15-167">No</span><span class="sxs-lookup"><span data-stu-id="30a15-167">No</span></span>|<span data-ttu-id="30a15-168">No</span><span class="sxs-lookup"><span data-stu-id="30a15-168">No</span></span>|<span data-ttu-id="30a15-169">No</span><span class="sxs-lookup"><span data-stu-id="30a15-169">No</span></span>|
|<span data-ttu-id="30a15-170">Service</span><span class="sxs-lookup"><span data-stu-id="30a15-170">Service</span></span>|<span data-ttu-id="30a15-171">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-171">Yes</span></span>|<span data-ttu-id="30a15-172">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-172">Yes</span></span>|<span data-ttu-id="30a15-173">Yes</span><span class="sxs-lookup"><span data-stu-id="30a15-173">Yes</span></span>|<span data-ttu-id="30a15-174">No</span><span class="sxs-lookup"><span data-stu-id="30a15-174">No</span></span>|<span data-ttu-id="30a15-175">No</span><span class="sxs-lookup"><span data-stu-id="30a15-175">No</span></span>|<span data-ttu-id="30a15-176">No</span><span class="sxs-lookup"><span data-stu-id="30a15-176">No</span></span>|<span data-ttu-id="30a15-177">No</span><span class="sxs-lookup"><span data-stu-id="30a15-177">No</span></span>|<span data-ttu-id="30a15-178">No</span><span class="sxs-lookup"><span data-stu-id="30a15-178">No</span></span>|<span data-ttu-id="30a15-179">No</span><span class="sxs-lookup"><span data-stu-id="30a15-179">No</span></span>|<span data-ttu-id="30a15-180">No</span><span class="sxs-lookup"><span data-stu-id="30a15-180">No</span></span>|<span data-ttu-id="30a15-181">No</span><span class="sxs-lookup"><span data-stu-id="30a15-181">No</span></span>|<span data-ttu-id="30a15-182">No</span><span class="sxs-lookup"><span data-stu-id="30a15-182">No</span></span>|<span data-ttu-id="30a15-183">No</span><span class="sxs-lookup"><span data-stu-id="30a15-183">No</span></span>|<span data-ttu-id="30a15-184">No</span><span class="sxs-lookup"><span data-stu-id="30a15-184">No</span></span>|<span data-ttu-id="30a15-185">No</span><span class="sxs-lookup"><span data-stu-id="30a15-185">No</span></span>|<span data-ttu-id="30a15-186">No</span><span class="sxs-lookup"><span data-stu-id="30a15-186">No</span></span>|

> [!NOTE]
> <span data-ttu-id="30a15-187">Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalogue items.</span><span class="sxs-lookup"><span data-stu-id="30a15-187">Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalog items.</span></span> <span data-ttu-id="30a15-188">Catalogue items are not to be mistaken with regular items of type Non-Inventory.</span><span class="sxs-lookup"><span data-stu-id="30a15-188">Catalog items are not to be mistaken with regular items of type Non-Inventory.</span></span> <span data-ttu-id="30a15-189">For more information, see [Work with Catalogue Items](inventory-how-work-nonstock-items.md).</span><span class="sxs-lookup"><span data-stu-id="30a15-189">For more information, see [Work with Catalog Items](inventory-how-work-nonstock-items.md).</span></span>

> [!NOTE]
> <span data-ttu-id="30a15-190">Customers' items that you perform service on, such as a printer, are called service items.</span><span class="sxs-lookup"><span data-stu-id="30a15-190">Customers' items that you perform service on, such as a printer, are called service items.</span></span> <span data-ttu-id="30a15-191">Service items have nothing to do with regular or catalogue items.</span><span class="sxs-lookup"><span data-stu-id="30a15-191">Service items have nothing to do with regular or catalog items.</span></span> <span data-ttu-id="30a15-192">However, service components can be regular items.</span><span class="sxs-lookup"><span data-stu-id="30a15-192">However, service components can be regular items.</span></span> <span data-ttu-id="30a15-193">For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).</span><span class="sxs-lookup"><span data-stu-id="30a15-193">For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="30a15-194">See Also</span><span class="sxs-lookup"><span data-stu-id="30a15-194">See Also</span></span>
[<span data-ttu-id="30a15-195">Register New Items</span><span class="sxs-lookup"><span data-stu-id="30a15-195">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="30a15-196">Setting Up Inventory</span><span class="sxs-lookup"><span data-stu-id="30a15-196">Setting Up Inventory</span></span>](inventory-setup-inventory.md)  
[<span data-ttu-id="30a15-197">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="30a15-197">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="30a15-198">Inventory</span><span class="sxs-lookup"><span data-stu-id="30a15-198">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="30a15-199">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="30a15-199">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>