---
title: Field Mapping When Importing SEPA CAMT Files | Microsoft Docs
description: In European markets, you can import bank statement files in the regional SEPA standards (Single Euro Payments Area).
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: e2fcfb5e896f6da2f953ad15fb46bcd9b34be047
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "234236"
---
# <a name="field-mapping-when-importing-sepa-camt-files"></a><span data-ttu-id="be1aa-103">Field Mapping When Importing SEPA CAMT Files</span><span class="sxs-lookup"><span data-stu-id="be1aa-103">Field Mapping When Importing SEPA CAMT Files</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="be1aa-104">supports the regional SEPA standards (Single Euro Payments Area) for importing SEPA bank statements (CAMT format).</span><span class="sxs-lookup"><span data-stu-id="be1aa-104">supports the regional SEPA standards (Single Euro Payments Area) for importing SEPA bank statements (CAMT format).</span></span> <span data-ttu-id="be1aa-105">For more information, see [Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md).</span><span class="sxs-lookup"><span data-stu-id="be1aa-105">For more information, see [Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md).</span></span>  

 <span data-ttu-id="be1aa-106">The SEPA CAMT standard itself has local variations.</span><span class="sxs-lookup"><span data-stu-id="be1aa-106">The SEPA CAMT standard itself has local variations.</span></span> <span data-ttu-id="be1aa-107">Therefore, you may have to modify the generic data exchange definition (represented by the **SEPA CAMT** code on the **Posting Exchange Definitions** page) to adapt it to a local variation of the standard.</span><span class="sxs-lookup"><span data-stu-id="be1aa-107">Therefore, you may have to modify the generic data exchange definition (represented by the **SEPA CAMT** code on the **Posting Exchange Definitions** page) to adapt it to a local variation of the standard.</span></span> <span data-ttu-id="be1aa-108">The following tables show the element-to-field mapping for tables 81, 273, and 274 in the SEPA CAMT implementation in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="be1aa-108">The following tables show the element-to-field mapping for tables 81, 273, and 274 in the SEPA CAMT implementation in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

 <span data-ttu-id="be1aa-109">For information about creating or adjusting a data exchange definition, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="be1aa-109">For information about creating or adjusting a data exchange definition, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

## <a name="camt-data-mapping-to-fields-in-the-general-journal-table-81"></a><span data-ttu-id="be1aa-110">CAMT data mapping to fields in the General Journal table (81)</span><span class="sxs-lookup"><span data-stu-id="be1aa-110">CAMT data mapping to fields in the General Journal table (81)</span></span>  

