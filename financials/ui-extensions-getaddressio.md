---
title: Using the GetAddress.io UK Postcodes Extension | Microsoft Docs
description: Retrieve addresses for entities like customers, vendors, employees, and banks in the United Kingdom from the GetAddress.io service.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-financials
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: GetAddress.io, postcodes, postal, address, extension
ms.date: 04/20/2017
ms.author: bholtorf
ms.openlocfilehash: e7a6f4a9fad61214e1cf6778c8d810066843c5a6
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "271054"
---
# <a name="the-getaddressio-uk-postcodes-extension-to-microsoft-business-central"></a>The GetAddress.io UK Postcodes Extension to Microsoft Business Central 
The GetAddress.io UK Postcodes extension can save time and prevent mistakes when you enter addresses for entities like customers, vendors, bank accounts, and employees. For example, when you're creating a customer, you just choose a postcode and [!INCLUDE [d365fin](includes/d365fin_md.md)] shows a list of addresses. Pick the address you want, and presto, the address fields are filled out.  

## <a name="to-use-the-getaddressio-uk-postcodes-extension-when-you-enter-an-address"></a>To use the GetAddress.io UK Postcodes extension when you enter an address
1. Under **Address**, choose **Look up address from postcode**.  

    > [!NOTE]  
   >   The **Look up address from postcode** option is available only if the **Country/Region Code** field is either empty, or contains **GB**.
2. In the **Postcode Search** window, in the **Postcode** field, enter or choose the postcode.  
3. In the **Address Selection** window, choose the address.  

> [!TIP]  
>   If you know the street number, you can filter the addresses by entering some or all of the number in the **Delivery Point** field.


## <a name="see-also"></a>See Also
[Set up the GetAddress.io UK Postal Code extension](LocalFunctionality/UnitedKingdom/uk-setup-postal-code-service.md)
