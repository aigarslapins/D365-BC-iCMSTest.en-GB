---
title: How to Set Up Multiple Interest Rates
description: You can calculate finance charges with multiple interest rates for a specific period. The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 12/21/2017
ms.author: sgroespe
ms.openlocfilehash: 2894fb7a8283f7cd6e7306f5552e00edbcc8db92
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "230144"
---
# <a name="set-up-multiple-interest-rates"></a><span data-ttu-id="a2f78-104">Set Up Multiple Interest Rates</span><span class="sxs-lookup"><span data-stu-id="a2f78-104">Set Up Multiple Interest Rates</span></span>
<span data-ttu-id="a2f78-105">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span><span class="sxs-lookup"><span data-stu-id="a2f78-105">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span></span> <span data-ttu-id="a2f78-106">For example, a government specifies the maximum interest to be levied for a consumer.</span><span class="sxs-lookup"><span data-stu-id="a2f78-106">For example, a government specifies the maximum interest to be levied for a consumer.</span></span> <span data-ttu-id="a2f78-107">This interest rate can be changed twice a year on 01 January and 01 July.</span><span class="sxs-lookup"><span data-stu-id="a2f78-107">This interest rate can be changed twice a year on 01 January and 01 July.</span></span> <span data-ttu-id="a2f78-108">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span><span class="sxs-lookup"><span data-stu-id="a2f78-108">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span></span> <span data-ttu-id="a2f78-109">The announced rate is usually four percent more than the normal bank interest.</span><span class="sxs-lookup"><span data-stu-id="a2f78-109">The announced rate is usually four percent more than the normal bank interest.</span></span>

<span data-ttu-id="a2f78-110">When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods.</span><span class="sxs-lookup"><span data-stu-id="a2f78-110">When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods.</span></span> <span data-ttu-id="a2f78-111">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="a2f78-111">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>

## <a name="to-set-up-multiple-interest-rates"></a><span data-ttu-id="a2f78-112">To set up multiple interest rates</span><span class="sxs-lookup"><span data-stu-id="a2f78-112">To set up multiple interest rates</span></span>  
1.  <span data-ttu-id="a2f78-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a2f78-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a2f78-114">In the **Finance Charge Terms** window, select the required finance term, and then choose the **Interest Rates** action.</span><span class="sxs-lookup"><span data-stu-id="a2f78-114">In the **Finance Charge Terms** window, select the required finance term, and then choose the **Interest Rates** action.</span></span>  
3.  <span data-ttu-id="a2f78-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a2f78-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  <span data-ttu-id="a2f78-116">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a2f78-116">Choose the **OK** button.</span></span>  
5.  <span data-ttu-id="a2f78-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Reminder Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a2f78-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Reminder Terms**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="a2f78-118">In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.</span><span class="sxs-lookup"><span data-stu-id="a2f78-118">In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.</span></span>  
7.  <span data-ttu-id="a2f78-119">In the **Reminder Levels** window, select the **Calculate Interest** field.</span><span class="sxs-lookup"><span data-stu-id="a2f78-119">In the **Reminder Levels** window, select the **Calculate Interest** field.</span></span>  

<span data-ttu-id="a2f78-120">When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period.</span><span class="sxs-lookup"><span data-stu-id="a2f78-120">When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period.</span></span> <span data-ttu-id="a2f78-121">The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount.</span><span class="sxs-lookup"><span data-stu-id="a2f78-121">The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount.</span></span> <span data-ttu-id="a2f78-122">The opening entry on the memo is displayed in bold.</span><span class="sxs-lookup"><span data-stu-id="a2f78-122">The opening entry on the memo is displayed in bold.</span></span> <span data-ttu-id="a2f78-123">The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.</span><span class="sxs-lookup"><span data-stu-id="a2f78-123">The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a2f78-124">See Also</span><span class="sxs-lookup"><span data-stu-id="a2f78-124">See Also</span></span>  
[<span data-ttu-id="a2f78-125">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="a2f78-125">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="a2f78-126">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="a2f78-126">Setting Up Finance</span></span>](finance-setup-finance.md)