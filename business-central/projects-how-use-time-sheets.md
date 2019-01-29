---
title: Work with Time Sheets for Jobs| Microsoft Docs
description: Describes how to create a time sheet for a job, copy planning lines to it, define work types, fill in the time sheet, and submit it for approval.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff, resource
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 70d63dcc678a49fa1854b88bc3ca1f9ec8ecc69f
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "236191"
---
# <a name="use-time-sheets-for-jobs"></a><span data-ttu-id="bb650-103">Use Time Sheets for Jobs</span><span class="sxs-lookup"><span data-stu-id="bb650-103">Use Time Sheets for Jobs</span></span>
<span data-ttu-id="bb650-104">You use the **Create Time Sheets** batch job to set up time sheets for a specified number of time periods or weeks.</span><span class="sxs-lookup"><span data-stu-id="bb650-104">You use the **Create Time Sheets** batch job to set up time sheets for a specified number of time periods or weeks.</span></span> <span data-ttu-id="bb650-105">You must have permissions to be able to create time sheets.</span><span class="sxs-lookup"><span data-stu-id="bb650-105">You must have permissions to be able to create time sheets.</span></span>

<span data-ttu-id="bb650-106">You can copy and use your job planning lines in a time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-106">You can copy and use your job planning lines in a time sheet.</span></span> <span data-ttu-id="bb650-107">In that way, you must only enter the information in one place and the line information is always correct.</span><span class="sxs-lookup"><span data-stu-id="bb650-107">In that way, you must only enter the information in one place and the line information is always correct.</span></span>

<span data-ttu-id="bb650-108">After you have approved time sheet entries for a job, you can post them to the relevant job journal or resource journal.</span><span class="sxs-lookup"><span data-stu-id="bb650-108">After you have approved time sheet entries for a job, you can post them to the relevant job journal or resource journal.</span></span>

<span data-ttu-id="bb650-109">Before you can use time sheets, you must set up general information and specify an administrator and one or more approvers of time sheets.</span><span class="sxs-lookup"><span data-stu-id="bb650-109">Before you can use time sheets, you must set up general information and specify an administrator and one or more approvers of time sheets.</span></span> <span data-ttu-id="bb650-110">For more information, see [Set Up Time Sheets](projects-how-setup-time-sheets.md).</span><span class="sxs-lookup"><span data-stu-id="bb650-110">For more information, see [Set Up Time Sheets](projects-how-setup-time-sheets.md).</span></span>

## <a name="to-create-a-time-sheet"></a><span data-ttu-id="bb650-111">To create a time sheet</span><span class="sxs-lookup"><span data-stu-id="bb650-111">To create a time sheet</span></span>
<span data-ttu-id="bb650-112">You can use the **Create Time Sheets** batch job to set up time sheets for a specified number of time periods or weeks.</span><span class="sxs-lookup"><span data-stu-id="bb650-112">You can use the **Create Time Sheets** batch job to set up time sheets for a specified number of time periods or weeks.</span></span> <span data-ttu-id="bb650-113">Then, the time sheet owner can open it and record time that has been spent on a task.</span><span class="sxs-lookup"><span data-stu-id="bb650-113">Then, the time sheet owner can open it and record time that has been spent on a task.</span></span>

1. <span data-ttu-id="bb650-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span></span>
2. <span data-ttu-id="bb650-115">On the **Time Sheet List** page, choose the **Create Time Sheets** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-115">On the **Time Sheet List** page, choose the **Create Time Sheets** action.</span></span>
3. <span data-ttu-id="bb650-116">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bb650-116">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="bb650-117">The **Use Time Sheet** and **Time Sheet Owner User ID** fields must be filled in on the card for the resource of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-117">The **Use Time Sheet** and **Time Sheet Owner User ID** fields must be filled in on the card for the resource of the time sheet.</span></span>

1. <span data-ttu-id="bb650-118">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bb650-118">Choose the **OK** button.</span></span>  

<span data-ttu-id="bb650-119">You can view the time sheets that you have created on the **Time Sheet list** page.</span><span class="sxs-lookup"><span data-stu-id="bb650-119">You can view the time sheets that you have created on the **Time Sheet list** page.</span></span>

