---
title: How to Prepare a Configuration Package | Microsoft Docs
description: When you configure a new company, table relations are recognised and processed. Data is imported and applied in the correct order. Dimension tables are also imported if they are included in the configuration package.
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
ms.openlocfilehash: ea4a7671788ba5c4bd251a83dab1f2616cfbe706
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "284431"
---
# <a name="prepare-a-configuration-package"></a><span data-ttu-id="95497-105">Prepare a Configuration Package</span><span class="sxs-lookup"><span data-stu-id="95497-105">Prepare a Configuration Package</span></span>
<span data-ttu-id="95497-106">When you configure a new company, table relations are recognised and processed.</span><span class="sxs-lookup"><span data-stu-id="95497-106">When you configure a new company, table relations are recognized and processed.</span></span> <span data-ttu-id="95497-107">Data is imported and applied in the correct order.</span><span class="sxs-lookup"><span data-stu-id="95497-107">Data is imported and applied in the correct order.</span></span> <span data-ttu-id="95497-108">Dimension tables are also imported if they are included in the configuration package.</span><span class="sxs-lookup"><span data-stu-id="95497-108">Dimension tables are also imported if they are included in the configuration package.</span></span>  

<span data-ttu-id="95497-109">To help your customer use the configuration package, you may want to add a questionnaire or a set of questionnaires to the package.</span><span class="sxs-lookup"><span data-stu-id="95497-109">To help your customer use the configuration package, you may want to add a questionnaire or a set of questionnaires to the package.</span></span> <span data-ttu-id="95497-110">The questionnaire can help the customer in understanding the various setup options.</span><span class="sxs-lookup"><span data-stu-id="95497-110">The questionnaire can help the customer in understanding the various setup options.</span></span> <span data-ttu-id="95497-111">Typically, questionnaires are created for the major setup tables where a customer may require additional guidance about how to select an appropriate setting.</span><span class="sxs-lookup"><span data-stu-id="95497-111">Typically, questionnaires are created for the major setup tables where a customer may require additional guidance about how to select an appropriate setting.</span></span> <span data-ttu-id="95497-112">For more information, see [Gather Customer Setup Values](admin-gather-customer-setup-values.md).</span><span class="sxs-lookup"><span data-stu-id="95497-112">For more information, see [Gather Customer Setup Values](admin-gather-customer-setup-values.md).</span></span>

<span data-ttu-id="95497-113">Make sure that you are on the RapidStart Services Implementer Role Centre.</span><span class="sxs-lookup"><span data-stu-id="95497-113">Make sure that you are on the RapidStart Services Implementer Role Center.</span></span> <span data-ttu-id="95497-114">For more information, see [Use the RapidStart Services Implementer Role Centre](admin-how-to-use-the-rapidstart-services-role-center-to-track-progress.md).</span><span class="sxs-lookup"><span data-stu-id="95497-114">For more information, see [Use the RapidStart Services Implementer Role Center](admin-how-to-use-the-rapidstart-services-role-center-to-track-progress.md).</span></span>

