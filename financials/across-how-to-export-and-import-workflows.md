---
title: How to Export and Import Workflows | Microsoft Docs
description: To transfer workflows to other Business Central databases, for example to save time when creating new workflows, you can export and import workflows.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: c7e0244d8f095af48cb5eff0ef05fbd34776a013
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "274333"
---
# <a name="export-and-import-workflows"></a><span data-ttu-id="f5b61-103">Export and Import Workflows</span><span class="sxs-lookup"><span data-stu-id="f5b61-103">Export and Import Workflows</span></span>
<span data-ttu-id="f5b61-104">To transfer workflows to other [!INCLUDE [d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span><span class="sxs-lookup"><span data-stu-id="f5b61-104">To transfer workflows to other [!INCLUDE [d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="f5b61-105">Another way to quickly create workflows is to create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="f5b61-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="f5b61-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="f5b61-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="f5b61-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="f5b61-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="f5b61-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="f5b61-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="f5b61-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="f5b61-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="f5b61-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="f5b61-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="f5b61-111">To export a workflow</span><span class="sxs-lookup"><span data-stu-id="f5b61-111">To export a workflow</span></span>  
1.  <span data-ttu-id="f5b61-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f5b61-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f5b61-113">Select a workflow, and then choose the **Export to File** action.</span><span class="sxs-lookup"><span data-stu-id="f5b61-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="f5b61-114">In the **Export File** window, choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="f5b61-114">In the **Export File** window, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="f5b61-115">In the **Export** window, select a file location, and then choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="f5b61-115">In the **Export** window, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="f5b61-116">To import a workflow</span><span class="sxs-lookup"><span data-stu-id="f5b61-116">To import a workflow</span></span>  
1.  <span data-ttu-id="f5b61-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f5b61-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f5b61-118">Choose the **Import from File** action.</span><span class="sxs-lookup"><span data-stu-id="f5b61-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="f5b61-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="f5b61-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="f5b61-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span><span class="sxs-lookup"><span data-stu-id="f5b61-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f5b61-121">See Also</span><span class="sxs-lookup"><span data-stu-id="f5b61-121">See Also</span></span>  
 <span data-ttu-id="f5b61-122">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f5b61-122">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="f5b61-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="f5b61-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="f5b61-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="f5b61-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="f5b61-125">[Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f5b61-125">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="f5b61-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="f5b61-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="f5b61-127">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f5b61-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="f5b61-128">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f5b61-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="f5b61-129">Workflow</span><span class="sxs-lookup"><span data-stu-id="f5b61-129">Workflow</span></span>](across-workflow.md)   
