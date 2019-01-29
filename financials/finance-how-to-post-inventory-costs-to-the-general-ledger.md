---
title: How to Post Inventory Costs to the General Ledger| Microsoft Docs
description: Describes how to manage the physical products that you trade in, for example, handling the stock in your warehouse.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 07/05/2017
ms.author: sgroespe
ms.openlocfilehash: ab54fe80160ede591e6255726eed3842745abb56
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "235994"
---
# <a name="reconcile-inventory-costs-with-the-general-ledger"></a><span data-ttu-id="0d316-103">Reconcile Inventory Costs with the General Ledger</span><span class="sxs-lookup"><span data-stu-id="0d316-103">Reconcile Inventory Costs with the General Ledger</span></span>
<span data-ttu-id="0d316-104">When you post inventory transactions, such as sales shipments, purchase invoices, or inventory adjustments, the changed item costs are recorded in item value entries.</span><span class="sxs-lookup"><span data-stu-id="0d316-104">When you post inventory transactions, such as sales shipments, purchase invoices, or inventory adjustments, the changed item costs are recorded in item value entries.</span></span> <span data-ttu-id="0d316-105">To reflect this change of inventory value in your financial books, the inventory costs are automatically posted to the related inventory accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0d316-105">To reflect this change of inventory value in your financial books, the inventory costs are automatically posted to the related inventory accounts in the general ledger.</span></span> <span data-ttu-id="0d316-106">For each inventory transaction that you post, the appropriate values are posted to the inventory account, adjustment account, and COGS account in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0d316-106">For each inventory transaction that you post, the appropriate values are posted to the inventory account, adjustment account, and COGS account in the general ledger.</span></span>

<span data-ttu-id="0d316-107">Automatic cost posting is defined by the **Automatic Cost Posting** field in the **Inventory Setup** window.</span><span class="sxs-lookup"><span data-stu-id="0d316-107">Automatic cost posting is defined by the **Automatic Cost Posting** field in the **Inventory Setup** window.</span></span>

<span data-ttu-id="0d316-108">Even though inventory costs are automatically posted to the general ledger, it is still necessary to ensure that the costs of goods are forwarded to the related outbound sales transaction, especially in situations where you sell goods before you invoice the purchase of those goods.</span><span class="sxs-lookup"><span data-stu-id="0d316-108">Even though inventory costs are automatically posted to the general ledger, it is still necessary to ensure that the costs of goods are forwarded to the related outbound sales transaction, especially in situations where you sell goods before you invoice the purchase of those goods.</span></span> <span data-ttu-id="0d316-109">This is referred to as cost adjustment.</span><span class="sxs-lookup"><span data-stu-id="0d316-109">This is referred to as cost adjustment.</span></span> <span data-ttu-id="0d316-110">Item costs are automatically adjusted when you post item transactions, but you can also adjust item costs manually.</span><span class="sxs-lookup"><span data-stu-id="0d316-110">Item costs are automatically adjusted when you post item transactions, but you can also adjust item costs manually.</span></span> <span data-ttu-id="0d316-111">For more information, see [Adjust Item Costs](inventory-how-adjust-item-costs.md).</span><span class="sxs-lookup"><span data-stu-id="0d316-111">For more information, see [Adjust Item Costs](inventory-how-adjust-item-costs.md).</span></span>

## <a name="to-post-inventory-costs-manually"></a><span data-ttu-id="0d316-112">To post inventory costs manually</span><span class="sxs-lookup"><span data-stu-id="0d316-112">To post inventory costs manually</span></span>
1. <span data-ttu-id="0d316-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") ico, enter **Post Inventory Cost to G/L**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d316-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") ico, enter **Post Inventory Cost to G/L**, and then choose the related link.</span></span>
2. <span data-ttu-id="0d316-114">Post inventory costs to the general ledger manually by running the batch job.</span><span class="sxs-lookup"><span data-stu-id="0d316-114">Post inventory costs to the general ledger manually by running the batch job.</span></span> <span data-ttu-id="0d316-115">When you run this batch job, general ledger entries are created on the basis of value entries.</span><span class="sxs-lookup"><span data-stu-id="0d316-115">When you run this batch job, general ledger entries are created on the basis of value entries.</span></span> <span data-ttu-id="0d316-116">You can post the entries so that they are summarized per posting group.</span><span class="sxs-lookup"><span data-stu-id="0d316-116">You can post the entries so that they are summarized per posting group.</span></span>

