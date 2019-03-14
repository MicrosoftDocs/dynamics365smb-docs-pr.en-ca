---
title: Optional Activities for Closing Periods | Microsoft Docs
description: This topic outlines the optional processes and activities for closing accounting periods in Finance and Operations, Business edition.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 06/19/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 344e294083813d41b415ad07e6e8acdd3fe5047b
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="overview-of-tasks-to-close-accounting-periods"></a><span data-ttu-id="d9075-103">Overview of Tasks to Close Accounting Periods</span><span class="sxs-lookup"><span data-stu-id="d9075-103">Overview of Tasks to Close Accounting Periods</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="d9075-104"> does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span><span class="sxs-lookup"><span data-stu-id="d9075-104"> does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span></span> <span data-ttu-id="d9075-105">This topic provides an overview of optional processes and activities for closing periods.</span><span class="sxs-lookup"><span data-stu-id="d9075-105">This topic provides an overview of optional processes and activities for closing periods.</span></span>  

## <a name="general-ledger"></a><span data-ttu-id="d9075-106">General Ledger</span><span class="sxs-lookup"><span data-stu-id="d9075-106">General Ledger</span></span>
* <span data-ttu-id="d9075-107">Specify system-wide and user-specific posting periods.</span><span class="sxs-lookup"><span data-stu-id="d9075-107">Specify system-wide and user-specific posting periods.</span></span>  

    <span data-ttu-id="d9075-108">This specifies the dates between which you allow posting.</span><span class="sxs-lookup"><span data-stu-id="d9075-108">This specifies the dates between which you allow posting.</span></span> <span data-ttu-id="d9075-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span><span class="sxs-lookup"><span data-stu-id="d9075-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span></span> <span data-ttu-id="d9075-110">For more information, see [Specify Posting Periods](finance-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="d9075-110">For more information, see [Specify Posting Periods](finance-how-specify-posting-periods.md).</span></span>  
* <span data-ttu-id="d9075-111">Make all necessary G/L adjustments.</span><span class="sxs-lookup"><span data-stu-id="d9075-111">Make all necessary G/L adjustments.</span></span>  
* <span data-ttu-id="d9075-112">Update and post Recurring Journals.</span><span class="sxs-lookup"><span data-stu-id="d9075-112">Update and post Recurring Journals.</span></span>  
  <!--* Process Consolidations-->
* <span data-ttu-id="d9075-113">Run account schedules as follows:</span><span class="sxs-lookup"><span data-stu-id="d9075-113">Run account schedules as follows:</span></span>  
  * <span data-ttu-id="d9075-114">Open the **Account Schedule** window, and then choose the **Print** action.</span><span class="sxs-lookup"><span data-stu-id="d9075-114">Open the **Account Schedule** window, and then choose the **Print** action.</span></span>  

## <a name="sales-and-receivables"></a><span data-ttu-id="d9075-115">Sales and Receivables</span><span class="sxs-lookup"><span data-stu-id="d9075-115">Sales and Receivables</span></span>
* <span data-ttu-id="d9075-116">Post all sales orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="d9075-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="d9075-117">Post all cash receipt journals.</span><span class="sxs-lookup"><span data-stu-id="d9075-117">Post all cash receipt journals.</span></span>  
* <span data-ttu-id="d9075-118">Update and post recurring journals that are related to sales and receivables.</span><span class="sxs-lookup"><span data-stu-id="d9075-118">Update and post recurring journals that are related to sales and receivables.</span></span>  
* <span data-ttu-id="d9075-119">Reconcile accounts receivable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="d9075-119">Reconcile accounts receivable to the general ledger.</span></span>  
* <span data-ttu-id="d9075-120">Run the **Delete Invoiced Sales Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="d9075-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>  

## <a name="purchases-and-payables"></a><span data-ttu-id="d9075-121">Purchases and Payables</span><span class="sxs-lookup"><span data-stu-id="d9075-121">Purchases and Payables</span></span>
* <span data-ttu-id="d9075-122">Post all purchase orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="d9075-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="d9075-123">Post all payment journals.</span><span class="sxs-lookup"><span data-stu-id="d9075-123">Post all payment journals.</span></span>  
* <span data-ttu-id="d9075-124">Update and post recurring journals that are related to purchases & payables.</span><span class="sxs-lookup"><span data-stu-id="d9075-124">Update and post recurring journals that are related to purchases & payables.</span></span>  
* <span data-ttu-id="d9075-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="d9075-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>  
* <span data-ttu-id="d9075-126">Run the **Delete Invoiced Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="d9075-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>  

<span data-ttu-id="d9075-127">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="d9075-127">Fixed Assets</span></span>
* <span data-ttu-id="d9075-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span><span class="sxs-lookup"><span data-stu-id="d9075-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span></span>
* <span data-ttu-id="d9075-129">Post adjustments.</span><span class="sxs-lookup"><span data-stu-id="d9075-129">Post adjustments.</span></span>
* <span data-ttu-id="d9075-130">Post appreciation.</span><span class="sxs-lookup"><span data-stu-id="d9075-130">Post appreciation.</span></span>
* <span data-ttu-id="d9075-131">Post depreciation.</span><span class="sxs-lookup"><span data-stu-id="d9075-131">Post depreciation.</span></span>
* <span data-ttu-id="d9075-132">Update and post the recurring fixed asset journal.</span><span class="sxs-lookup"><span data-stu-id="d9075-132">Update and post the recurring fixed asset journal.</span></span>

<span data-ttu-id="d9075-133">Intercompany</span><span class="sxs-lookup"><span data-stu-id="d9075-133">Intercompany</span></span>
* <span data-ttu-id="d9075-134">Process Intercompany Transactions</span><span class="sxs-lookup"><span data-stu-id="d9075-134">Process Intercompany Transactions</span></span>

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="d9075-135">Calculate and Process Sales Tax</span><span class="sxs-lookup"><span data-stu-id="d9075-135">Calculate and Process Sales Tax</span></span>
* <span data-ttu-id="d9075-136">Complete Tax Statements.</span><span class="sxs-lookup"><span data-stu-id="d9075-136">Complete Tax Statements.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d9075-137">See Also</span><span class="sxs-lookup"><span data-stu-id="d9075-137">See Also</span></span>
[<span data-ttu-id="d9075-138">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="d9075-138">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="d9075-139">Closing Books</span><span class="sxs-lookup"><span data-stu-id="d9075-139">Closing Books</span></span>](year-close-books.md)  
<span data-ttu-id="d9075-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d9075-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
