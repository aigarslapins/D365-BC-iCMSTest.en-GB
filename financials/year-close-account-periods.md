---
title: Close Accounting Periods for a Fiscal Year | Microsoft Docs
description: Describes how to close the accounting periods that make up the fiscal year.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 06/02/2017
ms.author: jswymer
ms.openlocfilehash: 296a4663f14c02c8679bda78950c025263ca7590
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "250256"
---
# <a name="close-accounting-periods"></a><span data-ttu-id="f82bb-103">Close Accounting Periods</span><span class="sxs-lookup"><span data-stu-id="f82bb-103">Close Accounting Periods</span></span>
<span data-ttu-id="f82bb-104">When a fiscal year is over, you must close the periods that comprise it.</span><span class="sxs-lookup"><span data-stu-id="f82bb-104">When a fiscal year is over, you must close the periods that comprise it.</span></span>

## <a name="to-close-accounting-periods"></a><span data-ttu-id="f82bb-105">To close accounting periods</span><span class="sxs-lookup"><span data-stu-id="f82bb-105">To close accounting periods</span></span>
1. <span data-ttu-id="f82bb-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f82bb-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span></span>
2. <span data-ttu-id="f82bb-107">In the **Accounting Periods** window, choose the **Close Year** action.</span><span class="sxs-lookup"><span data-stu-id="f82bb-107">In the **Accounting Periods** window, choose the **Close Year** action.</span></span>

    <span data-ttu-id="f82bb-108">If more than one fiscal year is open, the earliest one is automatically selected to be closed.</span><span class="sxs-lookup"><span data-stu-id="f82bb-108">If more than one fiscal year is open, the earliest one is automatically selected to be closed.</span></span> <span data-ttu-id="f82bb-109">A message displays identifying the year that will close and the consequences of closing the year.</span><span class="sxs-lookup"><span data-stu-id="f82bb-109">A message displays identifying the year that will close and the consequences of closing the year.</span></span>
3. <span data-ttu-id="f82bb-110">To close the year, choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="f82bb-110">To close the year, choose the **Yes** button.</span></span>

<span data-ttu-id="f82bb-111">The fiscal year is closed, and the **Closed** and **Date Locked** fields for all the periods in the year are selected.</span><span class="sxs-lookup"><span data-stu-id="f82bb-111">The fiscal year is closed, and the **Closed** and **Date Locked** fields for all the periods in the year are selected.</span></span> <span data-ttu-id="f82bb-112">The fiscal year cannot be opened again and you cannot remove the check mark from the **Closed** or **Date Locked** fields.</span><span class="sxs-lookup"><span data-stu-id="f82bb-112">The fiscal year cannot be opened again and you cannot remove the check mark from the **Closed** or **Date Locked** fields.</span></span>

> [!NOTE]  
>   <span data-ttu-id="f82bb-113">You cannot close a fiscal year before you create a new one.</span><span class="sxs-lookup"><span data-stu-id="f82bb-113">You cannot close a fiscal year before you create a new one.</span></span> <span data-ttu-id="f82bb-114">Notice that when a fiscal year has been closed, you cannot change the starting date of the following fiscal year.</span><span class="sxs-lookup"><span data-stu-id="f82bb-114">Notice that when a fiscal year has been closed, you cannot change the starting date of the following fiscal year.</span></span>

<span data-ttu-id="f82bb-115">Even though a fiscal year has been closed, you can still post general ledger entries to it.</span><span class="sxs-lookup"><span data-stu-id="f82bb-115">Even though a fiscal year has been closed, you can still post general ledger entries to it.</span></span> <span data-ttu-id="f82bb-116">When you do this, the entries will be marked as posted to a closed fiscal year and the **Prior-Year Entry** field will be selected.</span><span class="sxs-lookup"><span data-stu-id="f82bb-116">When you do this, the entries will be marked as posted to a closed fiscal year and the **Prior-Year Entry** field will be selected.</span></span>

<span data-ttu-id="f82bb-117">After a fiscal year is closed, you must close the income statement accounts and transfer the year's results to an account in the balance sheet.</span><span class="sxs-lookup"><span data-stu-id="f82bb-117">After a fiscal year is closed, you must close the income statement accounts and transfer the year's results to an account in the balance sheet.</span></span> <span data-ttu-id="f82bb-118">You can repeat this every time that you post to the closed fiscal year.</span><span class="sxs-lookup"><span data-stu-id="f82bb-118">You can repeat this every time that you post to the closed fiscal year.</span></span>

## <a name="see-also"></a><span data-ttu-id="f82bb-119">See Also</span><span class="sxs-lookup"><span data-stu-id="f82bb-119">See Also</span></span>
[<span data-ttu-id="f82bb-120">Closing Books</span><span class="sxs-lookup"><span data-stu-id="f82bb-120">Closing Books</span></span>](year-close-books.md)  
[<span data-ttu-id="f82bb-121">Post the Year-End Closing Entry</span><span class="sxs-lookup"><span data-stu-id="f82bb-121">Post the Year-End Closing Entry</span></span>](year-how-post-year-end-close-entry.md)  
[<span data-ttu-id="f82bb-122">Open a New Fiscal Year</span><span class="sxs-lookup"><span data-stu-id="f82bb-122">Open a New Fiscal Year</span></span>](finance-how-open-new-fiscal-year.md)  
<span data-ttu-id="f82bb-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f82bb-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>