|<span data-ttu-id="be1aa-111">Element Path</span><span class="sxs-lookup"><span data-stu-id="be1aa-111">Element Path</span></span>|<span data-ttu-id="be1aa-112">Message Element</span><span class="sxs-lookup"><span data-stu-id="be1aa-112">Message Element</span></span>|<span data-ttu-id="be1aa-113">Data Type</span><span class="sxs-lookup"><span data-stu-id="be1aa-113">Data Type</span></span>|<span data-ttu-id="be1aa-114">Description</span><span class="sxs-lookup"><span data-stu-id="be1aa-114">Description</span></span>|<span data-ttu-id="be1aa-115">Negative-Sign Identifier</span><span class="sxs-lookup"><span data-stu-id="be1aa-115">Negative-Sign Identifier</span></span>|<span data-ttu-id="be1aa-116">Field No.</span><span class="sxs-lookup"><span data-stu-id="be1aa-116">Field No.</span></span>|<span data-ttu-id="be1aa-117">Field Name</span><span class="sxs-lookup"><span data-stu-id="be1aa-117">Field Name</span></span>|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|<span data-ttu-id="be1aa-118">Stmt/Ntry/Amt</span><span class="sxs-lookup"><span data-stu-id="be1aa-118">Stmt/Ntry/Amt</span></span>|<span data-ttu-id="be1aa-119">Amount</span><span class="sxs-lookup"><span data-stu-id="be1aa-119">Amount</span></span>|<span data-ttu-id="be1aa-120">Decimal</span><span class="sxs-lookup"><span data-stu-id="be1aa-120">Decimal</span></span>|<span data-ttu-id="be1aa-121">The amount of money in the cash entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-121">The amount of money in the cash entry</span></span>||<span data-ttu-id="be1aa-122">13</span><span class="sxs-lookup"><span data-stu-id="be1aa-122">13</span></span>|<span data-ttu-id="be1aa-123">Amount</span><span class="sxs-lookup"><span data-stu-id="be1aa-123">Amount</span></span>|  
|<span data-ttu-id="be1aa-124">Stmt/Ntry/CdtDbtInd</span><span class="sxs-lookup"><span data-stu-id="be1aa-124">Stmt/Ntry/CdtDbtInd</span></span>|<span data-ttu-id="be1aa-125">CreditDebitIndicator</span><span class="sxs-lookup"><span data-stu-id="be1aa-125">CreditDebitIndicator</span></span>|<span data-ttu-id="be1aa-126">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-126">Text</span></span>|<span data-ttu-id="be1aa-127">Indicates whether the entry is a credit or a debit entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-127">Indicates whether the entry is a credit or a debit entry</span></span>|<span data-ttu-id="be1aa-128">DBIT</span><span class="sxs-lookup"><span data-stu-id="be1aa-128">DBIT</span></span>|<span data-ttu-id="be1aa-129">13</span><span class="sxs-lookup"><span data-stu-id="be1aa-129">13</span></span>|<span data-ttu-id="be1aa-130">Amount</span><span class="sxs-lookup"><span data-stu-id="be1aa-130">Amount</span></span>|  
|<span data-ttu-id="be1aa-131">Stmt/Ntry/BookgDt/Dt</span><span class="sxs-lookup"><span data-stu-id="be1aa-131">Stmt/Ntry/BookgDt/Dt</span></span>|<span data-ttu-id="be1aa-132">Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-132">Date</span></span>|<span data-ttu-id="be1aa-133">Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-133">Date</span></span>|<span data-ttu-id="be1aa-134">The date when an entry is posted to an account on the account servicer's books</span><span class="sxs-lookup"><span data-stu-id="be1aa-134">The date when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="be1aa-135">5</span><span class="sxs-lookup"><span data-stu-id="be1aa-135">5</span></span>|<span data-ttu-id="be1aa-136">Posting Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-136">Posting Date</span></span>|  
|<span data-ttu-id="be1aa-137">Stmt/Ntry/BookgDt/DtTm</span><span class="sxs-lookup"><span data-stu-id="be1aa-137">Stmt/Ntry/BookgDt/DtTm</span></span>|<span data-ttu-id="be1aa-138">DateTime</span><span class="sxs-lookup"><span data-stu-id="be1aa-138">DateTime</span></span>|<span data-ttu-id="be1aa-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="be1aa-139">DateTime</span></span>|<span data-ttu-id="be1aa-140">The date and time when an entry is posted to an account on the account servicer's books</span><span class="sxs-lookup"><span data-stu-id="be1aa-140">The date and time when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="be1aa-141">5</span><span class="sxs-lookup"><span data-stu-id="be1aa-141">5</span></span>|<span data-ttu-id="be1aa-142">Posting Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-142">Posting Date</span></span>|  
|<span data-ttu-id="be1aa-143">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span><span class="sxs-lookup"><span data-stu-id="be1aa-143">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span></span>|<span data-ttu-id="be1aa-144">Name</span><span class="sxs-lookup"><span data-stu-id="be1aa-144">Name</span></span>|<span data-ttu-id="be1aa-145">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-145">Text</span></span>|<span data-ttu-id="be1aa-146">The name of the party that owes an amount of money to the (ultimate) creditor</span><span class="sxs-lookup"><span data-stu-id="be1aa-146">The name of the party that owes an amount of money to the (ultimate) creditor</span></span>||<span data-ttu-id="be1aa-147">1221</span><span class="sxs-lookup"><span data-stu-id="be1aa-147">1221</span></span>|<span data-ttu-id="be1aa-148">Payer Information</span><span class="sxs-lookup"><span data-stu-id="be1aa-148">Payer Information</span></span>|  
|<span data-ttu-id="be1aa-149">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span><span class="sxs-lookup"><span data-stu-id="be1aa-149">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span></span>|<span data-ttu-id="be1aa-150">Unstructured</span><span class="sxs-lookup"><span data-stu-id="be1aa-150">Unstructured</span></span>|<span data-ttu-id="be1aa-151">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-151">Text</span></span>|<span data-ttu-id="be1aa-152">Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form</span><span class="sxs-lookup"><span data-stu-id="be1aa-152">Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form</span></span>||<span data-ttu-id="be1aa-153">8</span><span class="sxs-lookup"><span data-stu-id="be1aa-153">8</span></span>|<span data-ttu-id="be1aa-154">Description</span><span class="sxs-lookup"><span data-stu-id="be1aa-154">Description</span></span>|  
|<span data-ttu-id="be1aa-155">Stmt/Ntry/AddtlNtryInf</span><span class="sxs-lookup"><span data-stu-id="be1aa-155">Stmt/Ntry/AddtlNtryInf</span></span>|<span data-ttu-id="be1aa-156">AdditionalEntryInformation</span><span class="sxs-lookup"><span data-stu-id="be1aa-156">AdditionalEntryInformation</span></span>|<span data-ttu-id="be1aa-157">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-157">Text</span></span>|<span data-ttu-id="be1aa-158">Additional information about the entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-158">Additional information about the entry</span></span>||<span data-ttu-id="be1aa-159">1222</span><span class="sxs-lookup"><span data-stu-id="be1aa-159">1222</span></span>|<span data-ttu-id="be1aa-160">Transaction Information</span><span class="sxs-lookup"><span data-stu-id="be1aa-160">Transaction Information</span></span>|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-table-273"></a><span data-ttu-id="be1aa-161">CAMT data mapping to fields in the Bank Acc. Reconciliation table (273)</span><span class="sxs-lookup"><span data-stu-id="be1aa-161">CAMT data mapping to fields in the Bank Acc. Reconciliation table (273)</span></span>  

