---
title: Record expenses or income directly in G/L| Microsoft Docs
description: For business activities that are not represented by a document in, such as smaller expenses or cash receipts, you can create the related transactions by posting journal lines in the General Journal page.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct posting, general ledger
ms.date: 11/27/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: add32e82465610830b68a979e238103bfa10d438
ms.openlocfilehash: a1e7137cdc08fb558b6a6d423ce9524fa47eec16
ms.contentlocale: en-ca
ms.lasthandoff: 11/29/2018

---
# <a name="post-transactions-directly-to-the-general-ledger"></a><span data-ttu-id="f0810-103">Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="f0810-103">Post Transactions Directly to the General Ledger</span></span>

<span data-ttu-id="f0810-104">You use general journals to post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, vendor, and employee accounts.</span><span class="sxs-lookup"><span data-stu-id="f0810-104">You use general journals to post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, vendor, and employee accounts.</span></span>  

<span data-ttu-id="f0810-105">A typical use of the general journal is to post employees' expenditure of own money during business activities, for later reimbursement.</span><span class="sxs-lookup"><span data-stu-id="f0810-105">A typical use of the general journal is to post employees' expenditure of own money during business activities, for later reimbursement.</span></span> <span data-ttu-id="f0810-106">For more information, see [Record and Reimburse Employees' Expenses](finance-how-record-reimburse-employee-expenses.md).</span><span class="sxs-lookup"><span data-stu-id="f0810-106">For more information, see [Record and Reimburse Employees' Expenses](finance-how-record-reimburse-employee-expenses.md).</span></span>

<span data-ttu-id="f0810-107">General journals post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, vendor, and employee accounts.</span><span class="sxs-lookup"><span data-stu-id="f0810-107">General journals post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, vendor, and employee accounts.</span></span> <span data-ttu-id="f0810-108">Posting with a general journal always creates entries on general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="f0810-108">Posting with a general journal always creates entries on general ledger accounts.</span></span> <span data-ttu-id="f0810-109">This is true even when, for example, you post a journal line to a customer account, because an entry is posted to a general ledger receivables account through a posting group.</span><span class="sxs-lookup"><span data-stu-id="f0810-109">This is true even when, for example, you post a journal line to a customer account, because an entry is posted to a general ledger receivables account through a posting group.</span></span> <span data-ttu-id="f0810-110">You can personalize your version of a general journal by setting up a journal batch or template.</span><span class="sxs-lookup"><span data-stu-id="f0810-110">You can personalize your version of a general journal by setting up a journal batch or template.</span></span> <span data-ttu-id="f0810-111">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="f0810-111">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>

<span data-ttu-id="f0810-112">Unlike for entries that are posted with documents, which require a credit memo process, you can correctly reverse entries that are posted with the general journal.</span><span class="sxs-lookup"><span data-stu-id="f0810-112">Unlike for entries that are posted with documents, which require a credit memo process, you can correctly reverse entries that are posted with the general journal.</span></span> <span data-ttu-id="f0810-113">For more information, see [Reverse Postings](finance-how-reverse-journal-posting.md).</span><span class="sxs-lookup"><span data-stu-id="f0810-113">For more information, see [Reverse Postings](finance-how-reverse-journal-posting.md).</span></span>

## <a name="to-post-a-transaction-directly-to-a-general-ledger-account"></a><span data-ttu-id="f0810-114">To post a transaction directly to a general ledger account</span><span class="sxs-lookup"><span data-stu-id="f0810-114">To post a transaction directly to a general ledger account</span></span>

1. <span data-ttu-id="f0810-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f0810-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="f0810-116">Open the relevant general journal batch.</span><span class="sxs-lookup"><span data-stu-id="f0810-116">Open the relevant general journal batch.</span></span> <span data-ttu-id="f0810-117">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="f0810-117">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="f0810-118">On a new journal line, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="f0810-118">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. <span data-ttu-id="f0810-119">Repeat step 3 for all the separate transactions that you want to post.</span><span class="sxs-lookup"><span data-stu-id="f0810-119">Repeat step 3 for all the separate transactions that you want to post.</span></span>

    > [!TIP]  
    > <span data-ttu-id="f0810-120">If you want to enter multiple transaction lines above one balance-account line, for example, for one bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span><span class="sxs-lookup"><span data-stu-id="f0810-120">If you want to enter multiple transaction lines above one balance-account line, for example, for one bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span></span> <span data-ttu-id="f0810-121">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the transactions.</span><span class="sxs-lookup"><span data-stu-id="f0810-121">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the transactions.</span></span>
5. <span data-ttu-id="f0810-122">Choose the **Post** action to record the transactions on the specified G/L accounts.</span><span class="sxs-lookup"><span data-stu-id="f0810-122">Choose the **Post** action to record the transactions on the specified G/L accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="f0810-123">See Also</span><span class="sxs-lookup"><span data-stu-id="f0810-123">See Also</span></span>

[<span data-ttu-id="f0810-124">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="f0810-124">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="f0810-125">Record and Reimburse Employees' Expenses</span><span class="sxs-lookup"><span data-stu-id="f0810-125">Record and Reimburse Employees' Expenses</span></span>](finance-how-record-reimburse-employee-expenses.md)  
[<span data-ttu-id="f0810-126">Reverse Postings</span><span class="sxs-lookup"><span data-stu-id="f0810-126">Reverse Postings</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="f0810-127">Finance</span><span class="sxs-lookup"><span data-stu-id="f0810-127">Finance</span></span>](finance.md)  
<span data-ttu-id="f0810-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f0810-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
