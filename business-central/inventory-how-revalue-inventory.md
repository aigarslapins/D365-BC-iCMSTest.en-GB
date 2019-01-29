---
title: Create New Value Entries for Items in the Inventory| Microsoft Docs
description: Describes how to appreciate or depreciate the value entries of one or more items in the inventory by posting their current, calculated value.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing, inventory cost, value entries
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 7dd38fc58ed7bd2aafafa09042a9e23c821c76e4
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "252616"
---
# <a name="revalue-inventory"></a><span data-ttu-id="9a0d3-103">Revalue Inventory</span><span class="sxs-lookup"><span data-stu-id="9a0d3-103">Revalue Inventory</span></span>
<span data-ttu-id="9a0d3-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="9a0d3-105">To revalue inventory</span><span class="sxs-lookup"><span data-stu-id="9a0d3-105">To revalue inventory</span></span>
1. <span data-ttu-id="9a0d3-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Revaluation Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="9a0d3-107">Choose the **Calculate Inventory Value** action.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="9a0d3-108">On the **Calculate Inventory Value** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-108">On the **Calculate Inventory Value** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="9a0d3-109">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="9a0d3-110">On each line on the **Revaluation Journal** page, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-110">On each line on the **Revaluation Journal** page, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="9a0d3-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="9a0d3-112">The relevant fields are automatically updated.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="9a0d3-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="9a0d3-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="9a0d3-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="9a0d3-116">New value entries are now created to reflect the revaluations that you have posted.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="9a0d3-117">You can see the new values on the respective item cards.</span><span class="sxs-lookup"><span data-stu-id="9a0d3-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="9a0d3-118">See Also</span><span class="sxs-lookup"><span data-stu-id="9a0d3-118">See Also</span></span>
[<span data-ttu-id="9a0d3-119">Design Details: Revaluation</span><span class="sxs-lookup"><span data-stu-id="9a0d3-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="9a0d3-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="9a0d3-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="9a0d3-121">Sales</span><span class="sxs-lookup"><span data-stu-id="9a0d3-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="9a0d3-122">Purchasing</span><span class="sxs-lookup"><span data-stu-id="9a0d3-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="9a0d3-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9a0d3-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>