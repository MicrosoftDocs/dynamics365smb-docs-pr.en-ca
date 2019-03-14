---
title: How to Flush Components According to Operation Output | Microsoft Docs
description: For items that are set up with backward flushing method, the default behaviour is to calculate and post component consumption when you change the status of a released production order to **Finished**. For more information, see Flushing Method.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: f61e3150f1978795a20d4ad68656d6d1e72402a0
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="flush-components-according-to-operation-output"></a><span data-ttu-id="53569-104">Flush Components According to Operation Output</span><span class="sxs-lookup"><span data-stu-id="53569-104">Flush Components According to Operation Output</span></span>
<span data-ttu-id="53569-105">For items that are set up with backward flushing method, the default behaviour is to calculate and post component consumption when you change the status of a released production order to **Finished**.</span><span class="sxs-lookup"><span data-stu-id="53569-105">For items that are set up with backward flushing method, the default behavior is to calculate and post component consumption when you change the status of a released production order to **Finished**.</span></span>  

<span data-ttu-id="53569-106">If you also define routing link codes, then calculation and posting occurs when each operation is finished, and the quantity that was actually consumed in the operation is posted.</span><span class="sxs-lookup"><span data-stu-id="53569-106">If you also define routing link codes, then calculation and posting occurs when each operation is finished, and the quantity that was actually consumed in the operation is posted.</span></span> <span data-ttu-id="53569-107">For more information, see [Create Routings](production-how-to-create-routings.md).</span><span class="sxs-lookup"><span data-stu-id="53569-107">For more information, see [Create Routings](production-how-to-create-routings.md).</span></span>  

<span data-ttu-id="53569-108">For example, if a production order to produce 800 meters requires 8 kg of a component, then when you post 200 meters as output, 2 kg are automatically posted as consumption.</span><span class="sxs-lookup"><span data-stu-id="53569-108">For example, if a production order to produce 800 meters requires 8 kg of a component, then when you post 200 meters as output, 2 kg are automatically posted as consumption.</span></span>  

<span data-ttu-id="53569-109">This functionality is useful for the following reasons:</span><span class="sxs-lookup"><span data-stu-id="53569-109">This functionality is useful for the following reasons:</span></span>  

-   <span data-ttu-id="53569-110">**Inventory Valuation** - Value entries for output and consumption are created in parallel as the production order progresses.</span><span class="sxs-lookup"><span data-stu-id="53569-110">**Inventory Valuation** - Value entries for output and consumption are created in parallel as the production order progresses.</span></span> <span data-ttu-id="53569-111">Without routing link codes, the inventory value will increase as output is posted and then decrease at a later point in time when the value of component consumption is posted together with the finished production order.</span><span class="sxs-lookup"><span data-stu-id="53569-111">Without routing link codes, the inventory value will increase as output is posted and then decrease at a later point in time when the value of component consumption is posted together with the finished production order.</span></span>  
-   <span data-ttu-id="53569-112">**Inventory Availability** - With gradual consumption posting, the availability of component items is more up-to-date, which is important to maintain the internal balance between demand and supply.</span><span class="sxs-lookup"><span data-stu-id="53569-112">**Inventory Availability** - With gradual consumption posting, the availability of component items is more up-to-date, which is important to maintain the internal balance between demand and supply.</span></span> <span data-ttu-id="53569-113">Without routing link codes, other demands for the component may believe that it is available as long as it is pending a delayed consumption posting.</span><span class="sxs-lookup"><span data-stu-id="53569-113">Without routing link codes, other demands for the component may believe that it is available as long as it is pending a delayed consumption posting.</span></span>  
-   <span data-ttu-id="53569-114">**Just-in-Time** – With the ability to customize products to customer requests, you can minimize waste by making sure that work and system changes only occur when it is necessary.</span><span class="sxs-lookup"><span data-stu-id="53569-114">**Just-in-Time** – With the ability to customize products to customer requests, you can minimize waste by making sure that work and system changes only occur when it is necessary.</span></span>  

<span data-ttu-id="53569-115">The following procedure shows how to combine backward flushing and routing link codes so that the quantity that is flushed for each operation is proportional to the actual output of the finished operation.</span><span class="sxs-lookup"><span data-stu-id="53569-115">The following procedure shows how to combine backward flushing and routing link codes so that the quantity that is flushed for each operation is proportional to the actual output of the finished operation.</span></span>  

## <a name="to-flush-components-according-to-operation-output"></a><span data-ttu-id="53569-116">To flush components according to operation output</span><span class="sxs-lookup"><span data-stu-id="53569-116">To flush components according to operation output</span></span>  
1.  <span data-ttu-id="53569-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="53569-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="53569-118">Choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="53569-118">Choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="53569-119">On the **Replenishment** FastTab, in the **Flushing Method** field, select **Forward**.</span><span class="sxs-lookup"><span data-stu-id="53569-119">On the **Replenishment** FastTab, in the **Flushing Method** field, select **Forward**.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="53569-120">Select **Pick+ Forward** if the component is used in a location that is set up for directed put-away and pick.</span><span class="sxs-lookup"><span data-stu-id="53569-120">Select **Pick+ Forward** if the component is used in a location that is set up for directed put-away and pick.</span></span>  

4.  <span data-ttu-id="53569-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="53569-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span></span>  
5.  <span data-ttu-id="53569-122">Define routing link codes for every operation that consumes the component.</span><span class="sxs-lookup"><span data-stu-id="53569-122">Define routing link codes for every operation that consumes the component.</span></span> <span data-ttu-id="53569-123">For more information, see [Create Routings ](production-how-to-create-routings.md).</span><span class="sxs-lookup"><span data-stu-id="53569-123">For more information, see [Create Routings ](production-how-to-create-routings.md).</span></span>  
6.  <span data-ttu-id="53569-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Production BOM**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="53569-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Production BOM**, and then choose the related link.</span></span>  
7.  <span data-ttu-id="53569-125">Define routing link codes from each instance of the component to the operation where it is consumed.</span><span class="sxs-lookup"><span data-stu-id="53569-125">Define routing link codes from each instance of the component to the operation where it is consumed.</span></span>

    > [!IMPORTANT]  
    >  <span data-ttu-id="53569-126">The component must have a routing link to the last operation in the routing.</span><span class="sxs-lookup"><span data-stu-id="53569-126">The component must have a routing link to the last operation in the routing.</span></span>  

## <a name="see-also"></a><span data-ttu-id="53569-127">See Also</span><span class="sxs-lookup"><span data-stu-id="53569-127">See Also</span></span>  
[<span data-ttu-id="53569-128">Create Production BOMs</span><span class="sxs-lookup"><span data-stu-id="53569-128">Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="53569-129">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="53569-129">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="53569-130">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="53569-130">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="53569-131">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="53569-131">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="53569-132">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="53569-132">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="53569-133">Purchasing</span><span class="sxs-lookup"><span data-stu-id="53569-133">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="53569-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="53569-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
