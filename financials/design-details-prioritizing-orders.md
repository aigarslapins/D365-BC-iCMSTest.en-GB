---
title: Design Details - Prioritising Orders | Microsoft Docs
description: Read about how to prioritise to meet both demand and supply requirements.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 05c088a2acf38b1965e2dbd570de5431dc0304da
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "230519"
---
# <a name="design-details-prioritizing-orders"></a><span data-ttu-id="0b07a-103">Design Details: Prioritising Orders</span><span class="sxs-lookup"><span data-stu-id="0b07a-103">Design Details: Prioritizing Orders</span></span>
<span data-ttu-id="0b07a-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span><span class="sxs-lookup"><span data-stu-id="0b07a-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span></span> <span data-ttu-id="0b07a-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span><span class="sxs-lookup"><span data-stu-id="0b07a-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span></span> <span data-ttu-id="0b07a-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span><span class="sxs-lookup"><span data-stu-id="0b07a-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span></span> <span data-ttu-id="0b07a-107">This is done according to order priorities.</span><span class="sxs-lookup"><span data-stu-id="0b07a-107">This is done according to order priorities.</span></span>  
  
<span data-ttu-id="0b07a-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span><span class="sxs-lookup"><span data-stu-id="0b07a-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span></span>  
  
## <a name="priorities-on-the-demand-side"></a><span data-ttu-id="0b07a-109">Priorities on the Demand Side</span><span class="sxs-lookup"><span data-stu-id="0b07a-109">Priorities on the Demand Side</span></span>  
1. <span data-ttu-id="0b07a-110">Already shipped: Item Ledger Entry</span><span class="sxs-lookup"><span data-stu-id="0b07a-110">Already shipped: Item Ledger Entry</span></span>  
2. <span data-ttu-id="0b07a-111">Purchase Return Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-111">Purchase Return Order</span></span>  
3. <span data-ttu-id="0b07a-112">Sales Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-112">Sales Order</span></span>  
4. <span data-ttu-id="0b07a-113">Service Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-113">Service Order</span></span>  
5. <span data-ttu-id="0b07a-114">Production Component Need</span><span class="sxs-lookup"><span data-stu-id="0b07a-114">Production Component Need</span></span>  
6. <span data-ttu-id="0b07a-115">Assembly Order Line</span><span class="sxs-lookup"><span data-stu-id="0b07a-115">Assembly Order Line</span></span>  
7. <span data-ttu-id="0b07a-116">Outbound Transfer Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-116">Outbound Transfer Order</span></span>  
8. <span data-ttu-id="0b07a-117">Blanket Order (that has not already been consumed by related sales orders)</span><span class="sxs-lookup"><span data-stu-id="0b07a-117">Blanket Order (that has not already been consumed by related sales orders)</span></span>  
9. <span data-ttu-id="0b07a-118">Forecast (that has not already been consumed by other sales orders)</span><span class="sxs-lookup"><span data-stu-id="0b07a-118">Forecast (that has not already been consumed by other sales orders)</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="0b07a-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span><span class="sxs-lookup"><span data-stu-id="0b07a-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span></span> <span data-ttu-id="0b07a-120">If not reserved, purchase returns play a role in the availability and are highly prioritised to avoid that the planning system suggests a supply order just to serve a purchase return.</span><span class="sxs-lookup"><span data-stu-id="0b07a-120">If not reserved, purchase returns play a role in the availability and are highly prioritized to avoid that the planning system suggests a supply order just to serve a purchase return.</span></span>  
  
## <a name="priorities-on-the-supply-side"></a><span data-ttu-id="0b07a-121">Priorities on the Supply Side</span><span class="sxs-lookup"><span data-stu-id="0b07a-121">Priorities on the Supply Side</span></span>  
1. <span data-ttu-id="0b07a-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="0b07a-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="0b07a-123">Sales Return Order (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="0b07a-123">Sales Return Order (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="0b07a-124">Inbound Transfer Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-124">Inbound Transfer Order</span></span>  
4. <span data-ttu-id="0b07a-125">Production Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-125">Production Order</span></span>  
5. <span data-ttu-id="0b07a-126">Assembly Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-126">Assembly Order</span></span>  
6. <span data-ttu-id="0b07a-127">Purchase Order</span><span class="sxs-lookup"><span data-stu-id="0b07a-127">Purchase Order</span></span>  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a><span data-ttu-id="0b07a-128">Priority Related to the State of Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="0b07a-128">Priority Related to the State of Demand and Supply</span></span>  
<span data-ttu-id="0b07a-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span><span class="sxs-lookup"><span data-stu-id="0b07a-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span></span> <span data-ttu-id="0b07a-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span><span class="sxs-lookup"><span data-stu-id="0b07a-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span></span>  
  
1. <span data-ttu-id="0b07a-131">Partly handled (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="0b07a-131">Partly handled (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="0b07a-132">Already in process in the warehouse (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="0b07a-132">Already in process in the warehouse (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="0b07a-133">Released – all order types (Planning Flexibility = Unlimited)</span><span class="sxs-lookup"><span data-stu-id="0b07a-133">Released – all order types (Planning Flexibility = Unlimited)</span></span>  
4. <span data-ttu-id="0b07a-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span><span class="sxs-lookup"><span data-stu-id="0b07a-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span></span>  
5. <span data-ttu-id="0b07a-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span><span class="sxs-lookup"><span data-stu-id="0b07a-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="0b07a-136">See Also</span><span class="sxs-lookup"><span data-stu-id="0b07a-136">See Also</span></span>  
<span data-ttu-id="0b07a-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="0b07a-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="0b07a-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="0b07a-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="0b07a-139">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="0b07a-139">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)