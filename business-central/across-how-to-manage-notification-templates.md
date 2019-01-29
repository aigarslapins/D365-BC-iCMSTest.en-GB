---
title: How to Manage Notification Templates | Microsoft Docs
description: Notifications are sent to workflow users to notify them about steps they must make or to inform them about the status of workflow steps. You set up who receives notification and when by setting up approval users, the users’ notification schedule, and the involved workflow responses to define the notification recipient.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/08/2018
ms.author: sgroespe
redirect_url: across-how-to-specify-when-and-how-to-receive-notifications
ms.openlocfilehash: 6c84e5e9e0284249ee7be3f92a82cca2a2fbb3d5
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "269977"
---
# <a name="manage-notification-templates"></a><span data-ttu-id="bc76e-104">Manage Notification Templates</span><span class="sxs-lookup"><span data-stu-id="bc76e-104">Manage Notification Templates</span></span>
<span data-ttu-id="bc76e-105">Notifications are sent to workflow users to notify them about steps they must make or to inform them about the status of workflow steps.</span><span class="sxs-lookup"><span data-stu-id="bc76e-105">Notifications are sent to workflow users to notify them about steps they must make or to inform them about the status of workflow steps.</span></span> <span data-ttu-id="bc76e-106">You set up who receives notification and when by setting up approval users, the users’ notification schedule, and the involved workflow responses to define the notification recipient.</span><span class="sxs-lookup"><span data-stu-id="bc76e-106">You set up who receives notification and when by setting up approval users, the users’ notification schedule, and the involved workflow responses to define the notification recipient.</span></span> <span data-ttu-id="bc76e-107">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="bc76e-107">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span></span>  

 <span data-ttu-id="bc76e-108">Notifications are based on templates that define the content and layout of the notification.</span><span class="sxs-lookup"><span data-stu-id="bc76e-108">Notifications are based on templates that define the content and layout of the notification.</span></span> <span data-ttu-id="bc76e-109">You can export the content of a notification template, edit it, and then import into the same or a new notification template.</span><span class="sxs-lookup"><span data-stu-id="bc76e-109">You can export the content of a notification template, edit it, and then import into the same or a new notification template.</span></span> <span data-ttu-id="bc76e-110">This is described in the following procedures.</span><span class="sxs-lookup"><span data-stu-id="bc76e-110">This is described in the following procedures.</span></span>  

 <span data-ttu-id="bc76e-111">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] contains three notification templates, one for notifying about approval requests, one for notifying about new records, and one for notifying about overdue approval requests.</span><span class="sxs-lookup"><span data-stu-id="bc76e-111">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] contains three notification templates, one for notifying about approval requests, one for notifying about new records, and one for notifying about overdue approval requests.</span></span> <span data-ttu-id="bc76e-112">The three predefined notification templates support **Email** and **Note** as notification method.</span><span class="sxs-lookup"><span data-stu-id="bc76e-112">The three predefined notification templates support **Email** and **Note** as notification method.</span></span> <span data-ttu-id="bc76e-113">To view the content of the three notification templates, see the “Content of the Notification Templates” section in this topic.</span><span class="sxs-lookup"><span data-stu-id="bc76e-113">To view the content of the three notification templates, see the “Content of the Notification Templates” section in this topic.</span></span>

## <a name="to-create-a-new-notification-template"></a><span data-ttu-id="bc76e-114">To create a new notification template</span><span class="sxs-lookup"><span data-stu-id="bc76e-114">To create a new notification template</span></span>  
1.  <span data-ttu-id="bc76e-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Notification Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bc76e-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Notification Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bc76e-116">On the **Notification Templates** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="bc76e-116">On the **Notification Templates** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="bc76e-117">Fill the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="bc76e-117">Fill the fields as described in the following table.</span></span>  

    |<span data-ttu-id="bc76e-118">Field</span><span class="sxs-lookup"><span data-stu-id="bc76e-118">Field</span></span>|<span data-ttu-id="bc76e-119">Description</span><span class="sxs-lookup"><span data-stu-id="bc76e-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="bc76e-120">**Code**</span><span class="sxs-lookup"><span data-stu-id="bc76e-120">**Code**</span></span>|<span data-ttu-id="bc76e-121">Identify the notification template.</span><span class="sxs-lookup"><span data-stu-id="bc76e-121">Identify the notification template.</span></span>|  
    |<span data-ttu-id="bc76e-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc76e-122">**Description**</span></span>|<span data-ttu-id="bc76e-123">Describe the notification template.</span><span class="sxs-lookup"><span data-stu-id="bc76e-123">Describe the notification template.</span></span>|  
    |<span data-ttu-id="bc76e-124">**Notification Method**</span><span class="sxs-lookup"><span data-stu-id="bc76e-124">**Notification Method**</span></span>|<span data-ttu-id="bc76e-125">Specify if the notification is sent as an email or as a note.</span><span class="sxs-lookup"><span data-stu-id="bc76e-125">Specify if the notification is sent as an email or as a note.</span></span>|  
    |<span data-ttu-id="bc76e-126">**Type**</span><span class="sxs-lookup"><span data-stu-id="bc76e-126">**Type**</span></span>|<span data-ttu-id="bc76e-127">Specify the business process that the notification will be used for.</span><span class="sxs-lookup"><span data-stu-id="bc76e-127">Specify the business process that the notification will be used for.</span></span><br /><br /> <span data-ttu-id="bc76e-128">Select one of the following types:</span><span class="sxs-lookup"><span data-stu-id="bc76e-128">Select one of the following types:</span></span><br /><br /> <span data-ttu-id="bc76e-129">-   **Approval** specifies that the template is used to notify users in approval workflows.</span><span class="sxs-lookup"><span data-stu-id="bc76e-129">-   **Approval** specifies that the template is used to notify users in approval workflows.</span></span><br /><span data-ttu-id="bc76e-130">-   **New Record** specifies that the template is to notify approvers when a new record, such as a customer card, needs their approval.</span><span class="sxs-lookup"><span data-stu-id="bc76e-130">-   **New Record** specifies that the template is to notify approvers when a new record, such as a customer card, needs their approval.</span></span><br /><span data-ttu-id="bc76e-131">-   **Overdue** specifies that the template is used to notify users about overdue approval requests.</span><span class="sxs-lookup"><span data-stu-id="bc76e-131">-   **Overdue** specifies that the template is used to notify users about overdue approval requests.</span></span>|  
    |<span data-ttu-id="bc76e-132">**Default**</span><span class="sxs-lookup"><span data-stu-id="bc76e-132">**Default**</span></span>|<span data-ttu-id="bc76e-133">Specify if the notification template will be used by default.</span><span class="sxs-lookup"><span data-stu-id="bc76e-133">Specify if the notification template will be used by default.</span></span>|  

