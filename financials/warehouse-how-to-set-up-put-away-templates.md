---
title: How to Set Up Put-away Templates | Microsoft Docs
description: With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5a81b904a9180d7370a00f94a129ec707398e89a
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-put-away-templates"></a><span data-ttu-id="13037-103">How to: Set Up Put-away Templates</span><span class="sxs-lookup"><span data-stu-id="13037-103">How to: Set Up Put-away Templates</span></span>
<span data-ttu-id="13037-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span><span class="sxs-lookup"><span data-stu-id="13037-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="13037-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span><span class="sxs-lookup"><span data-stu-id="13037-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="13037-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span><span class="sxs-lookup"><span data-stu-id="13037-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="13037-107">To set up put-away templates</span><span class="sxs-lookup"><span data-stu-id="13037-107">To set up put-away templates</span></span>  
1.  <span data-ttu-id="13037-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Put-away Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="13037-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="13037-109">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="13037-109">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="13037-110">Enter a code that is the unique identifier of the template you are about to create.</span><span class="sxs-lookup"><span data-stu-id="13037-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4.  <span data-ttu-id="13037-111">Enter a short description, if you wish.</span><span class="sxs-lookup"><span data-stu-id="13037-111">Enter a short description, if you wish.</span></span>  
5.  <span data-ttu-id="13037-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span><span class="sxs-lookup"><span data-stu-id="13037-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>  
6.  <span data-ttu-id="13037-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span><span class="sxs-lookup"><span data-stu-id="13037-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="13037-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span><span class="sxs-lookup"><span data-stu-id="13037-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7.  <span data-ttu-id="13037-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span><span class="sxs-lookup"><span data-stu-id="13037-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8.  <span data-ttu-id="13037-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="13037-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="13037-117">You can create various put-away templates and then apply them as you see fit.</span><span class="sxs-lookup"><span data-stu-id="13037-117">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="13037-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span><span class="sxs-lookup"><span data-stu-id="13037-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="13037-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span><span class="sxs-lookup"><span data-stu-id="13037-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="13037-120">See Also</span><span class="sxs-lookup"><span data-stu-id="13037-120">See Also</span></span>  
[<span data-ttu-id="13037-121">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="13037-121">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="13037-122">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="13037-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="13037-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="13037-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="13037-124">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="13037-124">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="13037-125">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="13037-125">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="13037-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="13037-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