## <a name="to-copy-job-planning-lines-to-a-time-sheet"></a><span data-ttu-id="bb650-120">To copy job planning lines to a time sheet</span><span class="sxs-lookup"><span data-stu-id="bb650-120">To copy job planning lines to a time sheet</span></span>
<span data-ttu-id="bb650-121">The following procedure describes how to quickly add job planning lines to a time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-121">The following procedure describes how to quickly add job planning lines to a time sheet.</span></span>

1. <span data-ttu-id="bb650-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bb650-123">On the **Time Sheet List** page, select a time sheet for the relevant time period, and then choose the **Edit Time Sheet** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-123">On the **Time Sheet List** page, select a time sheet for the relevant time period, and then choose the **Edit Time Sheet** action.</span></span>  
3. <span data-ttu-id="bb650-124">Choose the **Create lines from job planning** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-124">Choose the **Create lines from job planning** action.</span></span> <span data-ttu-id="bb650-125">Any job planning lines in the time sheet time period are copied to the time sheet for the person or machine in the **Resource No.** field on the time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-125">Any job planning lines in the time sheet time period are copied to the time sheet for the person or machine in the **Resource No.** field on the time sheet.</span></span>

## <a name="to-define-work-types-and-add-one-to-a-time-sheet"></a><span data-ttu-id="bb650-126">To define work types and add one to a time sheet</span><span class="sxs-lookup"><span data-stu-id="bb650-126">To define work types and add one to a time sheet</span></span>
<span data-ttu-id="bb650-127">You can define the work type for all time sheet lines for jobs.</span><span class="sxs-lookup"><span data-stu-id="bb650-127">You can define the work type for all time sheet lines for jobs.</span></span> <span data-ttu-id="bb650-128">In this way, you can add information that you need to bill the customer for different types of work.</span><span class="sxs-lookup"><span data-stu-id="bb650-128">In this way, you can add information that you need to bill the customer for different types of work.</span></span>

1. <span data-ttu-id="bb650-129">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-129">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span></span>   
2. <span data-ttu-id="bb650-130">Open the relevant time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-130">Open the relevant time sheet.</span></span>
3. <span data-ttu-id="bb650-131">Choose the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="bb650-131">Choose the **Description** field.</span></span>  
4. <span data-ttu-id="bb650-132">On the **Time Sheet Line Job Detail** page, choose the **Work Type Code** field, and select a work type from the list, such as **Miles**.</span><span class="sxs-lookup"><span data-stu-id="bb650-132">On the **Time Sheet Line Job Detail** page, choose the **Work Type Code** field, and select a work type from the list, such as **Miles**.</span></span>  
5. <span data-ttu-id="bb650-133">If no work types exist, chose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-133">If no work types exist, chose the **New** action.</span></span>
6. <span data-ttu-id="bb650-134">On the **Work Types** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bb650-134">On the **Work Types** page, fill in the fields as necessary.</span></span>
7. <span data-ttu-id="bb650-135">Repeat step 4 to assign the new work type to the time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-135">Repeat step 4 to assign the new work type to the time sheet.</span></span>

## <a name="to-reuse-time-sheet-lines-in-other-time-sheets"></a><span data-ttu-id="bb650-136">To reuse time sheet lines in other time sheets</span><span class="sxs-lookup"><span data-stu-id="bb650-136">To reuse time sheet lines in other time sheets</span></span>
<span data-ttu-id="bb650-137">If your time sheet information remains the same from time period to time period, you can save time by copying the lines from the previous time period.</span><span class="sxs-lookup"><span data-stu-id="bb650-137">If your time sheet information remains the same from time period to time period, you can save time by copying the lines from the previous time period.</span></span> <span data-ttu-id="bb650-138">Then, you just enter your time usage for the new period.</span><span class="sxs-lookup"><span data-stu-id="bb650-138">Then, you just enter your time usage for the new period.</span></span>

1. <span data-ttu-id="bb650-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bb650-140">Open the time sheet for a period later than the period for an existing time sheet with lines.</span><span class="sxs-lookup"><span data-stu-id="bb650-140">Open the time sheet for a period later than the period for an existing time sheet with lines.</span></span>  
3. <span data-ttu-id="bb650-141">Choose the **Copy Lines from Previous Time Sheet** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-141">Choose the **Copy Lines from Previous Time Sheet** action.</span></span>

