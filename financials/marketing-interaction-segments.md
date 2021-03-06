---
title: Keep Track of Segments and Related Interactions| Microsoft Docs
description: Learn about creating segments to define groups of contacts and specifying interactions for segments.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.openlocfilehash: e561f981a5914c3a280c9d69f9d2c830268e69ed
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "245053"
---
# <a name="managing-interactions-for-segments"></a>Managing Interactions for Segments
The **Segment** window is a type of worksheet where you can:

* Create segments.
* Save the segmentation criteria you have used to select contacts.
* Log the segment and record interactions involving the contacts within the segment.

## <a name="segmenting"></a>Segmenting
There are several ways to create segments:

* You can manually enter the contacts you want to include in the segment in the segment lines.
* You can select contacts.
* You can reuse a logged segment as the basis to create a new one.
* You can reuse saved segmentation criteria.

## <a name="interactions"></a>Interactions
In the **Segment** window, you can create interactions for several contacts simultaneously. For example, you can merge a segment with a Microsoft Word document, so that you can send a letter to all the contacts in the segment.

You can specify information about the interaction for the segment on the **Segment** header. For example, you can decide which interaction template you want to use for all the contacts, specify a description, a correspondence type, and so on. However, you can modify this information in the segment line for each particular contact, for example, by specifying another description for one contact. If you are merging a segment with a Microsoft Word document, you can personalise the document to be sent for one or several of the contacts within the segment, for example, by adding individualised comments to the document.

## <a name="logging"></a>Logging
In the **Segment** window, when you choose **Log**, the application records the interactions in the **Interaction Log Entry** window, and logs the segment. After you have logged the segment, you can only find it in the **Logged Segments** window.

In the **Logged Segments** window, you can decide to create a follow-up segment containing the same contacts as the segment you have logged.

## <a name="see-also"></a>See Also
[Create Segments](marketing-how-create-segment.md)  
[Create Interactions for Segments](marketing-how-create-interactions.md)  
[Managing Segments](marketing-segments.md)  
[Recording Interactions With Contacts](marketing-interactions.md)  
[Managing Sales Opportunities](marketing-manage-sales-opportunities.md)  
[Creating and Managing Contacts](marketing-contacts.md)  
[Working with Financials](ui-work-product.md)