> [!IMPORTANT]  
>  <span data-ttu-id="95497-115">When exporting and importing configuration packages between two company databases, the databases should have the same schema to ensure that all data is transferred successfully.</span><span class="sxs-lookup"><span data-stu-id="95497-115">When exporting and importing configuration packages between two company databases, the databases should have the same schema to ensure that all data is transferred successfully.</span></span> <span data-ttu-id="95497-116">This means that the databases should have the same table and field structure, in which the tables have the same primary keys and fields have the same IDs and data types.</span><span class="sxs-lookup"><span data-stu-id="95497-116">This means that the databases should have the same table and field structure, in which the tables have the same primary keys and fields have the same IDs and data types.</span></span>  
>   
>  <span data-ttu-id="95497-117">You can import a configuration package that has been exported from a database that has a different schema than that target database.</span><span class="sxs-lookup"><span data-stu-id="95497-117">You can import a configuration package that has been exported from a database that has a different schema than that target database.</span></span> <span data-ttu-id="95497-118">However, any tables or fields in the configuration package that are missing in the target database will not be imported.</span><span class="sxs-lookup"><span data-stu-id="95497-118">However, any tables or fields in the configuration package that are missing in the target database will not be imported.</span></span> <span data-ttu-id="95497-119">Tables with different primary keys and fields with different data types will also not successfully import.</span><span class="sxs-lookup"><span data-stu-id="95497-119">Tables with different primary keys and fields with different data types will also not successfully import.</span></span> <span data-ttu-id="95497-120">For example, if the configuration pack includes table **50000, Customer** that has primary key **Code20** and the database to which you import the pack includes table **50000, Customer Bank Account** that has the primary key **Code20 + Code 20**, then data will not be imported.</span><span class="sxs-lookup"><span data-stu-id="95497-120">For example, if the configuration pack includes table **50000, Customer** that has primary key **Code20** and the database to which you import the pack includes table **50000, Customer Bank Account** that has the primary key **Code20 + Code 20**, then data will not be imported.</span></span>  

## <a name="to-create-a-configuration-package"></a><span data-ttu-id="95497-121">To create a configuration package</span><span class="sxs-lookup"><span data-stu-id="95497-121">To create a configuration package</span></span>  
1. <span data-ttu-id="95497-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="95497-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span></span>  
2. <span data-ttu-id="95497-123">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="95497-123">Choose the **New** action.</span></span>  
3. <span data-ttu-id="95497-124">On the **General** FastTab, fill in the fields as appropriate.</span><span class="sxs-lookup"><span data-stu-id="95497-124">On the **General** FastTab, fill in the fields as appropriate.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="95497-125">To exclude the configuration questionnaires, configuration templates, and configuration worksheet tables from the package, select the **Exclude Configuration Tables** check box.</span><span class="sxs-lookup"><span data-stu-id="95497-125">To exclude the configuration questionnaires, configuration templates, and configuration worksheet tables from the package, select the **Exclude Configuration Tables** check box.</span></span> <span data-ttu-id="95497-126">Otherwise, these tables will be added to the list of package tables automatically when you export the package.</span><span class="sxs-lookup"><span data-stu-id="95497-126">Otherwise, these tables will be added to the list of package tables automatically when you export the package.</span></span>  
5. <span data-ttu-id="95497-127">Choose the **Get Tables** action.</span><span class="sxs-lookup"><span data-stu-id="95497-127">Choose the **Get Tables** action.</span></span> <span data-ttu-id="95497-128">The **Get Package Tables** batch job page opens.</span><span class="sxs-lookup"><span data-stu-id="95497-128">The **Get Package Tables** batch job page opens.</span></span>  
6. <span data-ttu-id="95497-129">Choose the **Select Tables** field.</span><span class="sxs-lookup"><span data-stu-id="95497-129">Choose the **Select Tables** field.</span></span> <span data-ttu-id="95497-130">The **Config. Selection** page opens.</span><span class="sxs-lookup"><span data-stu-id="95497-130">The **Config. Selection** page opens.</span></span>  
7. <span data-ttu-id="95497-131">Choose the **Select All** action to add all tables to the package, or select the **Selected** check box for each table in the list that you want to add.</span><span class="sxs-lookup"><span data-stu-id="95497-131">Choose the **Select All** action to add all tables to the package, or select the **Selected** check box for each table in the list that you want to add.</span></span>
8. <span data-ttu-id="95497-132">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-132">Choose the **OK** button.</span></span> <span data-ttu-id="95497-133">The count of tables that you have selected is indicated in the **Select Tables** field.</span><span class="sxs-lookup"><span data-stu-id="95497-133">The count of tables that you have selected is indicated in the **Select Tables** field.</span></span> <span data-ttu-id="95497-134">Specify additional options, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-134">Specify additional options, and then choose the **OK** button.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="95497-135">tables are added to the lines of the **Config. Package** page.</span><span class="sxs-lookup"><span data-stu-id="95497-135">tables are added to the lines of the **Config. Package** page.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="95497-136">You can also do this in the configuration worksheet.</span><span class="sxs-lookup"><span data-stu-id="95497-136">You can also do this in the configuration worksheet.</span></span> <span data-ttu-id="95497-137">Select the tables you want to include in the package, and then choose the **Assign Package** action.</span><span class="sxs-lookup"><span data-stu-id="95497-137">Select the tables you want to include in the package, and then choose the **Assign Package** action.</span></span>

