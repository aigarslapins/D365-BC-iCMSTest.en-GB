---
title: How to Block Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
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
ms.openlocfilehash: 0d5ad688cfa6fb58e8383692362105beeee386f8
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "243307"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="f48e5-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="f48e5-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="f48e5-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="f48e5-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="f48e5-105">The following table illustrates what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="f48e5-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="f48e5-106">Option</span><span class="sxs-lookup"><span data-stu-id="f48e5-106">Option</span></span>|<span data-ttu-id="f48e5-107">Description</span><span class="sxs-lookup"><span data-stu-id="f48e5-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="f48e5-108">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="f48e5-108">**Sales Blocked**</span></span>|<span data-ttu-id="f48e5-109">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="f48e5-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="f48e5-110">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="f48e5-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="f48e5-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="f48e5-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="f48e5-112">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="f48e5-112">**Blocked**</span></span>|<span data-ttu-id="f48e5-113">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="f48e5-113">You cannot use the item for any item transaction.</span></span> <span data-ttu-id="f48e5-114">For more information about blocking an item for all purposes, see Item Card.</span><span class="sxs-lookup"><span data-stu-id="f48e5-114">For more information about blocking an item for all purposes, see Item Card.</span></span>|  

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="f48e5-115">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="f48e5-115">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="f48e5-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f48e5-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f48e5-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="f48e5-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="f48e5-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="f48e5-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="f48e5-119">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="f48e5-119">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="f48e5-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f48e5-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f48e5-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="f48e5-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="f48e5-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="f48e5-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="f48e5-123">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="f48e5-123">To block an item from being posted</span></span>
1. <span data-ttu-id="f48e5-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f48e5-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="f48e5-125">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="f48e5-125">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="f48e5-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="f48e5-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="f48e5-127">See Also</span><span class="sxs-lookup"><span data-stu-id="f48e5-127">See Also</span></span>  
[<span data-ttu-id="f48e5-128">Register New Items</span><span class="sxs-lookup"><span data-stu-id="f48e5-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="f48e5-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="f48e5-129">Inventory</span></span>](inventory-manage-inventory.md)  