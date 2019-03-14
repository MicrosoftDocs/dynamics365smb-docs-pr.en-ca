---
title: Create a Sales Invoice or Sales Order | Microsoft Docs
description: Describes how to create a bill of sale, or a sales invoice or sales order, to record your agreement with a customer to sell products under specific terms.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bill, sale, invoice, order
ms.date: 03/12/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: a451a97f40fb329f4ae88eef2dd62dd3b8d06c62
ms.contentlocale: en-ca
ms.lasthandoff: 04/16/2018

---
# <a name="invoice-sales"></a><span data-ttu-id="3289c-103">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="3289c-103">Invoice Sales</span></span>
<span data-ttu-id="3289c-104">You create a sales invoice or sales order to record your agreement with a customer to sell certain products on certain delivery and payment terms.</span><span class="sxs-lookup"><span data-stu-id="3289c-104">You create a sales invoice or sales order to record your agreement with a customer to sell certain products on certain delivery and payment terms.</span></span>  

<span data-ttu-id="3289c-105">There are a couple of scenarios where you must use a sales order instead of a sales invoice:</span><span class="sxs-lookup"><span data-stu-id="3289c-105">There are a couple of scenarios where you must use a sales order instead of a sales invoice:</span></span>  

* <span data-ttu-id="3289c-106">If you need to ship only part of an order quantity, for example, because the full quantity is not on hand.</span><span class="sxs-lookup"><span data-stu-id="3289c-106">If you need to ship only part of an order quantity, for example, because the full quantity is not on hand.</span></span>  
* <span data-ttu-id="3289c-107">If you sell items that your vendor delivers directly to your customer, known as drop shipment.</span><span class="sxs-lookup"><span data-stu-id="3289c-107">If you sell items that your vendor delivers directly to your customer, known as drop shipment.</span></span> <span data-ttu-id="3289c-108">For more information, see [Make Drop Shipments](sales-how-drop-shipment.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-108">For more information, see [Make Drop Shipments](sales-how-drop-shipment.md).</span></span>  

<span data-ttu-id="3289c-109">In all other aspects, sales orders and sales invoices work in the same way.</span><span class="sxs-lookup"><span data-stu-id="3289c-109">In all other aspects, sales orders and sales invoices work in the same way.</span></span> <span data-ttu-id="3289c-110">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-110">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>

<span data-ttu-id="3289c-111">You can negotiate with the customer by first creating a sales quote, which you can convert to a sales invoice when you agree on the sale.</span><span class="sxs-lookup"><span data-stu-id="3289c-111">You can negotiate with the customer by first creating a sales quote, which you can convert to a sales invoice when you agree on the sale.</span></span> <span data-ttu-id="3289c-112">For more information, see [Make Offers](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-112">For more information, see [Make Offers](sales-how-make-offers.md).</span></span>

<span data-ttu-id="3289c-113">If the customer decides to buy, you post the sales invoice to create the related quantity and value entries.</span><span class="sxs-lookup"><span data-stu-id="3289c-113">If the customer decides to buy, you post the sales invoice to create the related quantity and value entries.</span></span> <span data-ttu-id="3289c-114">When you post the sales invoice, you can also email the document as a PDF attachment.</span><span class="sxs-lookup"><span data-stu-id="3289c-114">When you post the sales invoice, you can also email the document as a PDF attachment.</span></span> <span data-ttu-id="3289c-115">You can have the email body prefilled with a summary of the invoice and payment information, such as a link to PayPal.</span><span class="sxs-lookup"><span data-stu-id="3289c-115">You can have the email body prefilled with a summary of the invoice and payment information, such as a link to PayPal.</span></span> <span data-ttu-id="3289c-116">For more information, see [Send Documents by Email](ui-how-send-documents-email.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-116">For more information, see [Send Documents by Email](ui-how-send-documents-email.md).</span></span>

<span data-ttu-id="3289c-117">In business environments where the customer must pay before products are delivered, such as in retail, you must wait for the receipt of payment before you deliver the products.</span><span class="sxs-lookup"><span data-stu-id="3289c-117">In business environments where the customer must pay before products are delivered, such as in retail, you must wait for the receipt of payment before you deliver the products.</span></span> <span data-ttu-id="3289c-118">In most cases, you process incoming payments some weeks after delivery by applying the payments to their related posted, unpaid sales invoices.</span><span class="sxs-lookup"><span data-stu-id="3289c-118">In most cases, you process incoming payments some weeks after delivery by applying the payments to their related posted, unpaid sales invoices.</span></span> <span data-ttu-id="3289c-119">For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-119">For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span></span>

<span data-ttu-id="3289c-120">In business environments where the customer pays immediately, for example by cash, PayPal, or credit card, you can select the relevant method in the **Payment Method Code** field on the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="3289c-120">In business environments where the customer pays immediately, for example by cash, PayPal, or credit card, you can select the relevant method in the **Payment Method Code** field on the sales invoice.</span></span> <span data-ttu-id="3289c-121">Payment is then recorded immediately on the posted invoice.</span><span class="sxs-lookup"><span data-stu-id="3289c-121">Payment is then recorded immediately on the posted invoice.</span></span> <span data-ttu-id="3289c-122">For payment services, you must also fill in the **Payment Service** field.</span><span class="sxs-lookup"><span data-stu-id="3289c-122">For payment services, you must also fill in the **Payment Service** field.</span></span> <span data-ttu-id="3289c-123">For more information, see [Enable Customer Payments Through Payment Services](sales-how-enable-payment-service-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-123">For more information, see [Enable Customer Payments Through Payment Services](sales-how-enable-payment-service-extensions.md).</span></span>

<span data-ttu-id="3289c-124">You can even create directly paid invoices for non-registered customers by first setting up a "cash customer" card, which you point to on the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="3289c-124">You can even create directly paid invoices for non-registered customers by first setting up a "cash customer" card, which you point to on the sales invoice.</span></span> <span data-ttu-id="3289c-125">For more information, see [Set Up Cash Customers](finance-how-to-set-up-cash-customers.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-125">For more information, see [Set Up Cash Customers](finance-how-to-set-up-cash-customers.md).</span></span>  

<span data-ttu-id="3289c-126">You can easily correct or cancel a posted sales invoice before it is paid.</span><span class="sxs-lookup"><span data-stu-id="3289c-126">You can easily correct or cancel a posted sales invoice before it is paid.</span></span> <span data-ttu-id="3289c-127">For example, this is useful if you want to correct a typing mistake or if the customer requests a change early in the order process.</span><span class="sxs-lookup"><span data-stu-id="3289c-127">For example, this is useful if you want to correct a typing mistake or if the customer requests a change early in the order process.</span></span> <span data-ttu-id="3289c-128">For more information, see [Correct or Cancel Unpaid Sales Invoices](sales-how-correct-cancel-sales-invoice.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-128">For more information, see [Correct or Cancel Unpaid Sales Invoices](sales-how-correct-cancel-sales-invoice.md).</span></span> <span data-ttu-id="3289c-129">If the posted sales invoice is paid, then you must create a sales credit memo to reverse the sale.</span><span class="sxs-lookup"><span data-stu-id="3289c-129">If the posted sales invoice is paid, then you must create a sales credit memo to reverse the sale.</span></span> <span data-ttu-id="3289c-130">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-130">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>

<span data-ttu-id="3289c-131">Items can be both inventory items and services, denoted by the **Inventory** and **Service** types on the item card.</span><span class="sxs-lookup"><span data-stu-id="3289c-131">Items can be both inventory items and services, denoted by the **Inventory** and **Service** types on the item card.</span></span> <span data-ttu-id="3289c-132">The sales invoice process is the same for both item types.</span><span class="sxs-lookup"><span data-stu-id="3289c-132">The sales invoice process is the same for both item types.</span></span> <span data-ttu-id="3289c-133">For more information, see [Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-133">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span>

<span data-ttu-id="3289c-134">You can fill customer fields on the sales invoice in two ways depending on whether the customer is already registered.</span><span class="sxs-lookup"><span data-stu-id="3289c-134">You can fill customer fields on the sales invoice in two ways depending on whether the customer is already registered.</span></span> <span data-ttu-id="3289c-135">See steps 2 and 3 in the following procedure.</span><span class="sxs-lookup"><span data-stu-id="3289c-135">See steps 2 and 3 in the following procedure.</span></span>

## <a name="to-create-a-sales-invoice"></a><span data-ttu-id="3289c-136">To create a sales invoice</span><span class="sxs-lookup"><span data-stu-id="3289c-136">To create a sales invoice</span></span>
1. <span data-ttu-id="3289c-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3289c-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3289c-138">In the **Customer** field, enter the name of an existing customer.</span><span class="sxs-lookup"><span data-stu-id="3289c-138">In the **Customer** field, enter the name of an existing customer.</span></span>

   <span data-ttu-id="3289c-139">Other fields in the **Sales Invoice** window contain standard information about the selected customer.</span><span class="sxs-lookup"><span data-stu-id="3289c-139">Other fields in the **Sales Invoice** window contain standard information about the selected customer.</span></span> <span data-ttu-id="3289c-140">If the customer is not registered, follow these steps:</span><span class="sxs-lookup"><span data-stu-id="3289c-140">If the customer is not registered, follow these steps:</span></span>
3. <span data-ttu-id="3289c-141">In the **Customer** field, enter the name of the new customer.</span><span class="sxs-lookup"><span data-stu-id="3289c-141">In the **Customer** field, enter the name of the new customer.</span></span>
4. <span data-ttu-id="3289c-142">In the dialogue box about registering the new customer, choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="3289c-142">In the dialog box about registering the new customer, choose the **Yes** button.</span></span>
5. <span data-ttu-id="3289c-143">In the **Select a template for a new customer** window, choose a template to base the new customer card on, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="3289c-143">In the **Select a template for a new customer** window, choose a template to base the new customer card on, and then choose the **OK** button.</span></span>
6. <span data-ttu-id="3289c-144">A new customer card displays the information on the selected customer template.</span><span class="sxs-lookup"><span data-stu-id="3289c-144">A new customer card displays the information on the selected customer template.</span></span> <span data-ttu-id="3289c-145">Fill in the remaining fields.</span><span class="sxs-lookup"><span data-stu-id="3289c-145">Fill in the remaining fields.</span></span> <span data-ttu-id="3289c-146">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-146">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>  
7. <span data-ttu-id="3289c-147">When you have completed the customer card, choose the **OK** button to return to the **Sales Invoice** window.</span><span class="sxs-lookup"><span data-stu-id="3289c-147">When you have completed the customer card, choose the **OK** button to return to the **Sales Invoice** window.</span></span>

   <span data-ttu-id="3289c-148">Several fields on the sales invoice are now filled with information that you specified on the new customer card.</span><span class="sxs-lookup"><span data-stu-id="3289c-148">Several fields on the sales invoice are now filled with information that you specified on the new customer card.</span></span>  
8. <span data-ttu-id="3289c-149">Fill in the remaining fields in the **Sales Invoice** window as necessary.</span><span class="sxs-lookup"><span data-stu-id="3289c-149">Fill in the remaining fields in the **Sales Invoice** window as necessary.</span></span> [!INCLUDE [tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="3289c-150">You are now ready to fill in the sales invoice lines for products that you are selling to the customer or for any transaction with the customer that you want to record in a G/L account.</span><span class="sxs-lookup"><span data-stu-id="3289c-150">You are now ready to fill in the sales invoice lines for products that you are selling to the customer or for any transaction with the customer that you want to record in a G/L account.</span></span>   

<span data-ttu-id="3289c-151">If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.</span><span class="sxs-lookup"><span data-stu-id="3289c-151">If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.</span></span>  
9. <span data-ttu-id="3289c-152">On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction that you will post for the customer with the sales line.</span><span class="sxs-lookup"><span data-stu-id="3289c-152">On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction that you will post for the customer with the sales line.</span></span>
10. <span data-ttu-id="3289c-153">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="3289c-153">In the **No.**</span></span> <span data-ttu-id="3289c-154">field, select a record to post according to the value in the **Type** field.</span><span class="sxs-lookup"><span data-stu-id="3289c-154">field, select a record to post according to the value in the **Type** field.</span></span>

   <span data-ttu-id="3289c-155">You leave the **No.**</span><span class="sxs-lookup"><span data-stu-id="3289c-155">You leave the **No.**</span></span> <span data-ttu-id="3289c-156">field empty in the following cases: -If the line is for a comment.</span><span class="sxs-lookup"><span data-stu-id="3289c-156">field empty in the following cases: -If the line is for a comment.</span></span> <span data-ttu-id="3289c-157">Write the comment in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="3289c-157">Write the comment in the **Description** field.</span></span>
       <span data-ttu-id="3289c-158">-If the line is for a nonstock item.</span><span class="sxs-lookup"><span data-stu-id="3289c-158">-If the line is for a nonstock item.</span></span> <span data-ttu-id="3289c-159">Choose the **Select Nonstock Items** action.</span><span class="sxs-lookup"><span data-stu-id="3289c-159">Choose the **Select Nonstock Items** action.</span></span> <span data-ttu-id="3289c-160">For more information, see [Work With Nonstock Items](inventory-how-work-nonstock-items.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-160">For more information, see [Work With Nonstock Items](inventory-how-work-nonstock-items.md).</span></span>

11. <span data-ttu-id="3289c-161">In the **Quantity** field, enter how many units of the product, charge, or transaction that the line will record for the customer.</span><span class="sxs-lookup"><span data-stu-id="3289c-161">In the **Quantity** field, enter how many units of the product, charge, or transaction that the line will record for the customer.</span></span>  

   > [!NOTE]  
   >   <span data-ttu-id="3289c-162">If the item is of type **Service**, or the **Type** field contains **Resource**, then the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span><span class="sxs-lookup"><span data-stu-id="3289c-162">If the item is of type **Service**, or the **Type** field contains **Resource**, then the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span></span>  

   <span data-ttu-id="3289c-163">The value in the **Line Amount** field is calculated as *Unit Price* x *Quantity*.</span><span class="sxs-lookup"><span data-stu-id="3289c-163">The value in the **Line Amount** field is calculated as *Unit Price* x *Quantity*.</span></span>  

   <span data-ttu-id="3289c-164">The price and line amounts are with or without sales tax, depending on what you selected in the **Prices Including Tax** field on the customer card.</span><span class="sxs-lookup"><span data-stu-id="3289c-164">The price and line amounts are with or without sales tax, depending on what you selected in the **Prices Including Tax** field on the customer card.</span></span>  
12. <span data-ttu-id="3289c-165">If you want to give a discount, enter a percentage in the **Line Discount %** field.</span><span class="sxs-lookup"><span data-stu-id="3289c-165">If you want to give a discount, enter a percentage in the **Line Discount %** field.</span></span> <span data-ttu-id="3289c-166">The value in the **Line Amount** field updates accordingly.</span><span class="sxs-lookup"><span data-stu-id="3289c-166">The value in the **Line Amount** field updates accordingly.</span></span>  

   <span data-ttu-id="3289c-167">If special item prices are set up on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, the price and amount on the sales line automatically update if the price criteria is met.</span><span class="sxs-lookup"><span data-stu-id="3289c-167">If special item prices are set up on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, the price and amount on the sales line automatically update if the price criteria is met.</span></span> <span data-ttu-id="3289c-168">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-168">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>  
13. <span data-ttu-id="3289c-169">Repeat steps 9 through 12 for every product or charge you want to sell to the customer.</span><span class="sxs-lookup"><span data-stu-id="3289c-169">Repeat steps 9 through 12 for every product or charge you want to sell to the customer.</span></span>  

   <span data-ttu-id="3289c-170">The totals under the lines are automatically calculated as you create or modify lines.</span><span class="sxs-lookup"><span data-stu-id="3289c-170">The totals under the lines are automatically calculated as you create or modify lines.</span></span>  
14. <span data-ttu-id="3289c-171">In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.</span><span class="sxs-lookup"><span data-stu-id="3289c-171">In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.</span></span>

   <span data-ttu-id="3289c-172">If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field.</span><span class="sxs-lookup"><span data-stu-id="3289c-172">If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field.</span></span> <span data-ttu-id="3289c-173">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-173">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>  
15. <span data-ttu-id="3289c-174">When the sales invoice lines are completed, choose the **Post and Send** action.</span><span class="sxs-lookup"><span data-stu-id="3289c-174">When the sales invoice lines are completed, choose the **Post and Send** action.</span></span>  

<span data-ttu-id="3289c-175">The **Post and Send Confirmation** dialog box displays the customer's preferred method of receiving documents.</span><span class="sxs-lookup"><span data-stu-id="3289c-175">The **Post and Send Confirmation** dialog box displays the customer's preferred method of receiving documents.</span></span> <span data-ttu-id="3289c-176">You can change the sending method by choosing the lookup button for the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="3289c-176">You can change the sending method by choosing the lookup button for the **Send Document to** field.</span></span> <span data-ttu-id="3289c-177">For more information, see [Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="3289c-177">For more information, see [Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md).</span></span>

<span data-ttu-id="3289c-178">The related item and customer ledger entries are now created in your system, and the sales invoice is output as a PDF document.</span><span class="sxs-lookup"><span data-stu-id="3289c-178">The related item and customer ledger entries are now created in your system, and the sales invoice is output as a PDF document.</span></span> <span data-ttu-id="3289c-179">The sales invoice is removed from the list of sales invoices and replaced with a new document in the list of posted sales invoices.</span><span class="sxs-lookup"><span data-stu-id="3289c-179">The sales invoice is removed from the list of sales invoices and replaced with a new document in the list of posted sales invoices.</span></span>

## <a name="see-also"></a><span data-ttu-id="3289c-180">See Also</span><span class="sxs-lookup"><span data-stu-id="3289c-180">See Also</span></span>
[<span data-ttu-id="3289c-181">Sales</span><span class="sxs-lookup"><span data-stu-id="3289c-181">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="3289c-182">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="3289c-182">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="3289c-183">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="3289c-183">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="3289c-184">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="3289c-184">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
[<span data-ttu-id="3289c-185">Bulk Invoicing from Microsoft Bookings in Finance and Operations, Business edition </span><span class="sxs-lookup"><span data-stu-id="3289c-185">Bulk Invoicing from Microsoft Bookings in Finance and Operations, Business edition </span></span>](finance-bookings.md)  
<span data-ttu-id="3289c-186">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3289c-186">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
