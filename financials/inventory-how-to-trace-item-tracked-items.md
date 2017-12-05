---
title: How to Trace Item-Tracked Items | Microsoft Docs
description: You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned. You can also find all current instances of a specific serial or lot number in the database. You do this by using the Item Tracing and the Navigate features.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: c9944bc25131a5cb51015483511bd7d4854f4c1a
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-trace-item-tracked-items"></a><span data-ttu-id="635a8-105">How to: Trace Item-Tracked Items</span><span class="sxs-lookup"><span data-stu-id="635a8-105">How to: Trace Item-Tracked Items</span></span>
<span data-ttu-id="635a8-106">You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned.</span><span class="sxs-lookup"><span data-stu-id="635a8-106">You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned.</span></span> <span data-ttu-id="635a8-107">You can also find all current instances of a specific serial or lot number in the database.</span><span class="sxs-lookup"><span data-stu-id="635a8-107">You can also find all current instances of a specific serial or lot number in the database.</span></span> <span data-ttu-id="635a8-108">You do this by using the Item Tracing and the Navigate features.</span><span class="sxs-lookup"><span data-stu-id="635a8-108">You do this by using the Item Tracing and the Navigate features.</span></span>  

 <span data-ttu-id="635a8-109">These features can be particularly useful in quality control when you need to find out which customers received products with a particular lot number or when you need to find out which lot a defective component came from.</span><span class="sxs-lookup"><span data-stu-id="635a8-109">These features can be particularly useful in quality control when you need to find out which customers received products with a particular lot number or when you need to find out which lot a defective component came from.</span></span>  

 <span data-ttu-id="635a8-110">In the **Item Tracing** window, you can trace forwards and backwards in a sequence of posted inventory transactions for the serial or lot number.</span><span class="sxs-lookup"><span data-stu-id="635a8-110">In the **Item Tracing** window, you can trace forwards and backwards in a sequence of posted inventory transactions for the serial or lot number.</span></span>  

 <span data-ttu-id="635a8-111">In the **Navigate** window, you cannot see the sequence of transactions, but you can see all records of the serial or lot number, both posted entries and open records.</span><span class="sxs-lookup"><span data-stu-id="635a8-111">In the **Navigate** window, you cannot see the sequence of transactions, but you can see all records of the serial or lot number, both posted entries and open records.</span></span>  

 <span data-ttu-id="635a8-112">The two features can be used in combination by transferring a traced serial or lot number to the **Navigate** window to finish a complete trace scenario.</span><span class="sxs-lookup"><span data-stu-id="635a8-112">The two features can be used in combination by transferring a traced serial or lot number to the **Navigate** window to finish a complete trace scenario.</span></span> <span data-ttu-id="635a8-113">For more information, see [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).</span><span class="sxs-lookup"><span data-stu-id="635a8-113">For more information, see [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).</span></span>  

## <a name="to-trace-item-tracked-items"></a><span data-ttu-id="635a8-114">To trace item-tracked items</span><span class="sxs-lookup"><span data-stu-id="635a8-114">To trace item-tracked items</span></span>  

1.  <span data-ttu-id="635a8-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Tracing**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="635a8-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Tracing**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="635a8-116">In the filter fields at the top of the window, enter the specific item numbers or a filter on the item numbers that you would like to trace.</span><span class="sxs-lookup"><span data-stu-id="635a8-116">In the filter fields at the top of the window, enter the specific item numbers or a filter on the item numbers that you would like to trace.</span></span>  
3.  <span data-ttu-id="635a8-117">In the **Show Components** field, select whether you would like to also see where the components for the items came from.</span><span class="sxs-lookup"><span data-stu-id="635a8-117">In the **Show Components** field, select whether you would like to also see where the components for the items came from.</span></span> <span data-ttu-id="635a8-118">Your options in this field are as follows.</span><span class="sxs-lookup"><span data-stu-id="635a8-118">Your options in this field are as follows.</span></span>  

    |<span data-ttu-id="635a8-119">Field</span><span class="sxs-lookup"><span data-stu-id="635a8-119">Field</span></span>|<span data-ttu-id="635a8-120">Description</span><span class="sxs-lookup"><span data-stu-id="635a8-120">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="635a8-121">**No**</span><span class="sxs-lookup"><span data-stu-id="635a8-121">**No**</span></span>|<span data-ttu-id="635a8-122">Select this option if you do not want to see any components.</span><span class="sxs-lookup"><span data-stu-id="635a8-122">Select this option if you do not want to see any components.</span></span>|  
    |<span data-ttu-id="635a8-123">**Item-tracked Only**</span><span class="sxs-lookup"><span data-stu-id="635a8-123">**Item-tracked Only**</span></span>|<span data-ttu-id="635a8-124">Select this option if you want to see only components that have lot or serial numbers.</span><span class="sxs-lookup"><span data-stu-id="635a8-124">Select this option if you want to see only components that have lot or serial numbers.</span></span>|  
    |<span data-ttu-id="635a8-125">**All**</span><span class="sxs-lookup"><span data-stu-id="635a8-125">**All**</span></span>|<span data-ttu-id="635a8-126">Select this option if you want to see all components.</span><span class="sxs-lookup"><span data-stu-id="635a8-126">Select this option if you want to see all components.</span></span>|  

