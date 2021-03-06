---
title: Overview of Tasks to Manage Payments to Vendors| Microsoft Docs
description: Outlines tasks to manage payments to vendors or creditors, including posting payment lines and getting an overview of the balance due.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, vendor payment, creditor, debt, balance due, AP
ms.date: 12/07/2018
ms.author: edupont
ms.openlocfilehash: a0e5e6eefd3c02236e9c512462350dc307b2ae97
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "234524"
---
# <a name="making-payments"></a>Making Payments

When you make payments to vendors or customers, or reimburse your employees, you post the related payment lines on the **Payment Journal** page. The payment journal is a general journal that is optimised for making payments and includes a number of powerful functions such as the **Suggest Vendor Payments** function that finds vendor payments that are due, and the **Vendor - Summary Ageing** report that shows an overview of due vendor payments.  

You can start the process of making the payment from the lists, cards, and ledger entries for vendors, customers, and employees. Each of these pages has a button that starts the payment flow and helps you fill in the payment journal.  

From the payment journal, you can print computer cheques or record when cheques are written. If you select **Computer Cheque** in the **Bank Payment Type** field, then any lines representing cheques must be printed before the payment journal can be posted.

When the payments are posted, you can export them to a bank file for upload to your bank for processing.

After the payments are made at your bank, you must apply them to their related open vendor or employee ledger entries. You can do this manually or by importing a bank statement file and applying the payments automatically. For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).

The following table describes a sequence of tasks, with links to the topics that describe them.

| To | See |
| --- | --- |
|Understand basic functions of the **Payment Journal** page, which is a based on the general journal, to prepare to post payments to vendors or employees.|[Working with General Journals](ui-work-general-journals.md)|
|Post payments to vendors or employees and refunds to customers, and optionally apply the payments to the related unpaid invoices/credit memos to close them as paid.|[Record Payments and Refunds](payables-how-post-payments-refunds.md)|
| Use a function on the **Payment Journal** page to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity. |[Suggest Vendor Payments](payables-how-suggest-vendor-payments.md) |
| Issue cheques for vendor payments or customer refunds, either as print-outs or as computer cheques. Void cheques before or after posting. |[Make Cheque Payments](payables-how-work-checks.md) |
|Make electronic payments by exporting payments to a bank file that you upload to your bank for processing, including EFT (electronic funds transfer) in North America. |[Make Electronic Payments](payables-how-export-payments-bank-file.md)|
|Make electronic payments according to the EU SEPA Credit Transfer standard.|[Making Payments with Bank Data Conversion Service or SEPA Credit Transfer](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)|
| Pay a vendor by cash or cheque, and post the payment when you post the invoice. |[Settle Purchase Invoices Promptly](finance-how-to-settle-purchase-invoices-promptly.md) |
|Reimburse employees for personal expenses during business activities by making payment to their bank account.|[Record and Reimburse Employees' Expenses](finance-how-record-reimburse-employee-expenses.md)|
| Make sure that your bank only clears validated cheques and amounts by sending them a file that contains vendor, cheque, and payment information. |[Export a Positive Pay file](finance-how-positive-pay.md) |

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Managing Receivables](receivables-manage-receivables.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
