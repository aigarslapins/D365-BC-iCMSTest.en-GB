---
title: Allocation Status and Repair Status | Microsoft Docs
description: Learn about the relationship between the repair status of service items and the allocation status of the allocation entries for them.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resources, allocation, status, repairs
ms.date: 10/01/2018
ms.author: bholtorf
ms.openlocfilehash: 932abf3ee69f429c322fe82e150fa7a8f4aef8e8
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "271912"
---
# <a name="allocation-status-and-repair-status-of-service-items"></a>Allocation Status and Repair Status of Service Items
The repair status of service items and the allocation status of the allocation entries for the service items have a certain relationship in Service Management. The allocation status changes when you change the repair status of the service item to **Finished** or **Partly Serviced** and when you convert a service quote to a service order. The repair status of the service item changes when you cancel the service item allocation or reallocate the service item to another resource. You can view the repair status of service items on the **Service Tasks** page and you can update the repair status in the **Repair Status Code** field on the **Service Item Worksheet** page. You can view the allocation status in the **Status** field on the **Resource Allocations** page.  
  
## <a name="changing-repair-status"></a>Changing Repair Status  
When you change the repair status of a service item on a service item line, there is a search for a corresponding allocation entry for this service item that has the status **Active**. If such an allocation entry is found, the status is updated in one of the following ways:  
  
* If you change the repair status to **Finished**, the allocation status is changed from **Active** to **Finished**.  
* If you change the repair status to **Partly Serviced**, that is, some of the service has been completed, or **Referred**, that is, no service has been done, the allocation status is changed from **Active** to **Reallocation Needed**.  
* When a service order allocation entry is created that indicates that no resource has been allocated, the **Status** field on the **Resource Allocation** page is set to **Nonactive**.  
* The allocation entry status is set to **Cancelled** when you reallocate the referred service item in the service order allocation entry, which indicates that the allocated resource or resource group has not attempted the service task.  
  
The allocation status reflects when the service process is finished, or when another resource is necessary in order to finish the service of the service item.  
  
## <a name="converting-service-quotes-to-service-orders"></a>Converting Service Quotes to Service Orders  
When you convert a service quote to a service order, the service order, the service items in the order and their allocation entries are updated in the following ways:  
  
* The repair status of the service items is changed to **Initial**.  
* The service order status is changed to **Pending**.  
* There is a search for allocation entries for all the service items in the service order that have the status **Active**. If such allocation entries are found, their allocation status is changed from **Active** to **Reallocation Needed**.  
  
## <a name="canceling-allocations"></a>Cancelling Allocations  
When you cancel an allocation for a service item, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the allocation status of the corresponding allocation entry from **Active** to **Reallocation Needed**.

The repair status of the service item in the allocation entry is updated in the following ways:  
  
* If the repair status is **Initial**, the repair status is changed to **Referred** (no service has been started).  
* If the repair status is **In Process**, the repair status is changed to **Partly Serviced** (some service has been completed).  
  
## <a name="reallocating-an-active-allocation-entry"></a>Reallocating an Active Allocation Entry  
When you reallocate a service item in an allocation entry that is **Active**, the allocation entry is updated in the following ways:  
  
* If service was started when the allocation was **Active** (that is, if the repair status of the service item in the entry was changed to **In Process**), the allocation status is changed from **Active** to **Finished**.  
* If service was not started when the allocation was **Active**, the allocation status is changed from **Active** to **Cancelled**.  
  
The repair status of the service item in the allocation entry is updated in the same way as if you had cancelled the allocation:  
  
* If the repair status is **Initial**, the repair status is changed to **Referred** (no service has been started).  
* If the repair status is **In Process**, the repair status is changed to **Partly Serviced** (some service has been completed).  
  
A new allocation entry that contains the new resource is created that has the status **Active**.  
  
## <a name="reallocating-a-service-item"></a>Reallocating a Service Item  
When you reallocate a service item in an allocation entry that has the status **Reallocation Needed**, the allocation entry is updated in the following ways:  
  
* If service was started when the allocation was **Active** (that is, if the repair status of the service item in the entry was changed to **In Process**), the allocation status is changed from **Reallocation Needed** to **Finished**.  
* If service was not started when the allocation was **Active**, the allocation status is changed from **Reallocation Needed** to **Cancelled**.  
  
A new allocation entry that contains the new resource is created that has the status **Active**.  
  
## <a name="see-also"></a>See Also  
[Set Up Resource Allocations](service-how-setup-resource-allocation.md)  
[Allocate Resources](service-how-to-allocate-resources.md)  
