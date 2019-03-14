---
title: Move Items | Microsoft Docs
description: While in inventory, items may need to be moved between bins to support the daily warehouse activities involved in keeping items flowing through the warehouse. Some movements happen in direct relation to internal operations, such as a production order that needs components delivered or end items put away. Other movements happen as mere warehouse space optimization or as ad-hoc movements to and from operations.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: c31f41eedea63c61d3ca9484d64f8156ab485181
ms.contentlocale: en-ca
ms.lasthandoff: 09/28/2018

---
# <a name="moving-items"></a><span data-ttu-id="fc732-105">Moving Items</span><span class="sxs-lookup"><span data-stu-id="fc732-105">Moving Items</span></span>
<span data-ttu-id="fc732-106">The warehouse activity of moving items within the warehouse is performed in different ways depending on how warehouse management features are configured.</span><span class="sxs-lookup"><span data-stu-id="fc732-106">The warehouse activity of moving items within the warehouse is performed in different ways depending on how warehouse management features are configured.</span></span> <span data-ttu-id="fc732-107">The complexity can rank from no warehouse features, through basic warehouse configurations for order-by order handling in one or more activities only, to advanced configurations where all warehouse activities must be performed in a directed workflow.</span><span class="sxs-lookup"><span data-stu-id="fc732-107">The complexity can rank from no warehouse features, through basic warehouse configurations for order-by order handling in one or more activities only, to advanced configurations where all warehouse activities must be performed in a directed workflow.</span></span> <span data-ttu-id="fc732-108">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-108">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

<span data-ttu-id="fc732-109">While in one warehouse location, items may need to be moved between bins to support the daily warehouse activities involved in keeping items flowing through the warehouse.</span><span class="sxs-lookup"><span data-stu-id="fc732-109">While in one warehouse location, items may need to be moved between bins to support the daily warehouse activities involved in keeping items flowing through the warehouse.</span></span> <span data-ttu-id="fc732-110">Some movements happen in direct relation to internal operations, such as a production order that needs components delivered or end items put away.</span><span class="sxs-lookup"><span data-stu-id="fc732-110">Some movements happen in direct relation to internal operations, such as a production order that needs components delivered or end items put away.</span></span> <span data-ttu-id="fc732-111">Other movements happen as mere warehouse space optimization or as ad-hoc movements to and from operations.</span><span class="sxs-lookup"><span data-stu-id="fc732-111">Other movements happen as mere warehouse space optimization or as ad-hoc movements to and from operations.</span></span>

<span data-ttu-id="fc732-112">Moving items to other locations affects the item ledger entries and must therefore be done by transfer order.</span><span class="sxs-lookup"><span data-stu-id="fc732-112">Moving items to other locations affects the item ledger entries and must therefore be done by transfer order.</span></span> <span data-ttu-id="fc732-113">For more information, see [Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-113">For more information, see [Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>  

<span data-ttu-id="fc732-114">Additional movement tasks are to periodically replenish picking bins or shop floor bins and to modify bin content information.</span><span class="sxs-lookup"><span data-stu-id="fc732-114">Additional movement tasks are to periodically replenish picking bins or shop floor bins and to modify bin content information.</span></span>  

 <span data-ttu-id="fc732-115">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="fc732-115">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="fc732-116">**To**</span><span class="sxs-lookup"><span data-stu-id="fc732-116">**To**</span></span>|<span data-ttu-id="fc732-117">**See**</span><span class="sxs-lookup"><span data-stu-id="fc732-117">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="fc732-118">Move items between bins in basic warehouse configurations at any time and without source documents.</span><span class="sxs-lookup"><span data-stu-id="fc732-118">Move items between bins in basic warehouse configurations at any time and without source documents.</span></span>|[<span data-ttu-id="fc732-119">Move Items in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="fc732-119">Move Items in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)|
|<span data-ttu-id="fc732-120">Use the warehouse movement worksheet to move items in advanced warehouse configurations, both for source documents and ad hoc.</span><span class="sxs-lookup"><span data-stu-id="fc732-120">Use the warehouse movement worksheet to move items in advanced warehouse configurations, both for source documents and ad hoc.</span></span>|[<span data-ttu-id="fc732-121">Move Items in Advanced Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="fc732-121">Move Items in Advanced Warehouse Configurations</span></span>](warehouse-how-to-move-items-in-advanced-warehousing.md)|  
|<span data-ttu-id="fc732-122">Bring component items to internal operations in basic warehouse configurations as requested by source documents for those operations.</span><span class="sxs-lookup"><span data-stu-id="fc732-122">Bring component items to internal operations in basic warehouse configurations as requested by source documents for those operations.</span></span>|[<span data-ttu-id="fc732-123">Move Components to an Operation Area in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="fc732-123">Move Components to an Operation Area in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)|
|<span data-ttu-id="fc732-124">Plan which bins to fill or empty to maintain an efficient flow, such as emptying a bulk storage area before a large receipt.</span><span class="sxs-lookup"><span data-stu-id="fc732-124">Plan which bins to fill or empty to maintain an efficient flow, such as emptying a bulk storage area before a large receipt.</span></span>|[<span data-ttu-id="fc732-125">Plan Warehouse Movements in Worksheets</span><span class="sxs-lookup"><span data-stu-id="fc732-125">Plan Warehouse Movements in Worksheets</span></span>](warehouse-how-to-plan-warehouse-movements-in-worksheets.md)|
|<span data-ttu-id="fc732-126">Update the frequency at which bins, such as picking bins, must be replenished as a result of demand fluctuations.</span><span class="sxs-lookup"><span data-stu-id="fc732-126">Update the frequency at which bins, such as picking bins, must be replenished as a result of demand fluctuations.</span></span>|[<span data-ttu-id="fc732-127">Calculate Bin Replenishment</span><span class="sxs-lookup"><span data-stu-id="fc732-127">Calculate Bin Replenishment</span></span>](warehouse-how-to-calculate-bin-replenishment.md)|
|<span data-ttu-id="fc732-128">Restructure your warehouse with new bin codes and new bin characteristics and potentially move them around.</span><span class="sxs-lookup"><span data-stu-id="fc732-128">Restructure your warehouse with new bin codes and new bin characteristics and potentially move them around.</span></span>|[<span data-ttu-id="fc732-129">Restructure Warehouses</span><span class="sxs-lookup"><span data-stu-id="fc732-129">Restructure Warehouses</span></span>](warehouse-how-to-restructure-warehouses.md)|  

## <a name="see-also"></a><span data-ttu-id="fc732-130">See Also</span><span class="sxs-lookup"><span data-stu-id="fc732-130">See Also</span></span>  
[<span data-ttu-id="fc732-131">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="fc732-131">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="fc732-132">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="fc732-132">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="fc732-133">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="fc732-133">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="fc732-134">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="fc732-134">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="fc732-135">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="fc732-135">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="fc732-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fc732-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
