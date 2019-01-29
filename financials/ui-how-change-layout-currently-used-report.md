---
title: Change the Way a Report Looks by Selecting a Different Layout | Microsoft Docs
description: You can use different layouts for a report, and switch between layouts to change how a report looks.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 03/29/2017
ms.author: jswymer
ms.openlocfilehash: 8e1daaa77eaaf14348904c7ae013eb25bbec95ce
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "270541"
---
# <a name="change-which-layout-is-currently-used-on-a-report"></a><span data-ttu-id="64ab5-103">Change Which Layout is Currently Used on a Report</span><span class="sxs-lookup"><span data-stu-id="64ab5-103">Change Which Layout is Currently Used on a Report</span></span>
<span data-ttu-id="64ab5-104">A report can be set up with more than one report layout, which you can then switch among as needed.</span><span class="sxs-lookup"><span data-stu-id="64ab5-104">A report can be set up with more than one report layout, which you can then switch among as needed.</span></span>

<span data-ttu-id="64ab5-105">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span><span class="sxs-lookup"><span data-stu-id="64ab5-105">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span></span> <span data-ttu-id="64ab5-106">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="64ab5-106">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span></span>

## <a name="to-change-the-layout-that-is-used-on-a-report"></a><span data-ttu-id="64ab5-107">To change the layout that is used on a report</span><span class="sxs-lookup"><span data-stu-id="64ab5-107">To change the layout that is used on a report</span></span>
1. <span data-ttu-id="64ab5-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Layout Selection**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="64ab5-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Layout Selection**, and then choose the related link.</span></span>  
   <span data-ttu-id="64ab5-109">The **Report Layout Selection** window lists all the reports that are available for the company that is specified in the Company field at the top of the window.</span><span class="sxs-lookup"><span data-stu-id="64ab5-109">The **Report Layout Selection** window lists all the reports that are available for the company that is specified in the Company field at the top of the window.</span></span> <span data-ttu-id="64ab5-110">The Selected Layout field specifies the layout that is currently used on the report.</span><span class="sxs-lookup"><span data-stu-id="64ab5-110">The Selected Layout field specifies the layout that is currently used on the report.</span></span>
2. <span data-ttu-id="64ab5-111">Set the **Company** field at the top of the window to the company that includes the report.</span><span class="sxs-lookup"><span data-stu-id="64ab5-111">Set the **Company** field at the top of the window to the company that includes the report.</span></span>
3. <span data-ttu-id="64ab5-112">To change the layout that is used by a report, in the row for the report in the list, set the **Selected Layout** field to one of the following options:</span><span class="sxs-lookup"><span data-stu-id="64ab5-112">To change the layout that is used by a report, in the row for the report in the list, set the **Selected Layout** field to one of the following options:</span></span>
   * <span data-ttu-id="64ab5-113">RDLC (built-in), uses the built-in RDLC report layout on the report.</span><span class="sxs-lookup"><span data-stu-id="64ab5-113">RDLC (built-in), uses the built-in RDLC report layout on the report.</span></span>
   * <span data-ttu-id="64ab5-114">Word (built-in), uses the built-in Word report layout on the report.</span><span class="sxs-lookup"><span data-stu-id="64ab5-114">Word (built-in), uses the built-in Word report layout on the report.</span></span>
   * <span data-ttu-id="64ab5-115">Custom, uses a custom layout on the report.</span><span class="sxs-lookup"><span data-stu-id="64ab5-115">Custom, uses a custom layout on the report.</span></span>  
     <span data-ttu-id="64ab5-116">You can see which custom layouts are available for the report in the Report Layouts Part FactBox.</span><span class="sxs-lookup"><span data-stu-id="64ab5-116">You can see which custom layouts are available for the report in the Report Layouts Part FactBox.</span></span> <span data-ttu-id="64ab5-117">If there are no custom layouts for the report, then you will have to create one first.</span><span class="sxs-lookup"><span data-stu-id="64ab5-117">If there are no custom layouts for the report, then you will have to create one first.</span></span> <span data-ttu-id="64ab5-118">If you choose this option, go to the next procedure to specify the custom layout that you want to use.</span><span class="sxs-lookup"><span data-stu-id="64ab5-118">If you choose this option, go to the next procedure to specify the custom layout that you want to use.</span></span>

     > [!NOTE]  
     >   <span data-ttu-id="64ab5-119">If you choose **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span><span class="sxs-lookup"><span data-stu-id="64ab5-119">If you choose **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span></span>

<span data-ttu-id="64ab5-120">If you selected a built-in RDLC or Word report layout, then no further action is required and the layout will be used the next time the report is run.</span><span class="sxs-lookup"><span data-stu-id="64ab5-120">If you selected a built-in RDLC or Word report layout, then no further action is required and the layout will be used the next time the report is run.</span></span>

## <a name="to-specify-a-custom-layout-on-a-report"></a><span data-ttu-id="64ab5-121">To specify a custom layout on a report</span><span class="sxs-lookup"><span data-stu-id="64ab5-121">To specify a custom layout on a report</span></span>
1. <span data-ttu-id="64ab5-122">You specify which custom layout to use on the report from the **Custom Report Layouts** window.</span><span class="sxs-lookup"><span data-stu-id="64ab5-122">You specify which custom layout to use on the report from the **Custom Report Layouts** window.</span></span> <span data-ttu-id="64ab5-123">If the **Custom Report Layouts** window is not open, then in the **Report Layout Description** field, choose the lookup button.</span><span class="sxs-lookup"><span data-stu-id="64ab5-123">If the **Custom Report Layouts** window is not open, then in the **Report Layout Description** field, choose the lookup button.</span></span>
2. <span data-ttu-id="64ab5-124">In the **Custom Report Layouts** window, select the row for custom layout that you want to use, and then close the window.</span><span class="sxs-lookup"><span data-stu-id="64ab5-124">In the **Custom Report Layouts** window, select the row for custom layout that you want to use, and then close the window.</span></span>

<span data-ttu-id="64ab5-125">You return to the **Report Layout Selection** window.</span><span class="sxs-lookup"><span data-stu-id="64ab5-125">You return to the **Report Layout Selection** window.</span></span> <span data-ttu-id="64ab5-126">The name of the selected custom layout displays in the **Custom Layout Description** field.</span><span class="sxs-lookup"><span data-stu-id="64ab5-126">The name of the selected custom layout displays in the **Custom Layout Description** field.</span></span> <span data-ttu-id="64ab5-127">The custom layout will be used the next time that you run the report.</span><span class="sxs-lookup"><span data-stu-id="64ab5-127">The custom layout will be used the next time that you run the report.</span></span>

## <a name="see-also"></a><span data-ttu-id="64ab5-128">See Also</span><span class="sxs-lookup"><span data-stu-id="64ab5-128">See Also</span></span>
[<span data-ttu-id="64ab5-129">Managing Report Layouts</span><span class="sxs-lookup"><span data-stu-id="64ab5-129">Managing Report Layouts</span></span>](ui-manage-report-layouts.md)  
<span data-ttu-id="64ab5-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="64ab5-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>