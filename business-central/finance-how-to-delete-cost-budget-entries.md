---
title: How to Delete Cost Budget Entries | Microsoft Docs
description: You use the Delete Cost Budget Entries batch job to cancel cost budget entries from the cost budget register.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: e2f05388149e9e6587f916db79b652e64ad5d02e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774848"
---
# <a name="delete-cost-budget-entries"></a>Delete Cost Budget Entries
You use the **Delete Cost Budget Entries** batch job to cancel cost budget entries from the cost budget register.  

To prevent any gaps in the cost budget entries and cost register entries, you cannot delete a single entry or a batch of entries in the middle of the list of register entries.  

### <a name="to-delete-a-cost-budget-entry"></a>To delete a cost budget entry  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Cost Budget Entries**, and then choose the related link.  

    The **To Register No.** field contains the last register entry number and cannot be changed.  

    You can use the **From Register No.** field to select a register entry number from which the deletion should begin.  
2.  Choose the **OK** button to delete the selected cost budget entries.  

> [!NOTE]  
>  To avoid an accidental deletion of cost budget entries, you can close register entries by marking the lines as **Closed** in the **Closed** field on the **Cost Budget Registers** page.  

## <a name="see-also"></a>See Also  
[Accounting for Costs](finance-manage-cost-accounting.md)
[Creating Cost Budgets](finance-create-cost-budgets.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]