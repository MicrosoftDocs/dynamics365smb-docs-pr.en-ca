---
title: Design Details - Accounts in the General Ledger | Microsoft Docs
description: To reconcile inventory and capacity ledger entries with the general ledger, the related value entries are posted to different accounts in the general ledger.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 4e732015bda76183eca7102f39e7c2b73751160b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777932"
---
# <a name="design-details-accounts-in-the-general-ledger"></a>Design Details: Accounts in the General Ledger
To reconcile inventory and capacity ledger entries with the general ledger, the related value entries are posted to different accounts in the general ledger. For more information, see [Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md).  

## <a name="from-the-inventory-ledger"></a>From the Inventory Ledger  
The following table shows the relationship between different types of inventory value entries and the accounts and balancing accounts in the general ledger.  

|**Item Ledger Entry Type**|**Value Entry Ttype**|**Variance Type**|**Expected Cost**|**Account**|**Balancing Account**|  
|--------------------------------|--------------------------|-----------------------|-----------------------|-----------------|---------------------------|  
|Purchase|Direct Cost||Yes|Inventory  (Interim)|Invt. Accrual Acc. (Interim)|  
|Purchase|Direct Cost||No|Qty. on Hand|Direct Cost Applied|  
|Purchase|Indirect Cost||No|Qty. on Hand|Overhead Applied|  
|Purchase|Variance|Purchase|No|Qty. on Hand|Purchase Variance|  
|Purchase|Revaluation||No|Qty. on Hand|Inventory Adjmt.|  
|Purchase|Rounding||No|Qty. on Hand|Inventory Adjmt.|  
|Sale|Direct Cost||Yes|Inventory  (Interim)|COGS (Interim)|  
|Sale|Direct Cost||No|Qty. on Hand|COGS|  
|Sale|Revaluation||No|Qty. on Hand|Inventory Adjmt.|  
|Sale|Rounding||No|Qty. on Hand|Inventory Adjmt.|  
|Positive Adjmt.,Negative Adjmt., Transfer|Direct Cost||No|Qty. on Hand|Inventory Adjmt.|  
|Positive Adjmt.,Negative Adjmt., Transfer|Revaluation||No|Qty. on Hand|Inventory Adjmt.|  
|Positive Adjmt.,Negative Adjmt., Transfer|Rounding||No|Qty. on Hand|Inventory Adjmt.|  
|(Production) Consumption|Direct Cost||No|Qty. on Hand|WIP|  
|(Production) Consumption|Revaluation||No|Qty. on Hand|Inventory Adjmt.|  
|(Production) Consumption|Rounding||No|Qty. on Hand|Inventory Adjmt.|  
|Assembly Consumption|Direct Cost||No|Qty. on Hand|Inventory Adjmt.|  
|Assembly Consumption|Direct Cost||No|Direct Cost Applied|Inventory Adjmt.|  
|Assembly Consumption|Indirect Cost||No|Overhead Applied|Inventory Adjmt.|  
|(Production) Output|Direct Cost||Yes|Inventory  (Interim)|WIP|  
|(Production) Output|Direct Cost||No|Qty. on Hand|WIP|  
|(Production) Output|Indirect Cost||No|Qty. on Hand|Overhead Applied|  
|(Production) Output|Variance|Material|No|Qty. on Hand|Material Variance|  
|(Production) Output|Variance|Capacity|No|Qty. on Hand|Capacity Variance|  
|(Production) Output|Variance|Subcontracted|No|Qty. on Hand|Subcontracted Variance|  
|(Production) Output|Variance|Capacity Overhead|No|Qty. on Hand|Cap. Overhead Variance|  
|(Production) Output|Variance|Manufacturing Overhead|No|Qty. on Hand|Mfg. Overhead Variance|  
|(Production) Output|Revaluation||No|Qty. on Hand|Inventory Adjmt.|  
|(Production) Output|Rounding||No|Qty. on Hand|Inventory Adjmt.|  
|Assembly Output|Direct Cost||No|Qty. on Hand|Inventory Adjmt.|  
|Assembly Output|Revaluation||No|Qty. on Hand|Inventory Adjmt.|  
|Assembly Output|Indirect Cost||No|Qty. on Hand|Overhead Applied|  
|Assembly Output|Variance|Material|No|Qty. on Hand|Material Variance|  
|Assembly Output|Variance|Capacity|No|Qty. on Hand|Capacity Variance|  
|Assembly Output|Variance|Capacity Overhead|No|Qty. on Hand|Cap. Overhead Variance|  
|Assembly Output|Variance|Manufacturing Overhead|No|Qty. on Hand|Mfg. Overhead Variance|  
|Assembly Output|Rounding||No|Qty. on Hand|Inventory Adjmt.|  

## <a name="from-the-capacity-ledger"></a>From the Capacity Ledger  
 The following table shows the relationship between different types of capacity value entries and the accounts and balancing accounts in the general ledger. Capacity ledger entries represent labour time consumed in assembly or production work.  

|**Work Type**|**Capacity Ledger Entry Type**|**Value Entry Type**|**Account**|**Balancing Account**|  
|-------------------|------------------------------------|--------------------------|-----------------|---------------------------|  
|Assembly|Resource|Direct Cost|Direct Cost Applied|Inventory Adjmt.|  
|Assembly|Resource|Indirect Cost|Overhead Applied|Inventory Adjmt.|  
|Production|Machine Centre/Work Centre|Direct Cost|WIP Account|Direct Cost Applied|  
|Production|Machine Centre/Work Centre|Indirect Cost|WIP Account|Overhead Applied|  

## <a name="assembly-costs-are-always-actual"></a>Assembly Costs are Always Actual  
 As shown in the table above, assembly postings are not represented in interim accounts. This is because the concept of work in process (WIP) does not apply in assembly output posting, unlike in production output posting. Assembly costs are only posted as actual cost, never as expected cost.  

 For more information, see [Design Details: Assembly Order Posting](design-details-assembly-order-posting.md).  

## <a name="calculating-the-amount-to-post-to-the-general-ledger"></a>Calculating the Amount to Post to the General Ledger  
 The following fields in the **Value Entry** table are used to calculate the expected cost amount that is posted to the general ledger:  

-   Cost Amount (Actual)  
-   Cost Posted to G/L  
-   Cost Amount (Expected)  
-   Expected Cost Posted to G/L  

The following table shows how the amounts to post to the general ledger are calculated for the two different cost types.  

|Cost Type|Calculation|  
|---------------|-----------------|  
|Actual Cost|Cost Amount (Actual) – Cost Posted to G/L|  
|Expected Cost|Cost Amount (Expected) –  Expected Cost Posted to G/L|  

## <a name="see-also"></a>See Also  
 [Design Details: Inventory Costing](design-details-inventory-costing.md)   
 [Design Details: Inventory Posting](design-details-inventory-posting.md)   
 [Design Details: Expected Cost Posting](design-details-expected-cost-posting.md)  
 [Managing Inventory Costs](finance-manage-inventory-costs.md)  
 [Finance](finance.md)  
 [Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]