9. <span data-ttu-id="95497-138">To select the fields that you want to include from a table, select the table, and then, on the **Lines** tab, choose the **Fields** action.</span><span class="sxs-lookup"><span data-stu-id="95497-138">To select the fields that you want to include from a table, select the table, and then, on the **Lines** tab, choose the **Fields** action.</span></span>
<span data-ttu-id="95497-139">Specify which fields are included in the package.</span><span class="sxs-lookup"><span data-stu-id="95497-139">Specify which fields are included in the package.</span></span> <span data-ttu-id="95497-140">By default, all fields are included.</span><span class="sxs-lookup"><span data-stu-id="95497-140">By default, all fields are included.</span></span>

    - <span data-ttu-id="95497-141">To select just the fields you want to include, choose the **Clear Included** action.</span><span class="sxs-lookup"><span data-stu-id="95497-141">To select just the fields you want to include, choose the **Clear Included** action.</span></span> <span data-ttu-id="95497-142">To add all fields, choose the **Set Included** action.</span><span class="sxs-lookup"><span data-stu-id="95497-142">To add all fields, choose the **Set Included** action.</span></span>  
    - <span data-ttu-id="95497-143">To specify that the field data should not be validated, clear the **Validate Field** check box for the field.</span><span class="sxs-lookup"><span data-stu-id="95497-143">To specify that the field data should not be validated, clear the **Validate Field** check box for the field.</span></span>  

10. <span data-ttu-id="95497-144">Determine whether you have introduced potential errors, by choosing the **Validate Package** action.</span><span class="sxs-lookup"><span data-stu-id="95497-144">Determine whether you have introduced potential errors, by choosing the **Validate Package** action.</span></span> <span data-ttu-id="95497-145">This can occur when you do not include tables that your configuration relies on.</span><span class="sxs-lookup"><span data-stu-id="95497-145">This can occur when you do not include tables that your configuration relies on.</span></span>  
11. <span data-ttu-id="95497-146">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-146">Choose the **OK** button.</span></span>  

<span data-ttu-id="95497-147">After you have refined the list of fields to include from a table, you can check your results in Excel.</span><span class="sxs-lookup"><span data-stu-id="95497-147">After you have refined the list of fields to include from a table, you can check your results in Excel.</span></span>  

### <a name="to-filter-and-review-your-dataset"></a><span data-ttu-id="95497-148">To filter and review your dataset</span><span class="sxs-lookup"><span data-stu-id="95497-148">To filter and review your dataset</span></span>  
1. <span data-ttu-id="95497-149">To filter to a certain set of records to include in the package, on the **Lines** tab, choose the **Filters** action, and then specify the appropriate filter values.</span><span class="sxs-lookup"><span data-stu-id="95497-149">To filter to a certain set of records to include in the package, on the **Lines** tab, choose the **Filters** action, and then specify the appropriate filter values.</span></span>  
2. <span data-ttu-id="95497-150">On the package card, on the **Lines** tab, choose the **Export to Excel** action.</span><span class="sxs-lookup"><span data-stu-id="95497-150">On the package card, on the **Lines** tab, choose the **Export to Excel** action.</span></span>  
3. <span data-ttu-id="95497-151">Confirm the messages that enable the export of data to Excel.</span><span class="sxs-lookup"><span data-stu-id="95497-151">Confirm the messages that enable the export of data to Excel.</span></span> <span data-ttu-id="95497-152">The named .xlsx file opens.</span><span class="sxs-lookup"><span data-stu-id="95497-152">The named .xlsx file opens.</span></span> <span data-ttu-id="95497-153">Review the records that have been exported.</span><span class="sxs-lookup"><span data-stu-id="95497-153">Review the records that have been exported.</span></span>  
4. <span data-ttu-id="95497-154">Close Excel.</span><span class="sxs-lookup"><span data-stu-id="95497-154">Close Excel.</span></span>  

