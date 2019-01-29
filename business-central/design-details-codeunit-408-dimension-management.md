---
title: Design Details - Codeunit 408 Dimension Management | Microsoft Docs
description: Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 95d4afc18b0be620df2f4b2067a093237c7c4df2
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "240943"
---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="4649b-103">Design Details: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="4649b-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="4649b-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="4649b-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="4649b-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span><span class="sxs-lookup"><span data-stu-id="4649b-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="4649b-106">Many functions are deleted because there is no need for copying between dimension tables.</span><span class="sxs-lookup"><span data-stu-id="4649b-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="4649b-107">Modified Functions</span><span class="sxs-lookup"><span data-stu-id="4649b-107">Modified Functions</span></span>  

|<span data-ttu-id="4649b-108">Function Name</span><span class="sxs-lookup"><span data-stu-id="4649b-108">Function Name</span></span>|<span data-ttu-id="4649b-109">Modification Description</span><span class="sxs-lookup"><span data-stu-id="4649b-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="4649b-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="4649b-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="4649b-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span><span class="sxs-lookup"><span data-stu-id="4649b-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="4649b-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="4649b-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="4649b-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="4649b-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="4649b-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="4649b-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="4649b-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="4649b-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="4649b-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="4649b-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="4649b-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="4649b-117">CheckDimValueComb</span></span>|<span data-ttu-id="4649b-118">Delete.</span><span class="sxs-lookup"><span data-stu-id="4649b-118">Delete.</span></span> <span data-ttu-id="4649b-119">All usage should be changed to CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="4649b-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="4649b-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-120">GetDefaultDim</span></span>|<span data-ttu-id="4649b-121">Modify to return an integer Dimension Set ID instead of a set of records.</span><span class="sxs-lookup"><span data-stu-id="4649b-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="4649b-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="4649b-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="4649b-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="4649b-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="4649b-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="4649b-126">Modify to work with DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="4649b-127">Deleted Functions</span><span class="sxs-lookup"><span data-stu-id="4649b-127">Deleted Functions</span></span>  
 <span data-ttu-id="4649b-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span><span class="sxs-lookup"><span data-stu-id="4649b-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="4649b-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="4649b-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="4649b-130">If you have customisations that use one or more of the functions, you must upgrade that code accordingly.</span><span class="sxs-lookup"><span data-stu-id="4649b-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="4649b-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="4649b-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="4649b-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="4649b-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="4649b-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="4649b-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-136">InsertDocDim</span></span>  

 <span data-ttu-id="4649b-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="4649b-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="4649b-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="4649b-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="4649b-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="4649b-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="4649b-141">InsertServContractDim</span></span>  

 <span data-ttu-id="4649b-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="4649b-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="4649b-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="4649b-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="4649b-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-144">GetDocDim</span></span>  

 <span data-ttu-id="4649b-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-145">GetProdDocDim</span></span>  

 <span data-ttu-id="4649b-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="4649b-146">TypeToTableID1</span></span>  

 <span data-ttu-id="4649b-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="4649b-147">TypeToTableID2</span></span>  

 <span data-ttu-id="4649b-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="4649b-148">TypeToTableID3</span></span>  

 <span data-ttu-id="4649b-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="4649b-149">TypeToTableID4</span></span>  

 <span data-ttu-id="4649b-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="4649b-150">TypeToTableID5</span></span>  

 <span data-ttu-id="4649b-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="4649b-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-152">DeleteDocDim</span></span>  

 <span data-ttu-id="4649b-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="4649b-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="4649b-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="4649b-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="4649b-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="4649b-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="4649b-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="4649b-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="4649b-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="4649b-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="4649b-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-160">ShowDocDim</span></span>  

 <span data-ttu-id="4649b-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-161">SaveDocDim</span></span>  

 <span data-ttu-id="4649b-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="4649b-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="4649b-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="4649b-164">ShowTempDim</span></span>  

 <span data-ttu-id="4649b-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="4649b-165">SaveTempDim</span></span>  

 <span data-ttu-id="4649b-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="4649b-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="4649b-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="4649b-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="4649b-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="4649b-168">SaveServContractDim</span></span>  

 <span data-ttu-id="4649b-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="4649b-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="4649b-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="4649b-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="4649b-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="4649b-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="4649b-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="4649b-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="4649b-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="4649b-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="4649b-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="4649b-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="4649b-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="4649b-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="4649b-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="4649b-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="4649b-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="4649b-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="4649b-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="4649b-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="4649b-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="4649b-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="4649b-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="4649b-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="4649b-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="4649b-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="4649b-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="4649b-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="4649b-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="4649b-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="4649b-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="4649b-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="4649b-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="4649b-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="4649b-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="4649b-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="4649b-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="4649b-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="4649b-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="4649b-198">TestDimValue</span></span>  

 <span data-ttu-id="4649b-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="4649b-199">TestNewDimValue</span></span>  

 <span data-ttu-id="4649b-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="4649b-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="4649b-201">(Delete because the ItemBudgetDim Table is deleted.)</span><span class="sxs-lookup"><span data-stu-id="4649b-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="4649b-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="4649b-202">GetServContractDim</span></span>  

 <span data-ttu-id="4649b-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="4649b-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="4649b-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="4649b-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="4649b-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="4649b-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="4649b-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="4649b-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="4649b-207">See Also</span><span class="sxs-lookup"><span data-stu-id="4649b-207">See Also</span></span>
 <span data-ttu-id="4649b-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="4649b-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="4649b-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="4649b-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="4649b-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="4649b-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="4649b-211">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="4649b-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="4649b-212">Design Details: Code Examples of Changed Patterns in Modifications</span><span class="sxs-lookup"><span data-stu-id="4649b-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)