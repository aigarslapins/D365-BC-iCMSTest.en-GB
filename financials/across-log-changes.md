---
title: Track User Activity in a Change Log| Microsoft Docs
Description: You can activate a user log so that you have a history of any changes made to data in tracked tables.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-financials
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 06/02/2017
ms.author: edupont
ms.openlocfilehash: b4231b19bc79233eb88b4f16fc5cd8bd4fb5e29c
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "240491"
---
# <a name="logging-changes-in-business-central"></a><span data-ttu-id="fa5c4-102">Logging Changes in Business Central</span><span class="sxs-lookup"><span data-stu-id="fa5c4-102">Logging Changes in Business Central</span></span> 
<span data-ttu-id="fa5c4-103">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-103">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="fa5c4-104">The log is based on changes that are made to data in the tables that you track. In the change log, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-104">The log is based on changes that are made to data in the tables that you track. In the change log, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="fa5c4-105">The change log collects all changes that are made to the table.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-105">The change log collects all changes that are made to the table.</span></span>  

## <a name="working-with-the-change-log"></a><span data-ttu-id="fa5c4-106">Working with the Change Log</span><span class="sxs-lookup"><span data-stu-id="fa5c4-106">Working with the Change Log</span></span>
<span data-ttu-id="fa5c4-107">A common problem in many financial systems is to locate the origin of errors and changes in data.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-107">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="fa5c4-108">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-108">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="fa5c4-109">The change log lets you track all direct modifications a user makes to data in the database.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-109">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="fa5c4-110">You must specify each table and field that you want the system to log, and then you must activate the change log.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-110">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="fa5c4-111">You activate and deactivate the change log in the **Change Log Setup** window.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-111">You activate and deactivate the change log in the **Change Log Setup** window.</span></span> <span data-ttu-id="fa5c4-112">When you activate or deactivate the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-112">When you activate or deactivate the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span> <span data-ttu-id="fa5c4-113">This cannot be turned off.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-113">This cannot be turned off.</span></span>  

<span data-ttu-id="fa5c4-114">In the **Change Log Setup** window, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE [d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-114">In the **Change Log Setup** window, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE [d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="fa5c4-115">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes in the **Change Log Entries** window.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-115">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes in the **Change Log Entries** window.</span></span> <span data-ttu-id="fa5c4-116">If you want to delete entries, you can do that in the **Delete Change Log Entries** window, where you can set filters based on dates and time.</span><span class="sxs-lookup"><span data-stu-id="fa5c4-116">If you want to delete entries, you can do that in the **Delete Change Log Entries** window, where you can set filters based on dates and time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fa5c4-117">See Also</span><span class="sxs-lookup"><span data-stu-id="fa5c4-117">See Also</span></span>
[<span data-ttu-id="fa5c4-118">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="fa5c4-118">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="fa5c4-119">Sorting</span><span class="sxs-lookup"><span data-stu-id="fa5c4-119">Sorting</span></span>](ui-sorting.md)  
[<span data-ttu-id="fa5c4-120">Using Search for Page or Report</span><span class="sxs-lookup"><span data-stu-id="fa5c4-120">Using Search for Page or Report</span></span>](ui-search.md)  
<span data-ttu-id="fa5c4-121">[Manage Users and Permissions](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="fa5c4-121">[Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="fa5c4-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fa5c4-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  