### <a name="to-include-a-template-for-application-to-a-table"></a><span data-ttu-id="95497-155">To include a template for application to a table</span><span class="sxs-lookup"><span data-stu-id="95497-155">To include a template for application to a table</span></span>  
<span data-ttu-id="95497-156">For certain tables, such a table that will contain master data, you can specify a template to apply to the data.</span><span class="sxs-lookup"><span data-stu-id="95497-156">For certain tables, such a table that will contain master data, you can specify a template to apply to the data.</span></span> <span data-ttu-id="95497-157">The template can include the required fields that you want to apply to all master data and that you never want to vary.</span><span class="sxs-lookup"><span data-stu-id="95497-157">The template can include the required fields that you want to apply to all master data and that you never want to vary.</span></span> <span data-ttu-id="95497-158">For example, you can create a template that can be used with customer data.</span><span class="sxs-lookup"><span data-stu-id="95497-158">For example, you can create a template that can be used with customer data.</span></span> <span data-ttu-id="95497-159">The template can contain all the required fields, which then enables consistent import of standardised information.</span><span class="sxs-lookup"><span data-stu-id="95497-159">The template can contain all the required fields, which then enables consistent import of standardized information.</span></span> <span data-ttu-id="95497-160">Information that cannot be standardised, such as customer name, is then treated when you do an import of customer data.</span><span class="sxs-lookup"><span data-stu-id="95497-160">Information that cannot be standardized, such as customer name, is then treated when you do an import of customer data.</span></span>

1. <span data-ttu-id="95497-161">On the **Config. Package Card** page, select a table, and then choose the **Data Template** field.</span><span class="sxs-lookup"><span data-stu-id="95497-161">On the **Config. Package Card** page, select a table, and then choose the **Data Template** field.</span></span> <span data-ttu-id="95497-162">A list of templates based on the table is displayed.</span><span class="sxs-lookup"><span data-stu-id="95497-162">A list of templates based on the table is displayed.</span></span>
2. <span data-ttu-id="95497-163">Select a template, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-163">Select a template, and then choose the **OK** button.</span></span>  

<span data-ttu-id="95497-164">After the package is complete, follow the next procedure to save the package to a file.</span><span class="sxs-lookup"><span data-stu-id="95497-164">After the package is complete, follow the next procedure to save the package to a file.</span></span> <span data-ttu-id="95497-165">You can then give the package to a customer or partner to use.</span><span class="sxs-lookup"><span data-stu-id="95497-165">You can then give the package to a customer or partner to use.</span></span>

### <a name="to-save-and-export-a-configuration-package"></a><span data-ttu-id="95497-166">To save and export a configuration package</span><span class="sxs-lookup"><span data-stu-id="95497-166">To save and export a configuration package</span></span>  
- <span data-ttu-id="95497-167">On the **Config. Package Card** page, choose the **Export Package** action.</span><span class="sxs-lookup"><span data-stu-id="95497-167">On the **Config. Package Card** page, choose the **Export Package** action.</span></span>  

