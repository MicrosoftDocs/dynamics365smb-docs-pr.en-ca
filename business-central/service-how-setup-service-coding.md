---
title: Set Up Codes for Standard Services | Microsoft Docs
description: Learn how to set up codes for service activities that you often perform.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, service order, repairs, maintenance
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 494a3dd93906a8a9d663455f7410d27c9fc34eb9
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/31/2021
ms.locfileid: "5778231"
---
# <a name="set-up-standard-service-codes"></a>Set Up Standard Service Codes

When you perform typical service, you often have to create service documents that use service lines that contain similar information. To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines. When you choose the code on a service document, the lines are entered automatically. You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standard text linked to it. You create service lines of each standard service code on the **Standard Service Code** card. You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page. Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.  
  
> [!Tip]
> You can use the same concept to create lines on sales and purchase documents. For more information, see [Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).  
  
## <a name="to-set-up-a-standard-service-code"></a>To set up a standard service code

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Service Codes**, and then choose the related link.  
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Fill in the service lines linked to this service code.  

## <a name="to-assign-a-standard-service-code-to-a-service-item-group"></a>To assign a standard service code to a service item group

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service item Groups**, and then choose the related link.  
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Fill in the service lines linked to this service code.  

## <a name="see-also"></a>See Also

[Service Management](service-service.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]