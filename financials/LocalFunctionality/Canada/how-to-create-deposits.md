---
title: How to Create Deposits | Microsoft Docs
description: You can make deposits to maintain a transaction record that contains information that can be applied to outstanding invoices and credit memos.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 1e3314f38c205871c56fd0a8ecd330a609e2b6f8
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="create-deposits"></a><span data-ttu-id="9a11d-103">Create Deposits</span><span class="sxs-lookup"><span data-stu-id="9a11d-103">Create Deposits</span></span>
<span data-ttu-id="9a11d-104">You can make deposits to maintain a transaction record that contains information that can be applied to outstanding invoices and credit memos.</span><span class="sxs-lookup"><span data-stu-id="9a11d-104">You can make deposits to maintain a transaction record that contains information that can be applied to outstanding invoices and credit memos.</span></span>  

## <a name="to-create-a-deposit"></a><span data-ttu-id="9a11d-105">To create a deposit</span><span class="sxs-lookup"><span data-stu-id="9a11d-105">To create a deposit</span></span>  
1.  <span data-ttu-id="9a11d-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Deposits**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9a11d-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Deposits**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9a11d-107">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="9a11d-107">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="9a11d-108">On the **General** FastTab, fill in the required fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="9a11d-108">On the **General** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="9a11d-109">Field</span><span class="sxs-lookup"><span data-stu-id="9a11d-109">Field</span></span>|<span data-ttu-id="9a11d-110">Description</span><span class="sxs-lookup"><span data-stu-id="9a11d-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="9a11d-111">**No.**</span><span class="sxs-lookup"><span data-stu-id="9a11d-111">**No.**</span></span>|<span data-ttu-id="9a11d-112">The unique identification number for the deposit.</span><span class="sxs-lookup"><span data-stu-id="9a11d-112">The unique identification number for the deposit.</span></span>|  
    |<span data-ttu-id="9a11d-113">**Bank Account No.**</span><span class="sxs-lookup"><span data-stu-id="9a11d-113">**Bank Account No.**</span></span>|<span data-ttu-id="9a11d-114">The bank account number for the deposit.</span><span class="sxs-lookup"><span data-stu-id="9a11d-114">The bank account number for the deposit.</span></span>|  
    |<span data-ttu-id="9a11d-115">**Total Deposit Amount**</span><span class="sxs-lookup"><span data-stu-id="9a11d-115">**Total Deposit Amount**</span></span>|<span data-ttu-id="9a11d-116">The total deposit amount posted to the bank ledger.</span><span class="sxs-lookup"><span data-stu-id="9a11d-116">The total deposit amount posted to the bank ledger.</span></span><br /><br /> <span data-ttu-id="9a11d-117">You can post this deposit only if the sum of the deposit lines is equal to the value in this field.</span><span class="sxs-lookup"><span data-stu-id="9a11d-117">You can post this deposit only if the sum of the deposit lines is equal to the value in this field.</span></span>|  
    |<span data-ttu-id="9a11d-118">**Posting Date**</span><span class="sxs-lookup"><span data-stu-id="9a11d-118">**Posting Date**</span></span>|<span data-ttu-id="9a11d-119">The posting date for the deposit.</span><span class="sxs-lookup"><span data-stu-id="9a11d-119">The posting date for the deposit.</span></span>|  
    |<span data-ttu-id="9a11d-120">**Document Date**</span><span class="sxs-lookup"><span data-stu-id="9a11d-120">**Document Date**</span></span>|<span data-ttu-id="9a11d-121">The deposit document date.</span><span class="sxs-lookup"><span data-stu-id="9a11d-121">The deposit document date.</span></span>|  
