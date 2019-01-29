---
title: Track User Activity in a Change Log| Microsoft Docs
description: You can activate a user log so that you have a history of any changes made to data in tracked tables.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 11/14/2018
ms.author: edupont
ms.openlocfilehash: bc56e07a540c24f53b88651ad2b2ff5e1e56a571
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "244695"
---
# <a name="auditing-changes-in-business-central"></a><span data-ttu-id="bfdf5-103">Auditing Changes in Business Central</span><span class="sxs-lookup"><span data-stu-id="bfdf5-103">Auditing Changes in Business Central</span></span>

<span data-ttu-id="bfdf5-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="bfdf5-105">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-105">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="bfdf5-106">The change log collects all changes that are made to the table.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-106">The change log collects all changes that are made to the table.</span></span>

> [!Important]
> <span data-ttu-id="bfdf5-107">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span><span class="sxs-lookup"><span data-stu-id="bfdf5-107">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span></span>
<br />
> * <span data-ttu-id="bfdf5-108">The session expired and was refreshed.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-108">The session expired and was refreshed.</span></span>
> * <span data-ttu-id="bfdf5-109">The user selected another company or Role Centre.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-109">The user selected another company or Role Center.</span></span>
> * <span data-ttu-id="bfdf5-110">The user signed out and back in.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-110">The user signed out and back in.</span></span>

## <a name="working-with-the-change-log"></a><span data-ttu-id="bfdf5-111">Working with the Change Log</span><span class="sxs-lookup"><span data-stu-id="bfdf5-111">Working with the Change Log</span></span>

<span data-ttu-id="bfdf5-112">A common problem in many financial systems is to locate the origin of errors and changes in data.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-112">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="bfdf5-113">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-113">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="bfdf5-114">The change log lets you track all direct modifications a user makes to data in the database.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-114">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="bfdf5-115">You must specify each table and field that you want the system to log, and then you must activate the change log.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-115">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="bfdf5-116">You activate and deactivate the change log on the **Change Log Setup** page.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-116">You activate and deactivate the change log on the **Change Log Setup** page.</span></span> <span data-ttu-id="bfdf5-117">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-117">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span>

<span data-ttu-id="bfdf5-118">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-118">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="bfdf5-119">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-119">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span></span> <span data-ttu-id="bfdf5-120">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span><span class="sxs-lookup"><span data-stu-id="bfdf5-120">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bfdf5-121">See Also</span><span class="sxs-lookup"><span data-stu-id="bfdf5-121">See Also</span></span>
[<span data-ttu-id="bfdf5-122">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="bfdf5-122">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="bfdf5-123">Sorting</span><span class="sxs-lookup"><span data-stu-id="bfdf5-123">Sorting</span></span>](ui-sorting.md)  
[<span data-ttu-id="bfdf5-124">Using Search for Page or Report</span><span class="sxs-lookup"><span data-stu-id="bfdf5-124">Using Search for Page or Report</span></span>](ui-search.md)  
<span data-ttu-id="bfdf5-125">[Managing Users and Permissions](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="bfdf5-125">[Managing Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="bfdf5-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bfdf5-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  