## <a name="to-modify-a-notification-template"></a><span data-ttu-id="bc76e-134">To modify a notification template</span><span class="sxs-lookup"><span data-stu-id="bc76e-134">To modify a notification template</span></span>  
1.  <span data-ttu-id="bc76e-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Notification Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bc76e-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Notification Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bc76e-136">On the **Notification Templates** page, select the notification template that you want to modify.</span><span class="sxs-lookup"><span data-stu-id="bc76e-136">On the **Notification Templates** page, select the notification template that you want to modify.</span></span>  
3.  <span data-ttu-id="bc76e-137">Choose the **Export Template Content** action.</span><span class="sxs-lookup"><span data-stu-id="bc76e-137">Choose the **Export Template Content** action.</span></span>  
4.  <span data-ttu-id="bc76e-138">On the **Export File** page, choose the **Save** button, and then name and save the HTML file in an appropriate location.</span><span class="sxs-lookup"><span data-stu-id="bc76e-138">On the **Export File** page, choose the **Save** button, and then name and save the HTML file in an appropriate location.</span></span>  
5.  <span data-ttu-id="bc76e-139">Right-click the file, choose **Open with**, and then choose the relevant program.</span><span class="sxs-lookup"><span data-stu-id="bc76e-139">Right-click the file, choose **Open with**, and then choose the relevant program.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="bc76e-140">Content for notification templates of type Email are in HTML format.</span><span class="sxs-lookup"><span data-stu-id="bc76e-140">Content for notification templates of type Email are in HTML format.</span></span> <span data-ttu-id="bc76e-141">Content for notification templates of type Note are in TXT format.</span><span class="sxs-lookup"><span data-stu-id="bc76e-141">Content for notification templates of type Note are in TXT format.</span></span>  
6.  <span data-ttu-id="bc76e-142">Edit the content of the notification template by adding, changing, or removing parameter variables to define the content that you want, and then save it.</span><span class="sxs-lookup"><span data-stu-id="bc76e-142">Edit the content of the notification template by adding, changing, or removing parameter variables to define the content that you want, and then save it.</span></span> <span data-ttu-id="bc76e-143">For more information, see the “Content of the Notification Templates” section.</span><span class="sxs-lookup"><span data-stu-id="bc76e-143">For more information, see the “Content of the Notification Templates” section.</span></span>  

    <span data-ttu-id="bc76e-144">Proceed to import the modified content back into the same or a new notification template.</span><span class="sxs-lookup"><span data-stu-id="bc76e-144">Proceed to import the modified content back into the same or a new notification template.</span></span>  
7.  <span data-ttu-id="bc76e-145">To modify the notification template that you exported, on the **Notification Templates** page, select the template that you selected in step 2.</span><span class="sxs-lookup"><span data-stu-id="bc76e-145">To modify the notification template that you exported, on the **Notification Templates** page, select the template that you selected in step 2.</span></span>  

    <span data-ttu-id="bc76e-146">Alternatively, to import the modified template content into a new notification template, follow the “To create a new notification template” procedure, and then select the new notification template.</span><span class="sxs-lookup"><span data-stu-id="bc76e-146">Alternatively, to import the modified template content into a new notification template, follow the “To create a new notification template” procedure, and then select the new notification template.</span></span>  
