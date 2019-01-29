---
title: Walkthrough - Receiving and Putting Away in Basic Warehouse Configurations | Microsoft Docs
description: In Business Central, the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 0ba61572a237e177b763b7b8a2e13ca7ec93eea4
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "223232"
---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a><span data-ttu-id="f94d6-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="f94d6-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span></span>
<span data-ttu-id="f94d6-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span><span class="sxs-lookup"><span data-stu-id="f94d6-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="f94d6-105">Method</span><span class="sxs-lookup"><span data-stu-id="f94d6-105">Method</span></span>|<span data-ttu-id="f94d6-106">Inbound process</span><span class="sxs-lookup"><span data-stu-id="f94d6-106">Inbound process</span></span>|<span data-ttu-id="f94d6-107">Bins</span><span class="sxs-lookup"><span data-stu-id="f94d6-107">Bins</span></span>|<span data-ttu-id="f94d6-108">Receipts</span><span class="sxs-lookup"><span data-stu-id="f94d6-108">Receipts</span></span>|<span data-ttu-id="f94d6-109">Put-aways</span><span class="sxs-lookup"><span data-stu-id="f94d6-109">Put-aways</span></span>|<span data-ttu-id="f94d6-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="f94d6-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="f94d6-111">A</span><span class="sxs-lookup"><span data-stu-id="f94d6-111">A</span></span>|<span data-ttu-id="f94d6-112">Post receipt and put-away from the order line</span><span class="sxs-lookup"><span data-stu-id="f94d6-112">Post receipt and put-away from the order line</span></span>|<span data-ttu-id="f94d6-113">X</span><span class="sxs-lookup"><span data-stu-id="f94d6-113">X</span></span>|||<span data-ttu-id="f94d6-114">2</span><span class="sxs-lookup"><span data-stu-id="f94d6-114">2</span></span>|  
|<span data-ttu-id="f94d6-115">B</span><span class="sxs-lookup"><span data-stu-id="f94d6-115">B</span></span>|<span data-ttu-id="f94d6-116">Post receipt and put-away from an inventory put-away document</span><span class="sxs-lookup"><span data-stu-id="f94d6-116">Post receipt and put-away from an inventory put-away document</span></span>|||<span data-ttu-id="f94d6-117">X</span><span class="sxs-lookup"><span data-stu-id="f94d6-117">X</span></span>|<span data-ttu-id="f94d6-118">3</span><span class="sxs-lookup"><span data-stu-id="f94d6-118">3</span></span>|  
|<span data-ttu-id="f94d6-119">C</span><span class="sxs-lookup"><span data-stu-id="f94d6-119">C</span></span>|<span data-ttu-id="f94d6-120">Post receipt and put-away from a warehouse receipt document</span><span class="sxs-lookup"><span data-stu-id="f94d6-120">Post receipt and put-away from a warehouse receipt document</span></span>||<span data-ttu-id="f94d6-121">X</span><span class="sxs-lookup"><span data-stu-id="f94d6-121">X</span></span>||<span data-ttu-id="f94d6-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="f94d6-122">4/5/6</span></span>|  
|<span data-ttu-id="f94d6-123">D</span><span class="sxs-lookup"><span data-stu-id="f94d6-123">D</span></span>|<span data-ttu-id="f94d6-124">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span><span class="sxs-lookup"><span data-stu-id="f94d6-124">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span></span>||<span data-ttu-id="f94d6-125">X</span><span class="sxs-lookup"><span data-stu-id="f94d6-125">X</span></span>|<span data-ttu-id="f94d6-126">X</span><span class="sxs-lookup"><span data-stu-id="f94d6-126">X</span></span>|<span data-ttu-id="f94d6-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="f94d6-127">4/5/6</span></span>|  

<span data-ttu-id="f94d6-128">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="f94d6-128">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="f94d6-129">The following walkthrough demonstrates method B in the previous table.</span><span class="sxs-lookup"><span data-stu-id="f94d6-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="f94d6-130">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="f94d6-130">About This Walkthrough</span></span>  
<span data-ttu-id="f94d6-131">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** page to record and post put-away and receipt information for your inbound source documents.</span><span class="sxs-lookup"><span data-stu-id="f94d6-131">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** page to record and post put-away and receipt information for your inbound source documents.</span></span> <span data-ttu-id="f94d6-132">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span><span class="sxs-lookup"><span data-stu-id="f94d6-132">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span></span>

