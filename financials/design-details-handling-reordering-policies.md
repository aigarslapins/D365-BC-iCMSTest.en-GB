---
title: Design Details - Handling Reordering Policies | Microsoft Docs
description: Overview of tasks for defining a reorder policy in supply planning.
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
ms.openlocfilehash: 07af8e1cbcbeb23617ac829afca4e0b7934d1cf5
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "284454"
---
# <a name="design-details-handling-reordering-policies"></a><span data-ttu-id="ad985-103">Design Details: Handling Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="ad985-103">Design Details: Handling Reordering Policies</span></span>
<span data-ttu-id="ad985-104">For an item to participate in supply planning, a reorder policy must be defined.</span><span class="sxs-lookup"><span data-stu-id="ad985-104">For an item to participate in supply planning, a reorder policy must be defined.</span></span> <span data-ttu-id="ad985-105">The following four reordering policies exist:</span><span class="sxs-lookup"><span data-stu-id="ad985-105">The following four reordering policies exist:</span></span>  
  
* <span data-ttu-id="ad985-106">Fixed Reorder Qty.</span><span class="sxs-lookup"><span data-stu-id="ad985-106">Fixed Reorder Qty.</span></span>  
* <span data-ttu-id="ad985-107">Maximum Qty.</span><span class="sxs-lookup"><span data-stu-id="ad985-107">Maximum Qty.</span></span>  
* <span data-ttu-id="ad985-108">Order</span><span class="sxs-lookup"><span data-stu-id="ad985-108">Order</span></span>  
* <span data-ttu-id="ad985-109">Lot-for-Lot</span><span class="sxs-lookup"><span data-stu-id="ad985-109">Lot-for-Lot</span></span>  
  
<span data-ttu-id="ad985-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span><span class="sxs-lookup"><span data-stu-id="ad985-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span></span> <span data-ttu-id="ad985-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span><span class="sxs-lookup"><span data-stu-id="ad985-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span></span> <span data-ttu-id="ad985-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span><span class="sxs-lookup"><span data-stu-id="ad985-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span></span>  
  
## <a name="in-this-section"></a><span data-ttu-id="ad985-113">In This Section</span><span class="sxs-lookup"><span data-stu-id="ad985-113">In This Section</span></span>  
[<span data-ttu-id="ad985-114">Design Details: The Role of the Reorder Point</span><span class="sxs-lookup"><span data-stu-id="ad985-114">Design Details: The Role of the Reorder Point</span></span>](design-details-the-role-of-the-reorder-point.md)  
[<span data-ttu-id="ad985-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span><span class="sxs-lookup"><span data-stu-id="ad985-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[<span data-ttu-id="ad985-116">Design Details: The Role of the Time Bucket</span><span class="sxs-lookup"><span data-stu-id="ad985-116">Design Details: The Role of the Time Bucket</span></span>](design-details-the-role-of-the-time-bucket.md)  
[<span data-ttu-id="ad985-117">Design Details: Staying under the Overflow Level</span><span class="sxs-lookup"><span data-stu-id="ad985-117">Design Details: Staying under the Overflow Level</span></span>](design-details-staying-under-the-overflow-level.md)  
[<span data-ttu-id="ad985-118">Design Details: Handling Projected Negative Inventory</span><span class="sxs-lookup"><span data-stu-id="ad985-118">Design Details: Handling Projected Negative Inventory</span></span>](design-details-handling-projected-negative-inventory.md)  
[<span data-ttu-id="ad985-119">Design Details: Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="ad985-119">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)  
  
## <a name="see-also"></a><span data-ttu-id="ad985-120">See Also</span><span class="sxs-lookup"><span data-stu-id="ad985-120">See Also</span></span>  
<span data-ttu-id="ad985-121">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="ad985-121">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="ad985-122">[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md) </span><span class="sxs-lookup"><span data-stu-id="ad985-122">[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md) </span></span>  
<span data-ttu-id="ad985-123">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="ad985-123">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
<span data-ttu-id="ad985-124">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="ad985-124">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
[<span data-ttu-id="ad985-125">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="ad985-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)