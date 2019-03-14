---
title: Setting Up Unrealized Value Added Tax | Microsoft Docs
description: If you're using cash-based accounting, you can specify how to handle unrealized tax for sales and purchases.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash, VAT, unrealized, cash-based
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: b8bbfac583e1e7ec7eedae9e412b4fd3ac956d0f
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---

# <a name="set-up-unrealized-vat-for-cash-based-accounting"></a><span data-ttu-id="ea0db-103">Set Up Unrealized Tax for Cash-Based Accounting</span><span class="sxs-lookup"><span data-stu-id="ea0db-103">Set Up Unrealized VAT for Cash-Based Accounting</span></span>
<span data-ttu-id="ea0db-104">If you're using cash-based accounting methods, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to handle unrealized VAT.</span><span class="sxs-lookup"><span data-stu-id="ea0db-104">If you're using cash-based accounting methods, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to handle unrealized VAT.</span></span>

## <a name="to-use-general-ledger-accounts-for-unrealized-vat"></a><span data-ttu-id="ea0db-105">To use general ledger accounts for unrealized Tax</span><span class="sxs-lookup"><span data-stu-id="ea0db-105">To use general ledger accounts for unrealized VAT</span></span>
<span data-ttu-id="ea0db-106">You can choose to have tax amounts calculated and posted to a temporary general ledger account when an invoice is posted, and then posted to the correct general ledger account and included in tax statements when the actual payment of the invoice is posted.</span><span class="sxs-lookup"><span data-stu-id="ea0db-106">You can choose to have VAT amounts calculated and posted to a temporary general ledger account when an invoice is posted, and then posted to the correct general ledger account and included in VAT statements when the actual payment of the invoice is posted.</span></span> <span data-ttu-id="ea0db-107">Before you can do this, you must complete the tax posting setup.</span><span class="sxs-lookup"><span data-stu-id="ea0db-107">Before you can do this, you must complete the VAT posting setup.</span></span>

<span data-ttu-id="ea0db-108">To use accounts for unrealized tax, follow these steps:</span><span class="sxs-lookup"><span data-stu-id="ea0db-108">To use accounts for unrealized VAT, follow these steps:</span></span>
1. <span data-ttu-id="ea0db-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and enter **General Ledger Setup**.</span><span class="sxs-lookup"><span data-stu-id="ea0db-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and enter **General Ledger Setup**.</span></span>
2. <span data-ttu-id="ea0db-110">On the **General Ledger Setup** page, on the **General** FastTab, choose **Show More**, and then choose the **Unrealized VAT** check box.</span><span class="sxs-lookup"><span data-stu-id="ea0db-110">On the **General Ledger Setup** page, on the **General** FastTab, choose **Show More**, and then choose the **Unrealized VAT** check box.</span></span>
3. <span data-ttu-id="ea0db-111">Close the page.</span><span class="sxs-lookup"><span data-stu-id="ea0db-111">Close the page.</span></span>
4. <span data-ttu-id="ea0db-112">choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), and enter **VAT Posting Setup**.</span><span class="sxs-lookup"><span data-stu-id="ea0db-112">choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), and enter **VAT Posting Setup**.</span></span>
5. <span data-ttu-id="ea0db-113">On the **VAT Posting Setup** page, choose the VAT posting group, and then choose **Edit**.</span><span class="sxs-lookup"><span data-stu-id="ea0db-113">On the **VAT Posting Setup** page, choose the VAT posting group, and then choose **Edit**.</span></span>
6. <span data-ttu-id="ea0db-114">In the **Unrealized VAT Type** field, choose an option to specify how to allocate payments to the invoice amount (excluding VAT) and the VAT amount itself, and how to transfer VAT amounts from the unrealized VAT account to the realized account.</span><span class="sxs-lookup"><span data-stu-id="ea0db-114">In the **Unrealized VAT Type** field, choose an option to specify how to allocate payments to the invoice amount (excluding VAT) and the VAT amount itself, and how to transfer VAT amounts from the unrealized VAT account to the realized account.</span></span> <span data-ttu-id="ea0db-115">The following table describes the options.</span><span class="sxs-lookup"><span data-stu-id="ea0db-115">The following table describes the options.</span></span>

