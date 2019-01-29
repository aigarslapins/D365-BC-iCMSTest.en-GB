---
title: Design Details - Warehouse Management | Microsoft Docs
description: This topic provides an overview of the design, concepts, and principles behind the Warehouse Management features in Business Central.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/23/2017
ms.author: sgroespe
ms.openlocfilehash: d7018c5ed13d1826ff655b2ca935b45dc0d387ff
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "265250"
---
# <a name="design-details-warehouse-management"></a><span data-ttu-id="3ca33-103">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="3ca33-103">Design Details: Warehouse Management</span></span>
<span data-ttu-id="3ca33-104">This documentation gives an overview of the concepts and principles that are used in the Warehouse Management features in [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3ca33-104">This documentation gives an overview of the concepts and principles that are used in the Warehouse Management features in [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="3ca33-105">It explains the design behind central warehouse features and how warehousing integrates with other supply chain features.</span><span class="sxs-lookup"><span data-stu-id="3ca33-105">It explains the design behind central warehouse features and how warehousing integrates with other supply chain features.</span></span>  

<span data-ttu-id="3ca33-106">To differentiate the different complexity levels of the warehousing, this documentation is divided into two general groups, Basic and Advanced warehouse configurations, indicated by section titles.</span><span class="sxs-lookup"><span data-stu-id="3ca33-106">To differentiate the different complexity levels of the warehousing, this documentation is divided into two general groups, Basic and Advanced warehouse configurations, indicated by section titles.</span></span> <span data-ttu-id="3ca33-107">This simple differentiation covers different complexity levels as defined by product granules and location setup.</span><span class="sxs-lookup"><span data-stu-id="3ca33-107">This simple differentiation covers different complexity levels as defined by product granules and location setup.</span></span> <span data-ttu-id="3ca33-108">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="3ca33-108">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="3ca33-109">In This Section</span><span class="sxs-lookup"><span data-stu-id="3ca33-109">In This Section</span></span>  
[<span data-ttu-id="3ca33-110">Design Details: Warehouse Overview</span><span class="sxs-lookup"><span data-stu-id="3ca33-110">Design Details: Warehouse Overview</span></span>](design-details-warehouse-overview.md)  
[<span data-ttu-id="3ca33-111">Design Details: Warehouse Setup</span><span class="sxs-lookup"><span data-stu-id="3ca33-111">Design Details: Warehouse Setup</span></span>](design-details-warehouse-setup.md)  
[<span data-ttu-id="3ca33-112">Design Details: Inbound Warehouse Flow</span><span class="sxs-lookup"><span data-stu-id="3ca33-112">Design Details: Inbound Warehouse Flow</span></span>](design-details-inbound-warehouse-flow.md)  
[<span data-ttu-id="3ca33-113">Design Details: Internal Warehouse Flows</span><span class="sxs-lookup"><span data-stu-id="3ca33-113">Design Details: Internal Warehouse Flows</span></span>](design-details-internal-warehouse-flows.md)  
[<span data-ttu-id="3ca33-114">Design Details: Availability in the Warehouse</span><span class="sxs-lookup"><span data-stu-id="3ca33-114">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="3ca33-115">Design Details: Outbound Warehouse Flow</span><span class="sxs-lookup"><span data-stu-id="3ca33-115">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="3ca33-116">Design Details: Integration with Inventory</span><span class="sxs-lookup"><span data-stu-id="3ca33-116">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)