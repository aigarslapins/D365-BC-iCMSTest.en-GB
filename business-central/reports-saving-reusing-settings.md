---
title: Apply and Modify Saved Settings on Reports | Microsoft Docs
description: Describes using predefined options and filters to customise a report, and to generate the correct data.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customization, personalization
ms.date: 10/01/2018
ms.author: jswymer
ms.openlocfilehash: 9fd086831c0d145570d87c33c62a003c166aca87
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "267805"
---
# <a name="managing-saved-settings-on-reports"></a><span data-ttu-id="5811c-103">Managing Saved Settings on Reports</span><span class="sxs-lookup"><span data-stu-id="5811c-103">Managing Saved Settings on Reports</span></span>
<span data-ttu-id="5811c-104">When running a reports, users are typically presented with a page that lets them set certain options and filters for changing the data that is included in the generated report.</span><span class="sxs-lookup"><span data-stu-id="5811c-104">When running a reports, users are typically presented with a page that lets them set certain options and filters for changing the data that is included in the generated report.</span></span> <span data-ttu-id="5811c-105">This page is called the report request page.</span><span class="sxs-lookup"><span data-stu-id="5811c-105">This page is called the report request page.</span></span> <span data-ttu-id="5811c-106">A report can include one or more *saved settings* that users can apply to the report from the request page.</span><span class="sxs-lookup"><span data-stu-id="5811c-106">A report can include one or more *saved settings* that users can apply to the report from the request page.</span></span> <span data-ttu-id="5811c-107">*Saved settings* are basically predefined options and filters.</span><span class="sxs-lookup"><span data-stu-id="5811c-107">*Saved settings* are basically predefined options and filters.</span></span> <span data-ttu-id="5811c-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span><span class="sxs-lookup"><span data-stu-id="5811c-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span></span> <span data-ttu-id="5811c-109">For more information about how saved settings are used, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span><span class="sxs-lookup"><span data-stu-id="5811c-109">For more information about how saved settings are used, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span></span>

<span data-ttu-id="5811c-110">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in company.</span><span class="sxs-lookup"><span data-stu-id="5811c-110">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in company.</span></span> <span data-ttu-id="5811c-111">You can assign saved settings for a report to individual users or all users in the company.</span><span class="sxs-lookup"><span data-stu-id="5811c-111">You can assign saved settings for a report to individual users or all users in the company.</span></span>

<!-- 
## Apply saved settings to a report
1. Open the report.

   The report request page appears.    
2. In the **Saved Settings** section of the page, set the **Name** field  to the saved settings that you want to use.

   The **Saved Settings** section only appears if the report has been run before or if there are existing saved settings entries. The saved settings entry called **Last used options and filters** is always available. These settings are the option and filter values that were used the last time you ran the report.

-->

## <a name="create-and-modify-saved-settings-for-all-users"></a><span data-ttu-id="5811c-112">Create and modify saved settings for all users</span><span class="sxs-lookup"><span data-stu-id="5811c-112">Create and modify saved settings for all users</span></span>
<span data-ttu-id="5811c-113">You manage saved settings from page **1560 Reports Settings**.</span><span class="sxs-lookup"><span data-stu-id="5811c-113">You manage saved settings from page **1560 Reports Settings**.</span></span> <span data-ttu-id="5811c-114">There are two ways to open this page:</span><span class="sxs-lookup"><span data-stu-id="5811c-114">There are two ways to open this page:</span></span>
-   <span data-ttu-id="5811c-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Settings**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5811c-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Settings**, and then choose the related link.</span></span>
-   <span data-ttu-id="5811c-116">Open a report, choose the lookup next to the **Used default values from:** box, choose **Select from full list**.</span><span class="sxs-lookup"><span data-stu-id="5811c-116">Open a report, choose the lookup next to the **Used default values from:** box, choose **Select from full list**.</span></span>

