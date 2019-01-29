---
title: Best practices for global planning setup | Microsoft Docs
description: The **Planning** FastTab in the **Manufacturing Setup** window contains several fields that define global rules for supply planning.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/08/2017
ms.author: sgroespe
ms.openlocfilehash: 9df3b119d4482b51ba79cea219dc74c058431e66
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "273775"
---
# <a name="setup-best-practices-global-planning-setup"></a>Setup Best Practices: Global Planning Setup
The **Planning** FastTab in the **Manufacturing Setup** window contains several fields that define global rules for supply planning.  

 The following table provides best practices on how to set up selected global planning parameter fields. For more information about a field, choose the link in the **Setup field** column.  


|        Setup field        |                                                          Best practice                                                           |                                                                     Comment                                                                     |
|---------------------------|----------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| Use Forecast on Locations |                                       Select if you have forecasts for specific locations.                                       |                                                                                                                                                 |
|  Components at Location   |                        If items are not defined as SKUs, select the location code of your main warehouse.                        |                                          This also applies if you only use the requisition worksheet.                                           |
|   Blank Overflow Level    |              Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.               |                             Use only if you want to allow all or some of your items to overflow the reorder point.                              |
|  Default Dampener Period  | Set between 1D and 5D.<br /><br /> If new to planning in [!INCLUDE [d365fin](includes/d365fin_md.md)], then set a longer period. | When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions. |
| Default Dampener Quantity |                                       Set between 5 and 20 percent of the item’s lot size.                                       |                                                                                                                                                 |

## <a name="see-also"></a>See Also  
 [Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md)   
 [Design Details: Supply Planning](design-details-supply-planning.md)   
 [Set Up Complex Application Areas Using Best Practices](set-up-complex-application-areas-using-best-practices.md)  
 [Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