<span data-ttu-id="bb650-142">The lines are copied, including details such as type and description.</span><span class="sxs-lookup"><span data-stu-id="bb650-142">The lines are copied, including details such as type and description.</span></span> <span data-ttu-id="bb650-143">For example, if the line is related to a job, the **Job No.** is copied.</span><span class="sxs-lookup"><span data-stu-id="bb650-143">For example, if the line is related to a job, the **Job No.** is copied.</span></span> <span data-ttu-id="bb650-144">All copied lines have the status **Open**.</span><span class="sxs-lookup"><span data-stu-id="bb650-144">All copied lines have the status **Open**.</span></span> <span data-ttu-id="bb650-145">You can now modify the lines as needed.</span><span class="sxs-lookup"><span data-stu-id="bb650-145">You can now modify the lines as needed.</span></span>

## <a name="to-fill-in-a-time-sheet-lines-and-submit-for-approval"></a><span data-ttu-id="bb650-146">To fill in a time sheet lines and submit for approval</span><span class="sxs-lookup"><span data-stu-id="bb650-146">To fill in a time sheet lines and submit for approval</span></span>
<span data-ttu-id="bb650-147">Time sheet registration is tracked in hours, the standard base unit of measure for resources.</span><span class="sxs-lookup"><span data-stu-id="bb650-147">Time sheet registration is tracked in hours, the standard base unit of measure for resources.</span></span> <span data-ttu-id="bb650-148">By default, a time sheet shows the common work days of Monday through Friday.</span><span class="sxs-lookup"><span data-stu-id="bb650-148">By default, a time sheet shows the common work days of Monday through Friday.</span></span>

1. <span data-ttu-id="bb650-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bb650-150">Select a time sheet for the relevant time period, and then choose the **Edit Time Sheet** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-150">Select a time sheet for the relevant time period, and then choose the **Edit Time Sheet** action.</span></span>  
3. <span data-ttu-id="bb650-151">Fill in the fields on a line as necessary.</span><span class="sxs-lookup"><span data-stu-id="bb650-151">Fill in the fields on a line as necessary.</span></span> <span data-ttu-id="bb650-152">Enter the number of hours used by the resource on each day of the week.</span><span class="sxs-lookup"><span data-stu-id="bb650-152">Enter the number of hours used by the resource on each day of the week.</span></span>

    > [!TIP]  
    >   <span data-ttu-id="bb650-153">You can review the sum of time sheet hours that you have entered in the **Actual/Budgeted Summary** FactBox.</span><span class="sxs-lookup"><span data-stu-id="bb650-153">You can review the sum of time sheet hours that you have entered in the **Actual/Budgeted Summary** FactBox.</span></span>  
4. <span data-ttu-id="bb650-154">Repeat step 3 for other work types that the resource performs.</span><span class="sxs-lookup"><span data-stu-id="bb650-154">Repeat step 3 for other work types that the resource performs.</span></span>
5. <span data-ttu-id="bb650-155">Choose the **Submit** action, and then choose the **All open lines** action to submit all lines or the **Selected lines only** action to submit only the lines that are selected on the **Time Sheet** page.</span><span class="sxs-lookup"><span data-stu-id="bb650-155">Choose the **Submit** action, and then choose the **All open lines** action to submit all lines or the **Selected lines only** action to submit only the lines that are selected on the **Time Sheet** page.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="bb650-156">You can only submit time sheet lines for which you have entered time.</span><span class="sxs-lookup"><span data-stu-id="bb650-156">You can only submit time sheet lines for which you have entered time.</span></span>  
6. <span data-ttu-id="bb650-157">To modify information on a line that has been set to **Submitted**, select the line, and then choose the **Reopen** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-157">To modify information on a line that has been set to **Submitted**, select the line, and then choose the **Reopen** action.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="bb650-158">A manager may reject a time sheet line that is submitted for approval.</span><span class="sxs-lookup"><span data-stu-id="bb650-158">A manager may reject a time sheet line that is submitted for approval.</span></span> <span data-ttu-id="bb650-159">If a line has a status of **Rejected**, you can make changes to the line, and then choose **Submit** again.</span><span class="sxs-lookup"><span data-stu-id="bb650-159">If a line has a status of **Rejected**, you can make changes to the line, and then choose **Submit** again.</span></span>  
7. <span data-ttu-id="bb650-160">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bb650-160">Choose the **OK** button.</span></span>

