---
title: Transferring and Posting Cost Entries | Microsoft Docs
description: Before you define cost allocations, you must understand where cost entries come from.
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
ms.openlocfilehash: 43213f5d9e3056bdaa073624cd247e14b9925c1b
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "248076"
---
# <a name="transferring-and-posting-cost-entries"></a><span data-ttu-id="f567a-103">Transferring and Posting Cost Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-103">Transferring and Posting Cost Entries</span></span>
<span data-ttu-id="f567a-104">Before you define cost allocations, you must understand how cost entries come from the following sources:</span><span class="sxs-lookup"><span data-stu-id="f567a-104">Before you define cost allocations, you must understand how cost entries come from the following sources:</span></span>  

-   <span data-ttu-id="f567a-105">Automatic transfer of general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="f567a-105">Automatic transfer of general ledger entries.</span></span>  
-   <span data-ttu-id="f567a-106">Manual cost posting for pure cost entries, internal charges, and manual allocations.</span><span class="sxs-lookup"><span data-stu-id="f567a-106">Manual cost posting for pure cost entries, internal charges, and manual allocations.</span></span>  
-   <span data-ttu-id="f567a-107">Automatic allocation postings for actual costs.</span><span class="sxs-lookup"><span data-stu-id="f567a-107">Automatic allocation postings for actual costs.</span></span>  
-   <span data-ttu-id="f567a-108">Transfer of budget entries to actual.</span><span class="sxs-lookup"><span data-stu-id="f567a-108">Transfer of budget entries to actual.</span></span>

## <a name="criteria-for-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="f567a-109">Criteria for Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-109">Criteria for Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="f567a-110">It is important to understand the criteria for transferring general ledger entries to cost entries.</span><span class="sxs-lookup"><span data-stu-id="f567a-110">It is important to understand the criteria for transferring general ledger entries to cost entries.</span></span> <span data-ttu-id="f567a-111">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span><span class="sxs-lookup"><span data-stu-id="f567a-111">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span></span>  

<span data-ttu-id="f567a-112">General ledger entries are transferred if:</span><span class="sxs-lookup"><span data-stu-id="f567a-112">General ledger entries are transferred if:</span></span>  

-   <span data-ttu-id="f567a-113">The entries have dimension values corresponding to either a cost centre or a cost object.</span><span class="sxs-lookup"><span data-stu-id="f567a-113">The entries have dimension values corresponding to either a cost center or a cost object.</span></span>  
-   <span data-ttu-id="f567a-114">The entries have dimension values that correspond to a cost centre and a cost object.</span><span class="sxs-lookup"><span data-stu-id="f567a-114">The entries have dimension values that correspond to a cost center and a cost object.</span></span> <span data-ttu-id="f567a-115">For these entries, the cost centre takes precedence.</span><span class="sxs-lookup"><span data-stu-id="f567a-115">For these entries, the cost center takes precedence.</span></span> <span data-ttu-id="f567a-116">This helps avoid a situation where a cost type appears in both a cost object and a cost centre and is therefore counted twice in the statistics.</span><span class="sxs-lookup"><span data-stu-id="f567a-116">This helps avoid a situation where a cost type appears in both a cost object and a cost center and is therefore counted twice in the statistics.</span></span>  
-   <span data-ttu-id="f567a-117">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span><span class="sxs-lookup"><span data-stu-id="f567a-117">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span></span>  
-   <span data-ttu-id="f567a-118">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span><span class="sxs-lookup"><span data-stu-id="f567a-118">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span></span>  

<span data-ttu-id="f567a-119">General ledger entries are not transferred if:</span><span class="sxs-lookup"><span data-stu-id="f567a-119">General ledger entries are not transferred if:</span></span>  