> [!NOTE]
> <span data-ttu-id="f94d6-133">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span><span class="sxs-lookup"><span data-stu-id="f94d6-133">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span></span>  

<span data-ttu-id="f94d6-134">This walkthrough demonstrates the following tasks.</span><span class="sxs-lookup"><span data-stu-id="f94d6-134">This walkthrough demonstrates the following tasks.</span></span>  

-   <span data-ttu-id="f94d6-135">Setting up SILVER location for inventory put aways.</span><span class="sxs-lookup"><span data-stu-id="f94d6-135">Setting up SILVER location for inventory put aways.</span></span>  
-   <span data-ttu-id="f94d6-136">Setting up SILVER location for bin handling.</span><span class="sxs-lookup"><span data-stu-id="f94d6-136">Setting up SILVER location for bin handling.</span></span>  
-   <span data-ttu-id="f94d6-137">Defining a default bin for item LS-81.</span><span class="sxs-lookup"><span data-stu-id="f94d6-137">Defining a default bin for item LS-81.</span></span> <span data-ttu-id="f94d6-138">(LS-75 is already set up in CRONUS.)</span><span class="sxs-lookup"><span data-stu-id="f94d6-138">(LS-75 is already set up in CRONUS.)</span></span>  
-   <span data-ttu-id="f94d6-139">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span><span class="sxs-lookup"><span data-stu-id="f94d6-139">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span></span>  
-   <span data-ttu-id="f94d6-140">Verifying that the put-away bins are preset by setup.</span><span class="sxs-lookup"><span data-stu-id="f94d6-140">Verifying that the put-away bins are preset by setup.</span></span>  
-   <span data-ttu-id="f94d6-141">Releasing the purchase order for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="f94d6-141">Releasing the purchase order for warehouse handling.</span></span>  
-   <span data-ttu-id="f94d6-142">Creating an inventory put-away based on a released source document.</span><span class="sxs-lookup"><span data-stu-id="f94d6-142">Creating an inventory put-away based on a released source document.</span></span>  
-   <span data-ttu-id="f94d6-143">Verifying that the put-away bins are inherited from the purchase order.</span><span class="sxs-lookup"><span data-stu-id="f94d6-143">Verifying that the put-away bins are inherited from the purchase order.</span></span>  
-   <span data-ttu-id="f94d6-144">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span><span class="sxs-lookup"><span data-stu-id="f94d6-144">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span></span>  

## <a name="roles"></a><span data-ttu-id="f94d6-145">Roles</span><span class="sxs-lookup"><span data-stu-id="f94d6-145">Roles</span></span>  
<span data-ttu-id="f94d6-146">This walkthrough demonstrates tasks that are performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="f94d6-146">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

-   <span data-ttu-id="f94d6-147">Warehouse Manager</span><span class="sxs-lookup"><span data-stu-id="f94d6-147">Warehouse Manager</span></span>  
-   <span data-ttu-id="f94d6-148">Purchasing Agent</span><span class="sxs-lookup"><span data-stu-id="f94d6-148">Purchasing Agent</span></span>  
-   <span data-ttu-id="f94d6-149">Warehouse Worker</span><span class="sxs-lookup"><span data-stu-id="f94d6-149">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="f94d6-150">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="f94d6-150">Prerequisites</span></span>  
<span data-ttu-id="f94d6-151">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="f94d6-151">To complete this walkthrough, you will need:</span></span>  

-   <span data-ttu-id="f94d6-152">CRONUS International Ltd. installed.</span><span class="sxs-lookup"><span data-stu-id="f94d6-152">CRONUS International Ltd. installed.</span></span>  
-   <span data-ttu-id="f94d6-153">To make yourself a warehouse employee at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="f94d6-153">To make yourself a warehouse employee at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="f94d6-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f94d6-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="f94d6-155">Choose the **User ID** field, and select your own user account on the **Users** page.</span><span class="sxs-lookup"><span data-stu-id="f94d6-155">Choose the **User ID** field, and select your own user account on the **Users** page.</span></span>  
    3.  <span data-ttu-id="f94d6-156">In the **Location Code** field, enter SILVER.</span><span class="sxs-lookup"><span data-stu-id="f94d6-156">In the **Location Code** field, enter SILVER.</span></span>  
    4.  <span data-ttu-id="f94d6-157">Select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="f94d6-157">Select the **Default** field.</span></span>  

