---
title: Creating G/L Budgets| Microsoft Docs
description: Describes hos to create G/L budgets to forecast different financial activities and assign dimensions for business intelligence purposes.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: postpone
ms.date: 01/25/2018
ms.author: sgroespe
ms.openlocfilehash: 6bf167ebc1dfbf21d4af681257cf671d5837bd32
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "257161"
---
# <a name="create-gl-budgets"></a><span data-ttu-id="69750-103">Create G/L Budgets</span><span class="sxs-lookup"><span data-stu-id="69750-103">Create G/L Budgets</span></span>
<span data-ttu-id="69750-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span><span class="sxs-lookup"><span data-stu-id="69750-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span></span> <span data-ttu-id="69750-105">First, you set up the budget name and enter the budget figures.</span><span class="sxs-lookup"><span data-stu-id="69750-105">First, you set up the budget name and enter the budget figures.</span></span> <span data-ttu-id="69750-106">The budget name is then included on all the budget entries you create.</span><span class="sxs-lookup"><span data-stu-id="69750-106">The budget name is then included on all the budget entries you create.</span></span>  

 <span data-ttu-id="69750-107">When you create a budget, you can define four dimensions for each budget.</span><span class="sxs-lookup"><span data-stu-id="69750-107">When you create a budget, you can define four dimensions for each budget.</span></span> <span data-ttu-id="69750-108">These budget-specific dimensions are called budget dimensions.</span><span class="sxs-lookup"><span data-stu-id="69750-108">These budget-specific dimensions are called budget dimensions.</span></span> <span data-ttu-id="69750-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span><span class="sxs-lookup"><span data-stu-id="69750-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span></span> <span data-ttu-id="69750-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span><span class="sxs-lookup"><span data-stu-id="69750-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span></span> <span data-ttu-id="69750-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="69750-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span></span>

 <span data-ttu-id="69750-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analysing budgeted versus actual amounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="69750-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="69750-113">For more information, see [Business Intelligence](bi.md).</span><span class="sxs-lookup"><span data-stu-id="69750-113">For more information, see [Business Intelligence](bi.md).</span></span>

 <span data-ttu-id="69750-114">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analysing budgeted versus actual amounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="69750-114">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="69750-115">For more information, see [Business Intelligence](bi.md).</span><span class="sxs-lookup"><span data-stu-id="69750-115">For more information, see [Business Intelligence](bi.md).</span></span>

<span data-ttu-id="69750-116">In cost accounting, you work with cost budgets in a similar way.</span><span class="sxs-lookup"><span data-stu-id="69750-116">In cost accounting, you work with cost budgets in a similar way.</span></span> <span data-ttu-id="69750-117">For more information, see [Creating Cost Budgets](finance-create-cost-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="69750-117">For more information, see [Creating Cost Budgets](finance-create-cost-budgets.md).</span></span>    

## <a name="to-create-a-new-gl-budget"></a><span data-ttu-id="69750-118">To create a new G/L budget</span><span class="sxs-lookup"><span data-stu-id="69750-118">To create a new G/L budget</span></span>  
1. <span data-ttu-id="69750-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="69750-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="69750-120">Choose the **Edit List** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="69750-120">Choose the **Edit List** action, and then fill in the fields as necessary.</span></span> [!INCLUDE [tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="69750-121">Choose the **Edit Budget** action.</span><span class="sxs-lookup"><span data-stu-id="69750-121">Choose the **Edit Budget** action.</span></span>
4. <span data-ttu-id="69750-122">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span><span class="sxs-lookup"><span data-stu-id="69750-122">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span></span>  

    <span data-ttu-id="69750-123">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span><span class="sxs-lookup"><span data-stu-id="69750-123">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span></span> <span data-ttu-id="69750-124">Because the budget name has just been created, there are no entries that match the filter.</span><span class="sxs-lookup"><span data-stu-id="69750-124">Because the budget name has just been created, there are no entries that match the filter.</span></span> <span data-ttu-id="69750-125">Therefore, the window is empty.</span><span class="sxs-lookup"><span data-stu-id="69750-125">Therefore, the window is empty.</span></span>  
5. <span data-ttu-id="69750-126">To enter an amount, choose the relevant cell in the matrix.</span><span class="sxs-lookup"><span data-stu-id="69750-126">To enter an amount, choose the relevant cell in the matrix.</span></span> <span data-ttu-id="69750-127">The **G/L Budget Entries** window opens.</span><span class="sxs-lookup"><span data-stu-id="69750-127">The **G/L Budget Entries** window opens.</span></span>  
6. <span data-ttu-id="69750-128">Create a new line and fill in the **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="69750-128">Create a new line and fill in the **Amount** field.</span></span> <span data-ttu-id="69750-129">Close the **G/L Budget Entries** window.</span><span class="sxs-lookup"><span data-stu-id="69750-129">Close the **G/L Budget Entries** window.</span></span>  
7. <span data-ttu-id="69750-130">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span><span class="sxs-lookup"><span data-stu-id="69750-130">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="69750-131">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span><span class="sxs-lookup"><span data-stu-id="69750-131">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span></span>   

## <a name="see-also"></a><span data-ttu-id="69750-132">See Also</span><span class="sxs-lookup"><span data-stu-id="69750-132">See Also</span></span>
[<span data-ttu-id="69750-133">Finance</span><span class="sxs-lookup"><span data-stu-id="69750-133">Finance</span></span>](finance.md)  
[<span data-ttu-id="69750-134">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="69750-134">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="69750-135">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="69750-135">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="69750-136">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="69750-136">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="69750-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="69750-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  