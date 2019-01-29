---
title: Using the C5 Data Migration Extension | Microsoft Docs
description: Use this extension to migrate customers, vendors, items, and general ledger accounts from Microsoft Dynamics C5 2012 to Financials.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 11/21/2017
ms.author: bholtorf
ms.openlocfilehash: 81cb080deff18f88a1e563ce080b258aaee2173e
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "260202"
---
# <a name="the-c5-data-migration-extension-for-business-central"></a><span data-ttu-id="2864b-103">The C5 Data Migration Extension for Business Central</span><span class="sxs-lookup"><span data-stu-id="2864b-103">The C5 Data Migration Extension for Business Central</span></span>
<span data-ttu-id="2864b-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2864b-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="2864b-105">You can also migrate historical entries for general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="2864b-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="2864b-106">The company in [!INCLUDE [d365fin](includes/d365fin_md.md)] must not contain any data.</span><span class="sxs-lookup"><span data-stu-id="2864b-106">The company in [!INCLUDE [d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="2864b-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span><span class="sxs-lookup"><span data-stu-id="2864b-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="what-data-is-migrated"></a><span data-ttu-id="2864b-108">What Data is Migrated?</span><span class="sxs-lookup"><span data-stu-id="2864b-108">What Data is Migrated?</span></span>
<span data-ttu-id="2864b-109">The following data is migrated for each entity:</span><span class="sxs-lookup"><span data-stu-id="2864b-109">The following data is migrated for each entity:</span></span>

<span data-ttu-id="2864b-110">**Customers**</span><span class="sxs-lookup"><span data-stu-id="2864b-110">**Customers**</span></span>
* <span data-ttu-id="2864b-111">Location</span><span class="sxs-lookup"><span data-stu-id="2864b-111">Location</span></span>
* <span data-ttu-id="2864b-112">Country</span><span class="sxs-lookup"><span data-stu-id="2864b-112">Country</span></span>
* <span data-ttu-id="2864b-113">Customer dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="2864b-113">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="2864b-114">Shipment method</span><span class="sxs-lookup"><span data-stu-id="2864b-114">Shipment method</span></span>
* <span data-ttu-id="2864b-115">Sales Person</span><span class="sxs-lookup"><span data-stu-id="2864b-115">Sales Person</span></span>
* <span data-ttu-id="2864b-116">Payment terms</span><span class="sxs-lookup"><span data-stu-id="2864b-116">Payment terms</span></span>
* <span data-ttu-id="2864b-117">Payment method</span><span class="sxs-lookup"><span data-stu-id="2864b-117">Payment method</span></span>
* <span data-ttu-id="2864b-118">Customer price group</span><span class="sxs-lookup"><span data-stu-id="2864b-118">Customer price group</span></span>
* <span data-ttu-id="2864b-119">Customer invoice discount</span><span class="sxs-lookup"><span data-stu-id="2864b-119">Customer invoice discount</span></span>

<span data-ttu-id="2864b-120">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="2864b-120">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="2864b-121">Customer posting setup</span><span class="sxs-lookup"><span data-stu-id="2864b-121">Customer posting setup</span></span>
* <span data-ttu-id="2864b-122">General journal batch</span><span class="sxs-lookup"><span data-stu-id="2864b-122">General journal batch</span></span>
* <span data-ttu-id="2864b-123">Open transactions (customer ledger entries)</span><span class="sxs-lookup"><span data-stu-id="2864b-123">Open transactions (customer ledger entries)</span></span>

<span data-ttu-id="2864b-124">**Vendors**</span><span class="sxs-lookup"><span data-stu-id="2864b-124">**Vendors**</span></span>
* <span data-ttu-id="2864b-125">Location</span><span class="sxs-lookup"><span data-stu-id="2864b-125">Location</span></span>
* <span data-ttu-id="2864b-126">Country</span><span class="sxs-lookup"><span data-stu-id="2864b-126">Country</span></span>
* <span data-ttu-id="2864b-127">Vendor dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="2864b-127">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="2864b-128">Invoice discount</span><span class="sxs-lookup"><span data-stu-id="2864b-128">Invoice discount</span></span>
* <span data-ttu-id="2864b-129">Shipment method</span><span class="sxs-lookup"><span data-stu-id="2864b-129">Shipment method</span></span>
* <span data-ttu-id="2864b-130">Purchaser</span><span class="sxs-lookup"><span data-stu-id="2864b-130">Purchaser</span></span>
* <span data-ttu-id="2864b-131">Payment terms</span><span class="sxs-lookup"><span data-stu-id="2864b-131">Payment terms</span></span>
* <span data-ttu-id="2864b-132">Payment method</span><span class="sxs-lookup"><span data-stu-id="2864b-132">Payment method</span></span>
* <span data-ttu-id="2864b-133">Vendor invoice discount</span><span class="sxs-lookup"><span data-stu-id="2864b-133">Vendor invoice discount</span></span>

<span data-ttu-id="2864b-134">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="2864b-134">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="2864b-135">Vendor posting setup</span><span class="sxs-lookup"><span data-stu-id="2864b-135">Vendor posting setup</span></span>
* <span data-ttu-id="2864b-136">General journal batch</span><span class="sxs-lookup"><span data-stu-id="2864b-136">General journal batch</span></span>
* <span data-ttu-id="2864b-137">Open transactions (vendor ledger entries)</span><span class="sxs-lookup"><span data-stu-id="2864b-137">Open transactions (vendor ledger entries)</span></span>

<span data-ttu-id="2864b-138">**Items**</span><span class="sxs-lookup"><span data-stu-id="2864b-138">**Items**</span></span>
* <span data-ttu-id="2864b-139">Location</span><span class="sxs-lookup"><span data-stu-id="2864b-139">Location</span></span>
* <span data-ttu-id="2864b-140">Country</span><span class="sxs-lookup"><span data-stu-id="2864b-140">Country</span></span>
* <span data-ttu-id="2864b-141">Item dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="2864b-141">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="2864b-142">Sales line discounts</span><span class="sxs-lookup"><span data-stu-id="2864b-142">Sales line discounts</span></span>
* <span data-ttu-id="2864b-143">Customer discount groups</span><span class="sxs-lookup"><span data-stu-id="2864b-143">Customer discount groups</span></span>
* <span data-ttu-id="2864b-144">Item discount groups</span><span class="sxs-lookup"><span data-stu-id="2864b-144">Item discount groups</span></span>
* <span data-ttu-id="2864b-145">Sales price</span><span class="sxs-lookup"><span data-stu-id="2864b-145">Sales price</span></span>
* <span data-ttu-id="2864b-146">Commodity Code</span><span class="sxs-lookup"><span data-stu-id="2864b-146">Tariff number</span></span>
* <span data-ttu-id="2864b-147">Units of measure</span><span class="sxs-lookup"><span data-stu-id="2864b-147">Units of measure</span></span>
* <span data-ttu-id="2864b-148">Item tracking code</span><span class="sxs-lookup"><span data-stu-id="2864b-148">Item tracking code</span></span>
* <span data-ttu-id="2864b-149">Customer price group</span><span class="sxs-lookup"><span data-stu-id="2864b-149">Customer price group</span></span>

<span data-ttu-id="2864b-150">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="2864b-150">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="2864b-151">Inventory posting setup</span><span class="sxs-lookup"><span data-stu-id="2864b-151">Inventory posting setup</span></span>
* <span data-ttu-id="2864b-152">General posting setup</span><span class="sxs-lookup"><span data-stu-id="2864b-152">General posting setup</span></span>
* <span data-ttu-id="2864b-153">Item journal batch</span><span class="sxs-lookup"><span data-stu-id="2864b-153">Item journal batch</span></span>
* <span data-ttu-id="2864b-154">Open transactions (item ledger entries)</span><span class="sxs-lookup"><span data-stu-id="2864b-154">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="2864b-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span><span class="sxs-lookup"><span data-stu-id="2864b-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="2864b-156">Other exchange rates are not migrated.</span><span class="sxs-lookup"><span data-stu-id="2864b-156">Other exchange rates are not migrated.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="2864b-157">To migrate data</span><span class="sxs-lookup"><span data-stu-id="2864b-157">To migrate data</span></span>
<span data-ttu-id="2864b-158">There are just a few steps to export data from C5, and import it in [!INCLUDE [d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="2864b-158">There are just a few steps to export data from C5, and import it in [!INCLUDE [d365fin](includes/d365fin_md.md)]:</span></span>  

1. <span data-ttu-id="2864b-159">In C5, use the **Export Database** feature to export the data.</span><span class="sxs-lookup"><span data-stu-id="2864b-159">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="2864b-160">Then send the export folder to a compressed (zipped) folder.</span><span class="sxs-lookup"><span data-stu-id="2864b-160">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="2864b-161">In [!INCLUDE [d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span><span class="sxs-lookup"><span data-stu-id="2864b-161">In [!INCLUDE [d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="2864b-162">Complete the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="2864b-162">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="2864b-163">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span><span class="sxs-lookup"><span data-stu-id="2864b-163">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note]
> <span data-ttu-id="2864b-164">Companies often add fields to customise C5 for their specific line of business.</span><span class="sxs-lookup"><span data-stu-id="2864b-164">Companies often add fields to customize C5 for their specific line of business.</span></span> <span data-ttu-id="2864b-165">[!INCLUDE [d365fin](includes/d365fin_md.md)] does not migrate data from custom fields.</span><span class="sxs-lookup"><span data-stu-id="2864b-165">[!INCLUDE [d365fin](includes/d365fin_md.md)] does not migrate data from custom fields.</span></span> <span data-ttu-id="2864b-166">Also, migration will fail if you have more than 10 custom fields.</span><span class="sxs-lookup"><span data-stu-id="2864b-166">Also, migration will fail if you have more than 10 custom fields.</span></span>

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="2864b-167">Viewing the Status of the Migration</span><span class="sxs-lookup"><span data-stu-id="2864b-167">Viewing the Status of the Migration</span></span>
<span data-ttu-id="2864b-168">Use the **Data Migration Overview** page to monitor the success of the migration.</span><span class="sxs-lookup"><span data-stu-id="2864b-168">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="2864b-169">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span><span class="sxs-lookup"><span data-stu-id="2864b-169">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="2864b-170">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span><span class="sxs-lookup"><span data-stu-id="2864b-170">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="2864b-171">For more information, see the next section in this topic.</span><span class="sxs-lookup"><span data-stu-id="2864b-171">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="2864b-172">While you are waiting for the results of the migration, you must refresh the page to display the results.</span><span class="sxs-lookup"><span data-stu-id="2864b-172">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="correcting-errors"></a><span data-ttu-id="2864b-173">Correcting Errors</span><span class="sxs-lookup"><span data-stu-id="2864b-173">Correcting Errors</span></span>
<span data-ttu-id="2864b-174">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span><span class="sxs-lookup"><span data-stu-id="2864b-174">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="2864b-175">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span><span class="sxs-lookup"><span data-stu-id="2864b-175">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="2864b-176">The number in the **Error Count** field for the entity.</span><span class="sxs-lookup"><span data-stu-id="2864b-176">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="2864b-177">The entity, and then the **Show Errors** action.</span><span class="sxs-lookup"><span data-stu-id="2864b-177">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="2864b-178">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span><span class="sxs-lookup"><span data-stu-id="2864b-178">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="2864b-179">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span><span class="sxs-lookup"><span data-stu-id="2864b-179">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="2864b-180">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span><span class="sxs-lookup"><span data-stu-id="2864b-180">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="2864b-181">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span><span class="sxs-lookup"><span data-stu-id="2864b-181">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="2864b-182">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span><span class="sxs-lookup"><span data-stu-id="2864b-182">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="2864b-183">If an item variant is created first, the reference to the original item can cause an error message.</span><span class="sxs-lookup"><span data-stu-id="2864b-183">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="2864b-184">Verifying Data After Migrating</span><span class="sxs-lookup"><span data-stu-id="2864b-184">Verifying Data After Migrating</span></span>
<span data-ttu-id="2864b-185">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="2864b-185">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span>


| <span data-ttu-id="2864b-186">Microsoft Dynamcis C5 2012</span><span class="sxs-lookup"><span data-stu-id="2864b-186">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE [d365fin](includes/d365fin_md.md)] |
|----------------------------|----------------------------------------------|
|      <span data-ttu-id="2864b-187">Customer Entries</span><span class="sxs-lookup"><span data-stu-id="2864b-187">Customer Entries</span></span>      |               <span data-ttu-id="2864b-188">General Journals</span><span class="sxs-lookup"><span data-stu-id="2864b-188">General Journals</span></span>               |
|       <span data-ttu-id="2864b-189">Vendor Entries</span><span class="sxs-lookup"><span data-stu-id="2864b-189">Vendor Entries</span></span>       |               <span data-ttu-id="2864b-190">General Journals</span><span class="sxs-lookup"><span data-stu-id="2864b-190">General Journals</span></span>               |
|        <span data-ttu-id="2864b-191">Item Entries</span><span class="sxs-lookup"><span data-stu-id="2864b-191">Item Entries</span></span>        |                <span data-ttu-id="2864b-192">Item Journals</span><span class="sxs-lookup"><span data-stu-id="2864b-192">Item Journals</span></span>                 |

<span data-ttu-id="2864b-193">In [!INCLUDE [d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span><span class="sxs-lookup"><span data-stu-id="2864b-193">In [!INCLUDE [d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span></span>

## <a name="stopping-data-migration"></a><span data-ttu-id="2864b-194">Stopping Data Migration</span><span class="sxs-lookup"><span data-stu-id="2864b-194">Stopping Data Migration</span></span>
<span data-ttu-id="2864b-195">You can stop migrating data by choosing **Stop All Migrations**.</span><span class="sxs-lookup"><span data-stu-id="2864b-195">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="2864b-196">If you do, all pending migrations are also stopped.</span><span class="sxs-lookup"><span data-stu-id="2864b-196">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="2864b-197">See Also</span><span class="sxs-lookup"><span data-stu-id="2864b-197">See Also</span></span>
<span data-ttu-id="2864b-198">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="2864b-198">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="2864b-199">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="2864b-199">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  