## <a name="story"></a><span data-ttu-id="f94d6-158">Story</span><span class="sxs-lookup"><span data-stu-id="f94d6-158">Story</span></span>  
<span data-ttu-id="f94d6-159">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span><span class="sxs-lookup"><span data-stu-id="f94d6-159">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span></span> <span data-ttu-id="f94d6-160">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span><span class="sxs-lookup"><span data-stu-id="f94d6-160">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span></span> <span data-ttu-id="f94d6-161">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span><span class="sxs-lookup"><span data-stu-id="f94d6-161">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="f94d6-162">Setting up the Location</span><span class="sxs-lookup"><span data-stu-id="f94d6-162">Setting up the Location</span></span>  
 <span data-ttu-id="f94d6-163">The setup of the **Location Card** page defines the company’s warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="f94d6-163">The setup of the **Location Card** page defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="f94d6-164">To set up the location</span><span class="sxs-lookup"><span data-stu-id="f94d6-164">To set up the location</span></span>  

1.  <span data-ttu-id="f94d6-165">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f94d6-165">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f94d6-166">Open the SILVER location card.</span><span class="sxs-lookup"><span data-stu-id="f94d6-166">Open the SILVER location card.</span></span>  
3.  <span data-ttu-id="f94d6-167">Select the **Require Put-away** check box.</span><span class="sxs-lookup"><span data-stu-id="f94d6-167">Select the **Require Put-away** check box.</span></span>  

    <span data-ttu-id="f94d6-168">Proceed to set up a default bin for the two item numbers to control where they are put away.</span><span class="sxs-lookup"><span data-stu-id="f94d6-168">Proceed to set up a default bin for the two item numbers to control where they are put away.</span></span>  

4.  <span data-ttu-id="f94d6-169">Choose the **Bins** action.</span><span class="sxs-lookup"><span data-stu-id="f94d6-169">Choose the **Bins** action.</span></span>  
5.  <span data-ttu-id="f94d6-170">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span><span class="sxs-lookup"><span data-stu-id="f94d6-170">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span></span>  

    <span data-ttu-id="f94d6-171">Notice on the **Bin Content** page that item LS-75 is already set up as content in bin S-01-0001.</span><span class="sxs-lookup"><span data-stu-id="f94d6-171">Notice on the **Bin Content** page that item LS-75 is already set up as content in bin S-01-0001.</span></span>  

6.  <span data-ttu-id="f94d6-172">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="f94d6-172">Choose the **New** action.</span></span>  
7.  <span data-ttu-id="f94d6-173">Select the **Fixed** and the **Default** fields.</span><span class="sxs-lookup"><span data-stu-id="f94d6-173">Select the **Fixed** and the **Default** fields.</span></span>  
8.  <span data-ttu-id="f94d6-174">In the **Item No.** field, enter LS-81.</span><span class="sxs-lookup"><span data-stu-id="f94d6-174">In the **Item No.** field, enter LS-81.</span></span>  

## <a name="creating-the-purchase-order"></a><span data-ttu-id="f94d6-175">Creating the Purchase Order</span><span class="sxs-lookup"><span data-stu-id="f94d6-175">Creating the Purchase Order</span></span>  
<span data-ttu-id="f94d6-176">Purchase orders are the most common type of inbound source document.</span><span class="sxs-lookup"><span data-stu-id="f94d6-176">Purchase orders are the most common type of inbound source document.</span></span>  

### <a name="to-create-the-purchase-order"></a><span data-ttu-id="f94d6-177">To create the purchase order</span><span class="sxs-lookup"><span data-stu-id="f94d6-177">To create the purchase order</span></span>  

