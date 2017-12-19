---
title: How to Manage Customer Credit Information | Microsoft Docs
description: In Dynamics 365, you can add comments to customer credit information. You can also hold and block customers with bad credit before shipping or invoicing occurs.
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
ms.sourcegitcommit: aa56764b5f3210229ad21eae6891fb201462209c
ms.openlocfilehash: e206df2ec91b3a9f9533b9d871f2a286c33f2d3e
ms.contentlocale: en-ca
ms.lasthandoff: 12/14/2017

---
# <a name="how-to-manage-customer-credit-information"></a><span data-ttu-id="d8cba-104">How to: Manage Customer Credit Information</span><span class="sxs-lookup"><span data-stu-id="d8cba-104">How to: Manage Customer Credit Information</span></span>
<span data-ttu-id="d8cba-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can add comments to customer credit information.</span><span class="sxs-lookup"><span data-stu-id="d8cba-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can add comments to customer credit information.</span></span> <span data-ttu-id="d8cba-106">You can also hold and block customers with bad credit before shipping or invoicing occurs.</span><span class="sxs-lookup"><span data-stu-id="d8cba-106">You can also hold and block customers with bad credit before shipping or invoicing occurs.</span></span>  

## <a name="to-add-comments-to-customer-credit-information"></a><span data-ttu-id="d8cba-107">To add comments to customer credit information</span><span class="sxs-lookup"><span data-stu-id="d8cba-107">To add comments to customer credit information</span></span>  
1.  <span data-ttu-id="d8cba-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Credit Management**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d8cba-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Credit Management**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d8cba-109">In the **Customer List - Credit Mgmt.** window, select a customer, and then choose the **Comments** action.</span><span class="sxs-lookup"><span data-stu-id="d8cba-109">In the **Customer List - Credit Mgmt.** window, select a customer, and then choose the **Comments** action.</span></span>  
3.  <span data-ttu-id="d8cba-110">In the **Comment Sheet** window, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="d8cba-110">In the **Comment Sheet** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="d8cba-111">Field</span><span class="sxs-lookup"><span data-stu-id="d8cba-111">Field</span></span>|<span data-ttu-id="d8cba-112">Description</span><span class="sxs-lookup"><span data-stu-id="d8cba-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="d8cba-113">**Date**</span><span class="sxs-lookup"><span data-stu-id="d8cba-113">**Date**</span></span>|<span data-ttu-id="d8cba-114">The date of the comment.</span><span class="sxs-lookup"><span data-stu-id="d8cba-114">The date of the comment.</span></span>|  
    |<span data-ttu-id="d8cba-115">**Comment**</span><span class="sxs-lookup"><span data-stu-id="d8cba-115">**Comment**</span></span>|<span data-ttu-id="d8cba-116">The comment about the customer.</span><span class="sxs-lookup"><span data-stu-id="d8cba-116">The comment about the customer.</span></span> <span data-ttu-id="d8cba-117">You can enter a maximum of 80 alphanumeric characters.</span><span class="sxs-lookup"><span data-stu-id="d8cba-117">You can enter a maximum of 80 alphanumeric characters.</span></span>|  

4.  <span data-ttu-id="d8cba-118">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d8cba-118">Choose the **OK** button.</span></span>  

## <a name="to-prevent-an-order-from-shipping-or-invoicing"></a><span data-ttu-id="d8cba-119">To prevent an order from shipping or invoicing</span><span class="sxs-lookup"><span data-stu-id="d8cba-119">To prevent an order from shipping or invoicing</span></span>  
1.  <span data-ttu-id="d8cba-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d8cba-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d8cba-121">Select the customer, and the choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="d8cba-121">Select the customer, and the choose the **Ledger Entries** action.</span></span>  
3.  <span data-ttu-id="d8cba-122">In the **On Hold** field, enter the initials of the customer.</span><span class="sxs-lookup"><span data-stu-id="d8cba-122">In the **On Hold** field, enter the initials of the customer.</span></span>  
4.  <span data-ttu-id="d8cba-123">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d8cba-123">Choose the **OK** button.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="d8cba-124">You must have the proper security clearance to add or remove holds on individual sales orders using the **On Hold** field.</span><span class="sxs-lookup"><span data-stu-id="d8cba-124">You must have the proper security clearance to add or remove holds on individual sales orders using the **On Hold** field.</span></span>  

## <a name="to-block-a-sales-order-for-a-customer"></a><span data-ttu-id="d8cba-125">To block a sales order for a customer</span><span class="sxs-lookup"><span data-stu-id="d8cba-125">To block a sales order for a customer</span></span>  
1.  <span data-ttu-id="d8cba-126">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d8cba-126">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d8cba-127">Select a customer, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="d8cba-127">Select a customer, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="d8cba-128">On the **General** FastTab, in the **Blocked** field, select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="d8cba-128">On the **General** FastTab, in the **Blocked** field, select one of the following options:</span></span>  

    -   <span data-ttu-id="d8cba-129">**<Blank>** – Transaction is allowed for this customer.</span><span class="sxs-lookup"><span data-stu-id="d8cba-129">**<Blank>** – Transaction is allowed for this customer.</span></span>  
    -   <span data-ttu-id="d8cba-130">**Ship** – New orders and new shipments cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="d8cba-130">**Ship** – New orders and new shipments cannot be created for this customer.</span></span> <span data-ttu-id="d8cba-131">Existing shipments not yet invoiced can be invoiced.</span><span class="sxs-lookup"><span data-stu-id="d8cba-131">Existing shipments not yet invoiced can be invoiced.</span></span>  
    -   <span data-ttu-id="d8cba-132">**Invoice** – New orders, new shipments, and new invoices cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="d8cba-132">**Invoice** – New orders, new shipments, and new invoices cannot be created for this customer.</span></span> <span data-ttu-id="d8cba-133">Existing shipments not yet invoiced cannot be invoiced.</span><span class="sxs-lookup"><span data-stu-id="d8cba-133">Existing shipments not yet invoiced cannot be invoiced.</span></span>  
    -   <span data-ttu-id="d8cba-134">**All** – No transaction is allowed for this customer, including payments.</span><span class="sxs-lookup"><span data-stu-id="d8cba-134">**All** – No transaction is allowed for this customer, including payments.</span></span>  
4.  <span data-ttu-id="d8cba-135">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d8cba-135">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d8cba-136">See Also</span><span class="sxs-lookup"><span data-stu-id="d8cba-136">See Also</span></span>  
[<span data-ttu-id="d8cba-137">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="d8cba-137">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="d8cba-138">Finance</span><span class="sxs-lookup"><span data-stu-id="d8cba-138">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="d8cba-139">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="d8cba-139">Setting Up Finance</span></span>](../../finance.md)

