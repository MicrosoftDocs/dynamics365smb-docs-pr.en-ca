---
title: How to Convert Existing Locations to Warehouse Locations | Microsoft Docs
description: You can enable an existing inventory location to use zones and bins and to operate as a warehouse location.
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
ms.openlocfilehash: 7d4b2c86174386faa86ab6c09faa463d26d3d2ac
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="convert-existing-locations-to-warehouse-locations"></a><span data-ttu-id="2e4e0-103">Convert Existing Locations to Warehouse Locations</span><span class="sxs-lookup"><span data-stu-id="2e4e0-103">Convert Existing Locations to Warehouse Locations</span></span>
<span data-ttu-id="2e4e0-104">You can enable an existing inventory location to use zones and bins and to operate as a warehouse location.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-104">You can enable an existing inventory location to use zones and bins and to operate as a warehouse location.</span></span>  

<span data-ttu-id="2e4e0-105">The batch job to enable a location for warehouse operation creates initial warehouse entries for the warehouse adjustment bin for all items that have inventory in the location.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-105">The batch job to enable a location for warehouse operation creates initial warehouse entries for the warehouse adjustment bin for all items that have inventory in the location.</span></span> <span data-ttu-id="2e4e0-106">These initial entries will be balanced when warehouse physical inventory entries are entered after the batch job is run.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-106">These initial entries will be balanced when warehouse physical inventory entries are entered after the batch job is run.</span></span>  

<span data-ttu-id="2e4e0-107">You can create zones and bins either before or after the conversion.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-107">You can create zones and bins either before or after the conversion.</span></span> <span data-ttu-id="2e4e0-108">The only bin that you must create before the conversion is the one that is to be used as the future adjustment bin.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-108">The only bin that you must create before the conversion is the one that is to be used as the future adjustment bin.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="2e4e0-109">To clear all negative inventory and any open warehouse documents before you convert the location for warehouse handling, run a report to identify the items with negative inventory and open warehouse documents for the location.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-109">To clear all negative inventory and any open warehouse documents before you convert the location for warehouse handling, run a report to identify the items with negative inventory and open warehouse documents for the location.</span></span> <span data-ttu-id="2e4e0-110">For more information, see Check on Negative Inventory.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-110">For more information, see Check on Negative Inventory.</span></span>  

## <a name="to-enable-an-existing-location-to-operate-as-a-warehouse-location"></a><span data-ttu-id="2e4e0-111">To enable an existing location to operate as a warehouse location</span><span class="sxs-lookup"><span data-stu-id="2e4e0-111">To enable an existing location to operate as a warehouse location</span></span>  
1.  <span data-ttu-id="2e4e0-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Warehouse Location**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Warehouse Location**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2e4e0-113">In the **Location Code** field, specify the location that you want to enable for warehouse processing.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-113">In the **Location Code** field, specify the location that you want to enable for warehouse processing.</span></span>  
3.  <span data-ttu-id="2e4e0-114">In the **Adjustment Bin Code** field, specify the bin at the location where unsynchronized warehouse entries are stored.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-114">In the **Adjustment Bin Code** field, specify the bin at the location where unsynchronized warehouse entries are stored.</span></span> <span data-ttu-id="2e4e0-115">For more information, see the "To synchronize the adjusted warehouse entries with the related item ledger entries" section in [Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).</span><span class="sxs-lookup"><span data-stu-id="2e4e0-115">For more information, see the "To synchronize the adjusted warehouse entries with the related item ledger entries" section in [Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).</span></span>  

    <span data-ttu-id="2e4e0-116">Using the open item ledger entries for the specified location, warehouse journal lines are created that sum up every combination of Item No., Variant Code, Unit of Measure Code, and, if necessary, Lot No. and Serial No. in the item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-116">Using the open item ledger entries for the specified location, warehouse journal lines are created that sum up every combination of Item No., Variant Code, Unit of Measure Code, and, if necessary, Lot No. and Serial No. in the item ledger entries.</span></span> <span data-ttu-id="2e4e0-117">The warehouse journal lines are then posted.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-117">The warehouse journal lines are then posted.</span></span> <span data-ttu-id="2e4e0-118">This posting creates warehouse entries that place the inventory in the warehouse adjustment bin.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-118">This posting creates warehouse entries that place the inventory in the warehouse adjustment bin.</span></span> <span data-ttu-id="2e4e0-119">The **Adjustment Bin Code** on the location card is also set.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-119">The **Adjustment Bin Code** on the location card is also set.</span></span>  

4.  <span data-ttu-id="2e4e0-120">To see which items were added to the adjustment bin during the batch job, run the **Warehouse Adjustment Bin** report.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-120">To see which items were added to the adjustment bin during the batch job, run the **Warehouse Adjustment Bin** report.</span></span>  
5.  <span data-ttu-id="2e4e0-121">When the **Create Warehouse Location** batch job has completed, perform and post a warehouse physical inventory.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-121">When the **Create Warehouse Location** batch job has completed, perform and post a warehouse physical inventory.</span></span> <span data-ttu-id="2e4e0-122">For more information, see [Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).</span><span class="sxs-lookup"><span data-stu-id="2e4e0-122">For more information, see [Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2e4e0-123">It is recommended that you run the **Create Warehouse Location** batch job at a time when it will not impact the daily work in the system.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-123">It is recommended that you run the **Create Warehouse Location** batch job at a time when it will not impact the daily work in the system.</span></span> <span data-ttu-id="2e4e0-124">This job processes each entry in the **Item Ledger Entry** table, and if there are a large number of item ledger entries, the job can last several hours.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-124">This job processes each entry in the **Item Ledger Entry** table, and if there are a large number of item ledger entries, the job can last several hours.</span></span>  

 <span data-ttu-id="2e4e0-125">For those locations that did not use warehouse management documents before the conversion, you must re-open and release any source documents that were partially received or partially shipped before the conversion.</span><span class="sxs-lookup"><span data-stu-id="2e4e0-125">For those locations that did not use warehouse management documents before the conversion, you must re-open and release any source documents that were partially received or partially shipped before the conversion.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2e4e0-126">See Also</span><span class="sxs-lookup"><span data-stu-id="2e4e0-126">See Also</span></span>  
[<span data-ttu-id="2e4e0-127">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="2e4e0-127">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="2e4e0-128">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="2e4e0-128">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="2e4e0-129">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="2e4e0-129">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="2e4e0-130">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="2e4e0-130">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="2e4e0-131">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="2e4e0-131">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="2e4e0-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2e4e0-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
