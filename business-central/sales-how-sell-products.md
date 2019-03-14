---
title: Create a Sales Order and Sell Products | Microsoft Docs
description: Describes how to create a sales order to record your agreement with a customer to sell or trade products under specific terms.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 615002593edbb459b448ba75f98601e37cf59792
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="sell-products"></a><span data-ttu-id="cd9fa-103">Sell Products</span><span class="sxs-lookup"><span data-stu-id="cd9fa-103">Sell Products</span></span>
<span data-ttu-id="cd9fa-104">You create a sales order or sales invoice to record your agreement with a customer to sell certain products on certain delivery and payment terms.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-104">You create a sales order or sales invoice to record your agreement with a customer to sell certain products on certain delivery and payment terms.</span></span>

> [!NOTE]  
>   <span data-ttu-id="cd9fa-105">You use sales orders if your sales process requires that you can ship parts of an order quantity, for example, because the full quantity is not available at once.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-105">You use sales orders if your sales process requires that you can ship parts of an order quantity, for example, because the full quantity is not available at once.</span></span> <span data-ttu-id="cd9fa-106">If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use sales orders.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-106">If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use sales orders.</span></span> <span data-ttu-id="cd9fa-107">For more information, see [Make Drop Shipments](sales-how-drop-shipment.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-107">For more information, see [Make Drop Shipments](sales-how-drop-shipment.md).</span></span> <span data-ttu-id="cd9fa-108">In all other aspects, sales orders work the same way as sales invoices.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-108">In all other aspects, sales orders work the same way as sales invoices.</span></span> <span data-ttu-id="cd9fa-109">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-109">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span>

<span data-ttu-id="cd9fa-110">You can negotiate with the customer by first creating a sales quote, which you can convert to a sales order when you agree on the sale.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-110">You can negotiate with the customer by first creating a sales quote, which you can convert to a sales order when you agree on the sale.</span></span> <span data-ttu-id="cd9fa-111">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-111">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span>

<span data-ttu-id="cd9fa-112">After the customer has confirmed the agreement, for example after a quote process, you can send an order confirmation to record your obligation to deliver the products as agreed.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-112">After the customer has confirmed the agreement, for example after a quote process, you can send an order confirmation to record your obligation to deliver the products as agreed.</span></span>

<span data-ttu-id="cd9fa-113">When you deliver the products, either fully or partially, you post the sales order as shipped or as shipped and invoiced to create the related item and customer ledger entries in your system.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-113">When you deliver the products, either fully or partially, you post the sales order as shipped or as shipped and invoiced to create the related item and customer ledger entries in your system.</span></span> <span data-ttu-id="cd9fa-114">When you post the sales order, you can also email the document as a PDF attachment.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-114">When you post the sales order, you can also email the document as a PDF attachment.</span></span> <span data-ttu-id="cd9fa-115">You can have the email body prefilled with a summary of the order and payment information, such as a link to PayPal.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-115">You can have the email body prefilled with a summary of the order and payment information, such as a link to PayPal.</span></span> <span data-ttu-id="cd9fa-116">For more information, see [Send Documents by Email](ui-how-send-documents-email.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-116">For more information, see [Send Documents by Email](ui-how-send-documents-email.md).</span></span>

<span data-ttu-id="cd9fa-117">In business environments where the customer pays some time after delivery, according to the payment term, a posted sales invoice remains open (unpaid) until the Accounts Receivable department verifies that payment is received and applies the payment to the posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-117">In business environments where the customer pays some time after delivery, according to the payment term, a posted sales invoice remains open (unpaid) until the Accounts Receivable department verifies that payment is received and applies the payment to the posted sales invoice.</span></span> <span data-ttu-id="cd9fa-118">For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-118">For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span></span>

<span data-ttu-id="cd9fa-119">In business environments where the customer pays immediately, for example by PayPal or cash, payment is recorded immediately when you post the sales order as invoiced, that is, the posted sales invoice is closed as fully applied.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-119">In business environments where the customer pays immediately, for example by PayPal or cash, payment is recorded immediately when you post the sales order as invoiced, that is, the posted sales invoice is closed as fully applied.</span></span> <span data-ttu-id="cd9fa-120">You select the relevant method in the **Payment Method Code** field on the sales order.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-120">You select the relevant method in the **Payment Method Code** field on the sales order.</span></span> <span data-ttu-id="cd9fa-121">See under step 8.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-121">See under step 8.</span></span> <span data-ttu-id="cd9fa-122">For electronic payments, such as PayPal, you must also fill in the **Payment Service** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-122">For electronic payments, such as PayPal, you must also fill in the **Payment Service** field.</span></span> <span data-ttu-id="cd9fa-123">For more information, see [Enable Customer Payments Through Payment Services](sales-how-enable-payment-service-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-123">For more information, see [Enable Customer Payments Through Payment Services](sales-how-enable-payment-service-extensions.md).</span></span>

<span data-ttu-id="cd9fa-124">You can even create directly-paid orders for non-registered customers by first setting up a "cash customer" card, which you point to on the sales order.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-124">You can even create directly-paid orders for non-registered customers by first setting up a "cash customer" card, which you point to on the sales order.</span></span> <span data-ttu-id="cd9fa-125">For more information, see [Set Up Cash Customers](finance-how-to-set-up-cash-customers.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-125">For more information, see [Set Up Cash Customers](finance-how-to-set-up-cash-customers.md).</span></span>

<span data-ttu-id="cd9fa-126">You can easily correct or cancel a posted sales invoice resulting from a sales order before it is paid.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-126">You can easily correct or cancel a posted sales invoice resulting from a sales order before it is paid.</span></span> <span data-ttu-id="cd9fa-127">This is useful if you want to correct a typing mistake or if the customer requests a change early in the order process.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-127">This is useful if you want to correct a typing mistake or if the customer requests a change early in the order process.</span></span> <span data-ttu-id="cd9fa-128">For more information, see [Correct or Cancel Unpaid Sales Invoices](sales-how-correct-cancel-sales-invoice.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-128">For more information, see [Correct or Cancel Unpaid Sales Invoices](sales-how-correct-cancel-sales-invoice.md).</span></span> <span data-ttu-id="cd9fa-129">If the posted sales invoice is paid, then you must create a sales credit memo to reverse the sale.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-129">If the posted sales invoice is paid, then you must create a sales credit memo to reverse the sale.</span></span> <span data-ttu-id="cd9fa-130">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-130">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>

<span data-ttu-id="cd9fa-131">The item card can be of type **Inventory**, **Service**, and **Non-Inventory** to specify if the item is a physical inventory unit, a labour time unit, or a physical unit that is not kept on inventory.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-131">The item card can be of type **Inventory**, **Service**, and **Non-Inventory** to specify if the item is a physical inventory unit, a labor time unit, or a physical unit that is not kept on inventory.</span></span> <span data-ttu-id="cd9fa-132">For more information, see [Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-132">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span> <span data-ttu-id="cd9fa-133">The sales order process is the same for all three item types.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-133">The sales order process is the same for all three item types.</span></span>

<span data-ttu-id="cd9fa-134">You can fill customer fields on the sales order in two ways depending on whether the customer is already registered.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-134">You can fill customer fields on the sales order in two ways depending on whether the customer is already registered.</span></span> <span data-ttu-id="cd9fa-135">See steps 2 and 3 in the following procedure.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-135">See steps 2 and 3 in the following procedure.</span></span>

## <a name="to-create-a-sales-order"></a><span data-ttu-id="cd9fa-136">To create a sales order</span><span class="sxs-lookup"><span data-stu-id="cd9fa-136">To create a sales order</span></span>
1. <span data-ttu-id="cd9fa-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="cd9fa-138">In the **Customer** field, enter the name of an existing customer.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-138">In the **Customer** field, enter the name of an existing customer.</span></span>

    <span data-ttu-id="cd9fa-139">Other fields on the **Sales Order** page are now filled with the standard information of the selected customer.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-139">Other fields on the **Sales Order** page are now filled with the standard information of the selected customer.</span></span> <span data-ttu-id="cd9fa-140">If the customer is not registered, then follow these steps:</span><span class="sxs-lookup"><span data-stu-id="cd9fa-140">If the customer is not registered, then follow these steps:</span></span>
3. <span data-ttu-id="cd9fa-141">In the **Customer** field, enter the name of the new customer.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-141">In the **Customer** field, enter the name of the new customer.</span></span>
4. <span data-ttu-id="cd9fa-142">In the dialogue box about registering the new customer, choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-142">In the dialog box about registering the new customer, choose the **Yes** button.</span></span>
5. <span data-ttu-id="cd9fa-143">On the **Select a template for a new customer** page, choose a template to base the new customer card on, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-143">On the **Select a template for a new customer** page, choose a template to base the new customer card on, and then choose the **OK** button.</span></span>

    <span data-ttu-id="cd9fa-144">A new customer card opens, prefilled with the information on the selected customer template.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-144">A new customer card opens, prefilled with the information on the selected customer template.</span></span> <span data-ttu-id="cd9fa-145">The **Name** field is prefilled with the new customer’s name that you entered on the sales order.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-145">The **Name** field is prefilled with the new customer’s name that you entered on the sales order.</span></span>
6. <span data-ttu-id="cd9fa-146">Proceed to fill in the remaining fields on the customer card.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-146">Proceed to fill in the remaining fields on the customer card.</span></span> <span data-ttu-id="cd9fa-147">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-147">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>  
7. <span data-ttu-id="cd9fa-148">When you have completed the customer card, choose the **OK** button to return to the **Sales Order** page.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-148">When you have completed the customer card, choose the **OK** button to return to the **Sales Order** page.</span></span>

    <span data-ttu-id="cd9fa-149">Several fields on the sales order are now filled with information that you specified on the new customer card.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-149">Several fields on the sales order are now filled with information that you specified on the new customer card.</span></span>
8. <span data-ttu-id="cd9fa-150">Fill in the remaining fields on the **Sales Order** page as necessary.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-150">Fill in the remaining fields on the **Sales Order** page as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > <span data-ttu-id="cd9fa-151">If you allow the customer to pay immediately, for example, by credit card or PayPal, then fill in the **Payment Method Code** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-151">If you allow the customer to pay immediately, for example, by credit card or PayPal, then fill in the **Payment Method Code** field.</span></span> <span data-ttu-id="cd9fa-152">The payment is then recorded as soon as you post the sales order as invoiced.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-152">The payment is then recorded as soon as you post the sales order as invoiced.</span></span> <span data-ttu-id="cd9fa-153">If you select CASH, then the payment is recorded in a specified balancing account.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-153">If you select CASH, then the payment is recorded in a specified balancing account.</span></span>

    <span data-ttu-id="cd9fa-154">You are now ready to fill in the sales order lines with inventory items or services that you want to sell to the customer.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-154">You are now ready to fill in the sales order lines with inventory items or services that you want to sell to the customer.</span></span>

    <span data-ttu-id="cd9fa-155">If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-155">If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.</span></span>
9. <span data-ttu-id="cd9fa-156">On the **Lines** FastTab, in the **Item** field, enter the number of an inventory item or service.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-156">On the **Lines** FastTab, in the **Item** field, enter the number of an inventory item or service.</span></span>  
10. <span data-ttu-id="cd9fa-157">In the **Quantity** field, enter the number of items to be sold.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-157">In the **Quantity** field, enter the number of items to be sold.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="cd9fa-158">For items of type Service, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-158">For items of type Service, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span></span>

    <span data-ttu-id="cd9fa-159">The **Line Amount** field is updated to show the value in the **Unit Price** field multiplied by the value in the **Quantity** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-159">The **Line Amount** field is updated to show the value in the **Unit Price** field multiplied by the value in the **Quantity** field.</span></span>

    <span data-ttu-id="cd9fa-160">The price and line amounts are shown with or without sales tax depending on what you selected in the **Prices Including Tax** field on the customer card.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-160">The price and line amounts are shown with or without sales tax depending on what you selected in the **Prices Including Tax** field on the customer card.</span></span>
11. <span data-ttu-id="cd9fa-161">In the **Line Discount %** field, enter a percentage if you want to grant the customer a discount on the product.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-161">In the **Line Discount %** field, enter a percentage if you want to grant the customer a discount on the product.</span></span> <span data-ttu-id="cd9fa-162">The value in the **Line Amount** field is updated accordingly.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-162">The value in the **Line Amount** field is updated accordingly.</span></span>

    <span data-ttu-id="cd9fa-163">If you have set up special item prices on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, then the price and amount on the quote line are automatically updated if the agreed price criteria are met.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-163">If you have set up special item prices on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, then the price and amount on the quote line are automatically updated if the agreed price criteria are met.</span></span> <span data-ttu-id="cd9fa-164">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-164">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>
12. <span data-ttu-id="cd9fa-165">To add a comment about the quote line that the customer can see on the printed sales quote, write a text in the **Description** field on an empty line.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-165">To add a comment about the quote line that the customer can see on the printed sales quote, write a text in the **Description** field on an empty line.</span></span>  
13. <span data-ttu-id="cd9fa-166">Repeat steps 9 through 12 for every item that you want to sell to the customer.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-166">Repeat steps 9 through 12 for every item that you want to sell to the customer.</span></span>

    <span data-ttu-id="cd9fa-167">The totals under the lines are automatically calculated as you create or modify lines.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-167">The totals under the lines are automatically calculated as you create or modify lines.</span></span>
14. <span data-ttu-id="cd9fa-168">A new customer card displays the information on the selected customer template.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-168">A new customer card displays the information on the selected customer template.</span></span> <span data-ttu-id="cd9fa-169">Fill in the remaining fields.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-169">Fill in the remaining fields.</span></span> <span data-ttu-id="cd9fa-170">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-170">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>  
15. <span data-ttu-id="cd9fa-171">When you have completed the customer card, choose the **OK** button to return to the **Sales Order** page.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-171">When you have completed the customer card, choose the **OK** button to return to the **Sales Order** page.</span></span>

    <span data-ttu-id="cd9fa-172">Several fields on the sales order are now filled with information that you specified on the new customer card.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-172">Several fields on the sales order are now filled with information that you specified on the new customer card.</span></span>
16. <span data-ttu-id="cd9fa-173">Fill in the remaining fields on the **Sales Order** page as necessary.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-173">Fill in the remaining fields on the **Sales Order** page as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="cd9fa-174">You are now ready to fill in the sales order lines for products that you are selling to the customer or for any transaction with the customer that you want to record in a G/L account.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-174">You are now ready to fill in the sales order lines for products that you are selling to the customer or for any transaction with the customer that you want to record in a G/L account.</span></span>   

    <span data-ttu-id="cd9fa-175">If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-175">If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.</span></span>  
17. <span data-ttu-id="cd9fa-176">On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction that you will post for the customer with the sales line.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-176">On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction that you will post for the customer with the sales line.</span></span>

18. <span data-ttu-id="cd9fa-177">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="cd9fa-177">In the **No.**</span></span> <span data-ttu-id="cd9fa-178">field, select a record to post according to the value in the **Type** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-178">field, select a record to post according to the value in the **Type** field.</span></span>

    <span data-ttu-id="cd9fa-179">You leave the **No.**</span><span class="sxs-lookup"><span data-stu-id="cd9fa-179">You leave the **No.**</span></span> <span data-ttu-id="cd9fa-180">field empty in the following cases:</span><span class="sxs-lookup"><span data-stu-id="cd9fa-180">field empty in the following cases:</span></span>

    * <span data-ttu-id="cd9fa-181">If the line is for a comment.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-181">If the line is for a comment.</span></span> <span data-ttu-id="cd9fa-182">Write the comment in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-182">Write the comment in the **Description** field.</span></span>
    * <span data-ttu-id="cd9fa-183">If the line is for a catalogue item.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-183">If the line is for a catalog item.</span></span> <span data-ttu-id="cd9fa-184">Choose the **Select Catalogue Items** action.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-184">Choose the **Select Catalog Items** action.</span></span> <span data-ttu-id="cd9fa-185">For more information, see [Work With Catalogue Items](inventory-how-work-nonstock-items.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-185">For more information, see [Work With Catalog Items](inventory-how-work-nonstock-items.md).</span></span>

19. <span data-ttu-id="cd9fa-186">In the **Quantity** field, enter how many units of the product, charge, or transaction that the line will record for the customer.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-186">In the **Quantity** field, enter how many units of the product, charge, or transaction that the line will record for the customer.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="cd9fa-187">If the item is of type **Item - Service** or **Resource**, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-187">If the item is of type **Item - Service** or **Resource**, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span></span> <span data-ttu-id="cd9fa-188">For more information, see [Set Up Item Units of Measure](inventory-how-setup-units-of-measure.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-188">For more information, see [Set Up Item Units of Measure](inventory-how-setup-units-of-measure.md).</span></span>

    <span data-ttu-id="cd9fa-189">The value in the **Line Amount** field is calculated as *Unit Price* x *Quantity*.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-189">The value in the **Line Amount** field is calculated as *Unit Price* x *Quantity*.</span></span>  

    <span data-ttu-id="cd9fa-190">The price and line amounts are with or without sales tax, depending on what you selected in the **Prices Including Tax** field on the customer card.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-190">The price and line amounts are with or without sales tax, depending on what you selected in the **Prices Including Tax** field on the customer card.</span></span>  
20. <span data-ttu-id="cd9fa-191">If you want to give a discount, enter a percentage in the **Line Discount %** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-191">If you want to give a discount, enter a percentage in the **Line Discount %** field.</span></span> <span data-ttu-id="cd9fa-192">The value in the **Line Amount** field updates accordingly.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-192">The value in the **Line Amount** field updates accordingly.</span></span>  

    <span data-ttu-id="cd9fa-193">If special item prices are set up on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, the price and amount on the sales line automatically update if the price criteria is met.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-193">If special item prices are set up on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, the price and amount on the sales line automatically update if the price criteria is met.</span></span> <span data-ttu-id="cd9fa-194">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-194">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>  
21. <span data-ttu-id="cd9fa-195">Repeat steps 9 through 12 for every product or charge you want to sell to the customer.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-195">Repeat steps 9 through 12 for every product or charge you want to sell to the customer.</span></span>  

    <span data-ttu-id="cd9fa-196">The totals under the lines are automatically calculated as you create or modify lines.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-196">The totals under the lines are automatically calculated as you create or modify lines.</span></span>  
22. <span data-ttu-id="cd9fa-197">In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-197">In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.</span></span>

    <span data-ttu-id="cd9fa-198">If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-198">If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field.</span></span> <span data-ttu-id="cd9fa-199">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-199">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>
23. <span data-ttu-id="cd9fa-200">To only ship a part of the order quantity, enter that quantity in the **Qty. to Ship** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-200">To only ship a part of the order quantity, enter that quantity in the **Qty. to Ship** field.</span></span> <span data-ttu-id="cd9fa-201">The value is copied to the **Qty. to Invoice** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-201">The value is copied to the **Qty. to Invoice** field.</span></span>
24. <span data-ttu-id="cd9fa-202">To only invoice a part of the shipped quantity, enter that quantity in the **Qty. to Invoice** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-202">To only invoice a part of the shipped quantity, enter that quantity in the **Qty. to Invoice** field.</span></span> <span data-ttu-id="cd9fa-203">The quantity must be lower than the value in the **Qty. to Ship** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-203">The quantity must be lower than the value in the **Qty. to Ship** field.</span></span>   
25. <span data-ttu-id="cd9fa-204">When the sales order lines are completed, choose the **Post and Send** action.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-204">When the sales order lines are completed, choose the **Post and Send** action.</span></span>

<span data-ttu-id="cd9fa-205">The **Post and Send Confirmation** dialog box displays the customer's preferred method of receiving documents.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-205">The **Post and Send Confirmation** dialog box displays the customer's preferred method of receiving documents.</span></span> <span data-ttu-id="cd9fa-206">You can change the sending method by choosing the lookup button for the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-206">You can change the sending method by choosing the lookup button for the **Send Document to** field.</span></span> <span data-ttu-id="cd9fa-207">For more information, see [Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="cd9fa-207">For more information, see [Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md).</span></span>

<span data-ttu-id="cd9fa-208">The related item and customer ledger entries are now created in your system, and the sales order is output as a PDF document.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-208">The related item and customer ledger entries are now created in your system, and the sales order is output as a PDF document.</span></span> <span data-ttu-id="cd9fa-209">When the sales order is fully posted, it is removed from the list of sales orders and replaced with new documents in the list of posted sales invoices and the list of posted sales shipments.</span><span class="sxs-lookup"><span data-stu-id="cd9fa-209">When the sales order is fully posted, it is removed from the list of sales orders and replaced with new documents in the list of posted sales invoices and the list of posted sales shipments.</span></span>

## <a name="see-also"></a><span data-ttu-id="cd9fa-210">See Also</span><span class="sxs-lookup"><span data-stu-id="cd9fa-210">See Also</span></span>
[<span data-ttu-id="cd9fa-211">Sales</span><span class="sxs-lookup"><span data-stu-id="cd9fa-211">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="cd9fa-212">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="cd9fa-212">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="cd9fa-213">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="cd9fa-213">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="cd9fa-214">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="cd9fa-214">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="cd9fa-215">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cd9fa-215">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