|<span data-ttu-id="be1aa-162">Element Path</span><span class="sxs-lookup"><span data-stu-id="be1aa-162">Element Path</span></span>|<span data-ttu-id="be1aa-163">Message Element</span><span class="sxs-lookup"><span data-stu-id="be1aa-163">Message Element</span></span>|<span data-ttu-id="be1aa-164">Data Type</span><span class="sxs-lookup"><span data-stu-id="be1aa-164">Data Type</span></span>|<span data-ttu-id="be1aa-165">Description</span><span class="sxs-lookup"><span data-stu-id="be1aa-165">Description</span></span>|<span data-ttu-id="be1aa-166">Negative-Sign Identifier</span><span class="sxs-lookup"><span data-stu-id="be1aa-166">Negative-Sign Identifier</span></span>|<span data-ttu-id="be1aa-167">Field No.</span><span class="sxs-lookup"><span data-stu-id="be1aa-167">Field No.</span></span>|<span data-ttu-id="be1aa-168">Field Name</span><span class="sxs-lookup"><span data-stu-id="be1aa-168">Field Name</span></span>|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|<span data-ttu-id="be1aa-169">Stmt/CreDtTm</span><span class="sxs-lookup"><span data-stu-id="be1aa-169">Stmt/CreDtTm</span></span>|<span data-ttu-id="be1aa-170">CreationDateTime</span><span class="sxs-lookup"><span data-stu-id="be1aa-170">CreationDateTime</span></span>|<span data-ttu-id="be1aa-171">Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-171">Date</span></span>|<span data-ttu-id="be1aa-172">The date and time when the message was created</span><span class="sxs-lookup"><span data-stu-id="be1aa-172">The date and time when the message was created</span></span>||<span data-ttu-id="be1aa-173">3</span><span class="sxs-lookup"><span data-stu-id="be1aa-173">3</span></span>|<span data-ttu-id="be1aa-174">Statement Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-174">Statement Date</span></span>|  
|<span data-ttu-id="be1aa-175">Stmt/Bal/Amt</span><span class="sxs-lookup"><span data-stu-id="be1aa-175">Stmt/Bal/Amt</span></span>|<span data-ttu-id="be1aa-176">Amount</span><span class="sxs-lookup"><span data-stu-id="be1aa-176">Amount</span></span>|<span data-ttu-id="be1aa-177">Decimal</span><span class="sxs-lookup"><span data-stu-id="be1aa-177">Decimal</span></span>|<span data-ttu-id="be1aa-178">The amount resulting from the netted amounts for all debit and credit entries</span><span class="sxs-lookup"><span data-stu-id="be1aa-178">The amount resulting from the netted amounts for all debit and credit entries</span></span>||<span data-ttu-id="be1aa-179">4</span><span class="sxs-lookup"><span data-stu-id="be1aa-179">4</span></span>|<span data-ttu-id="be1aa-180">Statement Ending Balance</span><span class="sxs-lookup"><span data-stu-id="be1aa-180">Statement Ending Balance</span></span>|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-line-table-274"></a><span data-ttu-id="be1aa-181">CAMT data mapping to fields in the Bank Acc. Reconciliation Line table (274)</span><span class="sxs-lookup"><span data-stu-id="be1aa-181">CAMT data mapping to fields in the Bank Acc. Reconciliation Line table (274)</span></span>  

