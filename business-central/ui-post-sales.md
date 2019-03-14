---
title: Understanding How To Post Sales Documents | Microsoft Docs
description: Learn about the different posting functions to post sales documents.
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 7ada688f7946d7f857dc6d4a6518b8bcb4e5c707
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="posting-sales"></a><span data-ttu-id="9bded-103">Posting Sales</span><span class="sxs-lookup"><span data-stu-id="9bded-103">Posting Sales</span></span>
<span data-ttu-id="9bded-104">In the **Posting group** on a sales document, you can choose between the following posting functions:</span><span class="sxs-lookup"><span data-stu-id="9bded-104">In the **Posting group** on a sales document, you can choose between the following posting functions:</span></span>

* <span data-ttu-id="9bded-105">**Post**</span><span class="sxs-lookup"><span data-stu-id="9bded-105">**Post**</span></span>
* <span data-ttu-id="9bded-106">**Test Report**</span><span class="sxs-lookup"><span data-stu-id="9bded-106">**Test Report**</span></span>
* <span data-ttu-id="9bded-107">**Post and Send**</span><span class="sxs-lookup"><span data-stu-id="9bded-107">**Post and Send**</span></span>
* <span data-ttu-id="9bded-108">**Post and Print**</span><span class="sxs-lookup"><span data-stu-id="9bded-108">**Post and Print**</span></span>
* <span data-ttu-id="9bded-109">**Post and Email**</span><span class="sxs-lookup"><span data-stu-id="9bded-109">**Post and Email**</span></span>
* <span data-ttu-id="9bded-110">**Post Batch**</span><span class="sxs-lookup"><span data-stu-id="9bded-110">**Post Batch**</span></span>
* <span data-ttu-id="9bded-111">**Preview Posting**</span><span class="sxs-lookup"><span data-stu-id="9bded-111">**Preview Posting**</span></span>

<span data-ttu-id="9bded-112">When you have completed all the lines and entered all the information on the sales order, you can post it.</span><span class="sxs-lookup"><span data-stu-id="9bded-112">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="9bded-113">This creates a shipment and an invoice.</span><span class="sxs-lookup"><span data-stu-id="9bded-113">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="9bded-114">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span><span class="sxs-lookup"><span data-stu-id="9bded-114">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="9bded-115">For each sales order, a sales entry is created in the **G/L Entry** table.</span><span class="sxs-lookup"><span data-stu-id="9bded-115">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="9bded-116">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span><span class="sxs-lookup"><span data-stu-id="9bded-116">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="9bded-117">In addition, posting the order may result in a Tax entry and a general ledger entry for the discount amount.</span><span class="sxs-lookup"><span data-stu-id="9bded-117">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="9bded-118">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Sales & Receivables Setup** page.</span><span class="sxs-lookup"><span data-stu-id="9bded-118">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Sales & Receivables Setup** page.</span></span>

<span data-ttu-id="9bded-119">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span><span class="sxs-lookup"><span data-stu-id="9bded-119">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="9bded-120">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span><span class="sxs-lookup"><span data-stu-id="9bded-120">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="9bded-121">When you post an order, you can create both a shipment and an invoice.</span><span class="sxs-lookup"><span data-stu-id="9bded-121">When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="9bded-122">These can be done at the same time or independently.</span><span class="sxs-lookup"><span data-stu-id="9bded-122">These can be done at the same time or independently.</span></span> <span data-ttu-id="9bded-123">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span><span class="sxs-lookup"><span data-stu-id="9bded-123">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="9bded-124">Note that you cannot create an invoice for something that is not shipped.</span><span class="sxs-lookup"><span data-stu-id="9bded-124">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="9bded-125">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span><span class="sxs-lookup"><span data-stu-id="9bded-125">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span>

<span data-ttu-id="9bded-126">When the posting is completed, the posted sales lines are removed from the order.</span><span class="sxs-lookup"><span data-stu-id="9bded-126">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="9bded-127">A message tells you when the posting is completed.</span><span class="sxs-lookup"><span data-stu-id="9bded-127">A message tells you when the posting is completed.</span></span> <span data-ttu-id="9bded-128">After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** pages.</span><span class="sxs-lookup"><span data-stu-id="9bded-128">After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** pages.</span></span>

## <a name="see-also"></a><span data-ttu-id="9bded-129">See Also</span><span class="sxs-lookup"><span data-stu-id="9bded-129">See Also</span></span>
[<span data-ttu-id="9bded-130">Sales</span><span class="sxs-lookup"><span data-stu-id="9bded-130">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="9bded-131">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="9bded-131">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="9bded-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9bded-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

