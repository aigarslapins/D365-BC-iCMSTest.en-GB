---
title: How to Sell Inventory Items in Assemble-to-Order Flows | Microsoft Docs
description: If the item is set up for card of assemble-to-order, then the default sales order process assumes that the item is not in inventory and must be assembled for that specific sales order. Therefore, a linked assembly order is automatically created when you add the item to a sales order line.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/15/2017
ms.author: sgroespe
ms.openlocfilehash: 84dd5eef99df9c5942a2c99ebe94860cb8be512a
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "246051"
---
# <a name="sell-inventory-items-in-assemble-to-order-flows"></a><span data-ttu-id="5cbe1-104">Sell Inventory Items in Assemble-to-Order Flows</span><span class="sxs-lookup"><span data-stu-id="5cbe1-104">Sell Inventory Items in Assemble-to-Order Flows</span></span>
<span data-ttu-id="5cbe1-105">If the **Assembly Policy** field on the item card of an assembly item contains **Assemble-to-Order**, then the default sales order process assumes that the item is not in inventory and must be assembled for that specific sales order.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-105">If the **Assembly Policy** field on the item card of an assembly item contains **Assemble-to-Order**, then the default sales order process assumes that the item is not in inventory and must be assembled for that specific sales order.</span></span> <span data-ttu-id="5cbe1-106">Therefore, a linked assembly order is automatically created when you add the item to a sales order line.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-106">Therefore, a linked assembly order is automatically created when you add the item to a sales order line.</span></span> <span data-ttu-id="5cbe1-107">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="5cbe1-107">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span> <span data-ttu-id="5cbe1-108">However, if a part of the sales order quantity is already available in inventory, then you can decrease the assembly order quantity by changing the **Qty. to Assemble to Order** field on the sales order line.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-108">However, if a part of the sales order quantity is already available in inventory, then you can decrease the assembly order quantity by changing the **Qty. to Assemble to Order** field on the sales order line.</span></span>  

<span data-ttu-id="5cbe1-109">This scenario is rare because assemble-to-order items are expected to always be customised, and the chance that they are in inventory in the configuration that is requested by another customer is low.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-109">This scenario is rare because assemble-to-order items are expected to always be customized, and the chance that they are in inventory in the configuration that is requested by another customer is low.</span></span> <span data-ttu-id="5cbe1-110">However, if a company does have assemble-to-order quantities in inventory because of returns or order cancellations, then these quantities should be picked and sold before new ones are assembled.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-110">However, if a company does have assemble-to-order quantities in inventory because of returns or order cancellations, then these quantities should be picked and sold before new ones are assembled.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5cbe1-111">No functionality exists on sales orders that automatically alerts or helps you deduct assembly order quantities that are already available.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-111">No functionality exists on sales orders that automatically alerts or helps you deduct assembly order quantities that are already available.</span></span> <span data-ttu-id="5cbe1-112">Instead, you must monitor availability information, such as in the **Sales Line Details** FactBox.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-112">Instead, you must monitor availability information, such as in the **Sales Line Details** FactBox.</span></span>  

<span data-ttu-id="5cbe1-113">Similar functionality is available when you are selling assembly items from inventory and a part or all of the quantity is unavailable and can be supplied by an assembly order.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-113">Similar functionality is available when you are selling assembly items from inventory and a part or all of the quantity is unavailable and can be supplied by an assembly order.</span></span> <span data-ttu-id="5cbe1-114">For more information, see [Sell Assemble-to-Order Items and Inventory Items Together](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).</span><span class="sxs-lookup"><span data-stu-id="5cbe1-114">For more information, see [Sell Assemble-to-Order Items and Inventory Items Together](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5cbe1-115">Certain rules apply to the **Qty. to Ship** field on sales order lines that contain a combination of assemble-to-order quantities and inventory quantities.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-115">Certain rules apply to the **Qty. to Ship** field on sales order lines that contain a combination of assemble-to-order quantities and inventory quantities.</span></span> <span data-ttu-id="5cbe1-116">For more information, see the Combination Scenarios section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).</span><span class="sxs-lookup"><span data-stu-id="5cbe1-116">For more information, see the Combination Scenarios section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).</span></span>  

<span data-ttu-id="5cbe1-117">In this procedure, you replace assemble-to-order quantities with inventory quantities on a sales order line.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-117">In this procedure, you replace assemble-to-order quantities with inventory quantities on a sales order line.</span></span> <span data-ttu-id="5cbe1-118">The steps include detecting that availability exists, deducting that quantity from the linked assembly order, and then reserving the inventory quantity to make sure that it is picked and shipped for the order.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-118">The steps include detecting that availability exists, deducting that quantity from the linked assembly order, and then reserving the inventory quantity to make sure that it is picked and shipped for the order.</span></span>  