| <span data-ttu-id="ea0db-116">Option</span><span class="sxs-lookup"><span data-stu-id="ea0db-116">Option</span></span> | <span data-ttu-id="ea0db-117">Description</span><span class="sxs-lookup"><span data-stu-id="ea0db-117">Description</span></span> |
| --- | --- |
| <span data-ttu-id="ea0db-118">Blank</span><span class="sxs-lookup"><span data-stu-id="ea0db-118">Blank</span></span> | <span data-ttu-id="ea0db-119">Choose this option if you don't want to use the unrealized tax feature.</span><span class="sxs-lookup"><span data-stu-id="ea0db-119">Choose this option if you don't want to use the unrealized VAT feature.</span></span> |
| <span data-ttu-id="ea0db-120">Percentage</span><span class="sxs-lookup"><span data-stu-id="ea0db-120">Percentage</span></span> | <span data-ttu-id="ea0db-121">Payments covers both tax and the invoice amount in proportion to the payment's percentage of the remaining invoice amount.</span><span class="sxs-lookup"><span data-stu-id="ea0db-121">Payments covers both VAT and the invoice amount in proportion to the payment's percentage of the remaining invoice amount.</span></span> <span data-ttu-id="ea0db-122">The paid tax amount is transferred from the unrealized tax account to the realized tax account.</span><span class="sxs-lookup"><span data-stu-id="ea0db-122">The paid VAT amount is transferred from the unrealized VAT account to the realized VAT account.</span></span> |
| <span data-ttu-id="ea0db-123">First</span><span class="sxs-lookup"><span data-stu-id="ea0db-123">First</span></span> | <span data-ttu-id="ea0db-124">Payments cover tax first and then invoice amounts.</span><span class="sxs-lookup"><span data-stu-id="ea0db-124">Payments cover VAT first and then invoice amounts.</span></span> <span data-ttu-id="ea0db-125">In this case, the amount transferred from the unrealized tax account to the tax account will equal the amount of the payment until the total tax has been paid.</span><span class="sxs-lookup"><span data-stu-id="ea0db-125">In this case, the amount transferred from the unrealized VAT account to the VAT account will equal the amount of the payment until the total VAT has been paid.</span></span> |
| <span data-ttu-id="ea0db-126">Last</span><span class="sxs-lookup"><span data-stu-id="ea0db-126">Last</span></span> | <span data-ttu-id="ea0db-127">Payments cover the invoice amount first and then tax.</span><span class="sxs-lookup"><span data-stu-id="ea0db-127">Payments cover the invoice amount first and then VAT.</span></span> <span data-ttu-id="ea0db-128">In this case, no amount will be transferred from the unrealized tax account to the tax account until the total amount of the invoice, excluding tax, has been paid.</span><span class="sxs-lookup"><span data-stu-id="ea0db-128">In this case, no amount will be transferred from the unrealized VAT account to the VAT account until the total amount of the invoice, excluding VAT, has been paid.</span></span> |
| <span data-ttu-id="ea0db-129">First (Fully Paid)</span><span class="sxs-lookup"><span data-stu-id="ea0db-129">First (Fully Paid)</span></span> | <span data-ttu-id="ea0db-130">Payments will cover VAT first (like the _First_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span><span class="sxs-lookup"><span data-stu-id="ea0db-130">Payments will cover VAT first (like the _First_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span></span> |
| <span data-ttu-id="ea0db-131">Last (Fully Paid)</span><span class="sxs-lookup"><span data-stu-id="ea0db-131">Last (Fully Paid)</span></span> | <span data-ttu-id="ea0db-132">Payments will cover invoice amount first (like the _Last_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span><span class="sxs-lookup"><span data-stu-id="ea0db-132">Payments will cover invoice amount first (like the _Last_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span></span> |

6. <span data-ttu-id="ea0db-133">In the **Sales VAT Unreal. Account** field, choose the account for unrealized sales VAT.</span><span class="sxs-lookup"><span data-stu-id="ea0db-133">In the **Sales VAT Unreal. Account** field, choose the account for unrealized sales VAT.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="ea0db-134">The Tax amount will be posted to this account, and stay there until the customer payment is posted.</span><span class="sxs-lookup"><span data-stu-id="ea0db-134">The VAT amount will be posted to this account, and stay there until the customer payment is posted.</span></span> <span data-ttu-id="ea0db-135">The amount is then transferred to the account for sales tax.</span><span class="sxs-lookup"><span data-stu-id="ea0db-135">The amount is then transferred to the account for sales VAT.</span></span>
7. <span data-ttu-id="ea0db-136">In the **Purch. VAT Unreal. Account** field, enter the general ledger account for unrealized purchase VAT.</span><span class="sxs-lookup"><span data-stu-id="ea0db-136">In the **Purch. VAT Unreal. Account** field, enter the general ledger account for unrealized purchase VAT.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="ea0db-137">The Tax amount will be posted to this account, and stay there until the customer payment is posted.</span><span class="sxs-lookup"><span data-stu-id="ea0db-137">The VAT amount will be posted to this account, and stay there until the customer payment is posted.</span></span> <span data-ttu-id="ea0db-138">The amount is then transferred to the account for purchase tax.</span><span class="sxs-lookup"><span data-stu-id="ea0db-138">The amount is then transferred to the account for purchase VAT.</span></span>

## <a name="see-also"></a><span data-ttu-id="ea0db-139">See Also</span><span class="sxs-lookup"><span data-stu-id="ea0db-139">See Also</span></span>
[<span data-ttu-id="ea0db-140">Setting Up Value Added Tax</span><span class="sxs-lookup"><span data-stu-id="ea0db-140">Setting Up Value Added Tax</span></span>](finance-setup-vat.md)
