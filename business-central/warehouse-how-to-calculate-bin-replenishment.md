---
title: How to Calculate Bin Replenishment | Microsoft Docs
description: When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.
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
ms.openlocfilehash: 9708b248eb9e9f8f1f0e14f9b8d9f02ea84767fa
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "256994"
---
# <a name="calculate-bin-replenishment"></a><span data-ttu-id="c68a1-103">Calculate Bin Replenishment</span><span class="sxs-lookup"><span data-stu-id="c68a1-103">Calculate Bin Replenishment</span></span>
<span data-ttu-id="c68a1-104">When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.</span><span class="sxs-lookup"><span data-stu-id="c68a1-104">When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.</span></span> <span data-ttu-id="c68a1-105">Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings.</span><span class="sxs-lookup"><span data-stu-id="c68a1-105">Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings.</span></span> <span data-ttu-id="c68a1-106">Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.</span><span class="sxs-lookup"><span data-stu-id="c68a1-106">Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.</span></span>  

<span data-ttu-id="c68a1-107">But inventory does not always arrive in a steady trickle.</span><span class="sxs-lookup"><span data-stu-id="c68a1-107">But inventory does not always arrive in a steady trickle.</span></span> <span data-ttu-id="c68a1-108">Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost.</span><span class="sxs-lookup"><span data-stu-id="c68a1-108">Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost.</span></span> <span data-ttu-id="c68a1-109">Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.</span><span class="sxs-lookup"><span data-stu-id="c68a1-109">Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.</span></span>  

<span data-ttu-id="c68a1-110">It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.</span><span class="sxs-lookup"><span data-stu-id="c68a1-110">It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.</span></span>  

<span data-ttu-id="c68a1-111">Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.</span><span class="sxs-lookup"><span data-stu-id="c68a1-111">Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.</span></span>  

## <a name="to-replenish-pick-bins"></a><span data-ttu-id="c68a1-112">To replenish pick bins</span><span class="sxs-lookup"><span data-stu-id="c68a1-112">To replenish pick bins</span></span>  
1.  <span data-ttu-id="c68a1-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c68a1-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c68a1-114">Choose the **Calculate Bin Replenishment** action to open the report request page.</span><span class="sxs-lookup"><span data-stu-id="c68a1-114">Choose the **Calculate Bin Replenishment** action to open the report request page.</span></span>  
3.  <span data-ttu-id="c68a1-115">Fill in the batch job request page to limit the scope of the replenishment suggestions that will be calculated.</span><span class="sxs-lookup"><span data-stu-id="c68a1-115">Fill in the batch job request page to limit the scope of the replenishment suggestions that will be calculated.</span></span> <span data-ttu-id="c68a1-116">For example, you might be concerned with particular items, zones, or bins.</span><span class="sxs-lookup"><span data-stu-id="c68a1-116">For example, you might be concerned with particular items, zones, or bins.</span></span>  
4.  <span data-ttu-id="c68a1-117">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="c68a1-117">Choose the **OK** button.</span></span> <span data-ttu-id="c68a1-118">Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.</span><span class="sxs-lookup"><span data-stu-id="c68a1-118">Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.</span></span>  
5.  <span data-ttu-id="c68a1-119">If you want to perform all the suggested replenishments, choose the **Create Movement** action.</span><span class="sxs-lookup"><span data-stu-id="c68a1-119">If you want to perform all the suggested replenishments, choose the **Create Movement** action.</span></span> <span data-ttu-id="c68a1-120">Employees can now find instructions in the **Movements** menu item, carry them out and register them.</span><span class="sxs-lookup"><span data-stu-id="c68a1-120">Employees can now find instructions in the **Movements** menu item, carry them out and register them.</span></span>  
6.  <span data-ttu-id="c68a1-121">If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.</span><span class="sxs-lookup"><span data-stu-id="c68a1-121">If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.</span></span>  

<span data-ttu-id="c68a1-122">The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.</span><span class="sxs-lookup"><span data-stu-id="c68a1-122">The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c68a1-123">If the following conditions are met for an item:</span><span class="sxs-lookup"><span data-stu-id="c68a1-123">If the following conditions are met for an item:</span></span>  
>   
>  -   <span data-ttu-id="c68a1-124">The item has an expiration date, and</span><span class="sxs-lookup"><span data-stu-id="c68a1-124">The item has an expiration date, and</span></span>  
> -   <span data-ttu-id="c68a1-125">The **Pick According to FEFO** field on the location card is selected, and</span><span class="sxs-lookup"><span data-stu-id="c68a1-125">The **Pick According to FEFO** field on the location card is selected, and</span></span>  
> -   <span data-ttu-id="c68a1-126">You use the **Calculate Bin Replenishment** functionality</span><span class="sxs-lookup"><span data-stu-id="c68a1-126">You use the **Calculate Bin Replenishment** functionality</span></span>  
>   
>  <span data-ttu-id="c68a1-127">then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.</span><span class="sxs-lookup"><span data-stu-id="c68a1-127">then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c68a1-128">See Also</span><span class="sxs-lookup"><span data-stu-id="c68a1-128">See Also</span></span>  
[<span data-ttu-id="c68a1-129">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="c68a1-129">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="c68a1-130">Picking by FEFO</span><span class="sxs-lookup"><span data-stu-id="c68a1-130">Picking by FEFO</span></span>](warehouse-picking-by-fefo.md)  
[<span data-ttu-id="c68a1-131">Inventory</span><span class="sxs-lookup"><span data-stu-id="c68a1-131">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="c68a1-132">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="c68a1-132">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="c68a1-133">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="c68a1-133">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="c68a1-134">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="c68a1-134">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="c68a1-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c68a1-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>