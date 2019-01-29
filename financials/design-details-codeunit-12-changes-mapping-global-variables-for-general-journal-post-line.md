---
title: Design Details - Codeunit 12 Changes in Mapping Global Variables for General Journal Post Line | Microsoft Docs
description: The following changes have been implemented in this release of Business Central.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 880bbeaf87e5969fdd637373692baff66dd0ac4b
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "233130"
---
# <a name="codeunit-12-changes-mapping-global-variables-for-general-journal-post-line"></a><span data-ttu-id="2ea88-103">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="2ea88-103">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>
<span data-ttu-id="2ea88-104">The following changes have been implemented in this release of [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2ea88-104">The following changes have been implemented in this release of [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span>  

|<span data-ttu-id="2ea88-105">**Microsoft Dynamics NAV 2009 R2**</span><span class="sxs-lookup"><span data-stu-id="2ea88-105">**Microsoft Dynamics NAV 2009 R2**</span></span>|<span data-ttu-id="2ea88-106">**Microsoft Dynamics NAV 2013 R2**</span><span class="sxs-lookup"><span data-stu-id="2ea88-106">**Microsoft Dynamics NAV 2013 R2**</span></span>|<span data-ttu-id="2ea88-107">**Comment**</span><span class="sxs-lookup"><span data-stu-id="2ea88-107">**Comment**</span></span>|  
|----------------------------------------|----------------------------------------|-----------------|  
|<span data-ttu-id="2ea88-108">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="2ea88-108">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="2ea88-109">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="2ea88-109">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="2ea88-110">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-110">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-111">SalesSetup@1010 : Record 311;</span><span class="sxs-lookup"><span data-stu-id="2ea88-111">SalesSetup@1010 : Record 311;</span></span>||<span data-ttu-id="2ea88-112">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-112">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-113">PurchSetup@1011 : Record 312;</span><span class="sxs-lookup"><span data-stu-id="2ea88-113">PurchSetup@1011 : Record 312;</span></span>||<span data-ttu-id="2ea88-114">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-114">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-115">AccountingPeriod@1012 : Record 50;</span><span class="sxs-lookup"><span data-stu-id="2ea88-115">AccountingPeriod@1012 : Record 50;</span></span>||<span data-ttu-id="2ea88-116">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-116">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-117">GLAcc@1013 : Record 15;</span><span class="sxs-lookup"><span data-stu-id="2ea88-117">GLAcc@1013 : Record 15;</span></span>||<span data-ttu-id="2ea88-118">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-118">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-119">GLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-119">GLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="2ea88-120">GlobalGLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-120">GlobalGLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="2ea88-121">Renamed</span><span class="sxs-lookup"><span data-stu-id="2ea88-121">Renamed</span></span>|  
|<span data-ttu-id="2ea88-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="2ea88-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="2ea88-124">Renamed</span><span class="sxs-lookup"><span data-stu-id="2ea88-124">Renamed</span></span>|  
|<span data-ttu-id="2ea88-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="2ea88-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="2ea88-127">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-127">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-128">OrigGLEntry@1017 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-128">OrigGLEntry@1017 : Record 17;</span></span>||<span data-ttu-id="2ea88-129">Deleted</span><span class="sxs-lookup"><span data-stu-id="2ea88-129">Deleted</span></span>|  
|<span data-ttu-id="2ea88-130">VATPostingSetup@1019 : Record 325;</span><span class="sxs-lookup"><span data-stu-id="2ea88-130">VATPostingSetup@1019 : Record 325;</span></span>||<span data-ttu-id="2ea88-131">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-131">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-132">Cust@1020 : Record 18;</span><span class="sxs-lookup"><span data-stu-id="2ea88-132">Cust@1020 : Record 18;</span></span>||<span data-ttu-id="2ea88-133">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-133">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-134">Vend@1021 : Record 23;</span><span class="sxs-lookup"><span data-stu-id="2ea88-134">Vend@1021 : Record 23;</span></span>||<span data-ttu-id="2ea88-135">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-135">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-136">GenJnlLine@1022 : Record 81;</span><span class="sxs-lookup"><span data-stu-id="2ea88-136">GenJnlLine@1022 : Record 81;</span></span>||<span data-ttu-id="2ea88-137">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-137">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-138">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="2ea88-138">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="2ea88-139">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="2ea88-139">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="2ea88-140">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-140">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-141">CustPostingGr@1030 : Record 92;</span><span class="sxs-lookup"><span data-stu-id="2ea88-141">CustPostingGr@1030 : Record 92;</span></span>||<span data-ttu-id="2ea88-142">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-142">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-143">VendPostingGr@1031 : Record 93;</span><span class="sxs-lookup"><span data-stu-id="2ea88-143">VendPostingGr@1031 : Record 93;</span></span>||<span data-ttu-id="2ea88-144">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-144">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-145">Currency@1032 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="2ea88-145">Currency@1032 : Record 4;</span></span>||<span data-ttu-id="2ea88-146">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-146">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-147">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="2ea88-147">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="2ea88-148">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="2ea88-148">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="2ea88-149">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-149">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-150">ApplnCurrency@1034 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="2ea88-150">ApplnCurrency@1034 : Record 4;</span></span>||<span data-ttu-id="2ea88-151">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-151">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-152">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="2ea88-152">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="2ea88-153">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="2ea88-153">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="2ea88-154">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-154">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-155">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="2ea88-155">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="2ea88-156">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="2ea88-156">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="2ea88-157">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-157">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-158">BankAcc@1039 : Record 270;</span><span class="sxs-lookup"><span data-stu-id="2ea88-158">BankAcc@1039 : Record 270;</span></span>||<span data-ttu-id="2ea88-159">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-159">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-160">BankAccLedgEntry@1040 : Record 271;</span><span class="sxs-lookup"><span data-stu-id="2ea88-160">BankAccLedgEntry@1040 : Record 271;</span></span>||<span data-ttu-id="2ea88-161">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-161">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-162">CheckLedgEntry@1041 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="2ea88-162">CheckLedgEntry@1041 : Record 272;</span></span>||<span data-ttu-id="2ea88-163">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-163">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-164">CheckLedgEntry2@1042 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="2ea88-164">CheckLedgEntry2@1042 : Record 272;</span></span>||<span data-ttu-id="2ea88-165">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-165">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-166">BankAccPostingGr@1043 : Record 277;</span><span class="sxs-lookup"><span data-stu-id="2ea88-166">BankAccPostingGr@1043 : Record 277;</span></span>||<span data-ttu-id="2ea88-167">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-167">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-168">GenJnlTemplate@1044 : Record 80;</span><span class="sxs-lookup"><span data-stu-id="2ea88-168">GenJnlTemplate@1044 : Record 80;</span></span>||<span data-ttu-id="2ea88-169">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-169">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-170">TaxJurisdiction@1045 : Record 320;</span><span class="sxs-lookup"><span data-stu-id="2ea88-170">TaxJurisdiction@1045 : Record 320;</span></span>||<span data-ttu-id="2ea88-171">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-171">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-172">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="2ea88-172">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="2ea88-173">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="2ea88-173">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="2ea88-174">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-174">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span><span class="sxs-lookup"><span data-stu-id="2ea88-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span></span>||<span data-ttu-id="2ea88-176">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-176">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-177">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="2ea88-177">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="2ea88-178">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="2ea88-178">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="2ea88-179">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-179">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-180">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="2ea88-180">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="2ea88-181">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="2ea88-181">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="2ea88-182">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-182">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-183">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="2ea88-183">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="2ea88-184">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="2ea88-184">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="2ea88-185">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-185">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-186">TempVATEntry@1088 : TEMPORARY Record 254;</span><span class="sxs-lookup"><span data-stu-id="2ea88-186">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="2ea88-187">TempVATEntry@1088 : TEMPORARY Record 254;</span><span class="sxs-lookup"><span data-stu-id="2ea88-187">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="2ea88-188">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-188">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="2ea88-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span></span>||<span data-ttu-id="2ea88-190">Moved to Codeunit17</span><span class="sxs-lookup"><span data-stu-id="2ea88-190">Moved to Codeunit17</span></span>|  
|<span data-ttu-id="2ea88-191">CostAccSetup@1092 : Record 1108;</span><span class="sxs-lookup"><span data-stu-id="2ea88-191">CostAccSetup@1092 : Record 1108;</span></span>||<span data-ttu-id="2ea88-192">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-192">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-193">GenJnlCheckLine@1048 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="2ea88-193">GenJnlCheckLine@1048 : Codeunit 11;</span></span>|<span data-ttu-id="2ea88-194">GenJnlCheckLine@1001 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="2ea88-194">GenJnlCheckLine@1001 : Codeunit 11;</span></span>|<span data-ttu-id="2ea88-195">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-195">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span><span class="sxs-lookup"><span data-stu-id="2ea88-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span></span>||<span data-ttu-id="2ea88-197">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-197">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-198">FAJnlPostLine@1050 : Codeunit 5632;</span><span class="sxs-lookup"><span data-stu-id="2ea88-198">FAJnlPostLine@1050 : Codeunit 5632;</span></span>||<span data-ttu-id="2ea88-199">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-199">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-200">SalesTaxCalculate@1051 : Codeunit 398;</span><span class="sxs-lookup"><span data-stu-id="2ea88-200">SalesTaxCalculate@1051 : Codeunit 398;</span></span>||<span data-ttu-id="2ea88-201">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-201">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-202">GenJnlApply@1052 : Codeunit 225;</span><span class="sxs-lookup"><span data-stu-id="2ea88-202">GenJnlApply@1052 : Codeunit 225;</span></span>||<span data-ttu-id="2ea88-203">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-203">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-204">DimMgt@1053 : Codeunit 408;</span><span class="sxs-lookup"><span data-stu-id="2ea88-204">DimMgt@1053 : Codeunit 408;</span></span>||<span data-ttu-id="2ea88-205">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-205">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-206">JobPostLine@1028 : Codeunit 1001;</span><span class="sxs-lookup"><span data-stu-id="2ea88-206">JobPostLine@1028 : Codeunit 1001;</span></span>||<span data-ttu-id="2ea88-207">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-207">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span><span class="sxs-lookup"><span data-stu-id="2ea88-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span></span>||<span data-ttu-id="2ea88-209">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-209">Changed to Local</span></span>|  
||<span data-ttu-id="2ea88-210">PaymentToleranceMgt@1002 : Codeunit 426;</span><span class="sxs-lookup"><span data-stu-id="2ea88-210">PaymentToleranceMgt@1002 : Codeunit 426;</span></span>|<span data-ttu-id="2ea88-211">Added</span><span class="sxs-lookup"><span data-stu-id="2ea88-211">Added</span></span>|  
||<span data-ttu-id="2ea88-212">AddCurrencyCode@1117 : Code[10];</span><span class="sxs-lookup"><span data-stu-id="2ea88-212">AddCurrencyCode@1117 : Code[10];</span></span>|<span data-ttu-id="2ea88-213">Added</span><span class="sxs-lookup"><span data-stu-id="2ea88-213">Added</span></span>|  
|<span data-ttu-id="2ea88-214">FiscalYearStartDate@1054 : Date;</span><span class="sxs-lookup"><span data-stu-id="2ea88-214">FiscalYearStartDate@1054 : Date;</span></span>|<span data-ttu-id="2ea88-215">FiscalYearStartDate@1011 : Date;</span><span class="sxs-lookup"><span data-stu-id="2ea88-215">FiscalYearStartDate@1011 : Date;</span></span>|<span data-ttu-id="2ea88-216">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-216">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-217">NextEntryNo@1055 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-217">NextEntryNo@1055 : Integer;</span></span>|<span data-ttu-id="2ea88-218">NextEntryNo@1022 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-218">NextEntryNo@1022 : Integer;</span></span>|<span data-ttu-id="2ea88-219">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-219">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-220">BalanceCheckAmount@1056 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-220">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="2ea88-221">BalanceCheckAmount@1056 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-221">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="2ea88-222">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-222">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-223">BalanceCheckAmount2@1057 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-223">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="2ea88-224">BalanceCheckAmount2@1057 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-224">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="2ea88-225">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-225">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="2ea88-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="2ea88-228">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-228">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="2ea88-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="2ea88-231">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-231">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-232">CurrentBalance@1060 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-232">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="2ea88-233">CurrentBalance@1060 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-233">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="2ea88-234">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-234">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-235">SalesTaxBaseAmount@1061 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-235">SalesTaxBaseAmount@1061 : Decimal;</span></span>||<span data-ttu-id="2ea88-236">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-236">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-237">TotalAddCurrAmount@1062 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-237">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="2ea88-238">TotalAddCurrAmount@1062 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-238">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="2ea88-239">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-239">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-240">TotalAmount@1063 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-240">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="2ea88-241">TotalAmount@1063 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-241">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="2ea88-242">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-242">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="2ea88-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="2ea88-245">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-245">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="2ea88-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="2ea88-248">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-248">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-249">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-249">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="2ea88-250">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-250">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="2ea88-251">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-251">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-252">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-252">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="2ea88-253">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-253">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="2ea88-254">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-254">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-255">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-255">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="2ea88-256">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-256">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="2ea88-257">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-257">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-258">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-258">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="2ea88-259">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-259">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="2ea88-260">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-260">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-261">InsertedTempGLEntryVAT@1068 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-261">InsertedTempGLEntryVAT@1068 : Integer;</span></span>|<span data-ttu-id="2ea88-262">InsertedTempGLEntryVAT@1027 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-262">InsertedTempGLEntryVAT@1027 : Integer;</span></span>|<span data-ttu-id="2ea88-263">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-263">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-264">LastDocNo@1069 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="2ea88-264">LastDocNo@1069 : Code[20];</span></span>|<span data-ttu-id="2ea88-265">LastDocNo@1023 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="2ea88-265">LastDocNo@1023 : Code[20];</span></span>|<span data-ttu-id="2ea88-266">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-266">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-267">LastLineNo@1070 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-267">LastLineNo@1070 : Integer;</span></span>||<span data-ttu-id="2ea88-268">Deleted</span><span class="sxs-lookup"><span data-stu-id="2ea88-268">Deleted</span></span>|  
|<span data-ttu-id="2ea88-269">LastDate@1071 : Date;</span><span class="sxs-lookup"><span data-stu-id="2ea88-269">LastDate@1071 : Date;</span></span>|<span data-ttu-id="2ea88-270">LastDate@1021 : Date;</span><span class="sxs-lookup"><span data-stu-id="2ea88-270">LastDate@1021 : Date;</span></span>|<span data-ttu-id="2ea88-271">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-271">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span><span class="sxs-lookup"><span data-stu-id="2ea88-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="2ea88-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span><span class="sxs-lookup"><span data-stu-id="2ea88-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="2ea88-274">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-274">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-275">NextCheckEntryNo@1073 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-275">NextCheckEntryNo@1073 : Integer;</span></span>|<span data-ttu-id="2ea88-276">NextCheckEntryNo@1028 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-276">NextCheckEntryNo@1028 : Integer;</span></span>|<span data-ttu-id="2ea88-277">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-277">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span></span>|<span data-ttu-id="2ea88-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span></span>|<span data-ttu-id="2ea88-280">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-280">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-281">CurrencyDate@1076 : Date;</span><span class="sxs-lookup"><span data-stu-id="2ea88-281">CurrencyDate@1076 : Date;</span></span>|<span data-ttu-id="2ea88-282">CurrencyDate@1020 : Date;</span><span class="sxs-lookup"><span data-stu-id="2ea88-282">CurrencyDate@1020 : Date;</span></span>|<span data-ttu-id="2ea88-283">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-283">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-284">CurrencyFactor@1077 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-284">CurrencyFactor@1077 : Decimal;</span></span>|<span data-ttu-id="2ea88-285">CurrencyFactor@1019 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-285">CurrencyFactor@1019 : Decimal;</span></span>|<span data-ttu-id="2ea88-286">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-286">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-287">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-287">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="2ea88-288">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-288">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="2ea88-289">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-289">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-290">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-290">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="2ea88-291">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-291">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="2ea88-292">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-292">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-293">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-293">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="2ea88-294">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-294">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="2ea88-295">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-295">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-296">AllApplied@1081 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-296">AllApplied@1081 : Boolean;</span></span>||<span data-ttu-id="2ea88-297">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="2ea88-297">Changed to Local</span></span>|  
|<span data-ttu-id="2ea88-298">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-298">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="2ea88-299">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-299">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="2ea88-300">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-300">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-301">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-301">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="2ea88-302">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-302">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="2ea88-303">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-303">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-304">Prepayment@1037 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-304">Prepayment@1037 : Boolean;</span></span>||<span data-ttu-id="2ea88-305">Deleted</span><span class="sxs-lookup"><span data-stu-id="2ea88-305">Deleted</span></span>|  
|<span data-ttu-id="2ea88-306">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-306">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="2ea88-307">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-307">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="2ea88-308">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-308">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-309">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-309">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="2ea88-310">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-310">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="2ea88-311">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-311">Unchanged</span></span>|  
|<span data-ttu-id="2ea88-312">GLEntryNo@1090 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-312">GLEntryNo@1090 : Integer;</span></span>|<span data-ttu-id="2ea88-313">GLEntryNo@1026 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-313">GLEntryNo@1026 : Integer;</span></span>|<span data-ttu-id="2ea88-314">Unchanged</span><span class="sxs-lookup"><span data-stu-id="2ea88-314">Unchanged</span></span>|  
||<span data-ttu-id="2ea88-315">GLSetupRead@1015 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="2ea88-315">GLSetupRead@1015 : Boolean;</span></span>|<span data-ttu-id="2ea88-316">Added</span><span class="sxs-lookup"><span data-stu-id="2ea88-316">Added</span></span>|  
||<span data-ttu-id="2ea88-317">AmountRoundingPrecision@1012 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="2ea88-317">AmountRoundingPrecision@1012 : Decimal;</span></span>|<span data-ttu-id="2ea88-318">Added</span><span class="sxs-lookup"><span data-stu-id="2ea88-318">Added</span></span>|  
||<span data-ttu-id="2ea88-319">CrCardTransactionEntryNo@1013 : Integer;</span><span class="sxs-lookup"><span data-stu-id="2ea88-319">CrCardTransactionEntryNo@1013 : Integer;</span></span>|<span data-ttu-id="2ea88-320">Added</span><span class="sxs-lookup"><span data-stu-id="2ea88-320">Added</span></span>|  

## <a name="see-also"></a><span data-ttu-id="2ea88-321">See Also</span><span class="sxs-lookup"><span data-stu-id="2ea88-321">See Also</span></span>  
 [<span data-ttu-id="2ea88-322">Design Details: Codeunit 12 Changes: Changes in General Journal Post Procedures</span><span class="sxs-lookup"><span data-stu-id="2ea88-322">Design Details: Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)