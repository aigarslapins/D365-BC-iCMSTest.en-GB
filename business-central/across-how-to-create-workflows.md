---
title: How to Create Workflows | Microsoft Docs
description: You can create workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
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
ms.openlocfilehash: b8085f02f30d28ed1362ee6cea32d398c86b1694
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "255827"
---
# <a name="create-workflows"></a><span data-ttu-id="414c9-105">Create Workflows</span><span class="sxs-lookup"><span data-stu-id="414c9-105">Create Workflows</span></span>
<span data-ttu-id="414c9-106">You can create workflows that connect business-process tasks performed by different users.</span><span class="sxs-lookup"><span data-stu-id="414c9-106">You can create workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="414c9-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span><span class="sxs-lookup"><span data-stu-id="414c9-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="414c9-108">Requesting and granting approval to create new records are typical workflow steps.</span><span class="sxs-lookup"><span data-stu-id="414c9-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

<span data-ttu-id="414c9-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="414c9-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="414c9-110">Each step consists of a workflow event moderated by event conditions and a workflow response with response options.</span><span class="sxs-lookup"><span data-stu-id="414c9-110">Each step consists of a workflow event moderated by event conditions and a workflow response with response options.</span></span> <span data-ttu-id="414c9-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="414c9-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

<span data-ttu-id="414c9-112">When you create workflows, you can copy the steps from existing workflows or from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="414c9-112">When you create workflows, you can copy the steps from existing workflows or from workflow templates.</span></span> <span data-ttu-id="414c9-113">Workflow templates represent non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="414c9-113">Workflow templates represent non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="414c9-114">The code for workflow templates that are added by Microsoft are prefixed with “MS-“, such as in “MS-PIW”.</span><span class="sxs-lookup"><span data-stu-id="414c9-114">The code for workflow templates that are added by Microsoft are prefixed with “MS-“, such as in “MS-PIW”.</span></span> <span data-ttu-id="414c9-115">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="414c9-115">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

<span data-ttu-id="414c9-116">If your business scenario requires workflow events or responses that are not supported, a Microsoft partner must implement them by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="414c9-116">If your business scenario requires workflow events or responses that are not supported, a Microsoft partner must implement them by customizing the application code.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="414c9-117">All notifications about workflow steps are sent through a job queue.</span><span class="sxs-lookup"><span data-stu-id="414c9-117">All notifications about workflow steps are sent through a job queue.</span></span> <span data-ttu-id="414c9-118">Make sure that the job queue in your installation is set up to handle workflow notifications, and that the **Start Automatically From NAS** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="414c9-118">Make sure that the job queue in your installation is set up to handle workflow notifications, and that the **Start Automatically From NAS** check box is selected.</span></span> <span data-ttu-id="414c9-119">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="414c9-119">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>  

## <a name="to-create-a-workflow"></a><span data-ttu-id="414c9-120">To create a workflow</span><span class="sxs-lookup"><span data-stu-id="414c9-120">To create a workflow</span></span>  
1. <span data-ttu-id="414c9-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="414c9-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2. <span data-ttu-id="414c9-122">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="414c9-122">Choose the **New** action.</span></span> <span data-ttu-id="414c9-123">The **Workflow** page opens.</span><span class="sxs-lookup"><span data-stu-id="414c9-123">The **Workflow** page opens.</span></span>  
3. <span data-ttu-id="414c9-124">In the **Code** field, enter a maximum of 20 characters to identify the workflow.</span><span class="sxs-lookup"><span data-stu-id="414c9-124">In the **Code** field, enter a maximum of 20 characters to identify the workflow.</span></span>  
4. <span data-ttu-id="414c9-125">To create the workflow from a workflow template, on the **Workflows** page, choose the **Create Workflow from Template** action.</span><span class="sxs-lookup"><span data-stu-id="414c9-125">To create the workflow from a workflow template, on the **Workflows** page, choose the **Create Workflow from Template** action.</span></span> <span data-ttu-id="414c9-126">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="414c9-126">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  
5. <span data-ttu-id="414c9-127">In the **Description** field, describe the workflow.</span><span class="sxs-lookup"><span data-stu-id="414c9-127">In the **Description** field, describe the workflow.</span></span>  
6. <span data-ttu-id="414c9-128">In the **Category** field, specify which category the workflow belongs to.</span><span class="sxs-lookup"><span data-stu-id="414c9-128">In the **Category** field, specify which category the workflow belongs to.</span></span>  
7. <span data-ttu-id="414c9-129">In the **When Event** field, specify the event that must occur to start the workflow step.</span><span class="sxs-lookup"><span data-stu-id="414c9-129">In the **When Event** field, specify the event that must occur to start the workflow step.</span></span>  

    <span data-ttu-id="414c9-130">When you choose the field, the **Workflow Events** page opens where you select from all the workflow events that exist.</span><span class="sxs-lookup"><span data-stu-id="414c9-130">When you choose the field, the **Workflow Events** page opens where you select from all the workflow events that exist.</span></span>  
