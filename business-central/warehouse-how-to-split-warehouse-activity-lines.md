---
title: How to Split Warehouse Activity Lines | Microsoft Docs
description: In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items. The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity. In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.
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
ms.openlocfilehash: 821d3bed8e90d7221fe343156b46663cdf601dcf
ms.contentlocale: en-ca
ms.lasthandoff: 09/28/2018

---
# <a name="split-warehouse-activity-lines"></a><span data-ttu-id="bc5fe-105">Split Warehouse Activity Lines</span><span class="sxs-lookup"><span data-stu-id="bc5fe-105">Split Warehouse Activity Lines</span></span>
<span data-ttu-id="bc5fe-106">In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-106">In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items.</span></span> <span data-ttu-id="bc5fe-107">The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-107">The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity.</span></span> <span data-ttu-id="bc5fe-108">In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-108">In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.</span></span>  

<span data-ttu-id="bc5fe-109">The following procedure applies to warehouse documents, such as warehouse put-away, movement, and pick lines, or inventory put-away, movement, and pick lines.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-109">The following procedure applies to warehouse documents, such as warehouse put-away, movement, and pick lines, or inventory put-away, movement, and pick lines.</span></span>  

## <a name="to-split-warehouse-activity-lines"></a><span data-ttu-id="bc5fe-110">To split warehouse activity lines</span><span class="sxs-lookup"><span data-stu-id="bc5fe-110">To split warehouse activity lines</span></span>  
1.  <span data-ttu-id="bc5fe-111">Open a warehouse activity line where you are trying to handle an insufficient quantity.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-111">Open a warehouse activity line where you are trying to handle an insufficient quantity.</span></span>  
2.  <span data-ttu-id="bc5fe-112">In the **Qty. to Handle** field, enter the reduced quantity that you are able to handle.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-112">In the **Qty. to Handle** field, enter the reduced quantity that you are able to handle.</span></span>  
3.  <span data-ttu-id="bc5fe-113">On the **Lines** FastTab, choose the **Actions** action, choose the **Functions** action, and then choose the **Split Line** action.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-113">On the **Lines** FastTab, choose the **Actions** action, choose the **Functions** action, and then choose the **Split Line** action.</span></span> <span data-ttu-id="bc5fe-114">A new line appears, which is a copy of the original line, except that the **Qty. to Handle** field contains the quantity that you removed from the original line.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-114">A new line appears, which is a copy of the original line, except that the **Qty. to Handle** field contains the quantity that you removed from the original line.</span></span>  
4.  <span data-ttu-id="bc5fe-115">Assign an appropriate bin and, if you are using directed put-away and pick, a zone, to this new line, or continue splitting the line as necessary until you find appropriate bins for all of the quantity.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-115">Assign an appropriate bin and, if you are using directed put-away and pick, a zone, to this new line, or continue splitting the line as necessary until you find appropriate bins for all of the quantity.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="bc5fe-116">If the location uses directed put-away and pick and you split the lines, you must be familiar with the warehouse and be able to choose a bin that matches the storage requirements of the item and that fulfills the general requirements of the warehouse document.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-116">If the location uses directed put-away and pick and you split the lines, you must be familiar with the warehouse and be able to choose a bin that matches the storage requirements of the item and that fulfills the general requirements of the warehouse document.</span></span> <span data-ttu-id="bc5fe-117">For example, you would not split a line on a pick document and place some items in the bulk storage.</span><span class="sxs-lookup"><span data-stu-id="bc5fe-117">For example, you would not split a line on a pick document and place some items in the bulk storage.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bc5fe-118">See Also</span><span class="sxs-lookup"><span data-stu-id="bc5fe-118">See Also</span></span>  
[<span data-ttu-id="bc5fe-119">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="bc5fe-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="bc5fe-120">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="bc5fe-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="bc5fe-121">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="bc5fe-121">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="bc5fe-122">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="bc5fe-122">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="bc5fe-123">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="bc5fe-123">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="bc5fe-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bc5fe-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