4.  <span data-ttu-id="9a11d-122">On the **Lines** FastTab, fill in the required fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="9a11d-122">On the **Lines** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="9a11d-123">Field</span><span class="sxs-lookup"><span data-stu-id="9a11d-123">Field</span></span>|<span data-ttu-id="9a11d-124">Description</span><span class="sxs-lookup"><span data-stu-id="9a11d-124">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="9a11d-125">**Account Type**</span><span class="sxs-lookup"><span data-stu-id="9a11d-125">**Account Type**</span></span>|<span data-ttu-id="9a11d-126">The account type.</span><span class="sxs-lookup"><span data-stu-id="9a11d-126">The account type.</span></span>|  
    |<span data-ttu-id="9a11d-127">**Account No.**</span><span class="sxs-lookup"><span data-stu-id="9a11d-127">**Account No.**</span></span>|<span data-ttu-id="9a11d-128">The unique identification account number that is associated with the selected account type, to which the entry will be posted.</span><span class="sxs-lookup"><span data-stu-id="9a11d-128">The unique identification account number that is associated with the selected account type, to which the entry will be posted.</span></span>|  
    |<span data-ttu-id="9a11d-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a11d-129">**Description**</span></span>|<span data-ttu-id="9a11d-130">The journal line entry description.</span><span class="sxs-lookup"><span data-stu-id="9a11d-130">The journal line entry description.</span></span>|  
    |<span data-ttu-id="9a11d-131">**Document Date**</span><span class="sxs-lookup"><span data-stu-id="9a11d-131">**Document Date**</span></span>|<span data-ttu-id="9a11d-132">The journal line entry document date.</span><span class="sxs-lookup"><span data-stu-id="9a11d-132">The journal line entry document date.</span></span>|  
    |<span data-ttu-id="9a11d-133">**Document Type**</span><span class="sxs-lookup"><span data-stu-id="9a11d-133">**Document Type**</span></span>|<span data-ttu-id="9a11d-134">The journal line entry document type.</span><span class="sxs-lookup"><span data-stu-id="9a11d-134">The journal line entry document type.</span></span>|  
    |<span data-ttu-id="9a11d-135">**Document No.**</span><span class="sxs-lookup"><span data-stu-id="9a11d-135">**Document No.**</span></span>|<span data-ttu-id="9a11d-136">The journal line entry document number.</span><span class="sxs-lookup"><span data-stu-id="9a11d-136">The journal line entry document number.</span></span>|  
    |<span data-ttu-id="9a11d-137">**Credit Amount**</span><span class="sxs-lookup"><span data-stu-id="9a11d-137">**Credit Amount**</span></span>|<span data-ttu-id="9a11d-138">The total credit amount on the journal line.</span><span class="sxs-lookup"><span data-stu-id="9a11d-138">The total credit amount on the journal line.</span></span>|  

5.  <span data-ttu-id="9a11d-139">Optionally, on the **Navigate** tab, choose **Dimensions**, and then add relevant dimensions in the **Dimension Set Entries** window.</span><span class="sxs-lookup"><span data-stu-id="9a11d-139">Optionally, on the **Navigate** tab, choose **Dimensions**, and then add relevant dimensions in the **Dimension Set Entries** window.</span></span>  

<span data-ttu-id="9a11d-140">After you have created a deposit, you must post it.</span><span class="sxs-lookup"><span data-stu-id="9a11d-140">After you have created a deposit, you must post it.</span></span>  

## <a name="to-post-a-deposit"></a><span data-ttu-id="9a11d-141">To post a deposit</span><span class="sxs-lookup"><span data-stu-id="9a11d-141">To post a deposit</span></span>  
1. <span data-ttu-id="9a11d-142">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="9a11d-142">Choose the **Post** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9a11d-143">You can post a deposit only if the amount displayed in the **Total Deposit Lines** field is equal to the amount in the **Total Deposit Amount** field.</span><span class="sxs-lookup"><span data-stu-id="9a11d-143">You can post a deposit only if the amount displayed in the **Total Deposit Lines** field is equal to the amount in the **Total Deposit Amount** field.</span></span>  

<span data-ttu-id="9a11d-144">Next, you can use the Deposit Test Report and Deposit reports to reconcile your posted deposits with outstanding invoices and credit memos.</span><span class="sxs-lookup"><span data-stu-id="9a11d-144">Next, you can use the Deposit Test Report and Deposit reports to reconcile your posted deposits with outstanding invoices and credit memos.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9a11d-145">See Also</span><span class="sxs-lookup"><span data-stu-id="9a11d-145">See Also</span></span>  
[<span data-ttu-id="9a11d-146">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="9a11d-146">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="9a11d-147">Finance</span><span class="sxs-lookup"><span data-stu-id="9a11d-147">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="9a11d-148">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="9a11d-148">Setting Up Finance</span></span>](../../finance.md)  