|<span data-ttu-id="be1aa-182">Element Path</span><span class="sxs-lookup"><span data-stu-id="be1aa-182">Element Path</span></span>|<span data-ttu-id="be1aa-183">Message Element</span><span class="sxs-lookup"><span data-stu-id="be1aa-183">Message Element</span></span>|<span data-ttu-id="be1aa-184">Data Type</span><span class="sxs-lookup"><span data-stu-id="be1aa-184">Data Type</span></span>|<span data-ttu-id="be1aa-185">Description</span><span class="sxs-lookup"><span data-stu-id="be1aa-185">Description</span></span>|<span data-ttu-id="be1aa-186">Negative-Sign Identifier</span><span class="sxs-lookup"><span data-stu-id="be1aa-186">Negative-Sign Identifier</span></span>|<span data-ttu-id="be1aa-187">Field No.</span><span class="sxs-lookup"><span data-stu-id="be1aa-187">Field No.</span></span>|<span data-ttu-id="be1aa-188">Field Name</span><span class="sxs-lookup"><span data-stu-id="be1aa-188">Field Name</span></span>|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|<span data-ttu-id="be1aa-189">Stmt/Ntry/Amt</span><span class="sxs-lookup"><span data-stu-id="be1aa-189">Stmt/Ntry/Amt</span></span>|<span data-ttu-id="be1aa-190">Amount</span><span class="sxs-lookup"><span data-stu-id="be1aa-190">Amount</span></span>|<span data-ttu-id="be1aa-191">Decimal</span><span class="sxs-lookup"><span data-stu-id="be1aa-191">Decimal</span></span>|<span data-ttu-id="be1aa-192">The amount of money in the cash entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-192">The amount of money in the cash entry</span></span>||<span data-ttu-id="be1aa-193">7</span><span class="sxs-lookup"><span data-stu-id="be1aa-193">7</span></span>|<span data-ttu-id="be1aa-194">Statement Amount</span><span class="sxs-lookup"><span data-stu-id="be1aa-194">Statement Amount</span></span>|  
|<span data-ttu-id="be1aa-195">Stmt/Ntry/CdtDbtInd</span><span class="sxs-lookup"><span data-stu-id="be1aa-195">Stmt/Ntry/CdtDbtInd</span></span>|<span data-ttu-id="be1aa-196">CreditDebitIndicator</span><span class="sxs-lookup"><span data-stu-id="be1aa-196">CreditDebitIndicator</span></span>|<span data-ttu-id="be1aa-197">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-197">Text</span></span>|<span data-ttu-id="be1aa-198">Indicates whether the entry is a credit or a debit entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-198">Indicates whether the entry is a credit or a debit entry</span></span>|<span data-ttu-id="be1aa-199">DBIT</span><span class="sxs-lookup"><span data-stu-id="be1aa-199">DBIT</span></span>|<span data-ttu-id="be1aa-200">7</span><span class="sxs-lookup"><span data-stu-id="be1aa-200">7</span></span>|<span data-ttu-id="be1aa-201">Statement Amount</span><span class="sxs-lookup"><span data-stu-id="be1aa-201">Statement Amount</span></span>|  
|<span data-ttu-id="be1aa-202">Stmt/Ntry/BookgDt/Dt</span><span class="sxs-lookup"><span data-stu-id="be1aa-202">Stmt/Ntry/BookgDt/Dt</span></span>|<span data-ttu-id="be1aa-203">Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-203">Date</span></span>|<span data-ttu-id="be1aa-204">Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-204">Date</span></span>|<span data-ttu-id="be1aa-205">The date when an entry is posted to an account on the account servicer's books</span><span class="sxs-lookup"><span data-stu-id="be1aa-205">The date when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="be1aa-206">5</span><span class="sxs-lookup"><span data-stu-id="be1aa-206">5</span></span>|<span data-ttu-id="be1aa-207">Transaction Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-207">Transaction Date</span></span>|  
|<span data-ttu-id="be1aa-208">Stmt/Ntry/BookgDt/DtTm</span><span class="sxs-lookup"><span data-stu-id="be1aa-208">Stmt/Ntry/BookgDt/DtTm</span></span>|<span data-ttu-id="be1aa-209">DateTime</span><span class="sxs-lookup"><span data-stu-id="be1aa-209">DateTime</span></span>|<span data-ttu-id="be1aa-210">DateTime</span><span class="sxs-lookup"><span data-stu-id="be1aa-210">DateTime</span></span>|<span data-ttu-id="be1aa-211">The date and time when an entry is posted to an account on the account servicer's books</span><span class="sxs-lookup"><span data-stu-id="be1aa-211">The date and time when an entry is posted to an account on the account servicer's books</span></span>||<span data-ttu-id="be1aa-212">5</span><span class="sxs-lookup"><span data-stu-id="be1aa-212">5</span></span>|<span data-ttu-id="be1aa-213">Transaction Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-213">Transaction Date</span></span>|  
|<span data-ttu-id="be1aa-214">Stmt/Ntry/ValDt/Dt</span><span class="sxs-lookup"><span data-stu-id="be1aa-214">Stmt/Ntry/ValDt/Dt</span></span>|<span data-ttu-id="be1aa-215">Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-215">Date</span></span>|<span data-ttu-id="be1aa-216">Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-216">Date</span></span>|<span data-ttu-id="be1aa-217">The date when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-217">The date when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry</span></span>||<span data-ttu-id="be1aa-218">12</span><span class="sxs-lookup"><span data-stu-id="be1aa-218">12</span></span>|<span data-ttu-id="be1aa-219">Value Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-219">Value Date</span></span>|  
|<span data-ttu-id="be1aa-220">Stmt/Ntry/ValDt/DtTm</span><span class="sxs-lookup"><span data-stu-id="be1aa-220">Stmt/Ntry/ValDt/DtTm</span></span>|<span data-ttu-id="be1aa-221">DateTime</span><span class="sxs-lookup"><span data-stu-id="be1aa-221">DateTime</span></span>|<span data-ttu-id="be1aa-222">DateTime</span><span class="sxs-lookup"><span data-stu-id="be1aa-222">DateTime</span></span>|<span data-ttu-id="be1aa-223">The date and time when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-223">The date and time when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry</span></span>||<span data-ttu-id="be1aa-224">12</span><span class="sxs-lookup"><span data-stu-id="be1aa-224">12</span></span>|<span data-ttu-id="be1aa-225">Value Date</span><span class="sxs-lookup"><span data-stu-id="be1aa-225">Value Date</span></span>|  
|<span data-ttu-id="be1aa-226">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span><span class="sxs-lookup"><span data-stu-id="be1aa-226">Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm</span></span>|<span data-ttu-id="be1aa-227">Name</span><span class="sxs-lookup"><span data-stu-id="be1aa-227">Name</span></span>|<span data-ttu-id="be1aa-228">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-228">Text</span></span>|<span data-ttu-id="be1aa-229">The name of the party that owes an amount of money to the (ultimate) creditor</span><span class="sxs-lookup"><span data-stu-id="be1aa-229">The name of the party that owes an amount of money to the (ultimate) creditor</span></span>||<span data-ttu-id="be1aa-230">15</span><span class="sxs-lookup"><span data-stu-id="be1aa-230">15</span></span>|<span data-ttu-id="be1aa-231">Payer Information</span><span class="sxs-lookup"><span data-stu-id="be1aa-231">Payer Information</span></span>|  
|<span data-ttu-id="be1aa-232">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span><span class="sxs-lookup"><span data-stu-id="be1aa-232">Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd</span></span>|<span data-ttu-id="be1aa-233">Unstructured</span><span class="sxs-lookup"><span data-stu-id="be1aa-233">Unstructured</span></span>|<span data-ttu-id="be1aa-234">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-234">Text</span></span>|<span data-ttu-id="be1aa-235">Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form</span><span class="sxs-lookup"><span data-stu-id="be1aa-235">Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form</span></span>||<span data-ttu-id="be1aa-236">6</span><span class="sxs-lookup"><span data-stu-id="be1aa-236">6</span></span>|<span data-ttu-id="be1aa-237">Description</span><span class="sxs-lookup"><span data-stu-id="be1aa-237">Description</span></span>|  
|<span data-ttu-id="be1aa-238">Stmt/Ntry/AddtlNtryInf</span><span class="sxs-lookup"><span data-stu-id="be1aa-238">Stmt/Ntry/AddtlNtryInf</span></span>|<span data-ttu-id="be1aa-239">AdditionalEntryInformation</span><span class="sxs-lookup"><span data-stu-id="be1aa-239">AdditionalEntryInformation</span></span>|<span data-ttu-id="be1aa-240">Text</span><span class="sxs-lookup"><span data-stu-id="be1aa-240">Text</span></span>|<span data-ttu-id="be1aa-241">Additional information about the entry</span><span class="sxs-lookup"><span data-stu-id="be1aa-241">Additional information about the entry</span></span>||<span data-ttu-id="be1aa-242">16</span><span class="sxs-lookup"><span data-stu-id="be1aa-242">16</span></span>|<span data-ttu-id="be1aa-243">Transaction Information</span><span class="sxs-lookup"><span data-stu-id="be1aa-243">Transaction Information</span></span>|  

 <span data-ttu-id="be1aa-244">Elements in the **Ntry** node that are imported into [!INCLUDE[d365fin](includes/d365fin_md.md)] but not mapped to any fields are stored in the **Posting Exch. Column Def** table.</span><span class="sxs-lookup"><span data-stu-id="be1aa-244">Elements in the **Ntry** node that are imported into [!INCLUDE[d365fin](includes/d365fin_md.md)] but not mapped to any fields are stored in the **Posting Exch. Column Def** table.</span></span> <span data-ttu-id="be1aa-245">Users can view these elements from the **Payment Reconciliation Journal**, **Payment Application**, and **Bank Acc. Reconciliation** pages by choosing the **Bank Statement Line Details** action.</span><span class="sxs-lookup"><span data-stu-id="be1aa-245">Users can view these elements from the **Payment Reconciliation Journal**, **Payment Application**, and **Bank Acc. Reconciliation** pages by choosing the **Bank Statement Line Details** action.</span></span> <span data-ttu-id="be1aa-246">For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="be1aa-246">For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span></span>  
## <a name="see-also"></a><span data-ttu-id="be1aa-247">See Also</span><span class="sxs-lookup"><span data-stu-id="be1aa-247">See Also</span></span>  
[<span data-ttu-id="be1aa-248">Setting Up Data Exchange</span><span class="sxs-lookup"><span data-stu-id="be1aa-248">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)  
[<span data-ttu-id="be1aa-249">Exchanging Data Electronically</span><span class="sxs-lookup"><span data-stu-id="be1aa-249">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
<span data-ttu-id="be1aa-250">[Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md) </span><span class="sxs-lookup"><span data-stu-id="be1aa-250">[Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md) </span></span>  
[<span data-ttu-id="be1aa-251">Use XML Schemas to Prepare Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="be1aa-251">Use XML Schemas to Prepare Data Exchange Definitions</span></span>](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)  
[<span data-ttu-id="be1aa-252">Reconcile Payments Using Automatic Application</span><span class="sxs-lookup"><span data-stu-id="be1aa-252">Reconcile Payments Using Automatic Application</span></span>](receivables-how-reconcile-payments-auto-application.md)  