<span data-ttu-id="5811c-117">The page displays all the existing save settings entries for all users.</span><span class="sxs-lookup"><span data-stu-id="5811c-117">The page displays all the existing save settings entries for all users.</span></span> <span data-ttu-id="5811c-118">If there is a user name in the **Assigned to** column, only that user can use the saved settings for the associated report.</span><span class="sxs-lookup"><span data-stu-id="5811c-118">If there is a user name in the **Assigned to** column, only that user can use the saved settings for the associated report.</span></span> <span data-ttu-id="5811c-119">If there is a check mark in the **Share with all users** column, all users can use the saved settings for the report.</span><span class="sxs-lookup"><span data-stu-id="5811c-119">If there is a check mark in the **Share with all users** column, all users can use the saved settings for the report.</span></span>

<span data-ttu-id="5811c-120">From the **Report Settings** page, you can:</span><span class="sxs-lookup"><span data-stu-id="5811c-120">From the **Report Settings** page, you can:</span></span>
-   <span data-ttu-id="5811c-121">Choose **New** to create a new saved settings entry from scratch.</span><span class="sxs-lookup"><span data-stu-id="5811c-121">Choose **New** to create a new saved settings entry from scratch.</span></span>
-   <span data-ttu-id="5811c-122">Select a saved settings entry from the list, and choose **Copy** to create a copy.</span><span class="sxs-lookup"><span data-stu-id="5811c-122">Select a saved settings entry from the list, and choose **Copy** to create a copy.</span></span>
-   <span data-ttu-id="5811c-123">Select a saved settings entry from the list, and choose **Edit** to modify a saved settings entry.</span><span class="sxs-lookup"><span data-stu-id="5811c-123">Select a saved settings entry from the list, and choose **Edit** to modify a saved settings entry.</span></span>


> [!Important]
> <span data-ttu-id="5811c-124">Consider the name that you give a saved settings entry.</span><span class="sxs-lookup"><span data-stu-id="5811c-124">Consider the name that you give a saved settings entry.</span></span> <span data-ttu-id="5811c-125">If you create a saved settings entry for all users, and you give it the same name as an existing saved settings entry that is assigned to a specific user only, then that user will not be able to use the saved settings entry that is assigned to everyone.</span><span class="sxs-lookup"><span data-stu-id="5811c-125">If you create a saved settings entry for all users, and you give it the same name as an existing saved settings entry that is assigned to a specific user only, then that user will not be able to use the saved settings entry that is assigned to everyone.</span></span>  <span data-ttu-id="5811c-126">Under **Saved Settings** on the report request page, the user will see two saved settings entries with the same name.</span><span class="sxs-lookup"><span data-stu-id="5811c-126">Under **Saved Settings** on the report request page, the user will see two saved settings entries with the same name.</span></span> <span data-ttu-id="5811c-127">However, no matter which option he chooses, the user-specific saved settings entry will be used.</span><span class="sxs-lookup"><span data-stu-id="5811c-127">However, no matter which option he chooses, the user-specific saved settings entry will be used.</span></span>

> [!NOTE]
> <span data-ttu-id="5811c-128">The saved settings feature is available only on reports where the [SaveValues property](https://docs.microsoft.com/en-us/dynamics-nav/savevalues-property) of the report's request page is set to `Yes`.</span><span class="sxs-lookup"><span data-stu-id="5811c-128">The saved settings feature is available only on reports where the [SaveValues property](https://docs.microsoft.com/en-us/dynamics-nav/savevalues-property) of the report's request page is set to `Yes`.</span></span> <span data-ttu-id="5811c-129">The **SaveValues** property is set in the development environment.</span><span class="sxs-lookup"><span data-stu-id="5811c-129">The **SaveValues** property is set in the development environment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5811c-130">See Also</span><span class="sxs-lookup"><span data-stu-id="5811c-130">See Also</span></span>
[<span data-ttu-id="5811c-131">Working with Reports</span><span class="sxs-lookup"><span data-stu-id="5811c-131">Working with Reports</span></span>](ui-work-report.md)  