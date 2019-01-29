---
title: Setting Up the Chart of Accounts| Microsoft Docs
description: You change the default accounts in the chart of accounts (COA), and you can add new accounts.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 06/02/2017
ms.author: edupont
ms.openlocfilehash: 628a1b7c3c558b6990197682d830f9fa4d0ca9bf
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "227863"
---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a><span data-ttu-id="5bb7e-103">Setting Up or Changing the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="5bb7e-103">Setting Up or Changing the Chart of Accounts</span></span>
<span data-ttu-id="5bb7e-104">The chart of accounts shows the ledger accounts that store your financial data.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-104">The chart of accounts shows the ledger accounts that store your financial data.</span></span> <span data-ttu-id="5bb7e-105">[!INCLUDE [d365fin](includes/d365fin_md.md)] includes a standard chart of accounts that is ready to support your business.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-105">[!INCLUDE [d365fin](includes/d365fin_md.md)] includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="5bb7e-106">However, you can change the default accounts, and you can add new accounts.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-106">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="5bb7e-107">Adding or Changing Accounts</span><span class="sxs-lookup"><span data-stu-id="5bb7e-107">Adding or Changing Accounts</span></span>
<span data-ttu-id="5bb7e-108">From the chart of accounts, you can open each G/L account and add or change settings.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-108">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

> [!NOTE]  
>   <span data-ttu-id="5bb7e-109">You can delete a general ledger account.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-109">You can delete a general ledger account.</span></span> <span data-ttu-id="5bb7e-110">However, before you delete it, the following must be true:</span><span class="sxs-lookup"><span data-stu-id="5bb7e-110">However, before you delete it, the following must be true:</span></span>  

* <span data-ttu-id="5bb7e-111">The balance on the account must be zero.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-111">The balance on the account must be zero.</span></span>  
* <span data-ttu-id="5bb7e-112">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-112">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
* <span data-ttu-id="5bb7e-113">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-113">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

<span data-ttu-id="5bb7e-114">[!INCLUDE [d365fin](includes/d365fin_md.md)] will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="5bb7e-114">[!INCLUDE [d365fin](includes/d365fin_md.md)] will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5bb7e-115">See Also</span><span class="sxs-lookup"><span data-stu-id="5bb7e-115">See Also</span></span>
[<span data-ttu-id="5bb7e-116">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="5bb7e-116">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
[<span data-ttu-id="5bb7e-117">Managing Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="5bb7e-117">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="5bb7e-118">Working with Dimensions</span><span class="sxs-lookup"><span data-stu-id="5bb7e-118">Working with Dimensions</span></span>](finance-dimensions.md)  
<span data-ttu-id="5bb7e-119">[Importing Data from Other Finance Systems](across-import-data-configuration-packages.md)(across-import-data-configuration-packages.md)</span><span class="sxs-lookup"><span data-stu-id="5bb7e-119">[Importing Data from Other Finance Systems](across-import-data-configuration-packages.md)(across-import-data-configuration-packages.md)</span></span>  
<span data-ttu-id="5bb7e-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5bb7e-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE [d365fin](includes/free_trial_md.md)]