-   <span data-ttu-id="f567a-120">The entries have dimension values that do not correspond to a cost centre or a cost object.</span><span class="sxs-lookup"><span data-stu-id="f567a-120">The entries have dimension values that do not correspond to a cost center or a cost object.</span></span>  
-   <span data-ttu-id="f567a-121">The entries have an amount of zero.</span><span class="sxs-lookup"><span data-stu-id="f567a-121">The entries have an amount of zero.</span></span>  
-   <span data-ttu-id="f567a-122">The entries have a general ledger account that has been deleted.</span><span class="sxs-lookup"><span data-stu-id="f567a-122">The entries have a general ledger account that has been deleted.</span></span>  
-   <span data-ttu-id="f567a-123">The entries have a general ledger account that is not of the type **Income Statement**.</span><span class="sxs-lookup"><span data-stu-id="f567a-123">The entries have a general ledger account that is not of the type **Income Statement**.</span></span>  
-   <span data-ttu-id="f567a-124">The entries have a general ledger account that is not assigned a cost type.</span><span class="sxs-lookup"><span data-stu-id="f567a-124">The entries have a general ledger account that is not assigned a cost type.</span></span>  
-   <span data-ttu-id="f567a-125">The entries have a posting date before the **Starting Date for G/L Transfer**.</span><span class="sxs-lookup"><span data-stu-id="f567a-125">The entries have a posting date before the **Starting Date for G/L Transfer**.</span></span>  
-   <span data-ttu-id="f567a-126">The entries have been posted with a closing date.</span><span class="sxs-lookup"><span data-stu-id="f567a-126">The entries have been posted with a closing date.</span></span> <span data-ttu-id="f567a-127">These are typically entries that set back the balance of the income statement at the end of the year.</span><span class="sxs-lookup"><span data-stu-id="f567a-127">These are typically entries that set back the balance of the income statement at the end of the year.</span></span>

## <a name="transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="f567a-128">Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-128">Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="f567a-129">You can transfer general ledger entries to cost entries.</span><span class="sxs-lookup"><span data-stu-id="f567a-129">You can transfer general ledger entries to cost entries.</span></span>  

<span data-ttu-id="f567a-130">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span><span class="sxs-lookup"><span data-stu-id="f567a-130">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span></span>  

### <a name="to-prepare-the-transfer"></a><span data-ttu-id="f567a-131">To prepare the transfer</span><span class="sxs-lookup"><span data-stu-id="f567a-131">To prepare the transfer</span></span>  

1.  <span data-ttu-id="f567a-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Accounting Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f567a-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Accounting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f567a-133">On the **Cost Accounting Setup** page, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span><span class="sxs-lookup"><span data-stu-id="f567a-133">On the **Cost Accounting Setup** page, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span></span>  
3.  <span data-ttu-id="f567a-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f567a-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="f567a-135">On the **Cost Type Card** page, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="f567a-135">On the **Cost Type Card** page, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span></span>  
5.  <span data-ttu-id="f567a-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f567a-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="f567a-137">For each relevant general ledger account, on the **G/L Account Card** page, verify that the **Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="f567a-137">For each relevant general ledger account, on the **G/L Account Card** page, verify that the **Cost Type No.**</span></span> <span data-ttu-id="f567a-138">field is linked correctly to a cost type.</span><span class="sxs-lookup"><span data-stu-id="f567a-138">field is linked correctly to a cost type.</span></span> <span data-ttu-id="f567a-139">For more information, see [Setting Up Cost Accounting](finance-set-up-cost-accounting.md).</span><span class="sxs-lookup"><span data-stu-id="f567a-139">For more information, see [Setting Up Cost Accounting](finance-set-up-cost-accounting.md).</span></span>  
7.  <span data-ttu-id="f567a-140">Verify that all relevant general ledger entries have dimension values that correspond to a cost centre and a cost object.</span><span class="sxs-lookup"><span data-stu-id="f567a-140">Verify that all relevant general ledger entries have dimension values that correspond to a cost center and a cost object.</span></span>  

### <a name="to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="f567a-141">To transfer general ledger entries to cost entries</span><span class="sxs-lookup"><span data-stu-id="f567a-141">To transfer general ledger entries to cost entries</span></span>  
1.  <span data-ttu-id="f567a-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f567a-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f567a-143">Choose the **Yes** button to start the transfer.</span><span class="sxs-lookup"><span data-stu-id="f567a-143">Choose the **Yes** button to start the transfer.</span></span> <span data-ttu-id="f567a-144">The process transfers all general ledger entries that have not already been transferred.</span><span class="sxs-lookup"><span data-stu-id="f567a-144">The process transfers all general ledger entries that have not already been transferred.</span></span>  

    <span data-ttu-id="f567a-145">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span><span class="sxs-lookup"><span data-stu-id="f567a-145">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span></span> <span data-ttu-id="f567a-146">This makes it possible to trace the source of cost entries.</span><span class="sxs-lookup"><span data-stu-id="f567a-146">This makes it possible to trace the source of cost entries.</span></span>

