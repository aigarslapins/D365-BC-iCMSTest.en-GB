---
title: Defining Cost Centres and Cost Objects for Chart of Accounts | Microsoft Docs
description: You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job. When you do the transfer, the system only transfers the entries that are already linked to a cost centre or a cost object. To establish a meaningful transfer, you must ensure that the cost centres and cost objects are correctly defined.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 0e3e84792314bf557a8be085b4d49067f0cd99ba
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "265203"
---
# <a name="defining-cost-centers-and-cost-objects-for-chart-of-accounts"></a>Defining Cost Centres and Cost Objects for Chart of Accounts
You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job. When you do the transfer, [!INCLUDE [d365fin](includes/d365fin_md.md)] only transfers the entries that are already linked to a cost center or a cost object. To establish a meaningful transfer, you must ensure that the cost centres and cost objects are correctly defined.  

## <a name="defining-default-dimension-values-for-general-ledger-accounts"></a>Defining Default Dimension Values for General Ledger Accounts  
For each general ledger account, you can define default dimension values in the **Default Dimension** table. The following example shows how to define that there should always be a DEPARTMENT cost centre, but never be a PROJECT cost object when posting to a general ledger account.  

|**Dimension Code**|**Value Posting**|  
|------------------------------------------|-----------------------------------------|  
|Department|Code Mandatory|  
|Project|No Code|  

## <a name="defining-dimension-values-for-overhead-costs-and-direct-costs"></a>Defining Dimension Values for Overhead Costs and Direct Costs  
 You can transfer overhead costs to a cost centre and direct costs to a cost object. The following table shows the optimal combination of the dimension setup values.  

|Transfer To|Cost Centre Posting|Cost Object Posting|  
|-----------------|-------------------------|-------------------------|  
|Cost Centre|Code Mandatory|No Code|  
|Cost Object|No Code|Code Mandatory|  

> [!NOTE]  
>  To make sure that the predefined cost center and cost object that you set up in the general ledger are automatically carried over to cost accounting, select the **Check G/L Postings** check box in the Cost Accounting Setup window.  

## <a name="see-also"></a>See Also  
[Accounting for Costs](finance-manage-cost-accounting.md)  
[Setting Up Cost Accounting](finance-set-up-cost-accounting.md)   
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
