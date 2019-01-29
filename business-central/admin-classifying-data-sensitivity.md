---
title: Classifying Data Sensitivity
description: You must specify which type of data you store about people so that you can respond to data subject requests.
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.date: 10/01/2018
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.openlocfilehash: 6195a6a6f1d712c7bcd33e5b8aafed6fddb6598d
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "244554"
---
# <a name="classifying-data-sensitivity"></a><span data-ttu-id="9aea1-103">Classifying Data Sensitivity</span><span class="sxs-lookup"><span data-stu-id="9aea1-103">Classifying Data Sensitivity</span></span>
<span data-ttu-id="9aea1-104">To classify the fields that hold sensitive or personal data, a Microsoft partner can set the ```DataClassification``` property on fields.</span><span class="sxs-lookup"><span data-stu-id="9aea1-104">To classify the fields that hold sensitive or personal data, a Microsoft partner can set the ```DataClassification``` property on fields.</span></span> <span data-ttu-id="9aea1-105">This requires access to the database tables, either through the development environment or by running a Windows PowerShell script.</span><span class="sxs-lookup"><span data-stu-id="9aea1-105">This requires access to the database tables, either through the development environment or by running a Windows PowerShell script.</span></span> <span data-ttu-id="9aea1-106">For more information, see [Classifying Data](https://docs.microsoft.com/en-us/dynamics-nav/classifying-data).</span><span class="sxs-lookup"><span data-stu-id="9aea1-106">For more information, see [Classifying Data](https://docs.microsoft.com/en-us/dynamics-nav/classifying-data).</span></span>  

<span data-ttu-id="9aea1-107">As a customer, you can add a second level of classification by specifying sensitivity levels for the data you store in standard and custom fields.</span><span class="sxs-lookup"><span data-stu-id="9aea1-107">As a customer, you can add a second level of classification by specifying sensitivity levels for the data you store in standard and custom fields.</span></span> <span data-ttu-id="9aea1-108">Classifying data sensitivity helps ensure that you know where you keep personal data in your system, and makes it easier to respond to requests from data subjects.</span><span class="sxs-lookup"><span data-stu-id="9aea1-108">Classifying data sensitivity helps ensure that you know where you keep personal data in your system, and makes it easier to respond to requests from data subjects.</span></span> <span data-ttu-id="9aea1-109">For example, if a contact or customer asks you to export their personal data.</span><span class="sxs-lookup"><span data-stu-id="9aea1-109">For example, if a contact or customer asks you to export their personal data.</span></span> <span data-ttu-id="9aea1-110">For more information, see [Responding to Requests About Personal Data](admin-responding-to-requests-about-personal-data.md).</span><span class="sxs-lookup"><span data-stu-id="9aea1-110">For more information, see [Responding to Requests About Personal Data](admin-responding-to-requests-about-personal-data.md).</span></span>

> [!Important]
> <span data-ttu-id="9aea1-111">Microsoft is providing this Data Sensitivity Classification feature as a matter of convenience only.</span><span class="sxs-lookup"><span data-stu-id="9aea1-111">Microsoft is providing this Data Sensitivity Classification feature as a matter of convenience only.</span></span> <span data-ttu-id="9aea1-112">It's your responsibility to classify the data appropriately and comply with any laws and regulations that are applicable to you.</span><span class="sxs-lookup"><span data-stu-id="9aea1-112">It's your responsibility to classify the data appropriately and comply with any laws and regulations that are applicable to you.</span></span> <span data-ttu-id="9aea1-113">Microsoft disclaims all responsibility towards any claims related to your classification of the data.</span><span class="sxs-lookup"><span data-stu-id="9aea1-113">Microsoft disclaims all responsibility towards any claims related to your classification of the data.</span></span>  

<span data-ttu-id="9aea1-114">The following table describes data sensitivity levels you can assign.</span><span class="sxs-lookup"><span data-stu-id="9aea1-114">The following table describes data sensitivity levels you can assign.</span></span>

|<span data-ttu-id="9aea1-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="9aea1-115">Sensitivity</span></span>|<span data-ttu-id="9aea1-116">Description</span><span class="sxs-lookup"><span data-stu-id="9aea1-116">Description</span></span>|
|----|----|
|<span data-ttu-id="9aea1-117">Sensitive</span><span class="sxs-lookup"><span data-stu-id="9aea1-117">Sensitive</span></span> | <span data-ttu-id="9aea1-118">Information about a data subject's racial or ethnic origin, political opinions, religious beliefs, involvement with trade unions, physical or mental health, sexuality, or details about criminal offenses.</span><span class="sxs-lookup"><span data-stu-id="9aea1-118">Information about a data subject's racial or ethnic origin, political opinions, religious beliefs, involvement with trade unions, physical or mental health, sexuality, or details about criminal offenses.</span></span> |
|<span data-ttu-id="9aea1-119">Personal</span><span class="sxs-lookup"><span data-stu-id="9aea1-119">Personal</span></span> | <span data-ttu-id="9aea1-120">Information that can be used to identify a data subject, either directly or in combination with other data or information.</span><span class="sxs-lookup"><span data-stu-id="9aea1-120">Information that can be used to identify a data subject, either directly or in combination with other data or information.</span></span>|
|<span data-ttu-id="9aea1-121">Confidential</span><span class="sxs-lookup"><span data-stu-id="9aea1-121">Confidential</span></span> | <span data-ttu-id="9aea1-122">Business data that you use for accounting or other business purposes, and do not want to expose to other entities.</span><span class="sxs-lookup"><span data-stu-id="9aea1-122">Business data that you use for accounting or other business purposes, and do not want to expose to other entities.</span></span> <span data-ttu-id="9aea1-123">For example, this might include ledger entries.</span><span class="sxs-lookup"><span data-stu-id="9aea1-123">For example, this might include ledger entries.</span></span>|
|<span data-ttu-id="9aea1-124">Normal</span><span class="sxs-lookup"><span data-stu-id="9aea1-124">Normal</span></span> | <span data-ttu-id="9aea1-125">General data that does not belong to any other categories.</span><span class="sxs-lookup"><span data-stu-id="9aea1-125">General data that does not belong to any other categories.</span></span>|

## <a name="how-do-i-classify-my-data"></a><span data-ttu-id="9aea1-126">How Do I Classify My Data?</span><span class="sxs-lookup"><span data-stu-id="9aea1-126">How Do I Classify My Data?</span></span>
<span data-ttu-id="9aea1-127">Classifying the sensitivity of a large number of fields one-by-one would take a long time.</span><span class="sxs-lookup"><span data-stu-id="9aea1-127">Classifying the sensitivity of a large number of fields one-by-one would take a long time.</span></span> <span data-ttu-id="9aea1-128">To help speed up the process, we provide tools that you can use to bulk classify the sensitivity of fields, and then fine-tune classifications for specific fields.</span><span class="sxs-lookup"><span data-stu-id="9aea1-128">To help speed up the process, we provide tools that you can use to bulk classify the sensitivity of fields, and then fine-tune classifications for specific fields.</span></span> <span data-ttu-id="9aea1-129">You can find tools on the Data Classification worksheet, which is available on the Administration of users, user groups, and permissions Role Centre.</span><span class="sxs-lookup"><span data-stu-id="9aea1-129">You can find tools on the Data Classification worksheet, which is available on the Administration of users, user groups, and permissions Role Center.</span></span> <span data-ttu-id="9aea1-130">You must be a system administrator to use the worksheet.</span><span class="sxs-lookup"><span data-stu-id="9aea1-130">You must be a system administrator to use the worksheet.</span></span>

> [!Important]
> <span data-ttu-id="9aea1-131">When you open the Data Classification worksheet for the first time, it will be empty.</span><span class="sxs-lookup"><span data-stu-id="9aea1-131">When you open the Data Classification worksheet for the first time, it will be empty.</span></span> <span data-ttu-id="9aea1-132">You must run the Data Classification guide to generate the list of fields.</span><span class="sxs-lookup"><span data-stu-id="9aea1-132">You must run the Data Classification guide to generate the list of fields.</span></span> <span data-ttu-id="9aea1-133">To start the guide, choose the **Set Up Data Classifications** action.</span><span class="sxs-lookup"><span data-stu-id="9aea1-133">To start the guide, choose the **Set Up Data Classifications** action.</span></span>

<span data-ttu-id="9aea1-134">For example, the Data Classification worksheet lets you do things like:</span><span class="sxs-lookup"><span data-stu-id="9aea1-134">For example, the Data Classification worksheet lets you do things like:</span></span>  

* <span data-ttu-id="9aea1-135">Use the Data Classification guide to export your fields to an Excel worksheet where you can bulk classify them.</span><span class="sxs-lookup"><span data-stu-id="9aea1-135">Use the Data Classification guide to export your fields to an Excel worksheet where you can bulk classify them.</span></span> <span data-ttu-id="9aea1-136">Using the Excel worksheet is particularly useful if you are collaborating with a Microsoft partner.</span><span class="sxs-lookup"><span data-stu-id="9aea1-136">Using the Excel worksheet is particularly useful if you are collaborating with a Microsoft partner.</span></span> <span data-ttu-id="9aea1-137">After you update the worksheet, you can use the guide to import and apply the classifications.</span><span class="sxs-lookup"><span data-stu-id="9aea1-137">After you update the worksheet, you can use the guide to import and apply the classifications.</span></span> <span data-ttu-id="9aea1-138">You can also use the guide to classify fields manually.</span><span class="sxs-lookup"><span data-stu-id="9aea1-138">You can also use the guide to classify fields manually.</span></span>  
* <span data-ttu-id="9aea1-139">Choose a field and then filter the list to find similar fields that are likely to belong to the same classification as the field you based the search on.</span><span class="sxs-lookup"><span data-stu-id="9aea1-139">Choose a field and then filter the list to find similar fields that are likely to belong to the same classification as the field you based the search on.</span></span>  
* <span data-ttu-id="9aea1-140">Investigate a field by viewing its contents.</span><span class="sxs-lookup"><span data-stu-id="9aea1-140">Investigate a field by viewing its contents.</span></span>  

> [!Tip]
> <span data-ttu-id="9aea1-141">We have defined sample sensitivity classifications for the tables and fields in the Cronus demonstration company.</span><span class="sxs-lookup"><span data-stu-id="9aea1-141">We have defined sample sensitivity classifications for the tables and fields in the Cronus demonstration company.</span></span> <span data-ttu-id="9aea1-142">You can use those classifications as inspiration when you classify your own tables and fields.</span><span class="sxs-lookup"><span data-stu-id="9aea1-142">You can use those classifications as inspiration when you classify your own tables and fields.</span></span>

## <a name="see-also"></a><span data-ttu-id="9aea1-143">See Also</span><span class="sxs-lookup"><span data-stu-id="9aea1-143">See Also</span></span>
[<span data-ttu-id="9aea1-144">Classifying Data</span><span class="sxs-lookup"><span data-stu-id="9aea1-144">Classifying Data</span></span>](https://docs.microsoft.com/en-us/dynamics-nav/classifying-data)  