<span data-ttu-id="95497-168">The package is created in a .rapidstart file, which delivers the package contents in a compressed format.</span><span class="sxs-lookup"><span data-stu-id="95497-168">The package is created in a .rapidstart file, which delivers the package contents in a compressed format.</span></span> <span data-ttu-id="95497-169">Configuration questionnaires, configuration templates, and the configuration worksheet are added to the package automatically unless you specifically decide to exclude them.</span><span class="sxs-lookup"><span data-stu-id="95497-169">Configuration questionnaires, configuration templates, and the configuration worksheet are added to the package automatically unless you specifically decide to exclude them.</span></span>  

<span data-ttu-id="95497-170">You can save the file with a name that is meaningful to you, but you cannot change the extension of the file.</span><span class="sxs-lookup"><span data-stu-id="95497-170">You can save the file with a name that is meaningful to you, but you cannot change the extension of the file.</span></span> <span data-ttu-id="95497-171">It must be .rapidstart.</span><span class="sxs-lookup"><span data-stu-id="95497-171">It must be .rapidstart.</span></span>  

### <a name="to-copy-a-configuration-package"></a><span data-ttu-id="95497-172">To copy a configuration package</span><span class="sxs-lookup"><span data-stu-id="95497-172">To copy a configuration package</span></span>  
<span data-ttu-id="95497-173">After you have created a package that meets most of your needs, you can use it as a basis for creating similar packages.</span><span class="sxs-lookup"><span data-stu-id="95497-173">After you have created a package that meets most of your needs, you can use it as a basis for creating similar packages.</span></span> <span data-ttu-id="95497-174">This can speed up implementation time and enhances the repeatability of RapidStart Services.</span><span class="sxs-lookup"><span data-stu-id="95497-174">This can speed up implementation time and enhances the repeatability of RapidStart Services.</span></span>

1. <span data-ttu-id="95497-175">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="95497-175">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span></span>  
2. <span data-ttu-id="95497-176">Select a package from the list, and then choose the **Copy Package** action.</span><span class="sxs-lookup"><span data-stu-id="95497-176">Select a package from the list, and then choose the **Copy Package** action.</span></span>  
3. <span data-ttu-id="95497-177">In the **New Package Code** field, enter a code for the new package.</span><span class="sxs-lookup"><span data-stu-id="95497-177">In the **New Package Code** field, enter a code for the new package.</span></span>  
4. <span data-ttu-id="95497-178">Select the **Copy Data** check box if you also want to copy database data from the existing package.</span><span class="sxs-lookup"><span data-stu-id="95497-178">Select the **Copy Data** check box if you also want to copy database data from the existing package.</span></span>  
5. <span data-ttu-id="95497-179">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-179">Choose the **OK** button.</span></span>

## <a name="to-customize-a-configuration-package"></a><span data-ttu-id="95497-180">To customise a configuration package</span><span class="sxs-lookup"><span data-stu-id="95497-180">To customize a configuration package</span></span>
<span data-ttu-id="95497-181">Use the configuration worksheet to gather and categorise the information that you want to use to configure a new company, and arrange tables in a logical way.</span><span class="sxs-lookup"><span data-stu-id="95497-181">Use the configuration worksheet to gather and categorize the information that you want to use to configure a new company, and arrange tables in a logical way.</span></span> <span data-ttu-id="95497-182">Formatting in the worksheet is based on a simple hierarchy: Areas contain groups, which in turn contain tables.</span><span class="sxs-lookup"><span data-stu-id="95497-182">Formatting in the worksheet is based on a simple hierarchy: Areas contain groups, which in turn contain tables.</span></span> <span data-ttu-id="95497-183">Areas and groups are optional, but are necessary to enable an overview of the configuration process on the RapidStart Services Role Centre.</span><span class="sxs-lookup"><span data-stu-id="95497-183">Areas and groups are optional, but are necessary to enable an overview of the configuration process on the RapidStart Services Role Center.</span></span>

