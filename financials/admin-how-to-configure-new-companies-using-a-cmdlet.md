---
title: How to Configure New Companies using a Cmdlet | Microsoft Docs
description: In a number of scenarios, you may want to load and import a configuration package without involving your users or using the RapidStart Services user interface. You can do so by using a Windows PowerShell cmdlet.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 03/06/2018
ms.author: sgroespe
ms.openlocfilehash: d57990378992494aa48733ecea6a0a3657a2d5f5
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "223468"
---
# <a name="configure-new-companies-using-a-cmdlet"></a>Configure New Companies using a Cmdlet
In a number of scenarios, you may want to load and import a configuration package without involving your users or using the RapidStart Services user interface. You can do so by using a Windows PowerShell cmdlet. Scenarios where this may be useful include:  

- Performing data import across multiple [!INCLUDE [d365fin](includes/d365fin_md.md)] installations.
- Configuring additional application areas for multiple customers.  

## <a name="to-deploy-a-configuration-package-using-a-cmdlet"></a>To deploy a configuration package using a cmdlet  

1. Prepare a RapidStart Services package. For example, you can create a package to import certain values and the names of the table and the fields to insert these values into.  
2. Place the package on a computer where you will run the cmdlet.  
3. Open the [!INCLUDE [d365fin](includes/d365fin_md.md)] administration shell.  
4. Enter **Invoke-NAVCodeUnit**, and specify information similar to the following example.  
    ```  
    Invoke-NAVCodeunit -Tenant Default -CompanyName "CRONUS International Ltd." -CodeunitId 8620 -MethodName ImportRapidStartPackage -Argument "C:TEMPRS_CONFIG.rapidstart" -ServerInstance DynamicsNAV71  

    ```
   The cmdlet imports the package into each company. Users can start to use the new functionality immediately.  

## <a name="see-also"></a>See Also  
[Configure New Companies](admin-how-to-configure-new-companies.md)  
[Apply Configurations to New Companies](admin-apply-configuration-to-new-companies.md)  
[Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Administration](admin-setup-and-administration.md)  
[Microsoft Dynamics NAV Windows PowerShell Cmdlets](/dynamics-nav/microsoft-dynamics-nav-windows-powershell-cmdlets)