## <a name="to-approve-or-reject-a-time-sheet"></a><span data-ttu-id="bb650-161">To approve or reject a time sheet</span><span class="sxs-lookup"><span data-stu-id="bb650-161">To approve or reject a time sheet</span></span>
<span data-ttu-id="bb650-162">A time sheet must be submitted for approval before it can be used.</span><span class="sxs-lookup"><span data-stu-id="bb650-162">A time sheet must be submitted for approval before it can be used.</span></span> <span data-ttu-id="bb650-163">You can approve and reject individual lines on a time sheet or send them back to the submitter for additional action.</span><span class="sxs-lookup"><span data-stu-id="bb650-163">You can approve and reject individual lines on a time sheet or send them back to the submitter for additional action.</span></span> <span data-ttu-id="bb650-164">A time sheet can be approved in two ways:</span><span class="sxs-lookup"><span data-stu-id="bb650-164">A time sheet can be approved in two ways:</span></span>

* <span data-ttu-id="bb650-165">A time sheet administrator can approve any time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-165">A time sheet administrator can approve any time sheet.</span></span>
* <span data-ttu-id="bb650-166">The person who is specified in the **Time Sheet Approver User ID** field on a resource card can approve that resource's time sheets.</span><span class="sxs-lookup"><span data-stu-id="bb650-166">The person who is specified in the **Time Sheet Approver User ID** field on a resource card can approve that resource's time sheets.</span></span> <span data-ttu-id="bb650-167">For more information, see [Set Up Time Sheets](projects-how-setup-time-sheets.md).</span><span class="sxs-lookup"><span data-stu-id="bb650-167">For more information, see [Set Up Time Sheets](projects-how-setup-time-sheets.md).</span></span>

1. <span data-ttu-id="bb650-168">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manager Time Sheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-168">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manager Time Sheets**, and then choose the related link.</span></span>
2. <span data-ttu-id="bb650-169">Select a time sheet from the list.</span><span class="sxs-lookup"><span data-stu-id="bb650-169">Select a time sheet from the list.</span></span>  
3. <span data-ttu-id="bb650-170">On the **Time Sheet** page, choose the **Approve** action, and then choose the **All submitted lines** action to approve all lines or the **Selected lines only** action to approve only the lines that are selected on the **Time Sheet** page.</span><span class="sxs-lookup"><span data-stu-id="bb650-170">On the **Time Sheet** page, choose the **Approve** action, and then choose the **All submitted lines** action to approve all lines or the **Selected lines only** action to approve only the lines that are selected on the **Time Sheet** page.</span></span>
4. <span data-ttu-id="bb650-171">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bb650-171">Choose the **OK** button.</span></span>  
5. <span data-ttu-id="bb650-172">Alternatively, choose the **Reject** action and follow steps 4 through 5.</span><span class="sxs-lookup"><span data-stu-id="bb650-172">Alternatively, choose the **Reject** action and follow steps 4 through 5.</span></span>  

> [!TIP]  
>   <span data-ttu-id="bb650-173">Use the **Time Sheet Status** and **Actual/Budgeted Summary** FactBoxes to get an overview of time sheet information.</span><span class="sxs-lookup"><span data-stu-id="bb650-173">Use the **Time Sheet Status** and **Actual/Budgeted Summary** FactBoxes to get an overview of time sheet information.</span></span>

<span data-ttu-id="bb650-174">After you have approved or rejected a time sheet, it cannot be modified unless it is first reopened.</span><span class="sxs-lookup"><span data-stu-id="bb650-174">After you have approved or rejected a time sheet, it cannot be modified unless it is first reopened.</span></span> <span data-ttu-id="bb650-175">The following procedure explains how to reopen an approved or rejected time sheet.</span><span class="sxs-lookup"><span data-stu-id="bb650-175">The following procedure explains how to reopen an approved or rejected time sheet.</span></span>

