---
title: How to Create Deposits | Microsoft Docs
description: You can make deposits to maintain a transaction record that contains information that can be applied to outstanding invoices and credit memos.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: d2c7378a4f96bbac27fa26bd43ced375c31dcd42
ms.sourcegitcommit: a1890e0c959f4a07a4e4d9807be98ec5fe20c0f7
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 04/09/2019
ms.locfileid: "938414"
---
# <a name="create-deposits"></a><span data-ttu-id="2fcd8-103">Create Deposits</span><span class="sxs-lookup"><span data-stu-id="2fcd8-103">Create Deposits</span></span>
<span data-ttu-id="2fcd8-104">You can make deposits to maintain a transaction record that contains information that can be applied to outstanding invoices and credit memos.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-104">You can make deposits to maintain a transaction record that contains information that can be applied to outstanding invoices and credit memos.</span></span>  

## <a name="to-create-a-deposit"></a><span data-ttu-id="2fcd8-105">To create a deposit</span><span class="sxs-lookup"><span data-stu-id="2fcd8-105">To create a deposit</span></span>  
1.  <span data-ttu-id="2fcd8-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Deposits**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Deposits**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2fcd8-107">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-107">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="2fcd8-108">On the **General** FastTab, fill in the required fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-108">On the **General** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="2fcd8-109">Field</span><span class="sxs-lookup"><span data-stu-id="2fcd8-109">Field</span></span>|<span data-ttu-id="2fcd8-110">Description</span><span class="sxs-lookup"><span data-stu-id="2fcd8-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |**<span data-ttu-id="2fcd8-111">No.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-111">No.</span></span>**|<span data-ttu-id="2fcd8-112">The unique identification number for the deposit.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-112">The unique identification number for the deposit.</span></span>|  
    |**<span data-ttu-id="2fcd8-113">Bank Account No.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-113">Bank Account No.</span></span>**|<span data-ttu-id="2fcd8-114">The bank account number for the deposit.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-114">The bank account number for the deposit.</span></span>|  
    |**<span data-ttu-id="2fcd8-115">Total Deposit Amount</span><span class="sxs-lookup"><span data-stu-id="2fcd8-115">Total Deposit Amount</span></span>**|<span data-ttu-id="2fcd8-116">The total deposit amount posted to the bank ledger.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-116">The total deposit amount posted to the bank ledger.</span></span><br /><br /> <span data-ttu-id="2fcd8-117">You can post this deposit only if the sum of the deposit lines is equal to the value in this field.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-117">You can post this deposit only if the sum of the deposit lines is equal to the value in this field.</span></span>|  
    |**<span data-ttu-id="2fcd8-118">Posting Date</span><span class="sxs-lookup"><span data-stu-id="2fcd8-118">Posting Date</span></span>**|<span data-ttu-id="2fcd8-119">The posting date for the deposit.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-119">The posting date for the deposit.</span></span>|  
    |**<span data-ttu-id="2fcd8-120">Document Date</span><span class="sxs-lookup"><span data-stu-id="2fcd8-120">Document Date</span></span>**|<span data-ttu-id="2fcd8-121">The deposit document date.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-121">The deposit document date.</span></span>|  
4.  <span data-ttu-id="2fcd8-122">On the **Lines** FastTab, fill in the required fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-122">On the **Lines** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="2fcd8-123">Field</span><span class="sxs-lookup"><span data-stu-id="2fcd8-123">Field</span></span>|<span data-ttu-id="2fcd8-124">Description</span><span class="sxs-lookup"><span data-stu-id="2fcd8-124">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |**<span data-ttu-id="2fcd8-125">Account Type</span><span class="sxs-lookup"><span data-stu-id="2fcd8-125">Account Type</span></span>**|<span data-ttu-id="2fcd8-126">The account type.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-126">The account type.</span></span>|  
    |**<span data-ttu-id="2fcd8-127">Account No.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-127">Account No.</span></span>**|<span data-ttu-id="2fcd8-128">The unique identification account number that is associated with the selected account type, to which the entry will be posted.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-128">The unique identification account number that is associated with the selected account type, to which the entry will be posted.</span></span>|  
    |**<span data-ttu-id="2fcd8-129">Description</span><span class="sxs-lookup"><span data-stu-id="2fcd8-129">Description</span></span>**|<span data-ttu-id="2fcd8-130">The journal line entry description.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-130">The journal line entry description.</span></span>|  
    |**<span data-ttu-id="2fcd8-131">Document Date</span><span class="sxs-lookup"><span data-stu-id="2fcd8-131">Document Date</span></span>**|<span data-ttu-id="2fcd8-132">The journal line entry document date.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-132">The journal line entry document date.</span></span>|  
    |**<span data-ttu-id="2fcd8-133">Document Type</span><span class="sxs-lookup"><span data-stu-id="2fcd8-133">Document Type</span></span>**|<span data-ttu-id="2fcd8-134">The journal line entry document type.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-134">The journal line entry document type.</span></span>|  
    |**<span data-ttu-id="2fcd8-135">Document No.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-135">Document No.</span></span>**|<span data-ttu-id="2fcd8-136">The journal line entry document number.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-136">The journal line entry document number.</span></span>|  
    |**<span data-ttu-id="2fcd8-137">Credit Amount</span><span class="sxs-lookup"><span data-stu-id="2fcd8-137">Credit Amount</span></span>**|<span data-ttu-id="2fcd8-138">The total credit amount on the journal line.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-138">The total credit amount on the journal line.</span></span>|  

5.  <span data-ttu-id="2fcd8-139">Optionally, on the **Navigate** tab, choose **Dimensions**, and then add relevant dimensions on the **Dimension Set Entries** page.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-139">Optionally, on the **Navigate** tab, choose **Dimensions**, and then add relevant dimensions on the **Dimension Set Entries** page.</span></span>  

<span data-ttu-id="2fcd8-140">After you have created a deposit, you must post it.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-140">After you have created a deposit, you must post it.</span></span>  

## <a name="to-post-a-deposit"></a><span data-ttu-id="2fcd8-141">To post a deposit</span><span class="sxs-lookup"><span data-stu-id="2fcd8-141">To post a deposit</span></span>  
1. <span data-ttu-id="2fcd8-142">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-142">Choose the **Post** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="2fcd8-143">You can post a deposit only if the amount displayed in the **Total Deposit Lines** field is equal to the amount in the **Total Deposit Amount** field.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-143">You can post a deposit only if the amount displayed in the **Total Deposit Lines** field is equal to the amount in the **Total Deposit Amount** field.</span></span>  

<span data-ttu-id="2fcd8-144">Next, you can use the Deposit Test Report and Deposit reports to reconcile your posted deposits with outstanding invoices and credit memos.</span><span class="sxs-lookup"><span data-stu-id="2fcd8-144">Next, you can use the Deposit Test Report and Deposit reports to reconcile your posted deposits with outstanding invoices and credit memos.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2fcd8-145">See Also</span><span class="sxs-lookup"><span data-stu-id="2fcd8-145">See Also</span></span>  
[<span data-ttu-id="2fcd8-146">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="2fcd8-146">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="2fcd8-147">Finance</span><span class="sxs-lookup"><span data-stu-id="2fcd8-147">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="2fcd8-148">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="2fcd8-148">Setting Up Finance</span></span>](../../finance.md)  
