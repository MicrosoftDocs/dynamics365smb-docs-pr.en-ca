---
title: Transfer Bank Funds| Microsoft Docs
description: You can transfer amounts from one bank account to another, including different currencies, by posting the transaction in the general journal.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: f19fbdd0f0059e62080d0076bdc419712560d4f2
ms.contentlocale: en-ca
ms.lasthandoff: 04/16/2018

---
# <a name="transfer-bank-funds"></a><span data-ttu-id="4be9f-103">Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="4be9f-103">Transfer Bank Funds</span></span>
<span data-ttu-id="4be9f-104">You may sometimes need to transfer an amount from one bank account to another.</span><span class="sxs-lookup"><span data-stu-id="4be9f-104">You may sometimes need to transfer an amount from one bank account to another.</span></span> <span data-ttu-id="4be9f-105">To do this, you must post the a transaction in the general journal.</span><span class="sxs-lookup"><span data-stu-id="4be9f-105">To do this, you must post the a transaction in the general journal.</span></span> <span data-ttu-id="4be9f-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span><span class="sxs-lookup"><span data-stu-id="4be9f-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="4be9f-107">To post a transfer between bank accounts with the same currency code</span><span class="sxs-lookup"><span data-stu-id="4be9f-107">To post a transfer between bank accounts with the same currency code</span></span>
1. <span data-ttu-id="4be9f-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4be9f-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="4be9f-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="4be9f-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="4be9f-110">In the **Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="4be9f-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="4be9f-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="4be9f-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="4be9f-112">In the **Amount** field, enter the amount to be transferred.</span><span class="sxs-lookup"><span data-stu-id="4be9f-112">In the **Amount** field, enter the amount to be transferred.</span></span>
6. <span data-ttu-id="4be9f-113">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="4be9f-113">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="4be9f-114">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="4be9f-114">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="4be9f-115">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="4be9f-115">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="4be9f-116">To post a transfer between bank accounts with different currency codes</span><span class="sxs-lookup"><span data-stu-id="4be9f-116">To post a transfer between bank accounts with different currency codes</span></span>
<span data-ttu-id="4be9f-117">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span><span class="sxs-lookup"><span data-stu-id="4be9f-117">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="4be9f-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4be9f-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="4be9f-119">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="4be9f-119">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="4be9f-120">On the first journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="4be9f-120">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="4be9f-121">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="4be9f-121">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="4be9f-122">In the **Amount** field, enter the amount in the currency of the bank account.</span><span class="sxs-lookup"><span data-stu-id="4be9f-122">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="4be9f-123">Enter credit amounts with a minus sign.</span><span class="sxs-lookup"><span data-stu-id="4be9f-123">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="4be9f-124">Enter debit amounts without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="4be9f-124">Enter debit amounts without a minus sign.</span></span>
6. <span data-ttu-id="4be9f-125">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="4be9f-125">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="4be9f-126">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="4be9f-126">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="4be9f-127">On the second journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="4be9f-127">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
9. <span data-ttu-id="4be9f-128">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="4be9f-128">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
10. <span data-ttu-id="4be9f-129">In the **Amount** field, enter the amount in the currency of the bank account.</span><span class="sxs-lookup"><span data-stu-id="4be9f-129">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="4be9f-130">Enter credit amounts with a minus sign.</span><span class="sxs-lookup"><span data-stu-id="4be9f-130">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="4be9f-131">Enter debit amounts without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="4be9f-131">Enter debit amounts without a minus sign.</span></span>
11. <span data-ttu-id="4be9f-132">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="4be9f-132">In the **Bal. Account Type** field, select **Bank Account**.</span></span>  
12. <span data-ttu-id="4be9f-133">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="4be9f-133">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="4be9f-134">If the exchange rates used in the journal are different than the exchange rates in the **Currency Exchange Rates** window, enter a third line for the exchange rate gain or loss.</span><span class="sxs-lookup"><span data-stu-id="4be9f-134">If the exchange rates used in the journal are different than the exchange rates in the **Currency Exchange Rates** window, enter a third line for the exchange rate gain or loss.</span></span> <span data-ttu-id="4be9f-135">Enter **G/L Account** in the **Account Type** field.</span><span class="sxs-lookup"><span data-stu-id="4be9f-135">Enter **G/L Account** in the **Account Type** field.</span></span> <span data-ttu-id="4be9f-136">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span><span class="sxs-lookup"><span data-stu-id="4be9f-136">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span> <span data-ttu-id="4be9f-137">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span><span class="sxs-lookup"><span data-stu-id="4be9f-137">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span></span>
13. <span data-ttu-id="4be9f-138">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="4be9f-138">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="4be9f-139">See Also</span><span class="sxs-lookup"><span data-stu-id="4be9f-139">See Also</span></span>
[<span data-ttu-id="4be9f-140">Managing Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="4be9f-140">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="4be9f-141">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="4be9f-141">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="4be9f-142">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="4be9f-142">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="4be9f-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4be9f-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