## <a name="to-reopen-a-time-sheet"></a><span data-ttu-id="bb650-176">To reopen a time sheet</span><span class="sxs-lookup"><span data-stu-id="bb650-176">To reopen a time sheet</span></span>
1. <span data-ttu-id="bb650-177">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manager Time Sheets** or **Time Sheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-177">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manager Time Sheets** or **Time Sheets**, and then choose the related link.</span></span>
2. <span data-ttu-id="bb650-178">Open a time sheet from the list.</span><span class="sxs-lookup"><span data-stu-id="bb650-178">Open a time sheet from the list.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="bb650-179">You can only reopen lines that have the status **Approved**.</span><span class="sxs-lookup"><span data-stu-id="bb650-179">You can only reopen lines that have the status **Approved**.</span></span> <span data-ttu-id="bb650-180">You cannot reopen lines that have the status **Rejected**.</span><span class="sxs-lookup"><span data-stu-id="bb650-180">You cannot reopen lines that have the status **Rejected**.</span></span> <span data-ttu-id="bb650-181">You cannot reopen a time sheet if it has been posted.</span><span class="sxs-lookup"><span data-stu-id="bb650-181">You cannot reopen a time sheet if it has been posted.</span></span>  
3. <span data-ttu-id="bb650-182">On the **Time Sheet** page, choose the **Reopen** action, and then choose the **All submitted lines** action to reopen all lines or the **Selected lines only** action to reopen only the lines that are selected on the **Time Sheet** page.</span><span class="sxs-lookup"><span data-stu-id="bb650-182">On the **Time Sheet** page, choose the **Reopen** action, and then choose the **All submitted lines** action to reopen all lines or the **Selected lines only** action to reopen only the lines that are selected on the **Time Sheet** page.</span></span>
4. <span data-ttu-id="bb650-183">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bb650-183">Choose the **OK** button.</span></span> <span data-ttu-id="bb650-184">The status of the time sheets line or lines is changes to **Submitted**.</span><span class="sxs-lookup"><span data-stu-id="bb650-184">The status of the time sheets line or lines is changes to **Submitted**.</span></span>  

## <a name="to-post-time-sheet-lines-in-a-resource-journal"></a><span data-ttu-id="bb650-185">To post time sheet lines in a resource journal</span><span class="sxs-lookup"><span data-stu-id="bb650-185">To post time sheet lines in a resource journal</span></span>
<span data-ttu-id="bb650-186">After you have approved time sheet entries for a resource, you can post them to the relevant resource journal.</span><span class="sxs-lookup"><span data-stu-id="bb650-186">After you have approved time sheet entries for a resource, you can post them to the relevant resource journal.</span></span>

1. <span data-ttu-id="bb650-187">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-187">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Journal**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bb650-188">Choose the **Suggest Lines from Time Sheets** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-188">Choose the **Suggest Lines from Time Sheets** action.</span></span>  
3. <span data-ttu-id="bb650-189">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bb650-189">Fill in the fields as necessary.</span></span>  
4. <span data-ttu-id="bb650-190">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bb650-190">Choose the **OK** button.</span></span> <span data-ttu-id="bb650-191">Entries for usage are created in the resource journal, where you can modify the information as needed.</span><span class="sxs-lookup"><span data-stu-id="bb650-191">Entries for usage are created in the resource journal, where you can modify the information as needed.</span></span>  
5. <span data-ttu-id="bb650-192">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-192">Choose the **Post** action.</span></span>  
6. <span data-ttu-id="bb650-193">To verify the posting, choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-193">To verify the posting, choose the **Ledger Entries** action.</span></span> <span data-ttu-id="bb650-194">The **Resource Ledger Entries** page opens showing the result of posting the resource journal.</span><span class="sxs-lookup"><span data-stu-id="bb650-194">The **Resource Ledger Entries** page opens showing the result of posting the resource journal.</span></span>

## <a name="to-post-time-sheet-lines-in-a-job-journal"></a><span data-ttu-id="bb650-195">To post time sheet lines in a job journal</span><span class="sxs-lookup"><span data-stu-id="bb650-195">To post time sheet lines in a job journal</span></span>
<span data-ttu-id="bb650-196">After you have approved time sheet entries for a job, you can post them to the relevant job journal.</span><span class="sxs-lookup"><span data-stu-id="bb650-196">After you have approved time sheet entries for a job, you can post them to the relevant job journal.</span></span>

