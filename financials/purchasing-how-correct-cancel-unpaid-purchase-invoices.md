---
title: Amend or Cancel Unpaid Purchase Invoices | Microsoft Docs
description: Explains how to correct, cancel, or undo a posted purchase invoice and automatically create a purchase credit memo.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 08/01/2017
ms.author: sgroespe
ms.openlocfilehash: e534fb93c963964d787478b48257638e17311d9c
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "259584"
---
# <a name="correct-or-cancel-unpaid-purchase-invoices"></a><span data-ttu-id="2cebc-103">Correct or Cancel Unpaid Purchase Invoices</span><span class="sxs-lookup"><span data-stu-id="2cebc-103">Correct or Cancel Unpaid Purchase Invoices</span></span>
<span data-ttu-id="2cebc-104">You can correct or cancel a posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="2cebc-104">You can correct or cancel a posted purchase invoice.</span></span> <span data-ttu-id="2cebc-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span><span class="sxs-lookup"><span data-stu-id="2cebc-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span></span>

<span data-ttu-id="2cebc-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span><span class="sxs-lookup"><span data-stu-id="2cebc-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span></span> <span data-ttu-id="2cebc-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span><span class="sxs-lookup"><span data-stu-id="2cebc-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span></span> <span data-ttu-id="2cebc-108">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="2cebc-108">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span></span>

<span data-ttu-id="2cebc-109">In the **Posted Purchase Invoice** window, you can choose the **Correct** button or the **Cancel** button.</span><span class="sxs-lookup"><span data-stu-id="2cebc-109">In the **Posted Purchase Invoice** window, you can choose the **Correct** button or the **Cancel** button.</span></span> <span data-ttu-id="2cebc-110">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span><span class="sxs-lookup"><span data-stu-id="2cebc-110">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span></span> <span data-ttu-id="2cebc-111">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span><span class="sxs-lookup"><span data-stu-id="2cebc-111">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span></span> <span data-ttu-id="2cebc-112">In the following the use of **Correct** and **Cancel** is described.</span><span class="sxs-lookup"><span data-stu-id="2cebc-112">In the following the use of **Correct** and **Cancel** is described.</span></span>

## <a name="to-correct-a-posted-purchase-invoice"></a><span data-ttu-id="2cebc-113">To correct a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="2cebc-113">To correct a posted purchase invoice</span></span>
1. <span data-ttu-id="2cebc-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2cebc-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2cebc-115">Select the posted purchase invoice that you want to correct.</span><span class="sxs-lookup"><span data-stu-id="2cebc-115">Select the posted purchase invoice that you want to correct.</span></span>  

    > [!NOTE]  
   >   <span data-ttu-id="2cebc-116">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span><span class="sxs-lookup"><span data-stu-id="2cebc-116">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="2cebc-117">In the **Posted Purchase Invoice** window, choose **Correct**.</span><span class="sxs-lookup"><span data-stu-id="2cebc-117">In the **Posted Purchase Invoice** window, choose **Correct**.</span></span>

    <span data-ttu-id="2cebc-118">A new purchase invoice with the same information is created where you can make the correction.</span><span class="sxs-lookup"><span data-stu-id="2cebc-118">A new purchase invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="2cebc-119">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="2cebc-119">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span> <span data-ttu-id="2cebc-120">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="2cebc-120">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>

    <span data-ttu-id="2cebc-121">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="2cebc-121">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span>
4. <span data-ttu-id="2cebc-122">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="2cebc-122">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="to-cancel-a-posted-purchase-invoice"></a><span data-ttu-id="2cebc-123">To cancel a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="2cebc-123">To cancel a posted purchase invoice</span></span>
1. <span data-ttu-id="2cebc-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2cebc-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2cebc-125">Select the posted purchase invoice that you want to cancel.</span><span class="sxs-lookup"><span data-stu-id="2cebc-125">Select the posted purchase invoice that you want to cancel.</span></span>

    > [!NOTE]  
   >   <span data-ttu-id="2cebc-126">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span><span class="sxs-lookup"><span data-stu-id="2cebc-126">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="2cebc-127">In the **Posted Purchase Invoice** window, choose **Cancel**.</span><span class="sxs-lookup"><span data-stu-id="2cebc-127">In the **Posted Purchase Invoice** window, choose **Cancel**.</span></span>

    <span data-ttu-id="2cebc-128">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="2cebc-128">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span> <span data-ttu-id="2cebc-129">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="2cebc-129">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>
4. <span data-ttu-id="2cebc-130">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="2cebc-130">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="see-also"></a><span data-ttu-id="2cebc-131">See Also</span><span class="sxs-lookup"><span data-stu-id="2cebc-131">See Also</span></span>
[<span data-ttu-id="2cebc-132">Purchasing</span><span class="sxs-lookup"><span data-stu-id="2cebc-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="2cebc-133">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="2cebc-133">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
<span data-ttu-id="2cebc-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2cebc-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>