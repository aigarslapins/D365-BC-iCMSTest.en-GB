---
title: How to Combine Receipts | Microsoft Docs
description: If you want to invoice more than one purchase receipt at a time, you can use the Combine Receipts function.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/14/2017
ms.author: sgroespe
ms.openlocfilehash: 08e401d2bc5f464a1560219aab4840d2392605fd
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "244765"
---
# <a name="combine-receipts-on-a-single-invoice"></a>Combine Receipts on a Single Invoice
If you want to invoice more than one purchase receipt at a time, you can use the **Combine Receipts** function.  

Before you can create a combined purchase receipt, more than one receipt from the same vendor in the same currency must be posted. In other words, you must have filled in two or more purchase orders and posted them as received, but not invoiced.  

When purchase receipts are combined on an invoice and posted, then a posted purchase invoice is created for the invoiced lines. The **Quantity Invoiced** field on the originating purchase order, or blanket purchase order, is updated based on the invoiced quantity. However, this original purchase document is not deleted, even if it has been fully received and invoiced, and you must therefore delete the purchase document.  

## <a name="to-combine-receipts"></a>To combine receipts  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.  
2. Choose the **New** action. For more information, see [Record Purchases](purchasing-how-record-purchases.md).  
3. On the **Lines** FastTab, choose the **Get Receipt Lines** action.  
4. Select multiple receipt lines that you want to include in the invoice.  

    If an incorrect receipt line was selected or you want to start over, you can just delete the lines on the purchase invoice and then use the **Get Receipt Lines** function again.  
5. To post the invoice, choose the **Post** action.  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a>To remove open purchase orders after combined receipt posting  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Purchase Orders**, and select the related link.  
2. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].
3. Choose the **OK** button.  

Alternatively, delete the individual orders manually.

Repeat steps 1 through 3 for any other affected documents, such as blanket purchase orders.

## <a name="see-also"></a>See Also  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
