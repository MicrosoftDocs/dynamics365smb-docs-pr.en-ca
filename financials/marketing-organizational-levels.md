---
title: Setting Up Organizational Levels for Contact Persons | Microsoft Docs
description: Describes organizational levels for contacts in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, client, prospect
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: bde26a2d5fcb7ec10dcd70fdd30c74893bcb34d5
ms.contentlocale: en-ca
ms.lasthandoff: 05/04/2017


---
# <a name="setting-up-organizational-levels-for-contact-persons"></a>Setting Up Organizational Levels for Contact Persons
You can use organizational levels on your contacts to specify which position they have in the company, for example, top management. You can use this information when entering information about your contacts.

Using organizational levels on contacts is a two-step process. First, you define the organizational level code. You only have to perform this step one time for each organizational level. Once you have an organizational level code, you can start to assign the code to contact persons.

## <a name="to-define-an-organizational-level-code"></a>to define an organizational level code
The organizational level code defines the type or category of the organizational level, such a CEO  or CFO. You can have several organizational level codes. To define the organizational level, you use the **Organizational Levels** window.

1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Organizational Levels**, and then choose the related link.
2. Choose the **New** action, and fill in a code and description. The code can be a maximum of 11 characters, and can be any combination of numbers and letters.

## <a name="to-assign-organizational-levels-to-a-contact-person"></a>to assign organizational levels to a contact person
You can assign organizational levels to contact persons only, not contact companies. You can only assign one organizational level to each contact.

1. Open the contact.
2. In the **Organizational Levels** field, select the code you want to assign.

After you have assigned organizational levels to your contacts, you can use this information to create segments.

After you have assigned job responsibilities to your contacts, you can use this information to select contacts for your segments. For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).

## <a name="see-also"></a>See Also
[Creating Contact Companies](marketing-create-contact-companies.md)  
[Creating Contact Persons](marketing-create-contact-persons.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