1.  <span data-ttu-id="95497-184">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="95497-184">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="95497-185">In the **Line Type** field, choose **Area**.</span><span class="sxs-lookup"><span data-stu-id="95497-185">In the **Line Type** field, choose **Area**.</span></span> <span data-ttu-id="95497-186">In the **Name** field, enter a descriptive name.</span><span class="sxs-lookup"><span data-stu-id="95497-186">In the **Name** field, enter a descriptive name.</span></span>  
3.  <span data-ttu-id="95497-187">In the **Line Type** field, choose **Group**.</span><span class="sxs-lookup"><span data-stu-id="95497-187">In the **Line Type** field, choose **Group**.</span></span> <span data-ttu-id="95497-188">In the **Name** field, enter a descriptive name.</span><span class="sxs-lookup"><span data-stu-id="95497-188">In the **Name** field, enter a descriptive name.</span></span>  
4.  <span data-ttu-id="95497-189">In the **Line Type** field, choose **Table**.</span><span class="sxs-lookup"><span data-stu-id="95497-189">In the **Line Type** field, choose **Table**.</span></span> <span data-ttu-id="95497-190">In the **Table ID** field, select the table you want to include in the worksheet.</span><span class="sxs-lookup"><span data-stu-id="95497-190">In the **Table ID** field, select the table you want to include in the worksheet.</span></span>  

<span data-ttu-id="95497-191">You can now assign the tables to specific configuration packages that you have created or plan to create.</span><span class="sxs-lookup"><span data-stu-id="95497-191">You can now assign the tables to specific configuration packages that you have created or plan to create.</span></span> <span data-ttu-id="95497-192">For more information, see the "To assign a table to a configuration package" section.</span><span class="sxs-lookup"><span data-stu-id="95497-192">For more information, see the "To assign a table to a configuration package" section.</span></span>

## <a name="to-work-with-promoted-tables"></a><span data-ttu-id="95497-193">To work with promoted tables</span><span class="sxs-lookup"><span data-stu-id="95497-193">To work with promoted tables</span></span>  
1. <span data-ttu-id="95497-194">Select the **Promoted Table** check box to indicate a table that is frequently used during the setup process by a typical customer, for example, the **G/L Account** table.</span><span class="sxs-lookup"><span data-stu-id="95497-194">Select the **Promoted Table** check box to indicate a table that is frequently used during the setup process by a typical customer, for example, the **G/L Account** table.</span></span> <span data-ttu-id="95497-195">When a table has this designation, a customer will be able to easily filter his worksheet to see just the list of promoted tables that require attention.</span><span class="sxs-lookup"><span data-stu-id="95497-195">When a table has this designation, a customer will be able to easily filter his worksheet to see just the list of promoted tables that require attention.</span></span>  
2. <span data-ttu-id="95497-196">To see the filtered view, choose the **Promoted Only** action.</span><span class="sxs-lookup"><span data-stu-id="95497-196">To see the filtered view, choose the **Promoted Only** action.</span></span> <span data-ttu-id="95497-197">The list of tables contains only those tables that have the check box selected.</span><span class="sxs-lookup"><span data-stu-id="95497-197">The list of tables contains only those tables that have the check box selected.</span></span>  

## <a name="to-assign-a-table-to-a-configuration-package"></a><span data-ttu-id="95497-198">To assign a table to a configuration package</span><span class="sxs-lookup"><span data-stu-id="95497-198">To assign a table to a configuration package</span></span>  
<span data-ttu-id="95497-199">After you have defined the tables that you want to treat as part of your configuration, you can easily assign the tables to configuration packages.</span><span class="sxs-lookup"><span data-stu-id="95497-199">After you have defined the tables that you want to treat as part of your configuration, you can easily assign the tables to configuration packages.</span></span> <span data-ttu-id="95497-200">You can assign a table to one package only.</span><span class="sxs-lookup"><span data-stu-id="95497-200">You can assign a table to one package only.</span></span> <span data-ttu-id="95497-201">In the following procedure, you assign the package from within configuration worksheet.</span><span class="sxs-lookup"><span data-stu-id="95497-201">In the following procedure, you assign the package from within configuration worksheet.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="95497-202">You can also create a package directly, and add tables to it.</span><span class="sxs-lookup"><span data-stu-id="95497-202">You can also create a package directly, and add tables to it.</span></span> <span data-ttu-id="95497-203">For more information, see the "To create a configuration package" section.</span><span class="sxs-lookup"><span data-stu-id="95497-203">For more information, see the "To create a configuration package" section.</span></span>

