---
title: Understanding How To Post Purchase Documents | Microsoft Docs
description: Learn about the different posting functions to post purchase documents.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 05/12/2017
ms.author: solsen
ms.openlocfilehash: f49326c17d5c244668e329cd1fd59795802af69d
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "243679"
---
# <a name="posting-purchases"></a><span data-ttu-id="a42a2-103">Posting Purchases</span><span class="sxs-lookup"><span data-stu-id="a42a2-103">Posting Purchases</span></span>
<span data-ttu-id="a42a2-104">In the **Posting group** on a purchase document, you can choose between the following posting functions:</span><span class="sxs-lookup"><span data-stu-id="a42a2-104">In the **Posting group** on a purchase document, you can choose between the following posting functions:</span></span>

* <span data-ttu-id="a42a2-105">**Post**</span><span class="sxs-lookup"><span data-stu-id="a42a2-105">**Post**</span></span>
* <span data-ttu-id="a42a2-106">**Preview Posting**</span><span class="sxs-lookup"><span data-stu-id="a42a2-106">**Preview Posting**</span></span>
* <span data-ttu-id="a42a2-107">**Post and Print**</span><span class="sxs-lookup"><span data-stu-id="a42a2-107">**Post and Print**</span></span>
* <span data-ttu-id="a42a2-108">**Test Report**</span><span class="sxs-lookup"><span data-stu-id="a42a2-108">**Test Report**</span></span>
* <span data-ttu-id="a42a2-109">**Post Batch**</span><span class="sxs-lookup"><span data-stu-id="a42a2-109">**Post Batch**</span></span>

<span data-ttu-id="a42a2-110">When you have completed all the lines and entered all the information on the purchase order, you can post it, that is, create a receipt and an invoice.</span><span class="sxs-lookup"><span data-stu-id="a42a2-110">When you have completed all the lines and entered all the information on the purchase order, you can post it, that is, create a receipt and an invoice.</span></span>

<span data-ttu-id="a42a2-111">When a purchase order is posted, the vendor's account, the general ledger, and the item ledger entries are updated.</span><span class="sxs-lookup"><span data-stu-id="a42a2-111">When a purchase order is posted, the vendor's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="a42a2-112">For each purchase order, a purchase entry is created in the **G/L Entry** table.</span><span class="sxs-lookup"><span data-stu-id="a42a2-112">For each purchase order, a purchase entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="a42a2-113">An entry is also created in the vendor's account in the **Vendor Ledger Entry** table and a G/L entry is created in the relevant payables account.</span><span class="sxs-lookup"><span data-stu-id="a42a2-113">An entry is also created in the vendor's account in the **Vendor Ledger Entry** table and a G/L entry is created in the relevant payables account.</span></span> <span data-ttu-id="a42a2-114">In addition, posting the order may result in a VAT entry and a G/L entry for the discount amount.</span><span class="sxs-lookup"><span data-stu-id="a42a2-114">In addition, posting the order may result in a VAT entry and a G/L entry for the discount amount.</span></span> <span data-ttu-id="a42a2-115">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Purchases & Payables Setup** window.</span><span class="sxs-lookup"><span data-stu-id="a42a2-115">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Purchases & Payables Setup** window.</span></span>

<span data-ttu-id="a42a2-116">For each purchase order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the purchase lines contain item numbers) or a G/L entry will be created in the **G/L Entry** table (if the purchase lines contain a G/L account).</span><span class="sxs-lookup"><span data-stu-id="a42a2-116">For each purchase order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the purchase lines contain item numbers) or a G/L entry will be created in the **G/L Entry** table (if the purchase lines contain a G/L account).</span></span> <span data-ttu-id="a42a2-117">In addition, purchase orders are always recorded in the **Purch. Recpt. Header** and **Purch. Inv. Header** tables.</span><span class="sxs-lookup"><span data-stu-id="a42a2-117">In addition, purchase orders are always recorded in the **Purch. Recpt. Header** and **Purch. Inv. Header** tables.</span></span>

