---
title: How to Sell Items Assembled to Order | Microsoft Docs
description: If the item is set up for assemble-to-order, then the item is not expected to be in inventory, and it must be assembled specifically to a sales order. When you enter the item on a sales order line, then an assembly order is automatically created and linked to the sales order.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: ca8cf74ca844b2ec0119497e79ccfc7cc7df5026
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="sell-items-assembled-to-order"></a><span data-ttu-id="62af6-104">Sell Items Assembled to Order</span><span class="sxs-lookup"><span data-stu-id="62af6-104">Sell Items Assembled to Order</span></span>
<span data-ttu-id="62af6-105">If the **Assembly Policy** field on the item card of an assembly item is **Assemble-to-Order**, then the item is not expected to be in inventory, and it must be assembled specifically to a sales order.</span><span class="sxs-lookup"><span data-stu-id="62af6-105">If the **Assembly Policy** field on the item card of an assembly item is **Assemble-to-Order**, then the item is not expected to be in inventory, and it must be assembled specifically to a sales order.</span></span> <span data-ttu-id="62af6-106">When you enter the item on a sales order line, then an assembly order is automatically created and linked to the sales order.</span><span class="sxs-lookup"><span data-stu-id="62af6-106">When you enter the item on a sales order line, then an assembly order is automatically created and linked to the sales order.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="62af6-107">If some assemble-to-order items are already in inventory, then you can deduct that quantity from the assembly order and reserve it from inventory.</span><span class="sxs-lookup"><span data-stu-id="62af6-107">If some assemble-to-order items are already in inventory, then you can deduct that quantity from the assembly order and reserve it from inventory.</span></span> <span data-ttu-id="62af6-108">For more information, see [Sell Inventory Items in Assemble-to-Order Flows](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).</span><span class="sxs-lookup"><span data-stu-id="62af6-108">For more information, see [Sell Inventory Items in Assemble-to-Order Flows](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).</span></span>  

<span data-ttu-id="62af6-109">In this procedure, you process the sale of an item that will be assembled according to specifications that are requested by the customer.</span><span class="sxs-lookup"><span data-stu-id="62af6-109">In this procedure, you process the sale of an item that will be assembled according to specifications that are requested by the customer.</span></span> <span data-ttu-id="62af6-110">The steps include initiating the sales order line, customizing the assembly item by editing its components and resources, checking availability to establish a delivery date, and releasing the sales order to be assembled and immediately shipped.</span><span class="sxs-lookup"><span data-stu-id="62af6-110">The steps include initiating the sales order line, customizing the assembly item by editing its components and resources, checking availability to establish a delivery date, and releasing the sales order to be assembled and immediately shipped.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="62af6-111">The following procedure does not include the standard sales order steps before the step where you enter the assemble-to-order item on a sales order line.</span><span class="sxs-lookup"><span data-stu-id="62af6-111">The following procedure does not include the standard sales order steps before the step where you enter the assemble-to-order item on a sales order line.</span></span>  

