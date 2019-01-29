---
title: Design Details - Warehouse Overview | Microsoft Docs
description: To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse. This is managed in the **Warehouse Entry** table. Each transaction is stored in a warehouse register.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/19/2018
ms.author: sgroespe
ms.openlocfilehash: 2d1fc180b971a7a0003847ea6b5830cc124cf5c7
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "263307"
---
# <a name="design-details-warehouse-overview"></a><span data-ttu-id="3cb12-105">Design Details: Warehouse Overview</span><span class="sxs-lookup"><span data-stu-id="3cb12-105">Design Details: Warehouse Overview</span></span>
<span data-ttu-id="3cb12-106">To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="3cb12-106">To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse.</span></span> <span data-ttu-id="3cb12-107">This is managed in the **Warehouse Entry** table.</span><span class="sxs-lookup"><span data-stu-id="3cb12-107">This is managed in the **Warehouse Entry** table.</span></span> <span data-ttu-id="3cb12-108">Each transaction is stored in a warehouse register.</span><span class="sxs-lookup"><span data-stu-id="3cb12-108">Each transaction is stored in a warehouse register.</span></span>  

<span data-ttu-id="3cb12-109">Warehouse documents and a warehouse journal are used to register item movements in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="3cb12-109">Warehouse documents and a warehouse journal are used to register item movements in the warehouse.</span></span> <span data-ttu-id="3cb12-110">Every time that an item in the warehouse is moved, received, put away, picked, shipped, or adjusted, warehouse entries are registered to store the physical information about zone, bin, and quantity.</span><span class="sxs-lookup"><span data-stu-id="3cb12-110">Every time that an item in the warehouse is moved, received, put away, picked, shipped, or adjusted, warehouse entries are registered to store the physical information about zone, bin, and quantity.</span></span>

<span data-ttu-id="3cb12-111">The **Bin Content** table is used to handle all the different dimensions of the contents of a bin per item, such as unit of measure, maximum quantity, and minimum quantity.</span><span class="sxs-lookup"><span data-stu-id="3cb12-111">The **Bin Content** table is used to handle all the different dimensions of the contents of a bin per item, such as unit of measure, maximum quantity, and minimum quantity.</span></span> <span data-ttu-id="3cb12-112">The **Bin Content** table also contains flow fields to the warehouse entries, warehouse instructions, and warehouse journal lines, which ensures that the availability of an item per bin and a bin for an item can be calculated quickly.</span><span class="sxs-lookup"><span data-stu-id="3cb12-112">The **Bin Content** table also contains flow fields to the warehouse entries, warehouse instructions, and warehouse journal lines, which ensures that the availability of an item per bin and a bin for an item can be calculated quickly.</span></span> <span data-ttu-id="3cb12-113">For more information, see [Design Details: Availability in the Warehouse](design-details-availability-in-the-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="3cb12-113">For more information, see [Design Details: Availability in the Warehouse](design-details-availability-in-the-warehouse.md).</span></span>  

<span data-ttu-id="3cb12-114">When item postings occur outside the warehouse module, a default adjustment bin per location is used to synchronise warehouse entries with inventory entries.</span><span class="sxs-lookup"><span data-stu-id="3cb12-114">When item postings occur outside the warehouse module, a default adjustment bin per location is used to synchronize warehouse entries with inventory entries.</span></span> <span data-ttu-id="3cb12-115">During physical inventory of the warehouse, any differences between the calculated and counted quantities are recorded in the adjustment bin and then posted as correcting item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="3cb12-115">During physical inventory of the warehouse, any differences between the calculated and counted quantities are recorded in the adjustment bin and then posted as correcting item ledger entries.</span></span> <span data-ttu-id="3cb12-116">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="3cb12-116">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span></span>  

<span data-ttu-id="3cb12-117">The following illustration outlines typical warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="3cb12-117">The following illustration outlines typical warehouse flows.</span></span>  

<span data-ttu-id="3cb12-118">![Overview of warehouse processes](media/design_details_warehouse_management_overview.png "Overview of warehouse processes")</span><span class="sxs-lookup"><span data-stu-id="3cb12-118">![Overview of warehouse processes](media/design_details_warehouse_management_overview.png "Overview of warehouse processes")</span></span>  

## <a name="basic-or-advanced-warehousing"></a><span data-ttu-id="3cb12-119">Basic or Advanced Warehousing</span><span class="sxs-lookup"><span data-stu-id="3cb12-119">Basic or Advanced Warehousing</span></span>  
<span data-ttu-id="3cb12-120">Warehouse functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)] can be implemented in different complexity levels, depending on a company’s processes and order volume.</span><span class="sxs-lookup"><span data-stu-id="3cb12-120">Warehouse functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)] can be implemented in different complexity levels, depending on a company’s processes and order volume.</span></span> <span data-ttu-id="3cb12-121">The main difference is that activities are performed order-by-order in basic warehousing when they are consolidated for multiple orders in advanced warehousing.</span><span class="sxs-lookup"><span data-stu-id="3cb12-121">The main difference is that activities are performed order-by-order in basic warehousing when they are consolidated for multiple orders in advanced warehousing.</span></span>  

 <span data-ttu-id="3cb12-122">To differentiate between the different complexity levels, this documentation refers to two general denominations, Basic and Advanced Warehousing.</span><span class="sxs-lookup"><span data-stu-id="3cb12-122">To differentiate between the different complexity levels, this documentation refers to two general denominations, Basic and Advanced Warehousing.</span></span> <span data-ttu-id="3cb12-123">This simple differentiation covers several different complexity levels as defined by product granules and location setup, each supported by different UI documents.</span><span class="sxs-lookup"><span data-stu-id="3cb12-123">This simple differentiation covers several different complexity levels as defined by product granules and location setup, each supported by different UI documents.</span></span> <span data-ttu-id="3cb12-124">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="3cb12-124">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="3cb12-125">The most advanced level of warehousing is referred to as “WMS installations” in this documentation, since this level requires the most advanced granule, Warehouse Management Systems.</span><span class="sxs-lookup"><span data-stu-id="3cb12-125">The most advanced level of warehousing is referred to as “WMS installations” in this documentation, since this level requires the most advanced granule, Warehouse Management Systems.</span></span>  

 <span data-ttu-id="3cb12-126">The following different UI documents are used in basic and advanced warehousing.</span><span class="sxs-lookup"><span data-stu-id="3cb12-126">The following different UI documents are used in basic and advanced warehousing.</span></span>  

