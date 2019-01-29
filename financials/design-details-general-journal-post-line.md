---
title: Design Details - General Journal Post Line | Microsoft Docs
description: This topic provides insight into the concepts and principles that are used to redesign the general journal posting line feature in Business Central.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 5e2d2c86b3662e11369ef2b0bb20b02541f51b6d
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "260414"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="b9bbc-103">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="b9bbc-103">Design Details: General Journal Post Line</span></span>
<span data-ttu-id="b9bbc-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b9bbc-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b9bbc-105">The redesign makes codeunit 12 simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="b9bbc-105">The redesign makes codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="b9bbc-106">The documentation starts by describing conceptual overviews of the redesign.</span><span class="sxs-lookup"><span data-stu-id="b9bbc-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="b9bbc-107">Then it explains the technical architecture to show the changes that result from the redesign.</span><span class="sxs-lookup"><span data-stu-id="b9bbc-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="b9bbc-108">In This Section</span><span class="sxs-lookup"><span data-stu-id="b9bbc-108">In This Section</span></span>  
[<span data-ttu-id="b9bbc-109">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="b9bbc-109">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="b9bbc-110">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="b9bbc-110">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="b9bbc-111">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="b9bbc-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="b9bbc-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="b9bbc-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>](design-details-codeunit-12-changes-mapping-global-variables-for-general-journal-post-line.md)  
[<span data-ttu-id="b9bbc-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span><span class="sxs-lookup"><span data-stu-id="b9bbc-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)  

## <a name="see-also"></a><span data-ttu-id="b9bbc-114">See Also</span><span class="sxs-lookup"><span data-stu-id="b9bbc-114">See Also</span></span>  
[<span data-ttu-id="b9bbc-115">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="b9bbc-115">Working with General Journals</span></span>](ui-work-general-journals.md)
