---
title: How to Set Up Cost Centres | Microsoft Docs
description: Cost centres are departments that are responsible for costs and income. The chart of cost centres is similar to the dimension information for the general ledger.
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 433526fbd2a13f32e64be94cc1936151445c19f5
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-cost-centers"></a><span data-ttu-id="b6755-104">How to: Set Up Cost centres</span><span class="sxs-lookup"><span data-stu-id="b6755-104">How to: Set Up Cost Centers</span></span>
<span data-ttu-id="b6755-105">Cost centers are departments that are responsible for costs and income.</span><span class="sxs-lookup"><span data-stu-id="b6755-105">Cost centers are departments that are responsible for costs and income.</span></span> <span data-ttu-id="b6755-106">The chart of cost centres is similar to the dimension information for the general ledger.</span><span class="sxs-lookup"><span data-stu-id="b6755-106">The chart of cost centers is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="b6755-107">You can set up the chart of cost centres in the following ways:</span><span class="sxs-lookup"><span data-stu-id="b6755-107">You can set up the chart of cost centers in the following ways:</span></span>  

-   <span data-ttu-id="b6755-108">Transfer dimension values in the general ledger to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="b6755-108">Transfer dimension values in the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="b6755-109">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="b6755-109">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="b6755-110">Create a new chart of cost centre that is independent of the general ledger or add a new cost centre to an existing chart of cost centre.</span><span class="sxs-lookup"><span data-stu-id="b6755-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span></span> <span data-ttu-id="b6755-111">You must create each cost centre individually.</span><span class="sxs-lookup"><span data-stu-id="b6755-111">You must create each cost center individually.</span></span>  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a><span data-ttu-id="b6755-112">To transfer dimension values in the general ledger to the chart of cost centres</span><span class="sxs-lookup"><span data-stu-id="b6755-112">To transfer dimension values in the general ledger to the chart of cost centers</span></span>  
1.  <span data-ttu-id="b6755-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span><span class="sxs-lookup"><span data-stu-id="b6755-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span></span> <span data-ttu-id="b6755-114">Only the values from this dimension are transferred.</span><span class="sxs-lookup"><span data-stu-id="b6755-114">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="b6755-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Centres**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b6755-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Centers**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="b6755-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost centres from Dimension** to transfer dimension values to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="b6755-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span></span> <span data-ttu-id="b6755-117">The function transfers the dimension values that you defined in step 1.</span><span class="sxs-lookup"><span data-stu-id="b6755-117">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="b6755-118">You can set up the **Align Cost Centre Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="b6755-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="b6755-119">You cannot define a synchronization of the chart of cost centres to dimension values from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="b6755-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span></span>  

<span data-ttu-id="b6755-120">The chart of cost centres now contains all specified dimension values from the general ledger and includes titles and subtotals.</span><span class="sxs-lookup"><span data-stu-id="b6755-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-window"></a><span data-ttu-id="b6755-121">To create new cost centers in the Chart of Cost Centers window</span><span class="sxs-lookup"><span data-stu-id="b6755-121">To create new cost centers in the Chart of Cost Centers window</span></span>  
<span data-ttu-id="b6755-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span><span class="sxs-lookup"><span data-stu-id="b6755-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span></span> <span data-ttu-id="b6755-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span><span class="sxs-lookup"><span data-stu-id="b6755-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span></span>  

1. <span data-ttu-id="b6755-124">Open the **Chart of Cost Centers** window in edit mode.</span><span class="sxs-lookup"><span data-stu-id="b6755-124">Open the **Chart of Cost Centers** window in edit mode.</span></span>  
2. <span data-ttu-id="b6755-125">In the **Code** field, enter the cost center code.</span><span class="sxs-lookup"><span data-stu-id="b6755-125">In the **Code** field, enter the cost center code.</span></span> <span data-ttu-id="b6755-126">All cost centres must have a code.</span><span class="sxs-lookup"><span data-stu-id="b6755-126">All cost centers must have a code.</span></span>  
3. <span data-ttu-id="b6755-127">In the **Name** field, enter the cost center name.</span><span class="sxs-lookup"><span data-stu-id="b6755-127">In the **Name** field, enter the cost center name.</span></span>  
4. <span data-ttu-id="b6755-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost centre.</span><span class="sxs-lookup"><span data-stu-id="b6755-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span></span>  

    - <span data-ttu-id="b6755-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span><span class="sxs-lookup"><span data-stu-id="b6755-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span></span> <span data-ttu-id="b6755-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span><span class="sxs-lookup"><span data-stu-id="b6755-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span></span>  
    - <span data-ttu-id="b6755-131">For cost centres of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span><span class="sxs-lookup"><span data-stu-id="b6755-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span></span>  
5.  <span data-ttu-id="b6755-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span><span class="sxs-lookup"><span data-stu-id="b6755-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span></span>  
6.  <span data-ttu-id="b6755-133">Choose the next empty line to create a new cost centre, and then repeat steps 2 through 5.</span><span class="sxs-lookup"><span data-stu-id="b6755-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="b6755-134">After you have set up all the cost centres, choose the **Indent Cost Centres** action.</span><span class="sxs-lookup"><span data-stu-id="b6755-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span></span> <span data-ttu-id="b6755-135">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="b6755-135">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="b6755-136">If you have entered definitions in the **Totalling** fields for **End-Total** cost centres before you run the indent function, then you must enter them again.</span><span class="sxs-lookup"><span data-stu-id="b6755-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="b6755-137">The function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="b6755-137">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b6755-138">See Also</span><span class="sxs-lookup"><span data-stu-id="b6755-138">See Also</span></span>  
[<span data-ttu-id="b6755-139">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="b6755-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="b6755-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="b6755-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="b6755-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="b6755-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="b6755-142">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="b6755-142">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="b6755-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b6755-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

