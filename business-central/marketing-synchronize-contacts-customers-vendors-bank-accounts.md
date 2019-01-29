---
title: Synchronise Contacts With Customers and Vendors| Microsoft Docs
description: You couple or synchronise contact information of contacts who are also customers, vendors, or bank accounts, so you only update information in one place.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, CRM, integration, couple
ms.date: 10/01/2018
ms.author: edupont
redirect_url: marketing-create-contact-companies
ms.openlocfilehash: 736d1329b3d3c2e9367972c2a2fb9e2af0080c85
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "262994"
---
# <a name="synchronizing-contacts-with-customers-vendors-and-bank-accounts"></a><span data-ttu-id="2bebc-103">Synchronising Contacts With Customers, Vendors, and Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="2bebc-103">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>
<span data-ttu-id="2bebc-104">If some of your contacts are also customers, vendors, or bank accounts, you can synchronise the contact information with the related customer, vendor, or bank account.</span><span class="sxs-lookup"><span data-stu-id="2bebc-104">If some of your contacts are also customers, vendors, or bank accounts, you can synchronize the contact information with the related customer, vendor, or bank account.</span></span> <span data-ttu-id="2bebc-105">Synchronisation makes information that is common between contacts and customers, vendors, or bank account the same.</span><span class="sxs-lookup"><span data-stu-id="2bebc-105">Synchronization makes information that is common between contacts and customers, vendors, or bank account the same.</span></span>  

<span data-ttu-id="2bebc-106">Before you can synchronise your contacts with customers, vendors, or bank accounts, you must specify a business relation code for customers, vendors, and bank accounts on the **Marketing Setup** page.</span><span class="sxs-lookup"><span data-stu-id="2bebc-106">Before you can synchronize your contacts with customers, vendors, or bank accounts, you must specify a business relation code for customers, vendors, and bank accounts on the **Marketing Setup** page.</span></span> <span data-ttu-id="2bebc-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span><span class="sxs-lookup"><span data-stu-id="2bebc-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span></span>

## <a name="different-ways-to-synchronize-contacts-with-customers-vendors-and-bank-accounts"></a><span data-ttu-id="2bebc-108">Different Ways to Synchronise Contacts with Customers, Vendors and Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="2bebc-108">Different Ways to Synchronize Contacts with Customers, Vendors and Bank Accounts</span></span>
<span data-ttu-id="2bebc-109">You can synchronise your contacts with customers, vendors, or bank accounts by three methods:</span><span class="sxs-lookup"><span data-stu-id="2bebc-109">You can synchronize your contacts with customers, vendors, or bank accounts by three methods:</span></span>

* <span data-ttu-id="2bebc-110">Link contacts with existing customers, vendors, or bank accounts from the contact card.</span><span class="sxs-lookup"><span data-stu-id="2bebc-110">Link contacts with existing customers, vendors, or bank accounts from the contact card.</span></span> <span data-ttu-id="2bebc-111">For more information, see [Link Contacts With Customers, Vendors, and Bank Accounts](marketing-how-link-contact.md).</span><span class="sxs-lookup"><span data-stu-id="2bebc-111">For more information, see [Link Contacts With Customers, Vendors, and Bank Accounts](marketing-how-link-contact.md).</span></span>
* <span data-ttu-id="2bebc-112">Create customers, vendors, or bank accounts from the contact.</span><span class="sxs-lookup"><span data-stu-id="2bebc-112">Create customers, vendors, or bank accounts from the contact.</span></span> <span data-ttu-id="2bebc-113">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="2bebc-113">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>
* <span data-ttu-id="2bebc-114">Create contacts from customers, vendors or bank accounts.</span><span class="sxs-lookup"><span data-stu-id="2bebc-114">Create contacts from customers, vendors or bank accounts.</span></span> <span data-ttu-id="2bebc-115">For more information, see [Create a company contact from a customer, vendor, or bank account](marketing-how-create-contact-companies.md).</span><span class="sxs-lookup"><span data-stu-id="2bebc-115">For more information, see [Create a company contact from a customer, vendor, or bank account](marketing-how-create-contact-companies.md).</span></span>

