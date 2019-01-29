---
title: Use Allocation Keys in General Journals | Microsoft Docs
description: Learn how you can use allocation keys in journals.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost accounting
ms.date: 03/29/2017
ms.author: edupont
ms.openlocfilehash: ecb0c2169e37c4da0e0c5308538272c618b15990
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "220157"
---
# <a name="use-allocation-keys-in-general-journals"></a><span data-ttu-id="19096-103">Use Allocation Keys in General Journals</span><span class="sxs-lookup"><span data-stu-id="19096-103">Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="19096-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span><span class="sxs-lookup"><span data-stu-id="19096-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="19096-105">The allocation can be made by quantity, percentage, or amount.</span><span class="sxs-lookup"><span data-stu-id="19096-105">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="19096-106">To set up allocation keys</span><span class="sxs-lookup"><span data-stu-id="19096-106">To set up allocation keys</span></span>
1. <span data-ttu-id="19096-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="19096-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="19096-108">Choose the **Batch Name** field to open the **General Journal Batches** window.</span><span class="sxs-lookup"><span data-stu-id="19096-108">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="19096-109">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span><span class="sxs-lookup"><span data-stu-id="19096-109">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
   * <span data-ttu-id="19096-110">To create a new batch, choose the **New** action, and go to the next step.</span><span class="sxs-lookup"><span data-stu-id="19096-110">To create a new batch, choose the **New** action, and go to the next step.</span></span>
   * <span data-ttu-id="19096-111">To change the allocations of an existing journal, select the journal and go to step 7.</span><span class="sxs-lookup"><span data-stu-id="19096-111">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="19096-112">In the **Name** field, enter a name for the batch, such as CLEANING.</span><span class="sxs-lookup"><span data-stu-id="19096-112">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="19096-113">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span><span class="sxs-lookup"><span data-stu-id="19096-113">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="19096-114">When you are done, close the window.</span><span class="sxs-lookup"><span data-stu-id="19096-114">When you are done, close the window.</span></span> <span data-ttu-id="19096-115">A new, empty recurring journal opens.</span><span class="sxs-lookup"><span data-stu-id="19096-115">A new, empty recurring journal opens.</span></span>
6. <span data-ttu-id="19096-116">Fill in the fields on the line.</span><span class="sxs-lookup"><span data-stu-id="19096-116">Fill in the fields on the line.</span></span>
7. <span data-ttu-id="19096-117">Choose the **Allocations** action.</span><span class="sxs-lookup"><span data-stu-id="19096-117">Choose the **Allocations** action.</span></span>
8. <span data-ttu-id="19096-118">Add a line for each allocation.</span><span class="sxs-lookup"><span data-stu-id="19096-118">Add a line for each allocation.</span></span> <span data-ttu-id="19096-119">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="19096-119">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="19096-120">You must also fill in the **Account No.** field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span><span class="sxs-lookup"><span data-stu-id="19096-120">You must also fill in the **Account No.** field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="19096-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span><span class="sxs-lookup"><span data-stu-id="19096-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="19096-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span><span class="sxs-lookup"><span data-stu-id="19096-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="19096-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span><span class="sxs-lookup"><span data-stu-id="19096-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="19096-124">The **Allocated Amt. (GBP)** field is filled in and matches the **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="19096-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="19096-125">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="19096-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="19096-126">To change an allocation key that has already been set up</span><span class="sxs-lookup"><span data-stu-id="19096-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="19096-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="19096-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="19096-128">In the **Recurring General Journal** window, select the journal with the allocation.</span><span class="sxs-lookup"><span data-stu-id="19096-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="19096-129">Choose the line with the allocation, and then choose **Allocations** action.</span><span class="sxs-lookup"><span data-stu-id="19096-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="19096-130">Change the relevant fields, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="19096-130">Change the relevant fields, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="19096-131">See Also</span><span class="sxs-lookup"><span data-stu-id="19096-131">See Also</span></span>
[<span data-ttu-id="19096-132">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="19096-132">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="19096-133">Posting Documents and Journals</span><span class="sxs-lookup"><span data-stu-id="19096-133">Posting Documents and Journals</span></span>](ui-post-documents-journals.md)  
<span data-ttu-id="19096-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="19096-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>