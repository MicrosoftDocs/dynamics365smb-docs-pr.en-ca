---
title: How to Manage Customer Credit Information | Microsoft Docs
description: In Business Central, you can add comments to customer credit information. You can also hold and block customers with bad credit before shipping or invoicing occurs.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: ../../receivables-how-block-customers
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 15f58025a038c0b8868fbceef51c5a74e0bbb61d
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="manage-customer-credit-information"></a><span data-ttu-id="47fd2-104">Manage Customer Credit Information</span><span class="sxs-lookup"><span data-stu-id="47fd2-104">Manage Customer Credit Information</span></span>
<span data-ttu-id="47fd2-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can add comments to customer credit information.</span><span class="sxs-lookup"><span data-stu-id="47fd2-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can add comments to customer credit information.</span></span> <span data-ttu-id="47fd2-106">You can also hold and block customers with bad credit before shipping or invoicing occurs.</span><span class="sxs-lookup"><span data-stu-id="47fd2-106">You can also hold and block customers with bad credit before shipping or invoicing occurs.</span></span>  

## <a name="to-add-comments-to-customer-credit-information"></a><span data-ttu-id="47fd2-107">To add comments to customer credit information</span><span class="sxs-lookup"><span data-stu-id="47fd2-107">To add comments to customer credit information</span></span>  
1.  <span data-ttu-id="47fd2-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Credit Management**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="47fd2-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Credit Management**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="47fd2-109">On the **Customer List - Credit Mgmt.** page, select a customer, and then choose the **Comments** action.</span><span class="sxs-lookup"><span data-stu-id="47fd2-109">On the **Customer List - Credit Mgmt.** page, select a customer, and then choose the **Comments** action.</span></span>  
3.  <span data-ttu-id="47fd2-110">On the **Comment Sheet** page, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="47fd2-110">On the **Comment Sheet** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="47fd2-111">Field</span><span class="sxs-lookup"><span data-stu-id="47fd2-111">Field</span></span>|<span data-ttu-id="47fd2-112">Description</span><span class="sxs-lookup"><span data-stu-id="47fd2-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="47fd2-113">**Date**</span><span class="sxs-lookup"><span data-stu-id="47fd2-113">**Date**</span></span>|<span data-ttu-id="47fd2-114">The date of the comment.</span><span class="sxs-lookup"><span data-stu-id="47fd2-114">The date of the comment.</span></span>|  
    |<span data-ttu-id="47fd2-115">**Comment**</span><span class="sxs-lookup"><span data-stu-id="47fd2-115">**Comment**</span></span>|<span data-ttu-id="47fd2-116">The comment about the customer.</span><span class="sxs-lookup"><span data-stu-id="47fd2-116">The comment about the customer.</span></span> <span data-ttu-id="47fd2-117">You can enter a maximum of 80 alphanumeric characters.</span><span class="sxs-lookup"><span data-stu-id="47fd2-117">You can enter a maximum of 80 alphanumeric characters.</span></span>|  

4.  <span data-ttu-id="47fd2-118">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="47fd2-118">Choose the **OK** button.</span></span>  

## <a name="to-prevent-an-order-from-shipping-or-invoicing"></a><span data-ttu-id="47fd2-119">To prevent an order from shipping or invoicing</span><span class="sxs-lookup"><span data-stu-id="47fd2-119">To prevent an order from shipping or invoicing</span></span>  
1.  <span data-ttu-id="47fd2-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="47fd2-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="47fd2-121">Select the customer, and the choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="47fd2-121">Select the customer, and the choose the **Ledger Entries** action.</span></span>  
3.  <span data-ttu-id="47fd2-122">In the **On Hold** field, enter the initials of the customer.</span><span class="sxs-lookup"><span data-stu-id="47fd2-122">In the **On Hold** field, enter the initials of the customer.</span></span>  
4.  <span data-ttu-id="47fd2-123">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="47fd2-123">Choose the **OK** button.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="47fd2-124">You must have the proper security clearance to add or remove holds on individual sales orders using the **On Hold** field.</span><span class="sxs-lookup"><span data-stu-id="47fd2-124">You must have the proper security clearance to add or remove holds on individual sales orders using the **On Hold** field.</span></span>  

## <a name="to-block-a-sales-order-for-a-customer"></a><span data-ttu-id="47fd2-125">To block a sales order for a customer</span><span class="sxs-lookup"><span data-stu-id="47fd2-125">To block a sales order for a customer</span></span>  
1.  <span data-ttu-id="47fd2-126">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="47fd2-126">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="47fd2-127">Select a customer, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="47fd2-127">Select a customer, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="47fd2-128">On the **General** FastTab, in the **Blocked** field, select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="47fd2-128">On the **General** FastTab, in the **Blocked** field, select one of the following options:</span></span>  

    -   <span data-ttu-id="47fd2-129">**<Blank>** – Transaction is allowed for this customer.</span><span class="sxs-lookup"><span data-stu-id="47fd2-129">**<Blank>** – Transaction is allowed for this customer.</span></span>  
    -   <span data-ttu-id="47fd2-130">**Ship** – New orders and new shipments cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="47fd2-130">**Ship** – New orders and new shipments cannot be created for this customer.</span></span> <span data-ttu-id="47fd2-131">Existing shipments not yet invoiced can be invoiced.</span><span class="sxs-lookup"><span data-stu-id="47fd2-131">Existing shipments not yet invoiced can be invoiced.</span></span>  
    -   <span data-ttu-id="47fd2-132">**Invoice** – New orders, new shipments, and new invoices cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="47fd2-132">**Invoice** – New orders, new shipments, and new invoices cannot be created for this customer.</span></span> <span data-ttu-id="47fd2-133">Existing shipments not yet invoiced cannot be invoiced.</span><span class="sxs-lookup"><span data-stu-id="47fd2-133">Existing shipments not yet invoiced cannot be invoiced.</span></span>  
    -   <span data-ttu-id="47fd2-134">**All** – No transaction is allowed for this customer, including payments.</span><span class="sxs-lookup"><span data-stu-id="47fd2-134">**All** – No transaction is allowed for this customer, including payments.</span></span>  
4.  <span data-ttu-id="47fd2-135">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="47fd2-135">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="47fd2-136">See Also</span><span class="sxs-lookup"><span data-stu-id="47fd2-136">See Also</span></span>  
[<span data-ttu-id="47fd2-137">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="47fd2-137">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="47fd2-138">Finance</span><span class="sxs-lookup"><span data-stu-id="47fd2-138">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="47fd2-139">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="47fd2-139">Setting Up Finance</span></span>](../../finance.md)