1. <span data-ttu-id="95497-204">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="95497-204">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span></span>
2. <span data-ttu-id="95497-205">In the configuration worksheet, select a line or group of lines that you want to assign to a configuration package, and then choose the **Assign Package** action.</span><span class="sxs-lookup"><span data-stu-id="95497-205">In the configuration worksheet, select a line or group of lines that you want to assign to a configuration package, and then choose the **Assign Package** action.</span></span>  
3.  <span data-ttu-id="95497-206">Select a package from the list, or choose the **New** action to create a new package, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-206">Select a package from the list, or choose the **New** action to create a new package, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="95497-207">If a table is not already included in the package, it will now be added.</span><span class="sxs-lookup"><span data-stu-id="95497-207">If a table is not already included in the package, it will now be added.</span></span> <span data-ttu-id="95497-208">The package code field on the worksheet line will be filled in with the code of the package that the table is assigned to.</span><span class="sxs-lookup"><span data-stu-id="95497-208">The package code field on the worksheet line will be filled in with the code of the package that the table is assigned to.</span></span>  
4. <span data-ttu-id="95497-209">If you choose an existing package, you can see how many tables are already in the package by reviewing the information in the **No. of Tables** field.</span><span class="sxs-lookup"><span data-stu-id="95497-209">If you choose an existing package, you can see how many tables are already in the package by reviewing the information in the **No. of Tables** field.</span></span>

## <a name="to-review-or-customize-existing-database-data"></a><span data-ttu-id="95497-210">To review or customise existing database data</span><span class="sxs-lookup"><span data-stu-id="95497-210">To review or customize existing database data</span></span>
<span data-ttu-id="95497-211">As you create a configuration package for a solution, you can view and customise the available database data to suit your customer needs.</span><span class="sxs-lookup"><span data-stu-id="95497-211">As you create a configuration package for a solution, you can view and customize the available database data to suit your customer needs.</span></span> <span data-ttu-id="95497-212">The database table must have an associated page.</span><span class="sxs-lookup"><span data-stu-id="95497-212">The database table must have an associated page.</span></span>  

1. <span data-ttu-id="95497-213">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="95497-213">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span></span>
2. <span data-ttu-id="95497-214">In the configuration worksheet, identify the tables whose data that you want to view or customise.</span><span class="sxs-lookup"><span data-stu-id="95497-214">In the configuration worksheet, identify the tables whose data that you want to view or customize.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="95497-215">Make sure that each table has a page ID assigned to it.</span><span class="sxs-lookup"><span data-stu-id="95497-215">Make sure that each table has a page ID assigned to it.</span></span> <span data-ttu-id="95497-216">For standard [!INCLUDE[d365fin](includes/d365fin_md.md)] tables, this value is automatically filled in.</span><span class="sxs-lookup"><span data-stu-id="95497-216">For standard [!INCLUDE[d365fin](includes/d365fin_md.md)] tables, this value is automatically filled in.</span></span> <span data-ttu-id="95497-217">For custom tables, you must provide the ID.</span><span class="sxs-lookup"><span data-stu-id="95497-217">For custom tables, you must provide the ID.</span></span>

