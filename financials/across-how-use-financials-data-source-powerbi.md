---
title: Setup Reporting for Business Central in Power BI | Microsoft Docs
description: You can make your Financials data available as a data source in Power BI and build powerful reports of the state of your business.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 12/21/2017
ms.author: edupont
ms.openlocfilehash: 3b66a0afb953d384bba73e8c297e80c17abe78c7
ms.sourcegitcommit: e10de72476c6a6e0cbd35bcb714a29b535c39f0e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/21/2019
ms.locfileid: "227909"
---
# <a name="using-include-d365finincludesd365finmdmd-as-power-bi-data-source-for-building-reports"></a>Using [!INCLUDE [d365fin](includes/d365fin_md.md)] as Power BI Data Source for Building Reports
You can make your [!INCLUDE [d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.  

> [!NOTE]
> You must have a valid account with [!INCLUDE [d365fin](includes/d365fin_md.md)] and with Power BI. Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).  

## <a name="to-add-include-d365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a>To add [!INCLUDE [d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop
1. In Power BI Desktop, in the left navigation pane, choose **Get Data**.
2. In the **Get Data** window, choose **Online Services**, choose **Dynamics 365 Business Central**, and then choose the **Connect** button.
3. Power BI displays a wizard that will guide you through the [connection process](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md). The first step will be to sign into the service. Select **Sign in** and choose the account you would like to sign in as. This should be the same account you sign into [!INCLUDE[d365fin](includes/d365fin_md.md)] with.
4. Choose the **Connect** button to continue. The Power BI wizard shows a list of [!INCLUDE [d365fin](includes/d365fin_md.md)] companies and data sources. These data source represent all the web services that you have published from each company in [!INCLUDE[d365fin](includes/d365fin_md.md)].
5. Alternatively, create a new web service URL in [!INCLUDE [d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.
6. Specify the data you want to add to your data model, and then choose the **Load** button.
7. Repeat the previous steps to add additional [!INCLUDE [d365fin](includes/d365fin_md.md)] data to your Power BI data model.

> [!NOTE]
> Once you have successfully connected to [!INCLUDE [d365fin](includes/d365fin_md.md)], you will not be prompted again to sign in.

Once the data is loaded it will appear in the right navigation on the page. At this point, you have successfully connected to your Business Central data and are ready to begin building your Power BI report. For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).

## <a name="see-also"></a>See Also
[Business Intelligence](bi.md)  
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)   
[Finance](finance.md)  
[Connecting Power BI to [!INCLUDE[d365fin](includes/d365fin_md.md)]](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md)  