1. <span data-ttu-id="bb650-197">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-197">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journal**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bb650-198">Choose the **Suggest Lines from Time Sheets** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-198">Choose the **Suggest Lines from Time Sheets** action.</span></span>  
3. <span data-ttu-id="bb650-199">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bb650-199">Fill in the fields as necessary.</span></span>  
4. <span data-ttu-id="bb650-200">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bb650-200">Choose the **OK** button.</span></span> <span data-ttu-id="bb650-201">Entries for usage are created in the job journal, where you can modify the information as needed.</span><span class="sxs-lookup"><span data-stu-id="bb650-201">Entries for usage are created in the job journal, where you can modify the information as needed.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="bb650-202">Information about work type and whether the work is chargeable is copied from the time sheet line.</span><span class="sxs-lookup"><span data-stu-id="bb650-202">Information about work type and whether the work is chargeable is copied from the time sheet line.</span></span> <span data-ttu-id="bb650-203">If needed, you can reduce the quantity of hours and do a partial posting.</span><span class="sxs-lookup"><span data-stu-id="bb650-203">If needed, you can reduce the quantity of hours and do a partial posting.</span></span> <span data-ttu-id="bb650-204">If you reduce the quantity, then the next time that you choose the **Suggest Lines From Time Sheets** action, the line that is created will contain the remaining quantity of hours.</span><span class="sxs-lookup"><span data-stu-id="bb650-204">If you reduce the quantity, then the next time that you choose the **Suggest Lines From Time Sheets** action, the line that is created will contain the remaining quantity of hours.</span></span>  
5. <span data-ttu-id="bb650-205">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-205">Choose the **Post** action.</span></span>  
6. <span data-ttu-id="bb650-206">To verify the posting, choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="bb650-206">To verify the posting, choose the **Ledger Entries** action.</span></span> <span data-ttu-id="bb650-207">The **Job Ledger Entries** page opens showing the result of posting the resource journal.</span><span class="sxs-lookup"><span data-stu-id="bb650-207">The **Job Ledger Entries** page opens showing the result of posting the resource journal.</span></span>

## <a name="to-archive-time-sheets"></a><span data-ttu-id="bb650-208">To archive time sheets</span><span class="sxs-lookup"><span data-stu-id="bb650-208">To archive time sheets</span></span>
<span data-ttu-id="bb650-209">After you have posted time sheets, you can archive them for future reference.</span><span class="sxs-lookup"><span data-stu-id="bb650-209">After you have posted time sheets, you can archive them for future reference.</span></span> <span data-ttu-id="bb650-210">All time sheets lines must be posted before a time sheet can be archived.</span><span class="sxs-lookup"><span data-stu-id="bb650-210">All time sheets lines must be posted before a time sheet can be archived.</span></span>

> [!NOTE]  
>   <span data-ttu-id="bb650-211">When you archive a time sheet, it is removed from the lists in both the **Time Sheets** page and the **Manager Time Sheets** page.</span><span class="sxs-lookup"><span data-stu-id="bb650-211">When you archive a time sheet, it is removed from the lists in both the **Time Sheets** page and the **Manager Time Sheets** page.</span></span>

1. <span data-ttu-id="bb650-212">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Move Time Sheets to Archive**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-212">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Move Time Sheets to Archive**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bb650-213">Fill in the fields as necessary, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bb650-213">Fill in the fields as necessary, and then choose the **OK** button.</span></span>  
3. <span data-ttu-id="bb650-214">To review archived time sheets, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheet Archives** or **Manager Time Sheet Archives**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bb650-214">To review archived time sheets, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheet Archives** or **Manager Time Sheet Archives**, and then choose the related link.</span></span>

## <a name="see-also"></a><span data-ttu-id="bb650-215">See Also</span><span class="sxs-lookup"><span data-stu-id="bb650-215">See Also</span></span>
[<span data-ttu-id="bb650-216">Project Management</span><span class="sxs-lookup"><span data-stu-id="bb650-216">Project Management</span></span>](projects-manage-projects.md)  
<span data-ttu-id="bb650-217">[Setting Up Project Management](projects-setup-projects.md)  </span><span class="sxs-lookup"><span data-stu-id="bb650-217">[Setting Up Project Management](projects-setup-projects.md)  </span></span>  
[<span data-ttu-id="bb650-218">Finance</span><span class="sxs-lookup"><span data-stu-id="bb650-218">Finance</span></span>](finance.md)  
<span data-ttu-id="bb650-219">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="bb650-219">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="bb650-220">[Sales](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="bb650-220">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="bb650-221">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bb650-221">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  