3. <span data-ttu-id="95497-218">Choose the **Database Data** action.</span><span class="sxs-lookup"><span data-stu-id="95497-218">Choose the **Database Data** action.</span></span> <span data-ttu-id="95497-219">The page for the related page opens.</span><span class="sxs-lookup"><span data-stu-id="95497-219">The page for the related page opens.</span></span>
4. <span data-ttu-id="95497-220">Review the available information.</span><span class="sxs-lookup"><span data-stu-id="95497-220">Review the available information.</span></span> <span data-ttu-id="95497-221">Modify it as necessary by deleting records that are not relevant or by adding new ones.</span><span class="sxs-lookup"><span data-stu-id="95497-221">Modify it as necessary by deleting records that are not relevant or by adding new ones.</span></span>    

## <a name="to-copy-data-from-a-test-environment-to-a-production-environment"></a><span data-ttu-id="95497-222">To copy data from a test environment to a production environment</span><span class="sxs-lookup"><span data-stu-id="95497-222">To copy data from a test environment to a production environment</span></span>  
<span data-ttu-id="95497-223">After you have vetted and tested all your setup information, you can proceed to copy data to your production environment.</span><span class="sxs-lookup"><span data-stu-id="95497-223">After you have vetted and tested all your setup information, you can proceed to copy data to your production environment.</span></span> <span data-ttu-id="95497-224">You create a new company in the same database.</span><span class="sxs-lookup"><span data-stu-id="95497-224">You create a new company in the same database.</span></span>

1. <span data-ttu-id="95497-225">Open and initialise the new company.</span><span class="sxs-lookup"><span data-stu-id="95497-225">Open and initialize the new company.</span></span>  
2. <span data-ttu-id="95497-226">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="95497-226">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Worksheet**, and then choose the related link.</span></span>  
3. <span data-ttu-id="95497-227">Choose the **Copy Data from the Company** action.</span><span class="sxs-lookup"><span data-stu-id="95497-227">Choose the **Copy Data from the Company** action.</span></span>  
4. <span data-ttu-id="95497-228">On the **Copy Company Data** page, choose the **Copy From** field.</span><span class="sxs-lookup"><span data-stu-id="95497-228">On the **Copy Company Data** page, choose the **Copy From** field.</span></span> <span data-ttu-id="95497-229">The **Companies** page opens.</span><span class="sxs-lookup"><span data-stu-id="95497-229">The **Companies** page opens.</span></span>  
5. <span data-ttu-id="95497-230">Select the company from which you want to copy data, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-230">Select the company from which you want to copy data, and then choose the **OK** button.</span></span> <span data-ttu-id="95497-231">A list of tables selected on the configuration worksheet opens.</span><span class="sxs-lookup"><span data-stu-id="95497-231">A list of tables selected on the configuration worksheet opens.</span></span> <span data-ttu-id="95497-232">Only tables that contain records are included in this list.</span><span class="sxs-lookup"><span data-stu-id="95497-232">Only tables that contain records are included in this list.</span></span>
6. <span data-ttu-id="95497-233">Select the tables that you want to copy data from, and then choose the **Copy Data** action.</span><span class="sxs-lookup"><span data-stu-id="95497-233">Select the tables that you want to copy data from, and then choose the **Copy Data** action.</span></span> <span data-ttu-id="95497-234">On the **Copy Company Data** page, choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="95497-234">On the **Copy Company Data** page, choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="95497-235">See Also</span><span class="sxs-lookup"><span data-stu-id="95497-235">See Also</span></span>  
[<span data-ttu-id="95497-236">Gather Customer Setup Values</span><span class="sxs-lookup"><span data-stu-id="95497-236">Gather Customer Setup Values</span></span>](admin-gather-customer-setup-values.md)  
[<span data-ttu-id="95497-237">Set Up Company Configuration</span><span class="sxs-lookup"><span data-stu-id="95497-237">Set Up Company Configuration</span></span>](admin-set-up-company-configuration.md)  
[<span data-ttu-id="95497-238">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="95497-238">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="95497-239">Administration</span><span class="sxs-lookup"><span data-stu-id="95497-239">Administration</span></span>](admin-setup-and-administration.md)