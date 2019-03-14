---
title: Record and Reimburse Employees' Business-Related Expenses | Microsoft Docs
description: Post employees' expenses with the general journal to the employee's account and later post a payment to the employee's bank account to reimburse for the business-related expense.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 11/27/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: add32e82465610830b68a979e238103bfa10d438
ms.openlocfilehash: 1042bfbd19a4779c72d4e945d6118a9d628301e8
ms.contentlocale: en-ca
ms.lasthandoff: 11/29/2018

---
# <a name="record-and-reimburse-employees-expenses"></a><span data-ttu-id="e4734-103">Record and Reimburse Employees' Expenses</span><span class="sxs-lookup"><span data-stu-id="e4734-103">Record and Reimburse Employees' Expenses</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="e4734-104">supports transactions for employee in a similar way as for vendors.</span><span class="sxs-lookup"><span data-stu-id="e4734-104">supports transactions for employee in a similar way as for vendors.</span></span> <span data-ttu-id="e4734-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="e4734-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span></span>

> [!NOTE]  
> <span data-ttu-id="e4734-106">Employee transactions can be posted in the local currency only.</span><span class="sxs-lookup"><span data-stu-id="e4734-106">Employee transactions can be posted in the local currency only.</span></span> <span data-ttu-id="e4734-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span><span class="sxs-lookup"><span data-stu-id="e4734-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span></span>

<span data-ttu-id="e4734-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span><span class="sxs-lookup"><span data-stu-id="e4734-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span></span> <span data-ttu-id="e4734-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span><span class="sxs-lookup"><span data-stu-id="e4734-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span></span>

## <a name="to-record-an-employees-expense"></a><span data-ttu-id="e4734-110">To record an employee's expense</span><span class="sxs-lookup"><span data-stu-id="e4734-110">To record an employee's expense</span></span>
<span data-ttu-id="e4734-111">You post employees' expenses on the **General Journal** page.</span><span class="sxs-lookup"><span data-stu-id="e4734-111">You post employees' expenses on the **General Journal** page.</span></span>
1. <span data-ttu-id="e4734-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4734-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4734-113">Open the relevant general journal batch.</span><span class="sxs-lookup"><span data-stu-id="e4734-113">Open the relevant general journal batch.</span></span> <span data-ttu-id="e4734-114">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="e4734-114">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="e4734-115">On a new journal line, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e4734-115">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. <span data-ttu-id="e4734-116">Repeat step 3 for all the expenses that the employee has incurred.</span><span class="sxs-lookup"><span data-stu-id="e4734-116">Repeat step 3 for all the expenses that the employee has incurred.</span></span>

    > [!TIP]  
    > <span data-ttu-id="e4734-117">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span><span class="sxs-lookup"><span data-stu-id="e4734-117">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span></span> <span data-ttu-id="e4734-118">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span><span class="sxs-lookup"><span data-stu-id="e4734-118">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span></span>
5. <span data-ttu-id="e4734-119">Choose the **Post** action to record the expenses on the employee's account.</span><span class="sxs-lookup"><span data-stu-id="e4734-119">Choose the **Post** action to record the expenses on the employee's account.</span></span>

## <a name="to-reimburse-an-employee"></a><span data-ttu-id="e4734-120">To reimburse an employee</span><span class="sxs-lookup"><span data-stu-id="e4734-120">To reimburse an employee</span></span>
<span data-ttu-id="e4734-121">You reimburse employees by posting payments to their bank account on the **Payment Journal** page.</span><span class="sxs-lookup"><span data-stu-id="e4734-121">You reimburse employees by posting payments to their bank account on the **Payment Journal** page.</span></span>
1. <span data-ttu-id="e4734-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4734-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4734-123">Open the relevant payment journal batch.</span><span class="sxs-lookup"><span data-stu-id="e4734-123">Open the relevant payment journal batch.</span></span> <span data-ttu-id="e4734-124">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="e4734-124">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="e4734-125">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e4734-125">Fill in the fields as necessary.</span></span> <span data-ttu-id="e4734-126">For more information, see [Making Payments](payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="e4734-126">For more information, see [Making Payments](payables-make-payments.md).</span></span>
4. <span data-ttu-id="e4734-127">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span><span class="sxs-lookup"><span data-stu-id="e4734-127">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span></span>
5. <span data-ttu-id="e4734-128">Choose the **Post** action to register the reimbursement.</span><span class="sxs-lookup"><span data-stu-id="e4734-128">Choose the **Post** action to register the reimbursement.</span></span>  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries"></a><span data-ttu-id="e4734-129">To reconcile reimbursements with employee ledger entries</span><span class="sxs-lookup"><span data-stu-id="e4734-129">To reconcile reimbursements with employee ledger entries</span></span>
<span data-ttu-id="e4734-130">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span><span class="sxs-lookup"><span data-stu-id="e4734-130">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span></span> <span data-ttu-id="e4734-131">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="e4734-131">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span> <span data-ttu-id="e4734-132">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span><span class="sxs-lookup"><span data-stu-id="e4734-132">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span></span> <span data-ttu-id="e4734-133">For more information, see the related [Reconcile Vendor Payments Manually](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="e4734-133">For more information, see the related [Reconcile Vendor Payments Manually](payables-how-apply-purchase-transactions-manually.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="e4734-134">See Also</span><span class="sxs-lookup"><span data-stu-id="e4734-134">See Also</span></span>
[<span data-ttu-id="e4734-135">Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="e4734-135">Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="e4734-136">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="e4734-136">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="e4734-137">Reverse Postings</span><span class="sxs-lookup"><span data-stu-id="e4734-137">Reverse Postings</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="e4734-138">Finance</span><span class="sxs-lookup"><span data-stu-id="e4734-138">Finance</span></span>](finance.md)  
<span data-ttu-id="e4734-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e4734-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