4.  <span data-ttu-id="635a8-127">In the **Trace Method** field, select the method you would like to use for tracing the item.</span><span class="sxs-lookup"><span data-stu-id="635a8-127">In the **Trace Method** field, select the method you would like to use for tracing the item.</span></span> <span data-ttu-id="635a8-128">The options are as follows</span><span class="sxs-lookup"><span data-stu-id="635a8-128">The options are as follows</span></span>  

    |<span data-ttu-id="635a8-129">Field</span><span class="sxs-lookup"><span data-stu-id="635a8-129">Field</span></span>|<span data-ttu-id="635a8-130">Description</span><span class="sxs-lookup"><span data-stu-id="635a8-130">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="635a8-131">**Usage->Origin**</span><span class="sxs-lookup"><span data-stu-id="635a8-131">**Usage->Origin**</span></span>|<span data-ttu-id="635a8-132">This method traces the item starting from where it was used to where it came from.</span><span class="sxs-lookup"><span data-stu-id="635a8-132">This method traces the item starting from where it was used to where it came from.</span></span> <span data-ttu-id="635a8-133">For instance, if a manufactured item was sold to a customer, the **Item Tracing** window shows this with the sales shipment line first, which you can then expand to see from which production order it came.</span><span class="sxs-lookup"><span data-stu-id="635a8-133">For instance, if a manufactured item was sold to a customer, the **Item Tracing** window shows this with the sales shipment line first, which you can then expand to see from which production order it came.</span></span>|  
    |<span data-ttu-id="635a8-134">**Origin->Usage**</span><span class="sxs-lookup"><span data-stu-id="635a8-134">**Origin->Usage**</span></span>|<span data-ttu-id="635a8-135">This method traces the item starting from where it came into inventory to where it was used.</span><span class="sxs-lookup"><span data-stu-id="635a8-135">This method traces the item starting from where it came into inventory to where it was used.</span></span> <span data-ttu-id="635a8-136">For instance, if a manufactured item was sold to a customer, the **Item Tracing** window shows this with the finished production order first, which you can then expand to see sale shipment lines where the item was used.</span><span class="sxs-lookup"><span data-stu-id="635a8-136">For instance, if a manufactured item was sold to a customer, the **Item Tracing** window shows this with the finished production order first, which you can then expand to see sale shipment lines where the item was used.</span></span>|  

5.  <span data-ttu-id="635a8-137">Choose the **Trace** action to run the trace.</span><span class="sxs-lookup"><span data-stu-id="635a8-137">Choose the **Trace** action to run the trace.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="635a8-138">If you have received the same lot on more transactions, then the **Item Tracing** window may not show all transactions.</span><span class="sxs-lookup"><span data-stu-id="635a8-138">If you have received the same lot on more transactions, then the **Item Tracing** window may not show all transactions.</span></span> <span data-ttu-id="635a8-139">Only applied transactions are shown.</span><span class="sxs-lookup"><span data-stu-id="635a8-139">Only applied transactions are shown.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="635a8-140">If additional transaction history under an item tracing line has already been traced by another line above it, then the **Already Traced** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="635a8-140">If additional transaction history under an item tracing line has already been traced by another line above it, then the **Already Traced** check box is selected.</span></span> <span data-ttu-id="635a8-141">To provide a simpler view, such underlying lines are not shown.</span><span class="sxs-lookup"><span data-stu-id="635a8-141">To provide a simpler view, such underlying lines are not shown.</span></span>  
>   
>  <span data-ttu-id="635a8-142">To find the item tracing lines where the transaction history has already been traced, choose the **Go to Already Traced** button.</span><span class="sxs-lookup"><span data-stu-id="635a8-142">To find the item tracing lines where the transaction history has already been traced, choose the **Go to Already Traced** button.</span></span> <span data-ttu-id="635a8-143">The item tracing line in question is selected, and all underlying lines are expanded.</span><span class="sxs-lookup"><span data-stu-id="635a8-143">The item tracing line in question is selected, and all underlying lines are expanded.</span></span>  

## <a name="to-find-item-tracked-items-with-navigate"></a><span data-ttu-id="635a8-144">To find item-tracked items with Navigate</span><span class="sxs-lookup"><span data-stu-id="635a8-144">To find item-tracked items with Navigate</span></span>  

1.  <span data-ttu-id="635a8-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Navigate**, and then select the related link.</span><span class="sxs-lookup"><span data-stu-id="635a8-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Navigate**, and then select the related link.</span></span>  
2.  <span data-ttu-id="635a8-146">On the **Item Tracking** FastTab, in the **Serial No.** and **Lot No.** fields, enter the item tracking numbers that you want to trace.</span><span class="sxs-lookup"><span data-stu-id="635a8-146">On the **Item Tracking** FastTab, in the **Serial No.** and **Lot No.** fields, enter the item tracking numbers that you want to trace.</span></span>  
3.  <span data-ttu-id="635a8-147">Choose the **Find** action to find all instances of the serial or lot number in the database.</span><span class="sxs-lookup"><span data-stu-id="635a8-147">Choose the **Find** action to find all instances of the serial or lot number in the database.</span></span>  

## <a name="see-also"></a><span data-ttu-id="635a8-148">See Also</span><span class="sxs-lookup"><span data-stu-id="635a8-148">See Also</span></span>  
[<span data-ttu-id="635a8-149">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="635a8-149">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="635a8-150">[Design Details: Item Tracking](design-details-item-tracking.md)
[Design Details - Item Tracking and Reservations](design-details-item-tracking-and-reservations.md)</span><span class="sxs-lookup"><span data-stu-id="635a8-150">[Design Details: Item Tracking](design-details-item-tracking.md)
[Design Details - Item Tracking and Reservations](design-details-item-tracking-and-reservations.md)</span></span>  
[<span data-ttu-id="635a8-151">How to: Reserve Items</span><span class="sxs-lookup"><span data-stu-id="635a8-151">How to: Reserve Items</span></span>](inventory-how-to-reserve-items.md)  
<span data-ttu-id="635a8-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
[Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md)</span><span class="sxs-lookup"><span data-stu-id="635a8-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
[Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md)</span></span>
