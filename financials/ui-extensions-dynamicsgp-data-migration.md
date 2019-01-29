---
title: Migrate Data from Dynamics GP with the Data Migration Extension | Microsoft Docs
description: Use the Dynamics GP Data Migration extension to migrate customers, vendors, inventory items, and accounts from Dynamics GP to Business Central.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.openlocfilehash: 06bbd41ab729e9d5ae955dfa12910c006668c4c2
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "236331"
---
# <a name="the-dynamics-gp-data-migration-extension-for-finance-and-operations-business-edition"></a><span data-ttu-id="5617a-103">The Dynamics GP Data Migration Extension for Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="5617a-103">The Dynamics GP Data Migration Extension for Finance and Operations, Business edition</span></span>
<span data-ttu-id="5617a-104">This extension makes it easy to migrate customers, vendors, inventory items, and accounts from Dynamics GP to [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5617a-104">This extension makes it easy to migrate customers, vendors, inventory items, and accounts from Dynamics GP to [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="5617a-105">If your business uses Dynamics GP today, you can export the relevant master records and then open an assisted setup guide to add the data to [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5617a-105">If your business uses Dynamics GP today, you can export the relevant master records and then open an assisted setup guide to add the data to [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="5617a-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="5617a-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span></span>

## <a name="exporting-data-from-dynamics-gp"></a><span data-ttu-id="5617a-107">Exporting Data from Dynamics GP</span><span class="sxs-lookup"><span data-stu-id="5617a-107">Exporting Data from Dynamics GP</span></span>
<span data-ttu-id="5617a-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to a file, using the Dynamics GP functionality for data export.</span><span class="sxs-lookup"><span data-stu-id="5617a-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to a file, using the Dynamics GP functionality for data export.</span></span> <span data-ttu-id="5617a-109">For the purposes of [!INCLUDE [d365fin](includes/d365fin_md.md)], you can export the following types of data:</span><span class="sxs-lookup"><span data-stu-id="5617a-109">For the purposes of [!INCLUDE [d365fin](includes/d365fin_md.md)], you can export the following types of data:</span></span>

* <span data-ttu-id="5617a-110">Account</span><span class="sxs-lookup"><span data-stu-id="5617a-110">Account</span></span>  
* <span data-ttu-id="5617a-111">Customer</span><span class="sxs-lookup"><span data-stu-id="5617a-111">Customer</span></span>  
* <span data-ttu-id="5617a-112">Item</span><span class="sxs-lookup"><span data-stu-id="5617a-112">Item</span></span>  
* <span data-ttu-id="5617a-113">Vendor</span><span class="sxs-lookup"><span data-stu-id="5617a-113">Vendor</span></span>  

<span data-ttu-id="5617a-114">The Dynamics GP Data Migration extension automatically maps the exported data so that your data is quickly available to you in your new [!INCLUDE [d365fin](includes/d365fin_md.md)] company.</span><span class="sxs-lookup"><span data-stu-id="5617a-114">The Dynamics GP Data Migration extension automatically maps the exported data so that your data is quickly available to you in your new [!INCLUDE [d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="5617a-115">During the process, supporting setup information is created, such as posting groups.</span><span class="sxs-lookup"><span data-stu-id="5617a-115">During the process, supporting setup information is created, such as posting groups.</span></span> <span data-ttu-id="5617a-116">Inventory items will be brought into the system with FIFO as the cost valuation method.</span><span class="sxs-lookup"><span data-stu-id="5617a-116">Inventory items will be brought into the system with FIFO as the cost valuation method.</span></span> <span data-ttu-id="5617a-117">Accounts will be set up as the main account segment from Dynamics GP with dimensions, because [!INCLUDE [d365fin](includes/d365fin_long_md.md)] does not have account segments.</span><span class="sxs-lookup"><span data-stu-id="5617a-117">Accounts will be set up as the main account segment from Dynamics GP with dimensions, because [!INCLUDE [d365fin](includes/d365fin_long_md.md)] does not have account segments.</span></span>

## <a name="see-also"></a><span data-ttu-id="5617a-118">See Also</span><span class="sxs-lookup"><span data-stu-id="5617a-118">See Also</span></span>
[<span data-ttu-id="5617a-119">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="5617a-119">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="5617a-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="5617a-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  