8.  <span data-ttu-id="bc76e-147">Choose the **Import Template Content** action.</span><span class="sxs-lookup"><span data-stu-id="bc76e-147">Choose the **Import Template Content** action.</span></span>  
9. <span data-ttu-id="bc76e-148">If you are modifying an existing notification template, choose the **Yes** button on the message about overwriting the existing template.</span><span class="sxs-lookup"><span data-stu-id="bc76e-148">If you are modifying an existing notification template, choose the **Yes** button on the message about overwriting the existing template.</span></span>  
10. <span data-ttu-id="bc76e-149">On the **Select a file to import** page, choose the HTML file that you modified in step 6, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="bc76e-149">On the **Select a file to import** page, choose the HTML file that you modified in step 6, and then choose the **Open** button.</span></span>  

<span data-ttu-id="bc76e-150">The existing or new notification template on the **Notification Templates** page is now updated with the modified content.</span><span class="sxs-lookup"><span data-stu-id="bc76e-150">The existing or new notification template on the **Notification Templates** page is now updated with the modified content.</span></span>  

### <a name="content-of-the-notification-templates"></a><span data-ttu-id="bc76e-151">Content of the Notification Templates</span><span class="sxs-lookup"><span data-stu-id="bc76e-151">Content of the Notification Templates</span></span>  
<span data-ttu-id="bc76e-152">The three notification template types, **New Record**, **Approval**, and **Overdue**, have different content.</span><span class="sxs-lookup"><span data-stu-id="bc76e-152">The three notification template types, **New Record**, **Approval**, and **Overdue**, have different content.</span></span>  

<span data-ttu-id="bc76e-153">Parameter values are automatically inserted in notifications according to the notification template type.</span><span class="sxs-lookup"><span data-stu-id="bc76e-153">Parameter values are automatically inserted in notifications according to the notification template type.</span></span>  

#### <a name="new-record"></a><span data-ttu-id="bc76e-154">New Record</span><span class="sxs-lookup"><span data-stu-id="bc76e-154">New Record</span></span>  
 <span data-ttu-id="bc76e-155">![NAV&#95;notification&#95;template&#95;new&#95;record&#95;type](media/nav_notification_template_new_record.png "NAV_notification_template_new_record")</span><span class="sxs-lookup"><span data-stu-id="bc76e-155">![NAV&#95;notification&#95;template&#95;new&#95;record&#95;type](media/nav_notification_template_new_record.png "NAV_notification_template_new_record")</span></span>  

#### <a name="approval"></a><span data-ttu-id="bc76e-156">Approval</span><span class="sxs-lookup"><span data-stu-id="bc76e-156">Approval</span></span>  
 <span data-ttu-id="bc76e-157">![NAV&#95;notification&#95;template&#95;approval&#95;type](media/nav_notification_template_approval_type.png "NAV_notification_template_approval_type")</span><span class="sxs-lookup"><span data-stu-id="bc76e-157">![NAV&#95;notification&#95;template&#95;approval&#95;type](media/nav_notification_template_approval_type.png "NAV_notification_template_approval_type")</span></span>  

#### <a name="overdue"></a><span data-ttu-id="bc76e-158">Overdue</span><span class="sxs-lookup"><span data-stu-id="bc76e-158">Overdue</span></span>  
 <span data-ttu-id="bc76e-159">![NAV&#95;notification&#95;overdue&#95;type](media/nav_notification_overdue_type.png "NAV_notification_overdue_type")</span><span class="sxs-lookup"><span data-stu-id="bc76e-159">![NAV&#95;notification&#95;overdue&#95;type](media/nav_notification_overdue_type.png "NAV_notification_overdue_type")</span></span>  

## <a name="see-also"></a><span data-ttu-id="bc76e-160">See Also</span><span class="sxs-lookup"><span data-stu-id="bc76e-160">See Also</span></span>  
 <span data-ttu-id="bc76e-161">[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md) </span><span class="sxs-lookup"><span data-stu-id="bc76e-161">[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md) </span></span>  
 <span data-ttu-id="bc76e-162">[Set up Email](admin-how-setup-email.md) </span><span class="sxs-lookup"><span data-stu-id="bc76e-162">[Set up Email](admin-how-setup-email.md) </span></span>  
 <span data-ttu-id="bc76e-163">[Set Up Workflow Users](across-how-to-set-up-workflow-users.md) </span><span class="sxs-lookup"><span data-stu-id="bc76e-163">[Set Up Workflow Users](across-how-to-set-up-workflow-users.md) </span></span>  
 <span data-ttu-id="bc76e-164">[Set Up Approval Users](across-how-to-set-up-approval-users.md) </span><span class="sxs-lookup"><span data-stu-id="bc76e-164">[Set Up Approval Users](across-how-to-set-up-approval-users.md) </span></span>  
 <span data-ttu-id="bc76e-165">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="bc76e-165">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="bc76e-166">[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md) </span><span class="sxs-lookup"><span data-stu-id="bc76e-166">[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md) </span></span>  
 [<span data-ttu-id="bc76e-167">Workflow</span><span class="sxs-lookup"><span data-stu-id="bc76e-167">Workflow</span></span>](across-workflow.md)   