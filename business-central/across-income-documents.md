---
title: Work with Incoming Documents| Microsoft Docs
description: You can manage incoming external business documents, such as payment receipts or PDFs, manage OCR tasks, and convert files to electronic documents and records.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 989fff07cb0608b8dbf6611a39163fc3cfe31459
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "229457"
---
# <a name="incoming-documents"></a><span data-ttu-id="4d5f6-103">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4d5f6-103">Incoming Documents</span></span>
<span data-ttu-id="4d5f6-104">Some business transactions are not recorded in [!INCLUDE[d365fin](includes/d365fin_md.md)] from the outset.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-104">Some business transactions are not recorded in [!INCLUDE[d365fin](includes/d365fin_md.md)] from the outset.</span></span> <span data-ttu-id="4d5f6-105">Instead, an external business document comes into your company as an email attachment or a paper copy that you scan to file.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-105">Instead, an external business document comes into your company as an email attachment or a paper copy that you scan to file.</span></span> <span data-ttu-id="4d5f6-106">This is typical of purchases, where such incoming document files represent payment receipts for expenses or small purchases.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-106">This is typical of purchases, where such incoming document files represent payment receipts for expenses or small purchases.</span></span>

<span data-ttu-id="4d5f6-107">From PDF or image files representing incoming documents, you can have an external OCR service (Optical Character Recognition) generate electronic documents that can then be converted to document records inside [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4d5f6-107">From PDF or image files representing incoming documents, you can have an external OCR service (Optical Character Recognition) generate electronic documents that can then be converted to document records inside [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="4d5f6-108">On the **Incoming Documents** page, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-108">On the **Incoming Documents** page, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="4d5f6-109">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-109">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="4d5f6-110">The incoming document process can consist of the following main activities:</span><span class="sxs-lookup"><span data-stu-id="4d5f6-110">The incoming document process can consist of the following main activities:</span></span>

* <span data-ttu-id="4d5f6-111">Record the external documents inside [!INCLUDE[d365fin](includes/d365fin_md.md)] by creating lines on the **Incoming Documents** page in either of the following ways:</span><span class="sxs-lookup"><span data-stu-id="4d5f6-111">Record the external documents inside [!INCLUDE[d365fin](includes/d365fin_md.md)] by creating lines on the **Incoming Documents** page in either of the following ways:</span></span>
  * <span data-ttu-id="4d5f6-112">Manually, by using simple functions, either from a PC or from a mobile device, in one of the following ways:</span><span class="sxs-lookup"><span data-stu-id="4d5f6-112">Manually, by using simple functions, either from a PC or from a mobile device, in one of the following ways:</span></span>
    * <span data-ttu-id="4d5f6-113">Use the **Create from File** button, and then fill relevant fields on the **Incoming Document** page.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-113">Use the **Create from File** button, and then fill relevant fields on the **Incoming Document** page.</span></span> <span data-ttu-id="4d5f6-114">The file is automatically attached.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-114">The file is automatically attached.</span></span>  
    * <span data-ttu-id="4d5f6-115">Use the **New** button, and then fill relevant fields on the **Incoming Document** page and manually attach the related file.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-115">Use the **New** button, and then fill relevant fields on the **Incoming Document** page and manually attach the related file.</span></span>
    * <span data-ttu-id="4d5f6-116">From a tablet or phone, use the **Create from Camera** button to create a new incoming document record, and then send the image to the OCR service, for example.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-116">From a tablet or phone, use the **Create from Camera** button to create a new incoming document record, and then send the image to the OCR service, for example.</span></span>
  * <span data-ttu-id="4d5f6-117">Automatically, by receiving the document from the OCR service as an electronic document after you have emailed the related PDF or image file to the OCR service.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-117">Automatically, by receiving the document from the OCR service as an electronic document after you have emailed the related PDF or image file to the OCR service.</span></span> <span data-ttu-id="4d5f6-118">The **Financial Information** FastTab is automatically filled on the **Incoming Document** page.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-118">The **Financial Information** FastTab is automatically filled on the **Incoming Document** page.</span></span>
* <span data-ttu-id="4d5f6-119">Use the OCR service to have PDF or image files turned into electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4d5f6-119">Use the OCR service to have PDF or image files turned into electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
* <span data-ttu-id="4d5f6-120">Create new documents or general journal lines for incoming document records by entering the information as you read it from incoming document files.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-120">Create new documents or general journal lines for incoming document records by entering the information as you read it from incoming document files.</span></span>
* <span data-ttu-id="4d5f6-121">Attach incoming document files to purchase and sales documents of any status, including to the vendor, customer, and general ledger entries that result from posting.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-121">Attach incoming document files to purchase and sales documents of any status, including to the vendor, customer, and general ledger entries that result from posting.</span></span>
* <span data-ttu-id="4d5f6-122">View incoming document records and their attachments from any purchase and sales document or entry, or find all general ledger entries without incoming document records from the **Chart of Accounts** page.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-122">View incoming document records and their attachments from any purchase and sales document or entry, or find all general ledger entries without incoming document records from the **Chart of Accounts** page.</span></span>

| <span data-ttu-id="4d5f6-123">To</span><span class="sxs-lookup"><span data-stu-id="4d5f6-123">To</span></span> | <span data-ttu-id="4d5f6-124">See</span><span class="sxs-lookup"><span data-stu-id="4d5f6-124">See</span></span> |
| --- | --- |
| <span data-ttu-id="4d5f6-125">Set up the Incoming Documents feature and set up the OCR service.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-125">Set up the Incoming Documents feature and set up the OCR service.</span></span> |[<span data-ttu-id="4d5f6-126">Set Up Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4d5f6-126">Set Up Incoming Documents</span></span>](across-how-setup-income-documents.md) |
| <span data-ttu-id="4d5f6-127">Create incoming document records, attach files, use OCR to turn PDF files into electronic documents, convert electronic documents to document records, audit incoming document records from posted sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="4d5f6-127">Create incoming document records, attach files, use OCR to turn PDF files into electronic documents, convert electronic documents to document records, audit incoming document records from posted sales and purchase documents.</span></span> |[<span data-ttu-id="4d5f6-128">Processing Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4d5f6-128">Processing Incoming Documents</span></span>](across-process-income-documents.md) |

## <a name="see-also"></a><span data-ttu-id="4d5f6-129">See Also</span><span class="sxs-lookup"><span data-stu-id="4d5f6-129">See Also</span></span>
[<span data-ttu-id="4d5f6-130">Purchasing</span><span class="sxs-lookup"><span data-stu-id="4d5f6-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="4d5f6-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4d5f6-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>