> [!NOTE]  
> <span data-ttu-id="0d316-117">When you run this batch job, you might encounter errors having to do with missing setup or incompatible dimension setup.</span><span class="sxs-lookup"><span data-stu-id="0d316-117">When you run this batch job, you might encounter errors having to do with missing setup or incompatible dimension setup.</span></span> <span data-ttu-id="0d316-118">If the batch job encounters errors in the dimension setup, it overrides these errors and uses the dimensions of the value entry.</span><span class="sxs-lookup"><span data-stu-id="0d316-118">If the batch job encounters errors in the dimension setup, it overrides these errors and uses the dimensions of the value entry.</span></span> <span data-ttu-id="0d316-119">For any other errors, the batch job skips posting the value entries and lists them at the end of the report in a section titled “Skipped Entries.”</span><span class="sxs-lookup"><span data-stu-id="0d316-119">For any other errors, the batch job skips posting the value entries and lists them at the end of the report in a section titled “Skipped Entries.”</span></span> <span data-ttu-id="0d316-120">To post these entries, you must fix the errors.</span><span class="sxs-lookup"><span data-stu-id="0d316-120">To post these entries, you must fix the errors.</span></span>

<span data-ttu-id="0d316-121">To see a list of errors before running the posting batch job, you can run the **Post Invt. Cost to G/L - Test** report.</span><span class="sxs-lookup"><span data-stu-id="0d316-121">To see a list of errors before running the posting batch job, you can run the **Post Invt. Cost to G/L - Test** report.</span></span> <span data-ttu-id="0d316-122">The test report lists all the errors encountered during a test posting.</span><span class="sxs-lookup"><span data-stu-id="0d316-122">The test report lists all the errors encountered during a test posting.</span></span> <span data-ttu-id="0d316-123">You can then fix the errors, and run the inventory cost posting batch job without skipping any entries.</span><span class="sxs-lookup"><span data-stu-id="0d316-123">You can then fix the errors, and run the inventory cost posting batch job without skipping any entries.</span></span>

<span data-ttu-id="0d316-124">If you would like to simply get an overview of what values could be posted to the general ledger without actually performing the posting, you can run the **Post Inventory Cost to G/L** batch job without actually posting the values to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0d316-124">If you would like to simply get an overview of what values could be posted to the general ledger without actually performing the posting, you can run the **Post Inventory Cost to G/L** batch job without actually posting the values to the general ledger.</span></span> <span data-ttu-id="0d316-125">You do this by clearing the check mark from the **Post** field on the request page.</span><span class="sxs-lookup"><span data-stu-id="0d316-125">You do this by clearing the check mark from the **Post** field on the request page.</span></span> <span data-ttu-id="0d316-126">This way, when you run the batch job, the report is produced showing the values that are ready to be posted to the general ledger, but they are not posted.</span><span class="sxs-lookup"><span data-stu-id="0d316-126">This way, when you run the batch job, the report is produced showing the values that are ready to be posted to the general ledger, but they are not posted.</span></span>

## <a name="to-audit-the-reconciliation-between-the-inventory-ledger-and-the-general-ledger"></a><span data-ttu-id="0d316-127">To audit the reconciliation between the inventory ledger and the general ledger</span><span class="sxs-lookup"><span data-stu-id="0d316-127">To audit the reconciliation between the inventory ledger and the general ledger</span></span>
<span data-ttu-id="0d316-128">The **Inventory - G/L Reconciliation** window provides the following:</span><span class="sxs-lookup"><span data-stu-id="0d316-128">The **Inventory - G/L Reconciliation** window provides the following:</span></span>