8. <span data-ttu-id="414c9-131">In the **Condition** field, specify one or more conditions that must be met before the event in the **When Event** field can occur.</span><span class="sxs-lookup"><span data-stu-id="414c9-131">In the **Condition** field, specify one or more conditions that must be met before the event in the **When Event** field can occur.</span></span>  

    <span data-ttu-id="414c9-132">When you choose the field, the **Event Conditions** page opens where you choose from a list of filter fields that are relevant as conditions for the event in question.</span><span class="sxs-lookup"><span data-stu-id="414c9-132">When you choose the field, the **Event Conditions** page opens where you choose from a list of filter fields that are relevant as conditions for the event in question.</span></span> <span data-ttu-id="414c9-133">You can add new filter fields that you want to use as event conditions.</span><span class="sxs-lookup"><span data-stu-id="414c9-133">You can add new filter fields that you want to use as event conditions.</span></span> <span data-ttu-id="414c9-134">You set event condition filters just as you set filters on report request pages.</span><span class="sxs-lookup"><span data-stu-id="414c9-134">You set event condition filters just as you set filters on report request pages.</span></span>  

    <span data-ttu-id="414c9-135">If the workflow event is the change of a specific field on a record, then the **Event Conditions** page opens with options to select the field and the type of change.</span><span class="sxs-lookup"><span data-stu-id="414c9-135">If the workflow event is the change of a specific field on a record, then the **Event Conditions** page opens with options to select the field and the type of change.</span></span>  

    1.  <span data-ttu-id="414c9-136">To specify a field change for the event, on the **Event Conditions** page, in the **Field** field, select the field that changes.</span><span class="sxs-lookup"><span data-stu-id="414c9-136">To specify a field change for the event, on the **Event Conditions** page, in the **Field** field, select the field that changes.</span></span>  
    2.  <span data-ttu-id="414c9-137">In the **Operator** field, select either **Decreased**, **Increased**, or **Changed**.</span><span class="sxs-lookup"><span data-stu-id="414c9-137">In the **Operator** field, select either **Decreased**, **Increased**, or **Changed**.</span></span>  
9. <span data-ttu-id="414c9-138">In the **Then Response** field, specify the response that will follow when the workflow event occurs.</span><span class="sxs-lookup"><span data-stu-id="414c9-138">In the **Then Response** field, specify the response that will follow when the workflow event occurs.</span></span>  

     <span data-ttu-id="414c9-139">When you choose the field, the **Workflow Responses** page opens where you select from all workflow responses that exist and set response options for the selected response.</span><span class="sxs-lookup"><span data-stu-id="414c9-139">When you choose the field, the **Workflow Responses** page opens where you select from all workflow responses that exist and set response options for the selected response.</span></span>  
