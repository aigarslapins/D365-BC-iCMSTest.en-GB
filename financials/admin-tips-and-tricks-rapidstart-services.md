---
title: Tips and Tricks - RapidStart Services | Microsoft Docs
description: When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.
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
ms.openlocfilehash: 8bd101b6f43ef6bf59e32464b9ef8e936d3f42ca
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "259988"
---
# <a name="tips-and-tricks-rapidstart-services"></a><span data-ttu-id="4bdf3-103">Tips and Tricks: RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="4bdf3-103">Tips and Tricks: RapidStart Services</span></span>
<span data-ttu-id="4bdf3-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span></span>  

## <a name="take-advantage-of-configuration-templates"></a><span data-ttu-id="4bdf3-105">Take advantage of configuration templates</span><span class="sxs-lookup"><span data-stu-id="4bdf3-105">Take advantage of configuration templates</span></span>  
<span data-ttu-id="4bdf3-106">Configuration templates can help you streamline your implementation process.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-106">Configuration templates can help you streamline your implementation process.</span></span> <span data-ttu-id="4bdf3-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span></span> <span data-ttu-id="4bdf3-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span></span>  

## <a name="configuration-questionnaires"></a><span data-ttu-id="4bdf3-109">Configuration questionnaires</span><span class="sxs-lookup"><span data-stu-id="4bdf3-109">Configuration questionnaires</span></span>  
<span data-ttu-id="4bdf3-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span></span>  

## <a name="batch-creation-of-journal-lines"></a><span data-ttu-id="4bdf3-111">Batch creation of journal lines</span><span class="sxs-lookup"><span data-stu-id="4bdf3-111">Batch creation of journal lines</span></span>  
<span data-ttu-id="4bdf3-112">We recommend that you use the data migration tools provided to migrate journal entries.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-112">We recommend that you use the data migration tools provided to migrate journal entries.</span></span> <span data-ttu-id="4bdf3-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span></span> <span data-ttu-id="4bdf3-114">The rest of the journal then has to be completed manually.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-114">The rest of the journal then has to be completed manually.</span></span>  

## <a name="migrating-transactions"></a><span data-ttu-id="4bdf3-115">Migrating transactions</span><span class="sxs-lookup"><span data-stu-id="4bdf3-115">Migrating transactions</span></span>  
<span data-ttu-id="4bdf3-116">We recommend that you migrate opening balances in the following order.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-116">We recommend that you migrate opening balances in the following order.</span></span>  

1.  <span data-ttu-id="4bdf3-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span></span> <span data-ttu-id="4bdf3-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span></span> <span data-ttu-id="4bdf3-119">Set up the offsetting accounts to enable direct postings.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-119">Set up the offsetting accounts to enable direct postings.</span></span>  
2.  <span data-ttu-id="4bdf3-120">Migrate open customer ledger entries.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-120">Migrate open customer ledger entries.</span></span>  
3.  <span data-ttu-id="4bdf3-121">Migrate open item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-121">Migrate open item ledger entries.</span></span>  
4.  <span data-ttu-id="4bdf3-122">Migrate open fixed asset entries.</span><span class="sxs-lookup"><span data-stu-id="4bdf3-122">Migrate open fixed asset entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4bdf3-123">See Also</span><span class="sxs-lookup"><span data-stu-id="4bdf3-123">See Also</span></span>  
[<span data-ttu-id="4bdf3-124">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="4bdf3-124">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="4bdf3-125">Administration</span><span class="sxs-lookup"><span data-stu-id="4bdf3-125">Administration</span></span>](admin-setup-and-administration.md)
