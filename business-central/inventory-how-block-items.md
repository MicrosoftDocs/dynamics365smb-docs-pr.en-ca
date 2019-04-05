---
title: How to Block Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 0d5ad688cfa6fb58e8383692362105beeee386f8
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/08/2019
ms.locfileid: "811514"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="c61a9-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="c61a9-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="c61a9-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="c61a9-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="c61a9-105">The following table illustrates what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="c61a9-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="c61a9-106">Option</span><span class="sxs-lookup"><span data-stu-id="c61a9-106">Option</span></span>|<span data-ttu-id="c61a9-107">Description</span><span class="sxs-lookup"><span data-stu-id="c61a9-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="c61a9-108">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="c61a9-108">**Sales Blocked**</span></span>|<span data-ttu-id="c61a9-109">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="c61a9-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="c61a9-110">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="c61a9-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="c61a9-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="c61a9-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="c61a9-112">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="c61a9-112">**Blocked**</span></span>|<span data-ttu-id="c61a9-113">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="c61a9-113">You cannot use the item for any item transaction.</span></span> <span data-ttu-id="c61a9-114">For more information about blocking an item for all purposes, see Item Card.</span><span class="sxs-lookup"><span data-stu-id="c61a9-114">For more information about blocking an item for all purposes, see Item Card.</span></span>|  

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="c61a9-115">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="c61a9-115">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="c61a9-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c61a9-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c61a9-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="c61a9-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="c61a9-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="c61a9-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="c61a9-119">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="c61a9-119">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="c61a9-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c61a9-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c61a9-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="c61a9-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="c61a9-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="c61a9-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="c61a9-123">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="c61a9-123">To block an item from being posted</span></span>
1. <span data-ttu-id="c61a9-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c61a9-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="c61a9-125">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="c61a9-125">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="c61a9-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="c61a9-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="c61a9-127">See Also</span><span class="sxs-lookup"><span data-stu-id="c61a9-127">See Also</span></span>  
[<span data-ttu-id="c61a9-128">Register New Items</span><span class="sxs-lookup"><span data-stu-id="c61a9-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="c61a9-129">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="c61a9-129">Inventory</span></span>](inventory-manage-inventory.md)  