## <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="f567a-147">Automatic Transfer and Combined Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-147">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="f567a-148">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span><span class="sxs-lookup"><span data-stu-id="f567a-148">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="f567a-149">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span><span class="sxs-lookup"><span data-stu-id="f567a-149">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="f567a-150">The following table describes the different options.</span><span class="sxs-lookup"><span data-stu-id="f567a-150">The following table describes the different options.</span></span>  

|<span data-ttu-id="f567a-151">Combine Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-151">Combine Entries</span></span>|<span data-ttu-id="f567a-152">Description</span><span class="sxs-lookup"><span data-stu-id="f567a-152">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="f567a-153">None</span><span class="sxs-lookup"><span data-stu-id="f567a-153">None</span></span>|<span data-ttu-id="f567a-154">Each general ledger entry is transferred individually to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="f567a-154">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="f567a-155">Day</span><span class="sxs-lookup"><span data-stu-id="f567a-155">Day</span></span>|<span data-ttu-id="f567a-156">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="f567a-156">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="f567a-157">Month</span><span class="sxs-lookup"><span data-stu-id="f567a-157">Month</span></span>|<span data-ttu-id="f567a-158">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="f567a-158">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="f567a-159">If you have selected the **Auto Transfer from G/L** check box on the **Cost Accounting Setup** page, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="f567a-159">If you have selected the **Auto Transfer from G/L** check box on the **Cost Accounting Setup** page, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="f567a-160">Combined entries are not possible.</span><span class="sxs-lookup"><span data-stu-id="f567a-160">Combined entries are not possible.</span></span>

## <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="f567a-161">Results of Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-161">Results of Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="f567a-162">During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="f567a-162">During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.</span></span>  

### <a name="general-ledger-entries"></a><span data-ttu-id="f567a-163">General Ledger Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-163">General Ledger Entries</span></span>  
<span data-ttu-id="f567a-164">For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.</span><span class="sxs-lookup"><span data-stu-id="f567a-164">For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.</span></span>  

### <a name="cost-entries"></a><span data-ttu-id="f567a-165">Cost Entries</span><span class="sxs-lookup"><span data-stu-id="f567a-165">Cost Entries</span></span>  
<span data-ttu-id="f567a-166">For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.</span><span class="sxs-lookup"><span data-stu-id="f567a-166">For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.</span></span>  

<span data-ttu-id="f567a-167">For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.</span><span class="sxs-lookup"><span data-stu-id="f567a-167">For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.</span></span>  

<span data-ttu-id="f567a-168">The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.</span><span class="sxs-lookup"><span data-stu-id="f567a-168">The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.</span></span>  

<span data-ttu-id="f567a-169">For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field.</span><span class="sxs-lookup"><span data-stu-id="f567a-169">For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field.</span></span> <span data-ttu-id="f567a-170">For combined entries, the text field shows these entries are transferred as combined entries.</span><span class="sxs-lookup"><span data-stu-id="f567a-170">For combined entries, the text field shows these entries are transferred as combined entries.</span></span> <span data-ttu-id="f567a-171">For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.</span><span class="sxs-lookup"><span data-stu-id="f567a-171">For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.</span></span>  

### <a name="cost-register"></a><span data-ttu-id="f567a-172">Cost Register</span><span class="sxs-lookup"><span data-stu-id="f567a-172">Cost Register</span></span>  
<span data-ttu-id="f567a-173">In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger.</span><span class="sxs-lookup"><span data-stu-id="f567a-173">In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger.</span></span> <span data-ttu-id="f567a-174">The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.</span><span class="sxs-lookup"><span data-stu-id="f567a-174">The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.</span></span>

## <a name="see-also"></a><span data-ttu-id="f567a-175">See Also</span><span class="sxs-lookup"><span data-stu-id="f567a-175">See Also</span></span>  
 <span data-ttu-id="f567a-176">[About Cost Accounting](finance-about-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f567a-176">[About Cost Accounting](finance-about-cost-accounting.md) </span></span>  
 <span data-ttu-id="f567a-177">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="f567a-177">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
 <span data-ttu-id="f567a-178">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="f567a-178">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 [<span data-ttu-id="f567a-179">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="f567a-179">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)