## <a name="to-sell-an-item-that-is-assembled-to-order"></a><span data-ttu-id="62af6-112">To sell an item that is assembled to order</span><span class="sxs-lookup"><span data-stu-id="62af6-112">To sell an item that is assembled to order</span></span>  
1.  <span data-ttu-id="62af6-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="62af6-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="62af6-114">Create a sales order.</span><span class="sxs-lookup"><span data-stu-id="62af6-114">Create a sales order.</span></span> <span data-ttu-id="62af6-115">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="62af6-115">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>  
3.  <span data-ttu-id="62af6-116">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="62af6-116">In the **No.**</span></span> <span data-ttu-id="62af6-117">field, enter an item that is set up to be assembled to order.</span><span class="sxs-lookup"><span data-stu-id="62af6-117">field, enter an item that is set up to be assembled to order.</span></span>  
4.  <span data-ttu-id="62af6-118">In the **Location Code** field, define which location the item will be sold from.</span><span class="sxs-lookup"><span data-stu-id="62af6-118">In the **Location Code** field, define which location the item will be sold from.</span></span> <span data-ttu-id="62af6-119">The assembly process will occur at that location.</span><span class="sxs-lookup"><span data-stu-id="62af6-119">The assembly process will occur at that location.</span></span>  
5.  <span data-ttu-id="62af6-120">In the **Quantity** field, enter how many units to sell.</span><span class="sxs-lookup"><span data-stu-id="62af6-120">In the **Quantity** field, enter how many units to sell.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="62af6-121">If one or more components of the requested assembly item quantity are not available, then a detailed availability warning window opens.</span><span class="sxs-lookup"><span data-stu-id="62af6-121">If one or more components of the requested assembly item quantity are not available, then a detailed availability warning window opens.</span></span> <span data-ttu-id="62af6-122">For more information, see Assembly Availability.</span><span class="sxs-lookup"><span data-stu-id="62af6-122">For more information, see Assembly Availability.</span></span>  

    <span data-ttu-id="62af6-123">An assembly order is now automatically created and linked to the sales order line.</span><span class="sxs-lookup"><span data-stu-id="62af6-123">An assembly order is now automatically created and linked to the sales order line.</span></span> <span data-ttu-id="62af6-124">The due date of this assembly order is synchronized with the shipment date of the sales order line.</span><span class="sxs-lookup"><span data-stu-id="62af6-124">The due date of this assembly order is synchronized with the shipment date of the sales order line.</span></span>  

    <span data-ttu-id="62af6-125">The quantity to sell is copied to the **Qty. to Assemble to Order** field, which indicates that the item setup expects the full quantity on the sales line to be assembled to the order.</span><span class="sxs-lookup"><span data-stu-id="62af6-125">The quantity to sell is copied to the **Qty. to Assemble to Order** field, which indicates that the item setup expects the full quantity on the sales line to be assembled to the order.</span></span> <span data-ttu-id="62af6-126">You can decrease the quantity to assemble to order, such as if you know that some items are already available.</span><span class="sxs-lookup"><span data-stu-id="62af6-126">You can decrease the quantity to assemble to order, such as if you know that some items are already available.</span></span> <span data-ttu-id="62af6-127">For more information, see [Sell Inventory Items in Assemble-to-Order Flows](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md).</span><span class="sxs-lookup"><span data-stu-id="62af6-127">For more information, see [Sell Inventory Items in Assemble-to-Order Flows](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md).</span></span>  

