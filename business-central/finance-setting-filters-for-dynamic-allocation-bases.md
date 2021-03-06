---
title: Setting Filters for Dynamic Allocation Keys | Microsoft Docs
description: The dynamic allocation method is based on changeable values. For example, the number of employees in a cost centre or the items sold of a cost object in a specific time period. There are nine pre-defined allocation bases and twelve dynamic date ranges. You set different filters based on the allocation base.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-define-and-allocate-costs
ms.openlocfilehash: fcf97328900bb21a85be51452b9e86da8398d195
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "223115"
---
# <a name="setting-filters-for-dynamic-allocation-bases"></a>Setting Filters for Dynamic Allocation Bases
The dynamic allocation method is based on changeable values. For example, the number of employees in a cost centre or the items sold of a cost object in a specific time period. There are nine pre-defined allocation bases and twelve dynamic date ranges. You set different filters based on the allocation base.  

## <a name="setting-filters-for-dynamic-allocation-bases"></a>Setting Filters for Dynamic Allocation Bases  
 The following table shows which filters are possible for different allocation bases and which values are valid in the **No. Filter** and **Group Filter** fields. Press F1 in the **Date Filter Code** field to read detailed descriptions.  

|**Base**|**No. Filter**|**Date Filter Code**|**Cost Centre Filter**|**Cost Object Filter**|**Group Filter**|  
|--------------|----------------------------------------|----------------------------------------------|------------------------------------------------|------------------------------------------------|------------------------------------------|  
|G/L Entries|G/L Account|Yes|Yes|Yes|N/A|  
|G/L Budget Entries|G/L Account|Yes|Yes|Yes|G/L Budget Name|  
|Cost Type Entries|Cost Type|Yes|Yes|Yes|N/A|  
|Cost Budget Entries|Cost Type|Yes|Yes|Yes|Budget Name|  
|No of Employees|N/A|Yes|Yes|Yes|N/A|  
|Items Sold (Qty)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Purchased (Qty)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Sold (Amount)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Purchased (Amount)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  

## <a name="see-also"></a>See Also  
[Defining and Allocating Costs](finance-define-and-allocate-costs.md)