## <a name="basic-ui-documents"></a><span data-ttu-id="3cb12-127">Basic UI Documents</span><span class="sxs-lookup"><span data-stu-id="3cb12-127">Basic UI Documents</span></span>  

-   <span data-ttu-id="3cb12-128">**Inventory Put-away**</span><span class="sxs-lookup"><span data-stu-id="3cb12-128">**Inventory Put-away**</span></span>  
-   <span data-ttu-id="3cb12-129">**Inventory Pick**</span><span class="sxs-lookup"><span data-stu-id="3cb12-129">**Inventory Pick**</span></span>  
-   <span data-ttu-id="3cb12-130">**Inventory Movement**</span><span class="sxs-lookup"><span data-stu-id="3cb12-130">**Inventory Movement**</span></span>  
-   <span data-ttu-id="3cb12-131">**Item Journal**</span><span class="sxs-lookup"><span data-stu-id="3cb12-131">**Item Journal**</span></span>  
-   <span data-ttu-id="3cb12-132">**Item Reclassification Journal**</span><span class="sxs-lookup"><span data-stu-id="3cb12-132">**Item Reclassification Journal**</span></span>  
-   <span data-ttu-id="3cb12-133">(Various reports)</span><span class="sxs-lookup"><span data-stu-id="3cb12-133">(Various reports)</span></span>  

## <a name="advanced-ui-documents"></a><span data-ttu-id="3cb12-134">Advanced UI Documents</span><span class="sxs-lookup"><span data-stu-id="3cb12-134">Advanced UI Documents</span></span>  