6.  <span data-ttu-id="62af6-128">To reflect that the customer wants an additional item in a kit, on the **Lines** FastTab, choose the **Line** action, choose the **Assemble to Order** action, and then choose the **Assemble-to-Order Lines** action to view and change the standard assembly components.</span><span class="sxs-lookup"><span data-stu-id="62af6-128">To reflect that the customer wants an additional item in a kit, on the **Lines** FastTab, choose the **Line** action, choose the **Assemble to Order** action, and then choose the **Assemble-to-Order Lines** action to view and change the standard assembly components.</span></span> <span data-ttu-id="62af6-129">Alternatively, choose the **Qty. to Assemble to Order** field.</span><span class="sxs-lookup"><span data-stu-id="62af6-129">Alternatively, choose the **Qty. to Assemble to Order** field.</span></span>  
7.  <span data-ttu-id="62af6-130">In the **Assemble-to-Order Lines** window, create a new line of type **Item** for the requested additional kit content.</span><span class="sxs-lookup"><span data-stu-id="62af6-130">In the **Assemble-to-Order Lines** window, create a new line of type **Item** for the requested additional kit content.</span></span> <span data-ttu-id="62af6-131">The line represents an additional assembly component.</span><span class="sxs-lookup"><span data-stu-id="62af6-131">The line represents an additional assembly component.</span></span>  

    <span data-ttu-id="62af6-132">You could also customize the order by increasing the quantity of one standard item in the kit.</span><span class="sxs-lookup"><span data-stu-id="62af6-132">You could also customize the order by increasing the quantity of one standard item in the kit.</span></span> <span data-ttu-id="62af6-133">You can do this by increasing the value in the **Quantity Per** field on the specific assembly order line.</span><span class="sxs-lookup"><span data-stu-id="62af6-133">You can do this by increasing the value in the **Quantity Per** field on the specific assembly order line.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="62af6-134">The **Assemble-to-Order Lines** window only contains the basic fields that a salesperson is expected to use to customize the component list, add item tracking numbers, or to solve component availability issues.</span><span class="sxs-lookup"><span data-stu-id="62af6-134">The **Assemble-to-Order Lines** window only contains the basic fields that a salesperson is expected to use to customize the component list, add item tracking numbers, or to solve component availability issues.</span></span> <span data-ttu-id="62af6-135">To see more assembly order information, such as the assembly order starting date, choose the **Show Documents** action.</span><span class="sxs-lookup"><span data-stu-id="62af6-135">To see more assembly order information, such as the assembly order starting date, choose the **Show Documents** action.</span></span> <span data-ttu-id="62af6-136">This opens a full view of the assembly order that is linked to the sales order line.</span><span class="sxs-lookup"><span data-stu-id="62af6-136">This opens a full view of the assembly order that is linked to the sales order line.</span></span> <span data-ttu-id="62af6-137">You cannot change the contents of most fields on the assembly order header, and you cannot post assembly output from it because you must use shipment posting of the sales order line.</span><span class="sxs-lookup"><span data-stu-id="62af6-137">You cannot change the contents of most fields on the assembly order header, and you cannot post assembly output from it because you must use shipment posting of the sales order line.</span></span>  
    >   
    >  <span data-ttu-id="62af6-138">On the header of linked assembly orders, only the **Starting Date** field can be changed to enable assembly workers to specify a date that is earlier than the due date when they will start the process.</span><span class="sxs-lookup"><span data-stu-id="62af6-138">On the header of linked assembly orders, only the **Starting Date** field can be changed to enable assembly workers to specify a date that is earlier than the due date when they will start the process.</span></span> <span data-ttu-id="62af6-139">All fields on the lines of the linked assembly order can be changed so that warehouse workers can enter consumption figures during the process.</span><span class="sxs-lookup"><span data-stu-id="62af6-139">All fields on the lines of the linked assembly order can be changed so that warehouse workers can enter consumption figures during the process.</span></span>  

8.  <span data-ttu-id="62af6-140">Review or react to component availability issues.</span><span class="sxs-lookup"><span data-stu-id="62af6-140">Review or react to component availability issues.</span></span> <span data-ttu-id="62af6-141">For example, select an available substitute item or establish a later due date.</span><span class="sxs-lookup"><span data-stu-id="62af6-141">For example, select an available substitute item or establish a later due date.</span></span>  
9. <span data-ttu-id="62af6-142">Close the **Assemble-to-Order Lines** window.</span><span class="sxs-lookup"><span data-stu-id="62af6-142">Close the **Assemble-to-Order Lines** window.</span></span> <span data-ttu-id="62af6-143">The linked assembly order is now ready to start to assemble the customized items by the due date.</span><span class="sxs-lookup"><span data-stu-id="62af6-143">The linked assembly order is now ready to start to assemble the customized items by the due date.</span></span>  
10. <span data-ttu-id="62af6-144">On the sales order, choose the **Release** action to notify the assembly department that the assembly process can start.</span><span class="sxs-lookup"><span data-stu-id="62af6-144">On the sales order, choose the **Release** action to notify the assembly department that the assembly process can start.</span></span>  
11. <span data-ttu-id="62af6-145">In the assembly department, perform the steps of assembling the items that are sold in this procedure.</span><span class="sxs-lookup"><span data-stu-id="62af6-145">In the assembly department, perform the steps of assembling the items that are sold in this procedure.</span></span> <span data-ttu-id="62af6-146">For more information, see [Assemble Items](assembly-how-to-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="62af6-146">For more information, see [Assemble Items](assembly-how-to-assemble-items.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="62af6-147">See Also</span><span class="sxs-lookup"><span data-stu-id="62af6-147">See Also</span></span>  
[<span data-ttu-id="62af6-148">Assembly Management</span><span class="sxs-lookup"><span data-stu-id="62af6-148">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="62af6-149">Work with Bills of Material</span><span class="sxs-lookup"><span data-stu-id="62af6-149">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="62af6-150">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="62af6-150">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="62af6-151">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="62af6-151">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="62af6-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="62af6-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