10. <span data-ttu-id="414c9-140">On the **Options for the Selected Response** FastTab, specify options for the workflow response, by selecting values in the different fields that appear, as follows:</span><span class="sxs-lookup"><span data-stu-id="414c9-140">On the **Options for the Selected Response** FastTab, specify options for the workflow response, by selecting values in the different fields that appear, as follows:</span></span>  

    1.  <span data-ttu-id="414c9-141">To specify options for a workflow response that involves sending a notification, fill the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="414c9-141">To specify options for a workflow response that involves sending a notification, fill the fields as described in the following table.</span></span>  

        |<span data-ttu-id="414c9-142">Field</span><span class="sxs-lookup"><span data-stu-id="414c9-142">Field</span></span>|<span data-ttu-id="414c9-143">Description</span><span class="sxs-lookup"><span data-stu-id="414c9-143">Description</span></span>|  
        |----------------------------------|---------------------------------------|  
        |<span data-ttu-id="414c9-144">**Recipient User ID**</span><span class="sxs-lookup"><span data-stu-id="414c9-144">**Recipient User ID**</span></span>|<span data-ttu-id="414c9-145">Specify the user who the notification must be sent to.</span><span class="sxs-lookup"><span data-stu-id="414c9-145">Specify the user who the notification must be sent to.</span></span> <span data-ttu-id="414c9-146">Note: This option is only available for workflow responses with a placeholder for a specific user.</span><span class="sxs-lookup"><span data-stu-id="414c9-146">Note: This option is only available for workflow responses with a placeholder for a specific user.</span></span> <span data-ttu-id="414c9-147">For workflow responses without placeholders for users, the notification recipient is typically defined by the approval user setup.</span><span class="sxs-lookup"><span data-stu-id="414c9-147">For workflow responses without placeholders for users, the notification recipient is typically defined by the approval user setup.</span></span>|  
        |<span data-ttu-id="414c9-148">**Link Target Page**</span><span class="sxs-lookup"><span data-stu-id="414c9-148">**Link Target Page**</span></span>|<span data-ttu-id="414c9-149">Specify another page in [!INCLUDE[d365fin](includes/d365fin_md.md)] that the link in the notification opens instead of the default page.</span><span class="sxs-lookup"><span data-stu-id="414c9-149">Specify another page in [!INCLUDE[d365fin](includes/d365fin_md.md)] that the link in the notification opens instead of the default page.</span></span>|  
        |<span data-ttu-id="414c9-150">**Custom Link**</span><span class="sxs-lookup"><span data-stu-id="414c9-150">**Custom Link**</span></span>|<span data-ttu-id="414c9-151">Specify the URL of a link that is added to the notification in addition to the link to page in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="414c9-151">Specify the URL of a link that is added to the notification in addition to the link to page in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|  
    2.  <span data-ttu-id="414c9-152">To specify options for a workflow response that involves creating an approval request, fill the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="414c9-152">To specify options for a workflow response that involves creating an approval request, fill the fields as described in the following table.</span></span>  

        |<span data-ttu-id="414c9-153">Field</span><span class="sxs-lookup"><span data-stu-id="414c9-153">Field</span></span>|<span data-ttu-id="414c9-154">Description</span><span class="sxs-lookup"><span data-stu-id="414c9-154">Description</span></span>|  
        |----------------------------------|---------------------------------------|  
        |<span data-ttu-id="414c9-155">**Due Date Formula**</span><span class="sxs-lookup"><span data-stu-id="414c9-155">**Due Date Formula**</span></span>|<span data-ttu-id="414c9-156">Specify in how many days the approval request must be resolved from the date when it was sent.</span><span class="sxs-lookup"><span data-stu-id="414c9-156">Specify in how many days the approval request must be resolved from the date when it was sent.</span></span>|  
        |<span data-ttu-id="414c9-157">**Delegate After**</span><span class="sxs-lookup"><span data-stu-id="414c9-157">**Delegate After**</span></span>|<span data-ttu-id="414c9-158">Specify if and when an approval request will automatically be delegated to the relevant substitute.</span><span class="sxs-lookup"><span data-stu-id="414c9-158">Specify if and when an approval request will automatically be delegated to the relevant substitute.</span></span> <span data-ttu-id="414c9-159">You can select to automatically delegate one, two, or five days after the date when the approval was requested.</span><span class="sxs-lookup"><span data-stu-id="414c9-159">You can select to automatically delegate one, two, or five days after the date when the approval was requested.</span></span>|  
        |<span data-ttu-id="414c9-160">**Approver Type**</span><span class="sxs-lookup"><span data-stu-id="414c9-160">**Approver Type**</span></span>|<span data-ttu-id="414c9-161">Specify who the approver is, according to the setup of approval users and workflow users.</span><span class="sxs-lookup"><span data-stu-id="414c9-161">Specify who the approver is, according to the setup of approval users and workflow users.</span></span><br /><br /> <span data-ttu-id="414c9-162">The following options exist:</span><span class="sxs-lookup"><span data-stu-id="414c9-162">The following options exist:</span></span><br /><br /> <span data-ttu-id="414c9-163">-   **Salesperson/Purchaser** specifies that the user who is set up in the **Salespers./Purch. Code** field on the **Approval User Setup** page determines the approver.</span><span class="sxs-lookup"><span data-stu-id="414c9-163">-   **Salesperson/Purchaser** specifies that the user who is set up in the **Salespers./Purch. Code** field on the **Approval User Setup** page determines the approver.</span></span> <span data-ttu-id="414c9-164">Approval request entries are then created according to the value in the **Approver Limit Type** field.</span><span class="sxs-lookup"><span data-stu-id="414c9-164">Approval request entries are then created according to the value in the **Approver Limit Type** field.</span></span><br />     <span data-ttu-id="414c9-165">For more information, see [Set Up Approval Users](across-how-to-set-up-workflow-users.md).</span><span class="sxs-lookup"><span data-stu-id="414c9-165">For more information, see [Set Up Approval Users](across-how-to-set-up-workflow-users.md).</span></span>|  
        |<span data-ttu-id="414c9-166">**Show Confirmation Message**</span><span class="sxs-lookup"><span data-stu-id="414c9-166">**Show Confirmation Message**</span></span>|<span data-ttu-id="414c9-167">Specify if a confirmation message is shown to users after they request an approval.</span><span class="sxs-lookup"><span data-stu-id="414c9-167">Specify if a confirmation message is shown to users after they request an approval.</span></span>|  
        |<span data-ttu-id="414c9-168">**Approver Limit Type**</span><span class="sxs-lookup"><span data-stu-id="414c9-168">**Approver Limit Type**</span></span>|<span data-ttu-id="414c9-169">Specify how approvers’ approval limits affect when approval request entries are created for them.</span><span class="sxs-lookup"><span data-stu-id="414c9-169">Specify how approvers’ approval limits affect when approval request entries are created for them.</span></span> <span data-ttu-id="414c9-170">A qualified approver is an approver whose approval limit is above the value on the request being made.</span><span class="sxs-lookup"><span data-stu-id="414c9-170">A qualified approver is an approver whose approval limit is above the value on the request being made.</span></span><br /><br /> <span data-ttu-id="414c9-171">The following options exist:</span><span class="sxs-lookup"><span data-stu-id="414c9-171">The following options exist:</span></span><br /><br /> <span data-ttu-id="414c9-172">1.  **Approver Chain** specifies that approval request entries are created for all the requester’s approvers up to and including the first qualified approver.</span><span class="sxs-lookup"><span data-stu-id="414c9-172">1.  **Approver Chain** specifies that approval request entries are created for all the requester’s approvers up to and including the first qualified approver.</span></span><br /><span data-ttu-id="414c9-173">2.  **Direct Approver** specifies that an approval request entry is only created for the requester’s immediate approver, regardless of the approver’s approval limit.</span><span class="sxs-lookup"><span data-stu-id="414c9-173">2.  **Direct Approver** specifies that an approval request entry is only created for the requester’s immediate approver, regardless of the approver’s approval limit.</span></span><br /><span data-ttu-id="414c9-174">3.  **First Qualified Approver** specifies that an approval request entry is only created for the requester’s first qualified approver.</span><span class="sxs-lookup"><span data-stu-id="414c9-174">3.  **First Qualified Approver** specifies that an approval request entry is only created for the requester’s first qualified approver.</span></span><br />|  
    3.  <span data-ttu-id="414c9-175">To specify options for a workflow response that involves creating journal lines, fill the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="414c9-175">To specify options for a workflow response that involves creating journal lines, fill the fields as described in the following table.</span></span>  

        |<span data-ttu-id="414c9-176">Field</span><span class="sxs-lookup"><span data-stu-id="414c9-176">Field</span></span>|<span data-ttu-id="414c9-177">Description</span><span class="sxs-lookup"><span data-stu-id="414c9-177">Description</span></span>|  
        |----------------------------------|---------------------------------------|  
        |<span data-ttu-id="414c9-178">**General Journal Template Name**</span><span class="sxs-lookup"><span data-stu-id="414c9-178">**General Journal Template Name**</span></span>|<span data-ttu-id="414c9-179">Specify the name of the general journal template that the specified journal lines are created in.</span><span class="sxs-lookup"><span data-stu-id="414c9-179">Specify the name of the general journal template that the specified journal lines are created in.</span></span>|  
        |<span data-ttu-id="414c9-180">**General Journal Batch Name**</span><span class="sxs-lookup"><span data-stu-id="414c9-180">**General Journal Batch Name**</span></span>|<span data-ttu-id="414c9-181">Specify the name of the general journal batch that the specified journal lines are created in.</span><span class="sxs-lookup"><span data-stu-id="414c9-181">Specify the name of the general journal batch that the specified journal lines are created in.</span></span>|  

