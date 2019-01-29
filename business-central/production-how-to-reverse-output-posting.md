---
title: How to Reverse Output Posting | Microsoft Docs
description: There are times when output posting must be reversed. An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.
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
ms.openlocfilehash: fb107d6d165ede233799ab165d735c030c0c8bba
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "239823"
---
# <a name="reverse-output-posting"></a><span data-ttu-id="de9ad-104">Reverse Output Posting</span><span class="sxs-lookup"><span data-stu-id="de9ad-104">Reverse Output Posting</span></span>
<span data-ttu-id="de9ad-105">There are times when output posting must be reversed.</span><span class="sxs-lookup"><span data-stu-id="de9ad-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="de9ad-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span><span class="sxs-lookup"><span data-stu-id="de9ad-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="de9ad-107">To reverse an output posting</span><span class="sxs-lookup"><span data-stu-id="de9ad-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="de9ad-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="de9ad-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="de9ad-109">Select your batch.</span><span class="sxs-lookup"><span data-stu-id="de9ad-109">Select your batch.</span></span>  
2. <span data-ttu-id="de9ad-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="de9ad-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="de9ad-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="de9ad-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="de9ad-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span><span class="sxs-lookup"><span data-stu-id="de9ad-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="de9ad-113">This reverses the capacity and item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="de9ad-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="de9ad-114">Post the reversal by posting the journal.</span><span class="sxs-lookup"><span data-stu-id="de9ad-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="de9ad-115">The output journal entries are posted to the item ledger as a positive adjustment.</span><span class="sxs-lookup"><span data-stu-id="de9ad-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="de9ad-116">See Also</span><span class="sxs-lookup"><span data-stu-id="de9ad-116">See Also</span></span>  
 <span data-ttu-id="de9ad-117">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="de9ad-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="de9ad-118">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="de9ad-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="de9ad-119">[Planning](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="de9ad-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="de9ad-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="de9ad-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="de9ad-121">Purchasing</span><span class="sxs-lookup"><span data-stu-id="de9ad-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="de9ad-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="de9ad-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  