1.  <span data-ttu-id="f94d6-178">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f94d6-178">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f94d6-179">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="f94d6-179">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="f94d6-180">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span><span class="sxs-lookup"><span data-stu-id="f94d6-180">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span></span>  

    |<span data-ttu-id="f94d6-181">Item</span><span class="sxs-lookup"><span data-stu-id="f94d6-181">Item</span></span>|<span data-ttu-id="f94d6-182">Location code</span><span class="sxs-lookup"><span data-stu-id="f94d6-182">Location code</span></span>|<span data-ttu-id="f94d6-183">Bin code</span><span class="sxs-lookup"><span data-stu-id="f94d6-183">Bin code</span></span>|<span data-ttu-id="f94d6-184">Quantity</span><span class="sxs-lookup"><span data-stu-id="f94d6-184">Quantity</span></span>|  
    |----------|-------------------|--------------|--------------|  
    |<span data-ttu-id="f94d6-185">LS_75</span><span class="sxs-lookup"><span data-stu-id="f94d6-185">LS_75</span></span>|<span data-ttu-id="f94d6-186">SILVER</span><span class="sxs-lookup"><span data-stu-id="f94d6-186">SILVER</span></span>|<span data-ttu-id="f94d6-187">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="f94d6-187">S-01-0001</span></span>|<span data-ttu-id="f94d6-188">10</span><span class="sxs-lookup"><span data-stu-id="f94d6-188">10</span></span>|  
    |<span data-ttu-id="f94d6-189">LS-81</span><span class="sxs-lookup"><span data-stu-id="f94d6-189">LS-81</span></span>|<span data-ttu-id="f94d6-190">SILVER</span><span class="sxs-lookup"><span data-stu-id="f94d6-190">SILVER</span></span>|<span data-ttu-id="f94d6-191">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="f94d6-191">S-01-0001</span></span>|<span data-ttu-id="f94d6-192">30</span><span class="sxs-lookup"><span data-stu-id="f94d6-192">30</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="f94d6-193">The bin code is entered automatically according to the setup that you performed in the “Setting up the Location” section.</span><span class="sxs-lookup"><span data-stu-id="f94d6-193">The bin code is entered automatically according to the setup that you performed in the “Setting up the Location” section.</span></span>  

    <span data-ttu-id="f94d6-194">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span><span class="sxs-lookup"><span data-stu-id="f94d6-194">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span></span>  

4.  <span data-ttu-id="f94d6-195">Choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="f94d6-195">Choose the **Release** action.</span></span>  

    <span data-ttu-id="f94d6-196">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span><span class="sxs-lookup"><span data-stu-id="f94d6-196">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span></span>  

## <a name="receiving-and-putting-the-items-away"></a><span data-ttu-id="f94d6-197">Receiving and Putting the Items Away</span><span class="sxs-lookup"><span data-stu-id="f94d6-197">Receiving and Putting the Items Away</span></span>  
<span data-ttu-id="f94d6-198">On the **Inventory Put-away** page, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span><span class="sxs-lookup"><span data-stu-id="f94d6-198">On the **Inventory Put-away** page, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span></span>  

### <a name="to-receive-and-put-the-items-away"></a><span data-ttu-id="f94d6-199">To receive and put the items away</span><span class="sxs-lookup"><span data-stu-id="f94d6-199">To receive and put the items away</span></span>  

1.  <span data-ttu-id="f94d6-200">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Put-aways**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f94d6-200">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Put-aways**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f94d6-201">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="f94d6-201">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="f94d6-202">Select the **Source Document** field, and then select **Purchase Order**.</span><span class="sxs-lookup"><span data-stu-id="f94d6-202">Select the **Source Document** field, and then select **Purchase Order**.</span></span>  
4.  <span data-ttu-id="f94d6-203">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="f94d6-203">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="f94d6-204">Alternatively, on the **Actions** tab, in the **Functions** group, choose **Get Source Document**, and then select the purchase order.</span><span class="sxs-lookup"><span data-stu-id="f94d6-204">Alternatively, on the **Actions** tab, in the **Functions** group, choose **Get Source Document**, and then select the purchase order.</span></span>  

5.  <span data-ttu-id="f94d6-205">Choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="f94d6-205">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="f94d6-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span><span class="sxs-lookup"><span data-stu-id="f94d6-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span></span>  

6.  <span data-ttu-id="f94d6-207">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="f94d6-207">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="f94d6-208">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span><span class="sxs-lookup"><span data-stu-id="f94d6-208">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f94d6-209">See Also</span><span class="sxs-lookup"><span data-stu-id="f94d6-209">See Also</span></span>  
 <span data-ttu-id="f94d6-210">[Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span><span class="sxs-lookup"><span data-stu-id="f94d6-210">[Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span></span>  
 <span data-ttu-id="f94d6-211">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span><span class="sxs-lookup"><span data-stu-id="f94d6-211">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span></span>  
 <span data-ttu-id="f94d6-212">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="f94d6-212">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="f94d6-213">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span><span class="sxs-lookup"><span data-stu-id="f94d6-213">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span></span>  
 <span data-ttu-id="f94d6-214">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="f94d6-214">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="f94d6-215">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span><span class="sxs-lookup"><span data-stu-id="f94d6-215">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span></span>  
 [<span data-ttu-id="f94d6-216">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="f94d6-216">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="f94d6-217">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f94d6-217">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>