- <span data-ttu-id="0d316-129">Exposes reconciliation differences by comparing what is recorded in G/L and what is recorded in the inventory ledger (value entries).</span><span class="sxs-lookup"><span data-stu-id="0d316-129">Exposes reconciliation differences by comparing what is recorded in G/L and what is recorded in the inventory ledger (value entries).</span></span>
- <span data-ttu-id="0d316-130">Displays unreconciled cost amounts in the value entries in the inventory ledger as if they were mapped to corresponding inventory-related accounts in G/L and compares those to the totals actually recorded in the same accounts in G/L.</span><span class="sxs-lookup"><span data-stu-id="0d316-130">Displays unreconciled cost amounts in the value entries in the inventory ledger as if they were mapped to corresponding inventory-related accounts in G/L and compares those to the totals actually recorded in the same accounts in G/L.</span></span>
- <span data-ttu-id="0d316-131">Reflects the double entry structure of G/L by visually presenting data as such.</span><span class="sxs-lookup"><span data-stu-id="0d316-131">Reflects the double entry structure of G/L by visually presenting data as such.</span></span> <span data-ttu-id="0d316-132">For example, a COGS entry has a corresponding inventory entry.</span><span class="sxs-lookup"><span data-stu-id="0d316-132">For example, a COGS entry has a corresponding inventory entry.</span></span>
- <span data-ttu-id="0d316-133">Lets users drill down and see the entries that make up the cost amounts.</span><span class="sxs-lookup"><span data-stu-id="0d316-133">Lets users drill down and see the entries that make up the cost amounts.</span></span>
- <span data-ttu-id="0d316-134">Includes filters to narrow the analysis by date, item, and location.</span><span class="sxs-lookup"><span data-stu-id="0d316-134">Includes filters to narrow the analysis by date, item, and location.</span></span>
- <span data-ttu-id="0d316-135">Explains reasons for reconciliation differences in informative messages.</span><span class="sxs-lookup"><span data-stu-id="0d316-135">Explains reasons for reconciliation differences in informative messages.</span></span>


<span data-ttu-id="0d316-136">The **Name** column on the far left in the grid lists the various G/L account types that are associated with inventory.</span><span class="sxs-lookup"><span data-stu-id="0d316-136">The **Name** column on the far left in the grid lists the various G/L account types that are associated with inventory.</span></span>

<span data-ttu-id="0d316-137">The **Inventory**, **Inventory (Interim)**, and **WIP Inventory** columns show the invoiced, non-invoiced, and WIP totals of each G/L account type.</span><span class="sxs-lookup"><span data-stu-id="0d316-137">The **Inventory**, **Inventory (Interim)**, and **WIP Inventory** columns show the invoiced, non-invoiced, and WIP totals of each G/L account type.</span></span> <span data-ttu-id="0d316-138">These are calculated from value entries, that is, they are projected onto the G/L account types where they will end when they are eventually posted to G/L.</span><span class="sxs-lookup"><span data-stu-id="0d316-138">These are calculated from value entries, that is, they are projected onto the G/L account types where they will end when they are eventually posted to G/L.</span></span>

<span data-ttu-id="0d316-139">The **Total** column shows the sum (in bold font) of the value entry amounts in the three inventory columns.</span><span class="sxs-lookup"><span data-stu-id="0d316-139">The **Total** column shows the sum (in bold font) of the value entry amounts in the three inventory columns.</span></span>

<span data-ttu-id="0d316-140">The **G/L Total** column shows the amounts (in bold font) for each G/L account type that exists in G/L.</span><span class="sxs-lookup"><span data-stu-id="0d316-140">The **G/L Total** column shows the amounts (in bold font) for each G/L account type that exists in G/L.</span></span> <span data-ttu-id="0d316-141">These are calculated from G/L entries, that is, they represent inventory costs already posted to G/L.</span><span class="sxs-lookup"><span data-stu-id="0d316-141">These are calculated from G/L entries, that is, they represent inventory costs already posted to G/L.</span></span>

