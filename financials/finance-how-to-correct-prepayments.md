---
title: How to Correct Prepayments | Microsoft Docs
description: You can make a correction to an order after you have posted a prepayment invoice for the order. You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/04/2017
ms.author: sgroespe
ms.openlocfilehash: 66dfe8f3da647208deae938ddf1c0db0a2b058c1
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "244459"
---
# <a name="correct-prepayments"></a><span data-ttu-id="50610-104">Correct Prepayments</span><span class="sxs-lookup"><span data-stu-id="50610-104">Correct Prepayments</span></span>
<span data-ttu-id="50610-105">You can make a correction to an order after you have posted a prepayment invoice for the order.</span><span class="sxs-lookup"><span data-stu-id="50610-105">You can make a correction to an order after you have posted a prepayment invoice for the order.</span></span> <span data-ttu-id="50610-106">You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.</span><span class="sxs-lookup"><span data-stu-id="50610-106">You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.</span></span>  

## <a name="to-correct-a-prepayment"></a><span data-ttu-id="50610-107">To correct a prepayment</span><span class="sxs-lookup"><span data-stu-id="50610-107">To correct a prepayment</span></span>
<span data-ttu-id="50610-108">The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.</span><span class="sxs-lookup"><span data-stu-id="50610-108">The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.</span></span>  
1. <span data-ttu-id="50610-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="50610-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="50610-110">Open the relevant sales order.</span><span class="sxs-lookup"><span data-stu-id="50610-110">Open the relevant sales order.</span></span>
3. <span data-ttu-id="50610-111">Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.</span><span class="sxs-lookup"><span data-stu-id="50610-111">Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.</span></span>  
4. <span data-ttu-id="50610-112">In the **Sales Credit Memo** window, proceed to correct the relevant entries, as for any sales credit memo.</span><span class="sxs-lookup"><span data-stu-id="50610-112">In the **Sales Credit Memo** window, proceed to correct the relevant entries, as for any sales credit memo.</span></span> <span data-ttu-id="50610-113">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="50610-113">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>     

    > [!NOTE]  
    > <span data-ttu-id="50610-114">To Reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.</span><span class="sxs-lookup"><span data-stu-id="50610-114">To Reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.</span></span>

5. <span data-ttu-id="50610-115">To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="50610-115">To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.</span></span>  
6. <span data-ttu-id="50610-116">To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="50610-116">To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice.</span></span> <span data-ttu-id="50610-117">A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.</span><span class="sxs-lookup"><span data-stu-id="50610-117">A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="50610-118">See Also</span><span class="sxs-lookup"><span data-stu-id="50610-118">See Also</span></span>  
[<span data-ttu-id="50610-119">Invoicing Prepayments</span><span class="sxs-lookup"><span data-stu-id="50610-119">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="50610-120">Walkthrough: Setting Up and Invoicing Sales Prepayments</span><span class="sxs-lookup"><span data-stu-id="50610-120">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="50610-121">Finance</span><span class="sxs-lookup"><span data-stu-id="50610-121">Finance</span></span>](finance.md)  
<span data-ttu-id="50610-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="50610-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>