## <a name="to-sell-inventory-items-in-assemble-to-order-flows"></a><span data-ttu-id="5cbe1-119">To sell inventory items in assemble-to-order flows</span><span class="sxs-lookup"><span data-stu-id="5cbe1-119">To sell inventory items in assemble-to-order flows</span></span>  
1.  <span data-ttu-id="5cbe1-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5cbe1-121">Create a sales order.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-121">Create a sales order.</span></span> <span data-ttu-id="5cbe1-122">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="5cbe1-122">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>  
3.  <span data-ttu-id="5cbe1-123">On a sales order line for an assemble-to-order item, in the **Quantity** field, enter the demanded quantity.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-123">On a sales order line for an assemble-to-order item, in the **Quantity** field, enter the demanded quantity.</span></span>  
4.  <span data-ttu-id="5cbe1-124">In the **Sales Line Details** FactBox, determine if all or some of the demanded quantity is available.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-124">In the **Sales Line Details** FactBox, determine if all or some of the demanded quantity is available.</span></span>  
5.  <span data-ttu-id="5cbe1-125">In the **Qty. to Assemble to Order** field, deduct the available quantity so that only the unavailable quantity is assembled to the order.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-125">In the **Qty. to Assemble to Order** field, deduct the available quantity so that only the unavailable quantity is assembled to the order.</span></span> <span data-ttu-id="5cbe1-126">The **Reserved Quantity** field is decreased accordingly to reflect that the order-to-order link, or reservation, only applies to the quantity to be assembled.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-126">The **Reserved Quantity** field is decreased accordingly to reflect that the order-to-order link, or reservation, only applies to the quantity to be assembled.</span></span>  
6.  <span data-ttu-id="5cbe1-127">On the **Lines** FastTab, choose **Functions**, and then choose the **Reserve** action.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-127">On the **Lines** FastTab, choose **Functions**, and then choose the **Reserve** action.</span></span>  
7.  <span data-ttu-id="5cbe1-128">In the **Reservation** window, select the item ledger entry line or lines that contain the available quantities, choose the **Reserve from Current Line** action, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-128">In the **Reservation** window, select the item ledger entry line or lines that contain the available quantities, choose the **Reserve from Current Line** action, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="5cbe1-129">In the **Sales Order** window, the **Reserved Quantity** field now shows that the whole order line quantity is reserved.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-129">In the **Sales Order** window, the **Reserved Quantity** field now shows that the whole order line quantity is reserved.</span></span> <span data-ttu-id="5cbe1-130">The **Qty. to Assemble to Order** field still reflects the subquantity that has to be assembled.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-130">The **Qty. to Assemble to Order** field still reflects the subquantity that has to be assembled.</span></span>  

8.  <span data-ttu-id="5cbe1-131">Release the sales order for picking of the inventory items and for assembly of the unavailable items.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-131">Release the sales order for picking of the inventory items and for assembly of the unavailable items.</span></span> <span data-ttu-id="5cbe1-132">For more information, see [Assemble Items](assembly-how-to-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="5cbe1-132">For more information, see [Assemble Items](assembly-how-to-assemble-items.md).</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="5cbe1-133">The **Bin Code** field on the sales order may be prefilled according to the **Assemble-to-Order Shpt. Bin Code** or the **From-Assembly Bin Code** field on the location card.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-133">The **Bin Code** field on the sales order may be prefilled according to the **Assemble-to-Order Shpt. Bin Code** or the **From-Assembly Bin Code** field on the location card.</span></span> <span data-ttu-id="5cbe1-134">In that case, the **Bin Code** field on the sales order line may be incorrect in this combination of assemble-to-order and assemble-to-stock quantities.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-134">In that case, the **Bin Code** field on the sales order line may be incorrect in this combination of assemble-to-order and assemble-to-stock quantities.</span></span> <span data-ttu-id="5cbe1-135">It is a good idea to look in the **Bin Code** field and ensure that the placement works for all quantities.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-135">It is a good idea to look in the **Bin Code** field and ensure that the placement works for all quantities.</span></span> <span data-ttu-id="5cbe1-136">Alternatively, enter the two different quantities on separate sales order lines.</span><span class="sxs-lookup"><span data-stu-id="5cbe1-136">Alternatively, enter the two different quantities on separate sales order lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5cbe1-137">See Also</span><span class="sxs-lookup"><span data-stu-id="5cbe1-137">See Also</span></span>  
[<span data-ttu-id="5cbe1-138">Assembly Management</span><span class="sxs-lookup"><span data-stu-id="5cbe1-138">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="5cbe1-139">Reserve Items</span><span class="sxs-lookup"><span data-stu-id="5cbe1-139">Reserve Items</span></span>](inventory-how-to-reserve-items.md)  
[<span data-ttu-id="5cbe1-140">Work with Bills of Material</span><span class="sxs-lookup"><span data-stu-id="5cbe1-140">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="5cbe1-141">Inventory</span><span class="sxs-lookup"><span data-stu-id="5cbe1-141">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="5cbe1-142">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5cbe1-142">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="5cbe1-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5cbe1-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>