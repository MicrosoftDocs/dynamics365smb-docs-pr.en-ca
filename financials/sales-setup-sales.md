---
title: Overview of Tasks to Configure Sales Processes | Microsoft Docs
description: Outlines tasks to set up rules and values to define your sales policies and processes.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, configure
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: a16201e48cc823e687c9941082d34044d9612a29
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-sales"></a><span data-ttu-id="41db5-103">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="41db5-103">Setting Up Sales</span></span>
<span data-ttu-id="41db5-104">Before you can manage sales processes, you must configure the rules and values that define the company's sales policies.</span><span class="sxs-lookup"><span data-stu-id="41db5-104">Before you can manage sales processes, you must configure the rules and values that define the company's sales policies.</span></span>

<span data-ttu-id="41db5-105">You must define the general setup, such as which sales documents are required and how their values are posted.</span><span class="sxs-lookup"><span data-stu-id="41db5-105">You must define the general setup, such as which sales documents are required and how their values are posted.</span></span> <span data-ttu-id="41db5-106">This general setup is typically performed once during the initial implementation.</span><span class="sxs-lookup"><span data-stu-id="41db5-106">This general setup is typically performed once during the initial implementation.</span></span>

<span data-ttu-id="41db5-107">A separate series of tasks related to registering new customers is to record any special price or discount agreements that you have with each customer.</span><span class="sxs-lookup"><span data-stu-id="41db5-107">A separate series of tasks related to registering new customers is to record any special price or discount agreements that you have with each customer.</span></span>

<span data-ttu-id="41db5-108">Finance-related sales setup, such as payment methods and currencies, are covered in the Finance Setup section.</span><span class="sxs-lookup"><span data-stu-id="41db5-108">Finance-related sales setup, such as payment methods and currencies, are covered in the Finance Setup section.</span></span> <span data-ttu-id="41db5-109">For more information, see [Setting Up Finance](finance-setup-finance.md).</span><span class="sxs-lookup"><span data-stu-id="41db5-109">For more information, see [Setting Up Finance](finance-setup-finance.md).</span></span>

| <span data-ttu-id="41db5-110">To</span><span class="sxs-lookup"><span data-stu-id="41db5-110">To</span></span> | <span data-ttu-id="41db5-111">See</span><span class="sxs-lookup"><span data-stu-id="41db5-111">See</span></span> |
| --- | --- |
| <span data-ttu-id="41db5-112">Create a customer card for each customer that you sell to.</span><span class="sxs-lookup"><span data-stu-id="41db5-112">Create a customer card for each customer that you sell to.</span></span> |[<span data-ttu-id="41db5-113">How to: Register New Customers</span><span class="sxs-lookup"><span data-stu-id="41db5-113">How to: Register New Customers</span></span>](sales-how-register-new-customers.md) |
| <span data-ttu-id="41db5-114">Enable customers to pay through PayPal by choosing the PayPal logo on sales documents.</span><span class="sxs-lookup"><span data-stu-id="41db5-114">Enable customers to pay through PayPal by choosing the PayPal logo on sales documents.</span></span> |[<span data-ttu-id="41db5-115">How to: Enable Customer Payment Through PayPal</span><span class="sxs-lookup"><span data-stu-id="41db5-115">How to: Enable Customer Payment Through PayPal</span></span>](sales-how-enable-payment-service-extensions.md) |
| <span data-ttu-id="41db5-116">Enter the different discounts and special prices that you grant to customers depending on item, quantities, and/or date.</span><span class="sxs-lookup"><span data-stu-id="41db5-116">Enter the different discounts and special prices that you grant to customers depending on item, quantities, and/or date.</span></span> |[<span data-ttu-id="41db5-117">How to: Record Sales Price, Discount, and Payment Agreements</span><span class="sxs-lookup"><span data-stu-id="41db5-117">How to: Record Sales Price, Discount, and Payment Agreements</span></span>](sales-how-record-sales-price-discount-payment-agreements.md) |
| <span data-ttu-id="41db5-118">Set up salespeople so that you can assign them to customer contacts or measure salespeople's performance as a basis for calculating the sales commission or bonus.</span><span class="sxs-lookup"><span data-stu-id="41db5-118">Set up salespeople so that you can assign them to customer contacts or measure salespeople's performance as a basis for calculating the sales commission or bonus.</span></span> |[<span data-ttu-id="41db5-119">How to: Set Up Salespeople</span><span class="sxs-lookup"><span data-stu-id="41db5-119">How to: Set Up Salespeople</span></span>](sales-how-setup-salespeople.md) |
| <span data-ttu-id="41db5-120">Specify for individual customers or for all customers how sales documents are sent by default when you choose the **Post and Send** action.</span><span class="sxs-lookup"><span data-stu-id="41db5-120">Specify for individual customers or for all customers how sales documents are sent by default when you choose the **Post and Send** action.</span></span> |[<span data-ttu-id="41db5-121">How to: Set Up Document Sending Profiles</span><span class="sxs-lookup"><span data-stu-id="41db5-121">How to: Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md) |
| <span data-ttu-id="41db5-122">Set your email up to contain a summary of information in the sales document that is being sent.</span><span class="sxs-lookup"><span data-stu-id="41db5-122">Set your email up to contain a summary of information in the sales document that is being sent.</span></span> |<span data-ttu-id="41db5-123">[How to: Send Documents by Email](ui-how-send-documents-email.md).</span><span class="sxs-lookup"><span data-stu-id="41db5-123">[How to: Send Documents by Email](ui-how-send-documents-email.md).</span></span> |
|<span data-ttu-id="41db5-124">Use an EU web service to verify a customer's GST/HST Registration number.</span><span class="sxs-lookup"><span data-stu-id="41db5-124">Use an EU web service to verify a customer's VAT registration number.</span></span>|[<span data-ttu-id="41db5-125">How to: Verify GST/HST Registration numbers</span><span class="sxs-lookup"><span data-stu-id="41db5-125">How to: Verify VAT Registration Numbers</span></span>](sales-how-to-verify-vat-registration-numbers.md)|
|<span data-ttu-id="41db5-126">Enter information about the different transportation vendors you use, including a link to their package tracking service.</span><span class="sxs-lookup"><span data-stu-id="41db5-126">Enter information about the different transportation vendors you use, including a link to their package tracking service.</span></span>|[<span data-ttu-id="41db5-127">How to: Set Up Shipping Agents</span><span class="sxs-lookup"><span data-stu-id="41db5-127">How to: Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)|

## <a name="see-also"></a><span data-ttu-id="41db5-128">See Also</span><span class="sxs-lookup"><span data-stu-id="41db5-128">See Also</span></span>
[<span data-ttu-id="41db5-129">Sales</span><span class="sxs-lookup"><span data-stu-id="41db5-129">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="41db5-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="41db5-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

