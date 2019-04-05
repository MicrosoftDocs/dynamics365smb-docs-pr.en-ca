---
title: Amend or Cancel Unpaid Purchase Invoices | Microsoft Docs
description: Explains how to correct, cancel, or undo a posted purchase invoice and automatically create a purchase credit memo.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 275b81fa2f4170208b166645a9b8778c1e6406a5
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/08/2019
ms.locfileid: "811825"
---
# <a name="correct-or-cancel-unpaid-purchase-invoices"></a><span data-ttu-id="fa59b-103">Correct or Cancel Unpaid Purchase Invoices</span><span class="sxs-lookup"><span data-stu-id="fa59b-103">Correct or Cancel Unpaid Purchase Invoices</span></span>
<span data-ttu-id="fa59b-104">You can correct or cancel a posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="fa59b-104">You can correct or cancel a posted purchase invoice.</span></span> <span data-ttu-id="fa59b-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span><span class="sxs-lookup"><span data-stu-id="fa59b-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span></span>

<span data-ttu-id="fa59b-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span><span class="sxs-lookup"><span data-stu-id="fa59b-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span></span> <span data-ttu-id="fa59b-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span><span class="sxs-lookup"><span data-stu-id="fa59b-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span></span> <span data-ttu-id="fa59b-108">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="fa59b-108">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span></span>

<span data-ttu-id="fa59b-109">On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button.</span><span class="sxs-lookup"><span data-stu-id="fa59b-109">On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button.</span></span> <span data-ttu-id="fa59b-110">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span><span class="sxs-lookup"><span data-stu-id="fa59b-110">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span></span> <span data-ttu-id="fa59b-111">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span><span class="sxs-lookup"><span data-stu-id="fa59b-111">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span></span> <span data-ttu-id="fa59b-112">In the following the use of **Correct** and **Cancel** is described.</span><span class="sxs-lookup"><span data-stu-id="fa59b-112">In the following the use of **Correct** and **Cancel** is described.</span></span>

## <a name="to-correct-a-posted-purchase-invoice"></a><span data-ttu-id="fa59b-113">To correct a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="fa59b-113">To correct a posted purchase invoice</span></span>
1. <span data-ttu-id="fa59b-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fa59b-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fa59b-115">Select the posted purchase invoice that you want to correct.</span><span class="sxs-lookup"><span data-stu-id="fa59b-115">Select the posted purchase invoice that you want to correct.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="fa59b-116">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span><span class="sxs-lookup"><span data-stu-id="fa59b-116">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="fa59b-117">On the **Posted Purchase Invoice** page, choose **Correct**.</span><span class="sxs-lookup"><span data-stu-id="fa59b-117">On the **Posted Purchase Invoice** page, choose **Correct**.</span></span>

    <span data-ttu-id="fa59b-118">A new purchase invoice with the same information is created where you can make the correction.</span><span class="sxs-lookup"><span data-stu-id="fa59b-118">A new purchase invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="fa59b-119">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="fa59b-119">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span> <span data-ttu-id="fa59b-120">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="fa59b-120">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>

    <span data-ttu-id="fa59b-121">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="fa59b-121">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span>
4. <span data-ttu-id="fa59b-122">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="fa59b-122">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="to-cancel-a-posted-purchase-invoice"></a><span data-ttu-id="fa59b-123">To cancel a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="fa59b-123">To cancel a posted purchase invoice</span></span>
1. <span data-ttu-id="fa59b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fa59b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fa59b-125">Select the posted purchase invoice that you want to cancel.</span><span class="sxs-lookup"><span data-stu-id="fa59b-125">Select the posted purchase invoice that you want to cancel.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="fa59b-126">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span><span class="sxs-lookup"><span data-stu-id="fa59b-126">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="fa59b-127">On the **Posted Purchase Invoice** page, choose **Cancel**.</span><span class="sxs-lookup"><span data-stu-id="fa59b-127">On the **Posted Purchase Invoice** page, choose **Cancel**.</span></span>

    <span data-ttu-id="fa59b-128">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="fa59b-128">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span> <span data-ttu-id="fa59b-129">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="fa59b-129">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>
4. <span data-ttu-id="fa59b-130">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="fa59b-130">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="see-also"></a><span data-ttu-id="fa59b-131">See Also</span><span class="sxs-lookup"><span data-stu-id="fa59b-131">See Also</span></span>
[<span data-ttu-id="fa59b-132">Purchasing</span><span class="sxs-lookup"><span data-stu-id="fa59b-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="fa59b-133">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="fa59b-133">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
<span data-ttu-id="fa59b-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fa59b-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