11. <span data-ttu-id="414c9-182">Choose the **Increase Indent** and **Decrease Indent** buttons to indent the event name in the **When** field to define the step’s position in the workflow.</span><span class="sxs-lookup"><span data-stu-id="414c9-182">Choose the **Increase Indent** and **Decrease Indent** buttons to indent the event name in the **When** field to define the step’s position in the workflow.</span></span>  
    1.  <span data-ttu-id="414c9-183">Indicate that the step is the next in the workflow sequence by indenting the event name under the event name of the previous step.</span><span class="sxs-lookup"><span data-stu-id="414c9-183">Indicate that the step is the next in the workflow sequence by indenting the event name under the event name of the previous step.</span></span>  
    2.  <span data-ttu-id="414c9-184">Indicate that the step is one of more alternative steps that may start depending on its condition by placing the event name at the same indentation as the other alternative steps.</span><span class="sxs-lookup"><span data-stu-id="414c9-184">Indicate that the step is one of more alternative steps that may start depending on its condition by placing the event name at the same indentation as the other alternative steps.</span></span> <span data-ttu-id="414c9-185">Order such optional steps according to priority by placing the most important step first.</span><span class="sxs-lookup"><span data-stu-id="414c9-185">Order such optional steps according to priority by placing the most important step first.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="414c9-186">You can only change the indent of a step that does not have a subsequent step.</span><span class="sxs-lookup"><span data-stu-id="414c9-186">You can only change the indent of a step that does not have a subsequent step.</span></span>  

