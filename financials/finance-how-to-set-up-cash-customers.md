---
title: How to Set Up Cash Customers | Microsoft Docs
description: This topic describes the steps to set up customer who pays in cash.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: a6be13d3f2fcc683e8d711691f9d994f64458f85
ms.contentlocale: en-ca
ms.lasthandoff: 04/16/2018

---
# <a name="set-up-cash-customers"></a><span data-ttu-id="40aa5-103">Set Up Cash Customers</span><span class="sxs-lookup"><span data-stu-id="40aa5-103">Set Up Cash Customers</span></span>
<span data-ttu-id="40aa5-104">You cannot create an invoice without a customer number.</span><span class="sxs-lookup"><span data-stu-id="40aa5-104">You cannot create an invoice without a customer number.</span></span> <span data-ttu-id="40aa5-105">This is true, even if you make a cash sale and do not have anything to record in a customer account.</span><span class="sxs-lookup"><span data-stu-id="40aa5-105">This is true, even if you make a cash sale and do not have anything to record in a customer account.</span></span>  

## <a name="to-set-up-a-cash-customer"></a><span data-ttu-id="40aa5-106">To set up a cash customer</span><span class="sxs-lookup"><span data-stu-id="40aa5-106">To set up a cash customer</span></span>  
1. <span data-ttu-id="40aa5-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="40aa5-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer**, and then choose the related link.</span></span>  
2. <span data-ttu-id="40aa5-108">Create a new **Customer** card.</span><span class="sxs-lookup"><span data-stu-id="40aa5-108">Create a new **Customer** card.</span></span> <span data-ttu-id="40aa5-109">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="40aa5-109">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>
3. <span data-ttu-id="40aa5-110">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="40aa5-110">In the **No.**</span></span> <span data-ttu-id="40aa5-111">field, enter **Cash**, for example.</span><span class="sxs-lookup"><span data-stu-id="40aa5-111">field, enter **Cash**, for example.</span></span>  
4. <span data-ttu-id="40aa5-112">In the **Name** field, enter **Cash Sale**, for example.</span><span class="sxs-lookup"><span data-stu-id="40aa5-112">In the **Name** field, enter **Cash Sale**, for example.</span></span>  
5. <span data-ttu-id="40aa5-113">On the **Invoicing** FastTab, fill in the **Customer Posting Group** and the **Gen. Bus. Posting Group** fields.</span><span class="sxs-lookup"><span data-stu-id="40aa5-113">On the **Invoicing** FastTab, fill in the **Customer Posting Group** and the **Gen. Bus. Posting Group** fields.</span></span>  

   <span data-ttu-id="40aa5-114">Now you have set up a customer that contains sufficient information for invoicing.</span><span class="sxs-lookup"><span data-stu-id="40aa5-114">Now you have set up a customer that contains sufficient information for invoicing.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="40aa5-115">You may have chosen a posting group that is also used for domestic credit sales.</span><span class="sxs-lookup"><span data-stu-id="40aa5-115">You may have chosen a posting group that is also used for domestic credit sales.</span></span> <span data-ttu-id="40aa5-116">If you want to maintain separate data on cash sales, for example, with a special sales or receivables account, you can set up an extra posting group for this purpose.</span><span class="sxs-lookup"><span data-stu-id="40aa5-116">If you want to maintain separate data on cash sales, for example, with a special sales or receivables account, you can set up an extra posting group for this purpose.</span></span>  
>   
>  <span data-ttu-id="40aa5-117">You must enter a number for a receivables account for the posting group, even though the balance in this account will always be 0 after you post an invoice.</span><span class="sxs-lookup"><span data-stu-id="40aa5-117">You must enter a number for a receivables account for the posting group, even though the balance in this account will always be 0 after you post an invoice.</span></span>  

## <a name="see-also"></a><span data-ttu-id="40aa5-118">See Also</span><span class="sxs-lookup"><span data-stu-id="40aa5-118">See Also</span></span>
[<span data-ttu-id="40aa5-119">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="40aa5-119">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="40aa5-120">[Register New Customers](sales-how-register-new-customers.md)  </span><span class="sxs-lookup"><span data-stu-id="40aa5-120">[Register New Customers](sales-how-register-new-customers.md)  </span></span>  
[<span data-ttu-id="40aa5-121">Finance</span><span class="sxs-lookup"><span data-stu-id="40aa5-121">Finance</span></span>](finance.md)  

