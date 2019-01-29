---
title: Design Details | Microsoft Docs
description: This content contains detailed technical information about complex application features in Business Central.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 3157fc6d93f4152447d7fe25139c2c45f13395fe
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "266935"
---
# <a name="design-details"></a><span data-ttu-id="72cfd-103">Design Details</span><span class="sxs-lookup"><span data-stu-id="72cfd-103">Design Details</span></span>
<span data-ttu-id="72cfd-104">This content contains detailed technical information about complex application features in [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="72cfd-104">This content contains detailed technical information about complex application features in [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span>  

 <span data-ttu-id="72cfd-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customise, or set up the features in question.</span><span class="sxs-lookup"><span data-stu-id="72cfd-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customize, or set up the features in question.</span></span>  

|<span data-ttu-id="72cfd-106">**To**</span><span class="sxs-lookup"><span data-stu-id="72cfd-106">**To**</span></span>|<span data-ttu-id="72cfd-107">**See**</span><span class="sxs-lookup"><span data-stu-id="72cfd-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="72cfd-108">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span><span class="sxs-lookup"><span data-stu-id="72cfd-108">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span></span>|[<span data-ttu-id="72cfd-109">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="72cfd-109">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)|  
|<span data-ttu-id="72cfd-110">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span><span class="sxs-lookup"><span data-stu-id="72cfd-110">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span>|[<span data-ttu-id="72cfd-111">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="72cfd-111">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)|  
|<span data-ttu-id="72cfd-112">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span><span class="sxs-lookup"><span data-stu-id="72cfd-112">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span></span>|[<span data-ttu-id="72cfd-113">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="72cfd-113">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  
|<span data-ttu-id="72cfd-114">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span><span class="sxs-lookup"><span data-stu-id="72cfd-114">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span></span>|[<span data-ttu-id="72cfd-115">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="72cfd-115">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)|  
|<span data-ttu-id="72cfd-116">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span><span class="sxs-lookup"><span data-stu-id="72cfd-116">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span></span>|[<span data-ttu-id="72cfd-117">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="72cfd-117">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)|  
|<span data-ttu-id="72cfd-118">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span><span class="sxs-lookup"><span data-stu-id="72cfd-118">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span></span>|[<span data-ttu-id="72cfd-119">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="72cfd-119">Design Details: General Journal Post Line</span></span>](design-details-general-journal-post-line.md)|  

## <a name="see-also"></a><span data-ttu-id="72cfd-120">See Also</span><span class="sxs-lookup"><span data-stu-id="72cfd-120">See Also</span></span>  
 <span data-ttu-id="72cfd-121">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="72cfd-121">[Planning](production-planning.md) </span></span>  
 <span data-ttu-id="72cfd-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="72cfd-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 <span data-ttu-id="72cfd-123">[Warehouse Management](warehouse-manage-warehouse.md) </span><span class="sxs-lookup"><span data-stu-id="72cfd-123">[Warehouse Management](warehouse-manage-warehouse.md) </span></span>  
 [<span data-ttu-id="72cfd-124">Setting Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="72cfd-124">Setting Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="72cfd-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="72cfd-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

 ## [!INCLUDE [d365fin](includes/free_trial_md.md)]  
 ## [!INCLUDE [d365fin](includes/training_link_md.md)]