## <a name="consequences-of-synchronization"></a><span data-ttu-id="2bebc-116">Consequences of Synchronisation</span><span class="sxs-lookup"><span data-stu-id="2bebc-116">Consequences of Synchronization</span></span>
<span data-ttu-id="2bebc-117">When the contact is synchronised with the customer, vendor, bank account:</span><span class="sxs-lookup"><span data-stu-id="2bebc-117">When the contact is synchronized with the customer, vendor, bank account:</span></span>

* <span data-ttu-id="2bebc-118">You only have to update information in one place.</span><span class="sxs-lookup"><span data-stu-id="2bebc-118">You only have to update information in one place.</span></span> <span data-ttu-id="2bebc-119">For example, if you modify the phone number on the contact, the phone number is automatically updated with the same modification on the customer, the vendor, or the bank account.</span><span class="sxs-lookup"><span data-stu-id="2bebc-119">For example, if you modify the phone number on the contact, the phone number is automatically updated with the same modification on the customer, the vendor, or the bank account.</span></span>
* <span data-ttu-id="2bebc-120">If you have specified a number series for contacts, when you create a customer card, a vendor card, or a bank account card, a contact card is automatically created for the customer, vendor or bank account.</span><span class="sxs-lookup"><span data-stu-id="2bebc-120">If you have specified a number series for contacts, when you create a customer card, a vendor card, or a bank account card, a contact card is automatically created for the customer, vendor or bank account.</span></span>
* <span data-ttu-id="2bebc-121">You can create sales quotes and orders, and purchase quotes and orders from the contact.</span><span class="sxs-lookup"><span data-stu-id="2bebc-121">You can create sales quotes and orders, and purchase quotes and orders from the contact.</span></span>
* <span data-ttu-id="2bebc-122">You can have your interactions recorded when you perform actions such as printing orders, blanket orders, creating sales service orders, sending e-mails, and so on.</span><span class="sxs-lookup"><span data-stu-id="2bebc-122">You can have your interactions recorded when you perform actions such as printing orders, blanket orders, creating sales service orders, sending e-mails, and so on.</span></span>
* <span data-ttu-id="2bebc-123">If you delete a contact linked to a customer, vendor or bank account, only the contact is removed.</span><span class="sxs-lookup"><span data-stu-id="2bebc-123">If you delete a contact linked to a customer, vendor or bank account, only the contact is removed.</span></span> <span data-ttu-id="2bebc-124">The customer, vendor, or bank account remains.</span><span class="sxs-lookup"><span data-stu-id="2bebc-124">The customer, vendor, or bank account remains.</span></span>
* <span data-ttu-id="2bebc-125">If you delete a customer, vendor, bank account linked to a contact, the contact remains.</span><span class="sxs-lookup"><span data-stu-id="2bebc-125">If you delete a customer, vendor, bank account linked to a contact, the contact remains.</span></span>

> [!NOTE]  
>   <span data-ttu-id="2bebc-126">Some details, such as invoicing and posting details, do not appear on the contact card.</span><span class="sxs-lookup"><span data-stu-id="2bebc-126">Some details, such as invoicing and posting details, do not appear on the contact card.</span></span> <span data-ttu-id="2bebc-127">Therefore, you may want to add them manually on the customer card, vendor card, or bank account card when you create contacts as customers, vendors or bank accounts.</span><span class="sxs-lookup"><span data-stu-id="2bebc-127">Therefore, you may want to add them manually on the customer card, vendor card, or bank account card when you create contacts as customers, vendors or bank accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="2bebc-128">See Also</span><span class="sxs-lookup"><span data-stu-id="2bebc-128">See Also</span></span>
[<span data-ttu-id="2bebc-129">Managing Contacts</span><span class="sxs-lookup"><span data-stu-id="2bebc-129">Managing Contacts</span></span>](marketing-contacts.md)  
<span data-ttu-id="2bebc-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2bebc-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>