---
title: How to Assign Default Bins to Items | Microsoft Docs
description: If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier. When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.
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
ms.openlocfilehash: 290c26639234f3379fb4f9b6790fc511e17f683e
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "246285"
---
# <a name="assign-default-bins-to-items"></a>Assign Default Bins to Items
If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier. When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item. Default bins are defined on the **Bin Content** page.  

## <a name="to-assign-a-default-bin-to-an-item"></a>To assign a default bin to an item
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.  
2.  Fill in the bin code and item information for each bin that you would like to set up as a default for an item. Make sure to select the **Default** field.  
3.  Choose the **Create Bin Content** action. Default bins are now assigned for your item.  

> [!NOTE]  
>  When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.  

## <a name="to-change-the-default-bin-for-an-item"></a>To change the default bin for an item  
You may need to change the default bin assignment for an item or assign a default bin to a new item.    
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.  
2.  In the **Location Filter** field, select the appropriate location code.  
3.  Find the current default bin content entry for the item and clear the **Default Bin** check box.  
4.  Find the bin content line for the bin that you would like as the new default bin. Select the **Default Bin** check box.  

> [!NOTE]  
>  When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.  

## <a name="see-also"></a>See Also  
[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