12. <span data-ttu-id="414c9-187">Repeat steps 7 through 11 to add more workflow steps, either before or after the step that you have just created.</span><span class="sxs-lookup"><span data-stu-id="414c9-187">Repeat steps 7 through 11 to add more workflow steps, either before or after the step that you have just created.</span></span>  
13. <span data-ttu-id="414c9-188">Select the **Enabled** check box to specify that the workflow will start as soon as the event on the first step of type **Entry Point** occurs.</span><span class="sxs-lookup"><span data-stu-id="414c9-188">Select the **Enabled** check box to specify that the workflow will start as soon as the event on the first step of type **Entry Point** occurs.</span></span> <span data-ttu-id="414c9-189">For more information, see [Using Workflows](across-use-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="414c9-189">For more information, see [Using Workflows](across-use-workflows.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="414c9-190">Do not enable a workflow until you are sure that the workflow is completed and that the involved workflow steps can start.</span><span class="sxs-lookup"><span data-stu-id="414c9-190">Do not enable a workflow until you are sure that the workflow is completed and that the involved workflow steps can start.</span></span>  

> [!TIP]  
>  <span data-ttu-id="414c9-191">To see relations between tables that are used in workflows, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, and then enter **Workflow – Table Relations**.</span><span class="sxs-lookup"><span data-stu-id="414c9-191">To see relations between tables that are used in workflows, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, and then enter **Workflow – Table Relations**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="414c9-192">See Also</span><span class="sxs-lookup"><span data-stu-id="414c9-192">See Also</span></span>  
<span data-ttu-id="414c9-193">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-193">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
<span data-ttu-id="414c9-194">[Set Up Approval Users](across-how-to-set-up-approval-users.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-194">[Set Up Approval Users](across-how-to-set-up-approval-users.md) </span></span>  
<span data-ttu-id="414c9-195">[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-195">[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md) </span></span>  
<span data-ttu-id="414c9-196">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-196">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
<span data-ttu-id="414c9-197">[Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-197">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
<span data-ttu-id="414c9-198">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-198">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
<span data-ttu-id="414c9-199">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-199">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
<span data-ttu-id="414c9-200">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="414c9-200">[Using Workflows](across-use-workflows.md) </span></span>  
[<span data-ttu-id="414c9-201">Workflow</span><span class="sxs-lookup"><span data-stu-id="414c9-201">Workflow</span></span>](across-workflow.md)      
