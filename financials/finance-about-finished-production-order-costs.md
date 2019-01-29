---
title: About Finished Production Order Costs | Microsoft Docs
description: Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced. Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/06/2017
ms.author: sgroespe
ms.openlocfilehash: a3745206a486d68757bd9aecdf567c4da9d796e3
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "264203"
---
# <a name="about-finished-production-order-costs"></a><span data-ttu-id="5ad5d-104">About Finished Production Order Costs</span><span class="sxs-lookup"><span data-stu-id="5ad5d-104">About Finished Production Order Costs</span></span>
<span data-ttu-id="5ad5d-105">Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-105">Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced.</span></span> <span data-ttu-id="5ad5d-106">Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-106">Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production.</span></span> <span data-ttu-id="5ad5d-107">For a production order to be considered for cost adjustment, the status must be **Finished**.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-107">For a production order to be considered for cost adjustment, the status must be **Finished**.</span></span> <span data-ttu-id="5ad5d-108">It is therefore critical that upon completion, the status of a production order is changed to **Finished**.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-108">It is therefore critical that upon completion, the status of a production order is changed to **Finished**.</span></span>  

## <a name="example"></a><span data-ttu-id="5ad5d-109">Example</span><span class="sxs-lookup"><span data-stu-id="5ad5d-109">Example</span></span>  
 <span data-ttu-id="5ad5d-110">In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labour and overhead go into WIP.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-110">In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labor and overhead go into WIP.</span></span> <span data-ttu-id="5ad5d-111">When the item is produced, WIP is reduced by the amount of the standard cost of the item.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-111">When the item is produced, WIP is reduced by the amount of the standard cost of the item.</span></span> <span data-ttu-id="5ad5d-112">Typically, these costs do not net to zero.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-112">Typically, these costs do not net to zero.</span></span> <span data-ttu-id="5ad5d-113">So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.</span><span class="sxs-lookup"><span data-stu-id="5ad5d-113">So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5ad5d-114">See Also</span><span class="sxs-lookup"><span data-stu-id="5ad5d-114">See Also</span></span>  
[<span data-ttu-id="5ad5d-115">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="5ad5d-115">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="5ad5d-116">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="5ad5d-116">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="5ad5d-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5ad5d-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>