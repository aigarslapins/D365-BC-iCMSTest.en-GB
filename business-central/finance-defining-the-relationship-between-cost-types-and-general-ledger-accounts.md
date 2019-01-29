---
title: Defining the Relationship Between Cost Types and General Ledger Accounts | Microsoft Docs
description: Learn how to define the relationship between the cost type and the general ledger account.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: f80e9b6276d26adffb5e3208ffefbf98d7f7ff96
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "237788"
---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a><span data-ttu-id="c43e2-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span><span class="sxs-lookup"><span data-stu-id="c43e2-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>
<span data-ttu-id="c43e2-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span><span class="sxs-lookup"><span data-stu-id="c43e2-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span></span>  

* <span data-ttu-id="c43e2-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span><span class="sxs-lookup"><span data-stu-id="c43e2-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span></span>  
* <span data-ttu-id="c43e2-106">The **Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="c43e2-106">The **Cost Type No.**</span></span> <span data-ttu-id="c43e2-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span><span class="sxs-lookup"><span data-stu-id="c43e2-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span></span>  

<span data-ttu-id="c43e2-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span><span class="sxs-lookup"><span data-stu-id="c43e2-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span></span>  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a><span data-ttu-id="c43e2-109">Relationship Between General Ledger Accounts and Cost Types</span><span class="sxs-lookup"><span data-stu-id="c43e2-109">Relationship Between General Ledger Accounts and Cost Types</span></span>  
<span data-ttu-id="c43e2-110">There is an n:1 relationship between general ledger accounts and cost types.</span><span class="sxs-lookup"><span data-stu-id="c43e2-110">There is an n:1 relationship between general ledger accounts and cost types.</span></span> <span data-ttu-id="c43e2-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span><span class="sxs-lookup"><span data-stu-id="c43e2-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span></span> <span data-ttu-id="c43e2-112">The following table describes the details in the relationship.</span><span class="sxs-lookup"><span data-stu-id="c43e2-112">The following table describes the details in the relationship.</span></span>  

|<span data-ttu-id="c43e2-113">Relationship</span><span class="sxs-lookup"><span data-stu-id="c43e2-113">Relationship</span></span>|<span data-ttu-id="c43e2-114">**G/L Account Range**</span><span class="sxs-lookup"><span data-stu-id="c43e2-114">**G/L Account Range**</span></span>|<span data-ttu-id="c43e2-115">**Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="c43e2-115">**Cost Type No.**</span></span>|  
|------------------|------------------------------------------------|-------------------------------------------|  
|<span data-ttu-id="c43e2-116">One general ledger account for each cost type</span><span class="sxs-lookup"><span data-stu-id="c43e2-116">One general ledger account for each cost type</span></span>|<span data-ttu-id="c43e2-117">One general ledger account</span><span class="sxs-lookup"><span data-stu-id="c43e2-117">One general ledger account</span></span>|<span data-ttu-id="c43e2-118">One cost type</span><span class="sxs-lookup"><span data-stu-id="c43e2-118">One cost type</span></span>|  
|<span data-ttu-id="c43e2-119">Several general ledger accounts for one cost type</span><span class="sxs-lookup"><span data-stu-id="c43e2-119">Several general ledger accounts for one cost type</span></span>|<span data-ttu-id="c43e2-120">General ledger account range, for example, 7110..7193 for each general ledger account</span><span class="sxs-lookup"><span data-stu-id="c43e2-120">General ledger account range, for example, 7110..7193 for each general ledger account</span></span>|<span data-ttu-id="c43e2-121">For each general ledger account in the range, there is only one cost type</span><span class="sxs-lookup"><span data-stu-id="c43e2-121">For each general ledger account in the range, there is only one cost type</span></span>|  
|<span data-ttu-id="c43e2-122">Cost types without corresponding general ledger accounts</span><span class="sxs-lookup"><span data-stu-id="c43e2-122">Cost types without corresponding general ledger accounts</span></span>|<Empty>||  
|<span data-ttu-id="c43e2-123">General ledger accounts whose entries will not be transferred</span><span class="sxs-lookup"><span data-stu-id="c43e2-123">General ledger accounts whose entries will not be transferred</span></span>||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a><span data-ttu-id="c43e2-124">Cost Types Without a Relationship to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="c43e2-124">Cost Types Without a Relationship to the General Ledger</span></span>  
<span data-ttu-id="c43e2-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span><span class="sxs-lookup"><span data-stu-id="c43e2-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span></span>  

* <span data-ttu-id="c43e2-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span><span class="sxs-lookup"><span data-stu-id="c43e2-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span></span>  
* <span data-ttu-id="c43e2-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span><span class="sxs-lookup"><span data-stu-id="c43e2-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span></span>  
* <span data-ttu-id="c43e2-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="c43e2-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c43e2-129">See Also</span><span class="sxs-lookup"><span data-stu-id="c43e2-129">See Also</span></span>  
[<span data-ttu-id="c43e2-130">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="c43e2-130">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="c43e2-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="c43e2-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
[<span data-ttu-id="c43e2-132">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="c43e2-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="c43e2-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c43e2-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
