---
title: Analyse Data by Dimensions| Microsoft Docs
description: Describes how to analyse various business data by dimensions.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 11/13/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: bfb5ce68e4570f4d96a4216ea01f9d1ecc3bc623
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
#  <a name="analyze-data-by-dimensions"></a><span data-ttu-id="b9b43-103">Analyse Data by Dimensions</span><span class="sxs-lookup"><span data-stu-id="b9b43-103">Analyze Data by Dimensions</span></span>
<span data-ttu-id="b9b43-104">In financial analysis, a dimension is data that you can add to an entry as a kind of marker.</span><span class="sxs-lookup"><span data-stu-id="b9b43-104">In financial analysis, a dimension is data that you can add to an entry as a kind of marker.</span></span> <span data-ttu-id="b9b43-105">This data is used to group entries with similar characteristics, such as customers, regions, products, and salesperson, and easily retrieve these groups for analysis.</span><span class="sxs-lookup"><span data-stu-id="b9b43-105">This data is used to group entries with similar characteristics, such as customers, regions, products, and salesperson, and easily retrieve these groups for analysis.</span></span> <span data-ttu-id="b9b43-106">Dimensions can be used on entries in journals, documents, and budgets.</span><span class="sxs-lookup"><span data-stu-id="b9b43-106">Dimensions can be used on entries in journals, documents, and budgets.</span></span> <span data-ttu-id="b9b43-107">The term dimension describes how analysis occurs.</span><span class="sxs-lookup"><span data-stu-id="b9b43-107">The term dimension describes how analysis occurs.</span></span> <span data-ttu-id="b9b43-108">A two-dimensional analysis, for example, would be sales per area.</span><span class="sxs-lookup"><span data-stu-id="b9b43-108">A two-dimensional analysis, for example, would be sales per area.</span></span> <span data-ttu-id="b9b43-109">However, by using more than two dimensions when creating an entry, you can carry out a more complex analysis, such as sales per sales campaign per customer group per area.</span><span class="sxs-lookup"><span data-stu-id="b9b43-109">However, by using more than two dimensions when creating an entry, you can carry out a more complex analysis, such as sales per sales campaign per customer group per area.</span></span> <span data-ttu-id="b9b43-110">For more information, see [Working with Dimensions](finance-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="b9b43-110">For more information, see [Working with Dimensions](finance-dimensions.md).</span></span>

<span data-ttu-id="b9b43-111">Analysing data by dimensions gives you greater insight into your business, so you can evaluate information, such as how well your business is operating, where it is thriving and where it is not, and where more resources should be allocated.</span><span class="sxs-lookup"><span data-stu-id="b9b43-111">Analyzing data by dimensions gives you greater insight into your business, so you can evaluate information, such as how well your business is operating, where it is thriving and where it is not, and where more resources should be allocated.</span></span>

> [!TIP]
> <span data-ttu-id="b9b43-112">As a quick way to analyse transactional data by dimensions, you can filter totals in the chart of accounts and entries in all **Entries** pages by dimensions.</span><span class="sxs-lookup"><span data-stu-id="b9b43-112">As a quick way to analyze transactional data by dimensions, you can filter totals in the chart of accounts and entries in all **Entries** pages by dimensions.</span></span> <span data-ttu-id="b9b43-113">Look for the **Set Dimension Filter** action.</span><span class="sxs-lookup"><span data-stu-id="b9b43-113">Look for the **Set Dimension Filter** action.</span></span>

## <a name="to-set-up-an-analysis-view"></a><span data-ttu-id="b9b43-114">To set up an analysis view</span><span class="sxs-lookup"><span data-stu-id="b9b43-114">To set up an analysis view</span></span>  
<span data-ttu-id="b9b43-115">An analysis by dimensions displays a selected combination of dimensions.</span><span class="sxs-lookup"><span data-stu-id="b9b43-115">An analysis by dimensions displays a selected combination of dimensions.</span></span> <span data-ttu-id="b9b43-116">You can store and retrieve each analysis you have set up.</span><span class="sxs-lookup"><span data-stu-id="b9b43-116">You can store and retrieve each analysis you have set up.</span></span> <span data-ttu-id="b9b43-117">The information for setting up an analysis is stored on an **Analysis View** card to simplify future analysis.</span><span class="sxs-lookup"><span data-stu-id="b9b43-117">The information for setting up an analysis is stored on an **Analysis View** card to simplify future analysis.</span></span>  

1. <span data-ttu-id="b9b43-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Analysis Views**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b9b43-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Analysis Views**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b9b43-119">On the **Analysis View List** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="b9b43-119">On the **Analysis View List** page, choose the **New** action.</span></span>
3. <span data-ttu-id="b9b43-120">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="b9b43-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="b9b43-121">To add other dimension codes in addition to the four on the **Dimensions** FastTab, choose the **Filter** action, fill in the fields, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b9b43-121">To add other dimension codes in addition to the four on the **Dimensions** FastTab, choose the **Filter** action, fill in the fields, and then choose the **OK** button.</span></span>  
5. <span data-ttu-id="b9b43-122">To update the view, choose the **Update** action.</span><span class="sxs-lookup"><span data-stu-id="b9b43-122">To update the view, choose the **Update** action.</span></span>

## <a name="to-analyze-by-dimensions"></a><span data-ttu-id="b9b43-123">To analyse by dimensions</span><span class="sxs-lookup"><span data-stu-id="b9b43-123">To analyze by dimensions</span></span>
<span data-ttu-id="b9b43-124">You can use the **Analysis by Dimensions** matrix to view the amounts in your general ledger by using the analysis views that you have already set up.</span><span class="sxs-lookup"><span data-stu-id="b9b43-124">You can use the **Analysis by Dimensions** matrix to view the amounts in your general ledger by using the analysis views that you have already set up.</span></span> <span data-ttu-id="b9b43-125">You fill on the **Analysis by Dimensions** page to define what will be shown in the matrix, and then you choose the **Show Matrix** action to view the matrix.</span><span class="sxs-lookup"><span data-stu-id="b9b43-125">You fill on the **Analysis by Dimensions** page to define what will be shown in the matrix, and then you choose the **Show Matrix** action to view the matrix.</span></span>  

1. <span data-ttu-id="b9b43-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Analysis Views**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b9b43-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Analysis Views**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b9b43-127">Select the relevant analysis view,  and then choose the **Analysis by Dimensions** action.</span><span class="sxs-lookup"><span data-stu-id="b9b43-127">Select the relevant analysis view,  and then choose the **Analysis by Dimensions** action.</span></span>
3. <span data-ttu-id="b9b43-128">On the **Analysis by Dimensions** page, fill in the fields to define which data is shown and how.</span><span class="sxs-lookup"><span data-stu-id="b9b43-128">On the **Analysis by Dimensions** page, fill in the fields to define which data is shown and how.</span></span>
4. <span data-ttu-id="b9b43-129">Choose the **Show Matrix** action to open the respective matrix page for the defined analysis view.</span><span class="sxs-lookup"><span data-stu-id="b9b43-129">Choose the **Show Matrix** action to open the respective matrix page for the defined analysis view.</span></span>
5. <span data-ttu-id="b9b43-130">To see a specification of an amount shown in the matrix page, choose the amount to drill down.</span><span class="sxs-lookup"><span data-stu-id="b9b43-130">To see a specification of an amount shown in the matrix page, choose the amount to drill down.</span></span>  

- <span data-ttu-id="b9b43-131">The leftmost columns contain information based on what you have selected in the **Show as Lines** field in the header.</span><span class="sxs-lookup"><span data-stu-id="b9b43-131">The leftmost columns contain information based on what you have selected in the **Show as Lines** field in the header.</span></span>  
- <span data-ttu-id="b9b43-132">The rightmost columns contain information based on to what you have selected in the **Show as Columns** field in the header.</span><span class="sxs-lookup"><span data-stu-id="b9b43-132">The rightmost columns contain information based on to what you have selected in the **Show as Columns** field in the header.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="b9b43-133">You cannot select a period length shorter than the period specified for the date compression on the **Analysis View** card.</span><span class="sxs-lookup"><span data-stu-id="b9b43-133">You cannot select a period length shorter than the period specified for the date compression on the **Analysis View** card.</span></span> <span data-ttu-id="b9b43-134">The **Next Set** and **Previous Set** commands are inactive if you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field.</span><span class="sxs-lookup"><span data-stu-id="b9b43-134">The **Next Set** and **Previous Set** commands are inactive if you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="b9b43-135">You can use the **Dimensions - Detail** report to display a detailed classification of how dimensions have been used on entries over a selected period.</span><span class="sxs-lookup"><span data-stu-id="b9b43-135">You can use the **Dimensions - Detail** report to display a detailed classification of how dimensions have been used on entries over a selected period.</span></span> <span data-ttu-id="b9b43-136">You can use the **Dimensions - Total** report to display only the total amounts.</span><span class="sxs-lookup"><span data-stu-id="b9b43-136">You can use the **Dimensions - Total** report to display only the total amounts.</span></span>  

> [!TIP]  
>   <span data-ttu-id="b9b43-137">You can also change the view by changing the contents of the **Show as Lines** field and **Show as Columns** field.</span><span class="sxs-lookup"><span data-stu-id="b9b43-137">You can also change the view by changing the contents of the **Show as Lines** field and **Show as Columns** field.</span></span> <span data-ttu-id="b9b43-138">To reverse a view setting, choose the **Reverse Lines and Columns** action.</span><span class="sxs-lookup"><span data-stu-id="b9b43-138">To reverse a view setting, choose the **Reverse Lines and Columns** action.</span></span>

## <a name="to-update-an-analysis-view"></a><span data-ttu-id="b9b43-139">To update an analysis view</span><span class="sxs-lookup"><span data-stu-id="b9b43-139">To update an analysis view</span></span>  
<span data-ttu-id="b9b43-140">The amounts that are displayed on the **Analysis by Dimensions** page give you a picture of the company’s state at the time of the last update.</span><span class="sxs-lookup"><span data-stu-id="b9b43-140">The amounts that are displayed on the **Analysis by Dimensions** page give you a picture of the company’s state at the time of the last update.</span></span> <span data-ttu-id="b9b43-141">To get a picture of the current state, you must update the analysis view by running the update function.</span><span class="sxs-lookup"><span data-stu-id="b9b43-141">To get a picture of the current state, you must update the analysis view by running the update function.</span></span>

<span data-ttu-id="b9b43-142">The following procedure is for updating an analysis view from the **Analysis by Dimensions** page.</span><span class="sxs-lookup"><span data-stu-id="b9b43-142">The following procedure is for updating an analysis view from the **Analysis by Dimensions** page.</span></span> <span data-ttu-id="b9b43-143">The steps are similar from the **Analysis View Card** and the **Analysis View List** pages.</span><span class="sxs-lookup"><span data-stu-id="b9b43-143">The steps are similar from the **Analysis View Card** and the **Analysis View List** pages.</span></span>  

1. <span data-ttu-id="b9b43-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Analysis Views**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b9b43-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Analysis Views**, and then choose the related link.</span></span>
2. <span data-ttu-id="b9b43-145">Select the relevant analysis view,  and then choose the **Analysis by Dimensions** action.</span><span class="sxs-lookup"><span data-stu-id="b9b43-145">Select the relevant analysis view,  and then choose the **Analysis by Dimensions** action.</span></span>
2. <span data-ttu-id="b9b43-146">On the **Analysis by Dimensions** page, choose the **Analysis View Code** field.</span><span class="sxs-lookup"><span data-stu-id="b9b43-146">On the **Analysis by Dimensions** page, choose the **Analysis View Code** field.</span></span>  
3. <span data-ttu-id="b9b43-147">Select the line with the relevant analysis view.</span><span class="sxs-lookup"><span data-stu-id="b9b43-147">Select the line with the relevant analysis view.</span></span>  
4. <span data-ttu-id="b9b43-148">On the **Analysis Views** page, select the analysis view, and then choose the **Update** action.</span><span class="sxs-lookup"><span data-stu-id="b9b43-148">On the **Analysis Views** page, select the analysis view, and then choose the **Update** action.</span></span>  

> [!TIP]  
>   <span data-ttu-id="b9b43-149">If you select the **Update on Posting** check box on an analysis view card, the view is automatically updated when an involved transaction is posted.</span><span class="sxs-lookup"><span data-stu-id="b9b43-149">If you select the **Update on Posting** check box on an analysis view card, the view is automatically updated when an involved transaction is posted.</span></span>

> [!NOTE]  
>   <span data-ttu-id="b9b43-150">To update some or all analysis views at the same time, you must use the **Update Analysis Views** batch job.</span><span class="sxs-lookup"><span data-stu-id="b9b43-150">To update some or all analysis views at the same time, you must use the **Update Analysis Views** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b9b43-151">See Also</span><span class="sxs-lookup"><span data-stu-id="b9b43-151">See Also</span></span>
[<span data-ttu-id="b9b43-152">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="b9b43-152">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="b9b43-153">Finance</span><span class="sxs-lookup"><span data-stu-id="b9b43-153">Finance</span></span>](finance.md)  
[<span data-ttu-id="b9b43-154">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="b9b43-154">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="b9b43-155">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="b9b43-155">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
[<span data-ttu-id="b9b43-156">Working with Dimensions</span><span class="sxs-lookup"><span data-stu-id="b9b43-156">Working with Dimensions</span></span>](finance-dimensions.md)  
<span data-ttu-id="b9b43-157">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b9b43-157">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
