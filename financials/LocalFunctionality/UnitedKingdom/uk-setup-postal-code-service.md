---
title: Set Up the GetAddress.io UK Postcodes Extension | Microsoft Docs
description: Describes the general functionality you use to interact with data in Business Central, such as entering values, sorting data, and changing views.
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: getaddress.io, postcodes, extension
ms.date: 03/05/2018
ms.author: bholtorf
ms.openlocfilehash: f4620f6a23d508127fdf3352e2a5b70b1b48b102
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "223219"
---
# <a name="set-up-the-getaddressio-uk-postcodes-extension"></a>Set Up the GetAddress.io UK Postcodes Extension
This extension makes it easy to enter addresses in the United Kingdom (UK) for entities like customers, contacts, employees, vendors, bank accounts, and so on.

The GetAddress.io UK Postcodes extension uses the getAddress API to find addresses in postcodes in the UK. To use the extension, you need to get a plan and an API Key for the getAddress API. We help you do that when you set up the GetAddress.io UK Postcodes extension. Plans are based on use, or what are sometimes referred to as "calls." A call, in this case, is when [!INCLUDE [d365fin](../../includes/d365fin_md.md)] displays a list of addresses in a postcode. Depending on how often you add addresses, choose the plan that is best for you. If you just choose **Get API Key** you will use the **Free** plan, which lets you add 20 addresses per day, and is valid for 30 days.

## <a name="to-set-up-the-getaddressio-uk-postcodes-extension"></a>To set up the GetAddress.io UK Postcodes extension
1. Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Connections**, and then choose the related link.  
2. In the **Service Connections** window, choose **UK Postcode Service**.
3. In the **Postcode provider configuration** page, choose **Disabled**.
4. In the **Postal code service selection** window, choose **GetAddress.io**.
5. In the **GetAddress.io Config** window, choose **Get API Key** to open the **Plans** page on the website for the getAddress API.  

    > [!NOTE]  
   >   You might need to allow pop-ups in your browser.

6. Purchase a plan, or just choose **Get API Key**, and then provide your email address.
7. Open the email from getAddress.io, and copy the API key. The key is under the **Your API Key** heading.
8. In the **GetAddress.io Config** window, paste the API key in the **API Key** field, and then choose **OK**.
9. In the **Service Connections** page, verify that the **Address Provider** field shows **GetAddress.io**. If it does, the service is enabled.

## <a name="see-also"></a>See Also
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)  
[GetAddress.io UK Postcodes](../../ui-extensions-getaddressio.md)  
[Customising [!INCLUDE[d365fin](../../includes/d365fin_md.md)] Using Extensions](../../ui-extensions.md)  
[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)  
