---
title: Design Details - Item Tracking Availability | Microsoft Docs
description: The Item Tracking Lines and Item Tracking Summary pages provide dynamic availability information for serial or lot numbers. The purpose of this is to increase transparency for users on outbound documents, such as sales orders, by showing them which serial numbers or how many units of a lot number are currently assigned on other open documents. This reduces uncertainty that is caused by double allocation and instills confidence in order processors that the item tracking numbers and dates that they are promising on unposted sales orders can be fulfilled.
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
ms.openlocfilehash: b4d4112358943f3c5aad963e3c69efaec8304f46
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "236700"
---
# <a name="design-details-item-tracking-availability"></a>Design Details: Item Tracking Availability
The **Item Tracking Lines** and **Item Tracking Summary** pages provide dynamic availability information for serial or lot numbers. The purpose of this is to increase transparency for users on outbound documents, such as sales orders, by showing them which serial numbers or how many units of a lot number are currently assigned on other open documents. This reduces uncertainty that is caused by double allocation and instills confidence in order processors that the item tracking numbers and dates that they are promising on unposted sales orders can be fulfilled. For more information, see [Design Details: Item Tracking Lines Page](design-details-item-tracking-lines-window.md).  

 When you open the **Item Tracking Lines** page, availability data is retrieved from the **Item Ledger Entry** table and the **Reservation Entry** table, with no date filter. When you choose the **Serial No.** field or the **Lot No.** field, the **Item Tracking Summary** page opens and shows a summary of the item tracking information in the **Reservation Entry** table. The summary contains the following information about each serial or lot number on the item tracking line:  

|Field|Description|  
|---------------------------------|---------------------------------------|  
|**Total Quantity**|The total quantity of the serial or lot number that is currently in inventory.|  
|**Total Requested Quantity**|The total quantity of the serial or lot number that is currently requested in all documents.|  
|**Current Pending Quantity**|The quantity that is entered in the current instance of the **Item Tracking Lines** page but is not yet committed to the database.|  
|**Total Available Quantity**|The quantity of the serial or lot number that is available for the user to request.<br /><br /> This quantity is calculated from other fields on the page as follows:<br /><br /> total quantity – (total requested quantity + current pending quantity).|  

> [!NOTE]  
>  You can also see the information in the preceding table by using the **Select Entries** function on the **Item Tracking Lines** page.  

 To preserve database performance, availability data is only retrieved once from the database when you open the **Item Tracking Lines** page and when you use the **Refresh Availability** function on the page.  

## <a name="calculation-formula"></a>Calculation Formula  
 As described in the preceding table, the availability of a given serial or lot number is calculated as follows.  

 total available quantity = quantity in inventory – (all demands + quantity not yet committed to the database)  

> [!IMPORTANT]  
>  This formula implies that the serial or lot number availability calculation considers only inventory and ignores projected receipts. Accordingly, supply that is not yet posted to inventory does not affect item tracking availability, as opposed to regular item availability where projected receipts are included.  

## <a name="see-also"></a>See Also  
 [Design Details: Item Tracking](design-details-item-tracking.md)
