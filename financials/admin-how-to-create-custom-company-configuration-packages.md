---
title: How to Create Custom Company Configuration Packages | Microsoft Docs
description: As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers. You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 03/05/2018
ms.author: sgroespe
ms.openlocfilehash: f8469a96ee65ffee8766557d381690bb90f9b509
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "234454"
---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="93a73-104">Create Custom Company Configuration Packages</span><span class="sxs-lookup"><span data-stu-id="93a73-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="93a73-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span><span class="sxs-lookup"><span data-stu-id="93a73-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="93a73-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span><span class="sxs-lookup"><span data-stu-id="93a73-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="93a73-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span><span class="sxs-lookup"><span data-stu-id="93a73-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="93a73-108">That lets you apply and set up new areas in a company as you need them</span><span class="sxs-lookup"><span data-stu-id="93a73-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="93a73-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span><span class="sxs-lookup"><span data-stu-id="93a73-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="93a73-110">Fixed Asset Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="93a73-111">General Ledger Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="93a73-112">Inventory Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-112">Inventory Setup</span></span>  
-   <span data-ttu-id="93a73-113">Manufacturing Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="93a73-114">Purchases and Payables Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="93a73-115">Marketing Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-115">Marketing Setup</span></span>  
-   <span data-ttu-id="93a73-116">Service Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-116">Service Setup</span></span>  
-   <span data-ttu-id="93a73-117">Sales and Receivables Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="93a73-118">Warehouse Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="93a73-119">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-119">General Posting Setup</span></span>  
-   <span data-ttu-id="93a73-120">VAT Posting Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="93a73-121">Inventory Posting Setup</span><span class="sxs-lookup"><span data-stu-id="93a73-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="93a73-122">To see a complete list of setup tables, Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="93a73-122">To see a complete list of setup tables, Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="93a73-123">To create a custom company configuration package</span><span class="sxs-lookup"><span data-stu-id="93a73-123">To create a custom company configuration package</span></span>  
1. <span data-ttu-id="93a73-124">Create a new [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="93a73-124">Create a new [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="93a73-125">***NOT POSSIBLE Link to help for "Creating a New Tenant"***.</span><span class="sxs-lookup"><span data-stu-id="93a73-125">***NOT POSSIBLE Link to help for "Creating a New Tenant"***.</span></span>   
2. <span data-ttu-id="93a73-126">Create a new company for the industry or solution template.</span><span class="sxs-lookup"><span data-stu-id="93a73-126">Create a new company for the industry or solution template.</span></span> <span data-ttu-id="93a73-127">For more information, see [Create a New Company](admin-how-to-create-a-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="93a73-127">For more information, see [Create a New Company](admin-how-to-create-a-new-company.md).</span></span>  
3. <span data-ttu-id="93a73-128">Setup the new company in the way you need.</span><span class="sxs-lookup"><span data-stu-id="93a73-128">Setup the new company in the way you need.</span></span> <span data-ttu-id="93a73-129">Fill in all required setup tables.</span><span class="sxs-lookup"><span data-stu-id="93a73-129">Fill in all required setup tables.</span></span>  
4. <span data-ttu-id="93a73-130">Open the new company.</span><span class="sxs-lookup"><span data-stu-id="93a73-130">Open the new company.</span></span>
5. <span data-ttu-id="93a73-131">Open the **Configuration Worksheet** window.</span><span class="sxs-lookup"><span data-stu-id="93a73-131">Open the **Configuration Worksheet** window.</span></span>  
6. <span data-ttu-id="93a73-132">Add the tables that you want to transfer to another company to the worksheet.</span><span class="sxs-lookup"><span data-stu-id="93a73-132">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="93a73-133">Assign the worksheet lines to the package.</span><span class="sxs-lookup"><span data-stu-id="93a73-133">Assign the worksheet lines to the package.</span></span>  
7. <span data-ttu-id="93a73-134">Create a questionnaire for the most frequently used setup tables.</span><span class="sxs-lookup"><span data-stu-id="93a73-134">Create a questionnaire for the most frequently used setup tables.</span></span>  
8. <span data-ttu-id="93a73-135">Create configuration templates to make it easier to create master data, such as customers or items.</span><span class="sxs-lookup"><span data-stu-id="93a73-135">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9. <span data-ttu-id="93a73-136">Export your package as a .rapidstart file.</span><span class="sxs-lookup"><span data-stu-id="93a73-136">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="93a73-137">See Also</span><span class="sxs-lookup"><span data-stu-id="93a73-137">See Also</span></span>  
[<span data-ttu-id="93a73-138">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="93a73-138">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="93a73-139">Administration</span><span class="sxs-lookup"><span data-stu-id="93a73-139">Administration</span></span>](admin-setup-and-administration.md)