-   <span data-ttu-id="3cb12-135">**Warehouse Receipt**</span><span class="sxs-lookup"><span data-stu-id="3cb12-135">**Warehouse Receipt**</span></span>  
-   <span data-ttu-id="3cb12-136">**Put-away Worksheet**</span><span class="sxs-lookup"><span data-stu-id="3cb12-136">**Put-away Worksheet**</span></span>  
-   <span data-ttu-id="3cb12-137">**Warehouse Put-away**</span><span class="sxs-lookup"><span data-stu-id="3cb12-137">**Warehouse Put-away**</span></span>  
-   <span data-ttu-id="3cb12-138">**Pick Worksheet**</span><span class="sxs-lookup"><span data-stu-id="3cb12-138">**Pick Worksheet**</span></span>  
-   <span data-ttu-id="3cb12-139">**Warehouse Pick**</span><span class="sxs-lookup"><span data-stu-id="3cb12-139">**Warehouse Pick**</span></span>  
-   <span data-ttu-id="3cb12-140">**Movement Worksheet**</span><span class="sxs-lookup"><span data-stu-id="3cb12-140">**Movement Worksheet**</span></span>  
-   <span data-ttu-id="3cb12-141">**Warehouse Movement**</span><span class="sxs-lookup"><span data-stu-id="3cb12-141">**Warehouse Movement**</span></span>  
-   <span data-ttu-id="3cb12-142">**Internal Whse. Pick**</span><span class="sxs-lookup"><span data-stu-id="3cb12-142">**Internal Whse. Pick**</span></span>  
-   <span data-ttu-id="3cb12-143">**Internal Whse. Put-away**</span><span class="sxs-lookup"><span data-stu-id="3cb12-143">**Internal Whse. Put-away**</span></span>  
-   <span data-ttu-id="3cb12-144">**Bin Creation Worksheet**</span><span class="sxs-lookup"><span data-stu-id="3cb12-144">**Bin Creation Worksheet**</span></span>  
-   <span data-ttu-id="3cb12-145">**Bin Content Creation Worksheet**</span><span class="sxs-lookup"><span data-stu-id="3cb12-145">**Bin Content Creation Worksheet**</span></span>  
-   <span data-ttu-id="3cb12-146">**Whse. Item Journal**</span><span class="sxs-lookup"><span data-stu-id="3cb12-146">**Whse. Item Journal**</span></span>  
-   <span data-ttu-id="3cb12-147">**Whse. Item Reclass. Journal**</span><span class="sxs-lookup"><span data-stu-id="3cb12-147">**Whse. Item Reclass. Journal**</span></span>  
-   <span data-ttu-id="3cb12-148">(Various reports)</span><span class="sxs-lookup"><span data-stu-id="3cb12-148">(Various reports)</span></span>  

<span data-ttu-id="3cb12-149">For more information about each document, see the respective page topics.</span><span class="sxs-lookup"><span data-stu-id="3cb12-149">For more information about each document, see the respective page topics.</span></span>  

### <a name="terminology"></a><span data-ttu-id="3cb12-150">Terminology</span><span class="sxs-lookup"><span data-stu-id="3cb12-150">Terminology</span></span>  
<span data-ttu-id="3cb12-151">To align with the financial concepts of purchases and sales, [!INCLUDE[d365fin](includes/d365fin_md.md)] warehouse documentation refers to the following terms for item flow in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="3cb12-151">To align with the financial concepts of purchases and sales, [!INCLUDE[d365fin](includes/d365fin_md.md)] warehouse documentation refers to the following terms for item flow in the warehouse.</span></span>  

|<span data-ttu-id="3cb12-152">Term</span><span class="sxs-lookup"><span data-stu-id="3cb12-152">Term</span></span>|<span data-ttu-id="3cb12-153">Description</span><span class="sxs-lookup"><span data-stu-id="3cb12-153">Description</span></span>|  
|----------|---------------------------------------|  
|<span data-ttu-id="3cb12-154">Inbound flow</span><span class="sxs-lookup"><span data-stu-id="3cb12-154">Inbound flow</span></span>|<span data-ttu-id="3cb12-155">Items moving into the warehouse location, such as purchases and inbound transfers.</span><span class="sxs-lookup"><span data-stu-id="3cb12-155">Items moving into the warehouse location, such as purchases and inbound transfers.</span></span>|  
|<span data-ttu-id="3cb12-156">Internal flow</span><span class="sxs-lookup"><span data-stu-id="3cb12-156">Internal flow</span></span>|<span data-ttu-id="3cb12-157">Items moving inside the warehouse location, such as production components and output.</span><span class="sxs-lookup"><span data-stu-id="3cb12-157">Items moving inside the warehouse location, such as production components and output.</span></span>|  
|<span data-ttu-id="3cb12-158">Outbound flow</span><span class="sxs-lookup"><span data-stu-id="3cb12-158">Outbound flow</span></span>|<span data-ttu-id="3cb12-159">Items moving out of the warehouse location, such as sales and outbound transfers.</span><span class="sxs-lookup"><span data-stu-id="3cb12-159">Items moving out of the warehouse location, such as sales and outbound transfers.</span></span>|  

## <a name="see-also"></a><span data-ttu-id="3cb12-160">See Also</span><span class="sxs-lookup"><span data-stu-id="3cb12-160">See Also</span></span>  
 [<span data-ttu-id="3cb12-161">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="3cb12-161">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)