<span data-ttu-id="0d316-142">The **Difference** column represents the difference between the value in the **G/L Total** and **Total** fields.</span><span class="sxs-lookup"><span data-stu-id="0d316-142">The **Difference** column represents the difference between the value in the **G/L Total** and **Total** fields.</span></span>

<span data-ttu-id="0d316-143">In the top of the **Inventory - G/L Reconciliation** window, you can enter filters to limit, for example, the period of time for which you want information.</span><span class="sxs-lookup"><span data-stu-id="0d316-143">In the top of the **Inventory - G/L Reconciliation** window, you can enter filters to limit, for example, the period of time for which you want information.</span></span>

<span data-ttu-id="0d316-144">If you select the **Show Warning** check box and if there are any discrepancies between the inventory totals and G/L totals, the programme shows messages in the **Warning** field of the grid that explain the discrepancy.</span><span class="sxs-lookup"><span data-stu-id="0d316-144">If you select the **Show Warning** check box and if there are any discrepancies between the inventory totals and G/L totals, the program shows messages in the **Warning** field of the grid that explain the discrepancy.</span></span> <span data-ttu-id="0d316-145">If you choose the Warning field, the program gives you more information on what the warning means.</span><span class="sxs-lookup"><span data-stu-id="0d316-145">If you choose the Warning field, the program gives you more information on what the warning means.</span></span>

<span data-ttu-id="0d316-146">When you have entered all relevant filters, choose the **Show Matrix** action.</span><span class="sxs-lookup"><span data-stu-id="0d316-146">When you have entered all relevant filters, choose the **Show Matrix** action.</span></span> <span data-ttu-id="0d316-147">The data is calculated and the matrix window appears.</span><span class="sxs-lookup"><span data-stu-id="0d316-147">The data is calculated and the matrix window appears.</span></span>

<span data-ttu-id="0d316-148">On the far left column in the grid, you see the various general ledger account types that are associated with inventory.</span><span class="sxs-lookup"><span data-stu-id="0d316-148">On the far left column in the grid, you see the various general ledger account types that are associated with inventory.</span></span> <span data-ttu-id="0d316-149">The grid then shows the invoiced, non-invoiced (interim), and WIP inventory totals for each of these account types.</span><span class="sxs-lookup"><span data-stu-id="0d316-149">The grid then shows the invoiced, non-invoiced (interim), and WIP inventory totals for each of these account types.</span></span> <span data-ttu-id="0d316-150">These totals are calculated from the value entries.</span><span class="sxs-lookup"><span data-stu-id="0d316-150">These totals are calculated from the value entries.</span></span>

<span data-ttu-id="0d316-151">The next columns show the totals for the same account types calculated from the general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="0d316-151">The next columns show the totals for the same account types calculated from the general ledger entries.</span></span>

<span data-ttu-id="0d316-152">Choose the  amount in any of the total fields to see the inventory report entries that were used to calculate the totals.</span><span class="sxs-lookup"><span data-stu-id="0d316-152">Choose the  amount in any of the total fields to see the inventory report entries that were used to calculate the totals.</span></span> <span data-ttu-id="0d316-153">For inventory totals, the inventory report entries are the sums of the value entries for the items.</span><span class="sxs-lookup"><span data-stu-id="0d316-153">For inventory totals, the inventory report entries are the sums of the value entries for the items.</span></span> <span data-ttu-id="0d316-154">For the G/L totals, the inventory report entries are the sums from the general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="0d316-154">For the G/L totals, the inventory report entries are the sums from the general ledger entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="0d316-155">See Also</span><span class="sxs-lookup"><span data-stu-id="0d316-155">See Also</span></span>  
[<span data-ttu-id="0d316-156">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="0d316-156">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="0d316-157">Purchasing</span><span class="sxs-lookup"><span data-stu-id="0d316-157">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="0d316-158">[Sales](sales-manage-sales.md)  </span><span class="sxs-lookup"><span data-stu-id="0d316-158">[Sales](sales-manage-sales.md)  </span></span>  
<span data-ttu-id="0d316-159">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0d316-159">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="0d316-160">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="0d316-160">General Business Functionality</span></span>](ui-across-business-areas.md)