<span data-ttu-id="a42a2-118">Before you start to post, you can print a test report that contains all the information in the purchase order and indicates any errors there.</span><span class="sxs-lookup"><span data-stu-id="a42a2-118">Before you start to post, you can print a test report that contains all the information in the purchase order and indicates any errors there.</span></span> <span data-ttu-id="a42a2-119">To print the report, choose **Posting**, and then choose **Test Report**.</span><span class="sxs-lookup"><span data-stu-id="a42a2-119">To print the report, choose **Posting**, and then choose **Test Report**.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="a42a2-120">When you post an order, you can create both a receipt and an invoice.</span><span class="sxs-lookup"><span data-stu-id="a42a2-120">When you post an order, you can create both a receipt and an invoice.</span></span> <span data-ttu-id="a42a2-121">These can be done simultaneously or independently.</span><span class="sxs-lookup"><span data-stu-id="a42a2-121">These can be done simultaneously or independently.</span></span> <span data-ttu-id="a42a2-122">You can also create a partial receipt and a partial invoice by completing the **Qty. to Receive** and **Qty. to Invoice** fields on the individual purchase order lines before you post.</span><span class="sxs-lookup"><span data-stu-id="a42a2-122">You can also create a partial receipt and a partial invoice by completing the **Qty. to Receive** and **Qty. to Invoice** fields on the individual purchase order lines before you post.</span></span> <span data-ttu-id="a42a2-123">Note that you cannot create an invoice for something that has not been received.</span><span class="sxs-lookup"><span data-stu-id="a42a2-123">Note that you cannot create an invoice for something that has not been received.</span></span> <span data-ttu-id="a42a2-124">That is, before you can invoice, you must have recorded a receipt, or you must choose to receive and invoice at the same time.</span><span class="sxs-lookup"><span data-stu-id="a42a2-124">That is, before you can invoice, you must have recorded a receipt, or you must choose to receive and invoice at the same time.</span></span>

<span data-ttu-id="a42a2-125">You can either post, or post and print.</span><span class="sxs-lookup"><span data-stu-id="a42a2-125">You can either post, or post and print.</span></span> <span data-ttu-id="a42a2-126">If you choose to post and print, a report is printed when the order is posted.</span><span class="sxs-lookup"><span data-stu-id="a42a2-126">If you choose to post and print, a report is printed when the order is posted.</span></span> <span data-ttu-id="a42a2-127">You can also choose the **Post Batch** function, which lets you post several orders at the same time.</span><span class="sxs-lookup"><span data-stu-id="a42a2-127">You can also choose the **Post Batch** function, which lets you post several orders at the same time.</span></span>

<span data-ttu-id="a42a2-128">When the posting is completed, the posted purchase lines are removed from the order.</span><span class="sxs-lookup"><span data-stu-id="a42a2-128">When the posting is completed, the posted purchase lines are removed from the order.</span></span> <span data-ttu-id="a42a2-129">A message tells you when the posting is completed.</span><span class="sxs-lookup"><span data-stu-id="a42a2-129">A message tells you when the posting is completed.</span></span> <span data-ttu-id="a42a2-130">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Vendor Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Purchase Receipts**, and **Posted Purchase Invoices** windows.</span><span class="sxs-lookup"><span data-stu-id="a42a2-130">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Vendor Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Purchase Receipts**, and **Posted Purchase Invoices** windows.</span></span>

## <a name="see-also"></a><span data-ttu-id="a42a2-131">See Also</span><span class="sxs-lookup"><span data-stu-id="a42a2-131">See Also</span></span>
[<span data-ttu-id="a42a2-132">Purchasing</span><span class="sxs-lookup"><span data-stu-id="a42a2-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="a42a2-133">Post Documents and Journals</span><span class="sxs-lookup"><span data-stu-id="a42a2-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)  
<span data-ttu-id="a42a2-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a42a2-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
