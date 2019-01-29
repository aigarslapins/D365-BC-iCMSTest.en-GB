---
title: Multiple Interest Rates Overview | Microsoft Docs
description: For each finance charge term code, you can specify multiple interest rates so that you can calculate finance charges with multiple interest rates for a specific period.
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
ms.openlocfilehash: 3d5bc80c8c5af365d111513965090d5c4a32124d
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "267676"
---
# <a name="multiple-interest-rates-overview"></a><span data-ttu-id="1309a-103">Multiple Interest Rates Overview</span><span class="sxs-lookup"><span data-stu-id="1309a-103">Multiple Interest Rates Overview</span></span>
<span data-ttu-id="1309a-104">For each finance charge term code, you can specify multiple interest rates so that you can calculate finance charges with multiple interest rates for a specific period.</span><span class="sxs-lookup"><span data-stu-id="1309a-104">For each finance charge term code, you can specify multiple interest rates so that you can calculate finance charges with multiple interest rates for a specific period.</span></span> <span data-ttu-id="1309a-105">This is helpful if you charge different interest on payments that are late.</span><span class="sxs-lookup"><span data-stu-id="1309a-105">This is helpful if you charge different interest on payments that are late.</span></span> <span data-ttu-id="1309a-106">The interest calculation is the same for each financial charge, with variation only in the rate of interest for a specific period.</span><span class="sxs-lookup"><span data-stu-id="1309a-106">The interest calculation is the same for each financial charge, with variation only in the rate of interest for a specific period.</span></span>  

## <a name="creating-finance-charges"></a><span data-ttu-id="1309a-107">Creating Finance Charges</span><span class="sxs-lookup"><span data-stu-id="1309a-107">Creating Finance Charges</span></span>  
 <span data-ttu-id="1309a-108">When you create a finance charge memo, the memo lines show the finance charges with different interest rates for each time period.</span><span class="sxs-lookup"><span data-stu-id="1309a-108">When you create a finance charge memo, the memo lines show the finance charges with different interest rates for each time period.</span></span> <span data-ttu-id="1309a-109">For finance charge terms, you can define descriptions for each term, and you can define a description that is used when multiple interest rates are used.</span><span class="sxs-lookup"><span data-stu-id="1309a-109">For finance charge terms, you can define descriptions for each term, and you can define a description that is used when multiple interest rates are used.</span></span>  

 <span data-ttu-id="1309a-110">To use multiple interest rates, you must first define a finance charge term, and you must then add multiple interest rate lines to the terms.</span><span class="sxs-lookup"><span data-stu-id="1309a-110">To use multiple interest rates, you must first define a finance charge term, and you must then add multiple interest rate lines to the terms.</span></span> <span data-ttu-id="1309a-111">For more information, see [Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md).</span><span class="sxs-lookup"><span data-stu-id="1309a-111">For more information, see [Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md).</span></span>  

 <span data-ttu-id="1309a-112">If no multiple interest rates exist, [!INCLUDE [d365fin](../../includes/d365fin_md.md)] will use the interest rate and period that is defined in the **Finance Charge Terms** window for the whole period of calculation.</span><span class="sxs-lookup"><span data-stu-id="1309a-112">If no multiple interest rates exist, [!INCLUDE [d365fin](../../includes/d365fin_md.md)] will use the interest rate and period that is defined in the **Finance Charge Terms** window for the whole period of calculation.</span></span>  

## <a name="delayed-payments"></a><span data-ttu-id="1309a-113">Delayed Payments</span><span class="sxs-lookup"><span data-stu-id="1309a-113">Delayed Payments</span></span>  
 <span data-ttu-id="1309a-114">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span><span class="sxs-lookup"><span data-stu-id="1309a-114">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span></span> <span data-ttu-id="1309a-115">For example, a government specifies the maximum interest to be levied for a consumer.</span><span class="sxs-lookup"><span data-stu-id="1309a-115">For example, a government specifies the maximum interest to be levied for a consumer.</span></span> <span data-ttu-id="1309a-116">This interest rate can be changed twice a year on 01 January and 01 July.</span><span class="sxs-lookup"><span data-stu-id="1309a-116">This interest rate can be changed twice a year on 01 January and 01 July.</span></span> <span data-ttu-id="1309a-117">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span><span class="sxs-lookup"><span data-stu-id="1309a-117">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span></span> <span data-ttu-id="1309a-118">The announced rate is usually four percent more than the normal bank interest.</span><span class="sxs-lookup"><span data-stu-id="1309a-118">The announced rate is usually four percent more than the normal bank interest.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1309a-119">See Also</span><span class="sxs-lookup"><span data-stu-id="1309a-119">See Also</span></span>  
[<span data-ttu-id="1309a-120">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="1309a-120">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  
 <span data-ttu-id="1309a-121">[Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md) </span><span class="sxs-lookup"><span data-stu-id="1309a-121">[Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md) </span></span>  
 [<span data-ttu-id="1309a-122">Collect Outstanding balances</span><span class="sxs-lookup"><span data-stu-id="1309a-122">Collect Outstanding balances</span></span>](../../receivables-collect-outstanding-balances.md)
