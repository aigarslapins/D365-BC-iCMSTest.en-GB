---
title: How to Restrict and Allow Usage of a Record | Microsoft Docs
description: If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 7cb9c035343ad9351304d5b6f277997f0f7cd603
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "265492"
---
# <a name="restrict-and-allow-usage-of-a-record"></a><span data-ttu-id="4551f-103">Restrict and Allow Usage of a Record</span><span class="sxs-lookup"><span data-stu-id="4551f-103">Restrict and Allow Usage of a Record</span></span>
<span data-ttu-id="4551f-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span><span class="sxs-lookup"><span data-stu-id="4551f-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span></span> <span data-ttu-id="4551f-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span><span class="sxs-lookup"><span data-stu-id="4551f-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="4551f-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span><span class="sxs-lookup"><span data-stu-id="4551f-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="4551f-107">Two responses exist in the generic version of [!INCLUDE [d365fin](includes/d365fin_md.md)] for this purpose: **Restrict usage of a record.**</span><span class="sxs-lookup"><span data-stu-id="4551f-107">Two responses exist in the generic version of [!INCLUDE [d365fin](includes/d365fin_md.md)] for this purpose: **Restrict usage of a record.**</span></span> <span data-ttu-id="4551f-108">and **Allow usage of a record.**.</span><span class="sxs-lookup"><span data-stu-id="4551f-108">and **Allow usage of a record.**.</span></span>

> [!NOTE]
>  <span data-ttu-id="4551f-109">The generic version of [!INCLUDE [d365fin](includes/d365fin_md.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a check.</span><span class="sxs-lookup"><span data-stu-id="4551f-109">The generic version of [!INCLUDE [d365fin](includes/d365fin_md.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a check.</span></span> <span data-ttu-id="4551f-110">To support other restrictions, a Microsoft partner must customise the application code.</span><span class="sxs-lookup"><span data-stu-id="4551f-110">To support other restrictions, a Microsoft partner must customize the application code.</span></span>  
> 
> [!NOTE]
>  <span data-ttu-id="4551f-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span><span class="sxs-lookup"><span data-stu-id="4551f-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span></span>

<span data-ttu-id="4551f-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span><span class="sxs-lookup"><span data-stu-id="4551f-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span></span> <span data-ttu-id="4551f-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span><span class="sxs-lookup"><span data-stu-id="4551f-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span></span>  

## <a name="to-create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a><span data-ttu-id="4551f-114">To create a workflow step that restricts posting of unapproved purchase orders</span><span class="sxs-lookup"><span data-stu-id="4551f-114">To create a workflow step that restricts posting of unapproved purchase orders</span></span>  
1. <span data-ttu-id="4551f-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4551f-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2. <span data-ttu-id="4551f-116">In the **Workflows** window, create a new workflow named Purchase Order Approval Workflow.</span><span class="sxs-lookup"><span data-stu-id="4551f-116">In the **Workflows** window, create a new workflow named Purchase Order Approval Workflow.</span></span> <span data-ttu-id="4551f-117">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="4551f-117">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  
3. <span data-ttu-id="4551f-118">Choose the **Copy From Workflow Template** action.</span><span class="sxs-lookup"><span data-stu-id="4551f-118">Choose the **Copy From Workflow Template** action.</span></span>  
4. <span data-ttu-id="4551f-119">Choose the **Source Workflow Code** field, and then, in the **Workflow Templates** window, choose the Purchase Invoice Approval Workflow workflow template.</span><span class="sxs-lookup"><span data-stu-id="4551f-119">Choose the **Source Workflow Code** field, and then, in the **Workflow Templates** window, choose the Purchase Invoice Approval Workflow workflow template.</span></span>  

     <span data-ttu-id="4551f-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="4551f-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span></span> <span data-ttu-id="4551f-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span><span class="sxs-lookup"><span data-stu-id="4551f-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span></span>  
5. <span data-ttu-id="4551f-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span><span class="sxs-lookup"><span data-stu-id="4551f-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span></span>  
6. <span data-ttu-id="4551f-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span><span class="sxs-lookup"><span data-stu-id="4551f-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4551f-124">See Also</span><span class="sxs-lookup"><span data-stu-id="4551f-124">See Also</span></span>  
<span data-ttu-id="4551f-125">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="4551f-125">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
[<span data-ttu-id="4551f-126">Workflow</span><span class="sxs-lookup"><span data-stu-id="4551f-126">Workflow</span></span>](across-workflow.md)   