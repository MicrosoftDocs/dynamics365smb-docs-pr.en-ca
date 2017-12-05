---
title: Walkthrough - Making Cash Flow Forecasts by Using Account Schedules | Microsoft Docs
description: This walkthrough describes how you can use account schedules to make cash flow forecasts. Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts. In the account schedules, you can set up subtotals for cash flow receipts and disbursements. These subtotals can be included in new totals that can then be used in making cash flow forecasts.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: c66fc5da322ddb1d217b61da0b563faab27b344e
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="walkthrough-making-cash-flow-forecasts-by-using-account-schedules"></a><span data-ttu-id="5e5c0-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span><span class="sxs-lookup"><span data-stu-id="5e5c0-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span></span>
<span data-ttu-id="5e5c0-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span></span> <span data-ttu-id="5e5c0-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span></span> <span data-ttu-id="5e5c0-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span></span> <span data-ttu-id="5e5c0-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="5e5c0-111">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="5e5c0-111">About This Walkthrough</span></span>  
<span data-ttu-id="5e5c0-112">This walkthrough describes the following tasks:</span><span class="sxs-lookup"><span data-stu-id="5e5c0-112">This walkthrough describes the following tasks:</span></span>  

- <span data-ttu-id="5e5c0-113">Setting up a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-113">Setting up a new cash flow account schedule name.</span></span>  
- <span data-ttu-id="5e5c0-114">Setting up account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-114">Setting up account schedule lines.</span></span>  
- <span data-ttu-id="5e5c0-115">Setting up a new column layout.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-115">Setting up a new column layout.</span></span>  
- <span data-ttu-id="5e5c0-116">Assigning a column layout to an account schedule.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-116">Assigning a column layout to an account schedule.</span></span>  
- <span data-ttu-id="5e5c0-117">Viewing and printing the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-117">Viewing and printing the cash flow forecast.</span></span>  

### <a name="prerequisites"></a><span data-ttu-id="5e5c0-118">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="5e5c0-118">Prerequisites</span></span>  
<span data-ttu-id="5e5c0-119">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="5e5c0-119">To complete this walkthrough, you will need:</span></span>  

- [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="5e5c0-120"> installed.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-120"> installed.</span></span>  
- <span data-ttu-id="5e5c0-121">The cash flow worksheet lines are registered.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-121">The cash flow worksheet lines are registered.</span></span>  

## <a name="roles"></a><span data-ttu-id="5e5c0-122">Roles</span><span class="sxs-lookup"><span data-stu-id="5e5c0-122">Roles</span></span>  
<span data-ttu-id="5e5c0-123">This walkthrough demonstrates tasks that are performed by the following user role:</span><span class="sxs-lookup"><span data-stu-id="5e5c0-123">This walkthrough demonstrates tasks that are performed by the following user role:</span></span>  

- <span data-ttu-id="5e5c0-124">Controller</span><span class="sxs-lookup"><span data-stu-id="5e5c0-124">Controller</span></span>  

## <a name="story"></a><span data-ttu-id="5e5c0-125">Story</span><span class="sxs-lookup"><span data-stu-id="5e5c0-125">Story</span></span>  
<span data-ttu-id="5e5c0-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span></span> <span data-ttu-id="5e5c0-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span></span>  

## <a name="setting-up-a-new-account-schedule-name"></a><span data-ttu-id="5e5c0-128">Setting Up a New Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="5e5c0-128">Setting Up a New Account Schedule Name</span></span>  
<span data-ttu-id="5e5c0-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span></span>  

### <a name="to-set-up-a-new-account-schedule-name"></a><span data-ttu-id="5e5c0-130">To set up a new account schedule name</span><span class="sxs-lookup"><span data-stu-id="5e5c0-130">To set up a new account schedule name</span></span>  

1.  <span data-ttu-id="5e5c0-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5e5c0-132">In the **Account Schedule Names** window, choose the **New** to create a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-132">In the **Account Schedule Names** window, choose the **New** to create a new cash flow account schedule name.</span></span>  
3.  <span data-ttu-id="5e5c0-133">In the **Name** field, enter **Forecast**.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-133">In the **Name** field, enter **Forecast**.</span></span>  
4.  <span data-ttu-id="5e5c0-134">In the **Description** field, enter **Cash Flow Forecast**.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-134">In the **Description** field, enter **Cash Flow Forecast**.</span></span>  
5.  <span data-ttu-id="5e5c0-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span></span>  

## <a name="setting-up-account-schedule-lines"></a><span data-ttu-id="5e5c0-136">Setting Up Account Schedule Lines</span><span class="sxs-lookup"><span data-stu-id="5e5c0-136">Setting Up Account Schedule Lines</span></span>  
<span data-ttu-id="5e5c0-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span></span> <span data-ttu-id="5e5c0-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span></span>  

### <a name="to-set-up-account-schedule-lines"></a><span data-ttu-id="5e5c0-139">To set up account schedule lines</span><span class="sxs-lookup"><span data-stu-id="5e5c0-139">To set up account schedule lines</span></span>  

1.  <span data-ttu-id="5e5c0-140">In the **Account Schedule Names** window, select the new **Forecast** account schedule name that you have created.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-140">In the **Account Schedule Names** window, select the new **Forecast** account schedule name that you have created.</span></span> <span data-ttu-id="5e5c0-141">On the **Home** tab, in the **Process** group, choose **Edit Account Schedule**.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-141">On the **Home** tab, in the **Process** group, choose **Edit Account Schedule**.</span></span>  
2.  <span data-ttu-id="5e5c0-142">In the **Account Schedule** window, enter each line exactly as shown in the following table.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-142">In the **Account Schedule** window, enter each line exactly as shown in the following table.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="5e5c0-143">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-143">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span></span>  

    <span data-ttu-id="5e5c0-144">|Row No.|Description|Totalling Type|Totalling|Row Type|Amount Type|Show|</span><span class="sxs-lookup"><span data-stu-id="5e5c0-144">|Row No.|Description|Totaling Type|Totaling|Row Type|Amount Type|Show|</span></span>  
    <span data-ttu-id="5e5c0-145">|-------|-----------|-------------|--------|--------|---  ------|----| |C10|Amount|Net Change|Entries|Net Amount|Always|</span><span class="sxs-lookup"><span data-stu-id="5e5c0-145">|-------|-----------|-------------|--------|--------|---  ------|----| |C10|Amount|Net Change|Entries|Net Amount|Always|</span></span>  
    <span data-ttu-id="5e5c0-146">|C20|Amount until Date|Balance at Date|Entries|Net Amount|Always|</span><span class="sxs-lookup"><span data-stu-id="5e5c0-146">|C20|Amount until Date|Balance at Date|Entries|Net Amount|Always|</span></span>  
    <span data-ttu-id="5e5c0-147">|C30|Entire Fiscal Year|Entire Fiscal Year|Entries|Net Amount|Always|</span><span class="sxs-lookup"><span data-stu-id="5e5c0-147">|C30|Entire Fiscal Year|Entire Fiscal Year|Entries|Net Amount|Always|</span></span>  

4.  <span data-ttu-id="5e5c0-148">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-148">Choose the **OK** button.</span></span>  

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="5e5c0-149">Assigning the Column Layout to the Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="5e5c0-149">Assigning the Column Layout to the Account Schedule Name</span></span>  
<span data-ttu-id="5e5c0-150">Ken is now ready to assign the column layout to the account schedule name.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-150">Ken is now ready to assign the column layout to the account schedule name.</span></span>  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="5e5c0-151">To assign the column layout to the account schedule name</span><span class="sxs-lookup"><span data-stu-id="5e5c0-151">To assign the column layout to the account schedule name</span></span>  

1.  <span data-ttu-id="5e5c0-152">In the **Account Schedule Names** window, select **Forecast** in the **Name** field.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-152">In the **Account Schedule Names** window, select **Forecast** in the **Name** field.</span></span>  
2.  <span data-ttu-id="5e5c0-153">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-153">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span></span>  

### <a name="to-view-and-print-the-cash-flow-forecast"></a><span data-ttu-id="5e5c0-154">To view and print the cash flow forecast</span><span class="sxs-lookup"><span data-stu-id="5e5c0-154">To view and print the cash flow forecast</span></span>  
1.  <span data-ttu-id="5e5c0-155">In the **Account Schedule Names** window, choose the **Overview** action to view the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-155">In the **Account Schedule Names** window, choose the **Overview** action to view the cash flow forecast.</span></span>  
2.  <span data-ttu-id="5e5c0-156">In the **Acc. Schedule Overview** window, you can select an amount and then view the cash flow forecast entries that make up the amount.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-156">In the **Acc. Schedule Overview** window, you can select an amount and then view the cash flow forecast entries that make up the amount.</span></span> <span data-ttu-id="5e5c0-157">In addition, you can view the formula that is used to calculate the amount.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-157">In addition, you can view the formula that is used to calculate the amount.</span></span> <span data-ttu-id="5e5c0-158">You can also filter the amounts by date and dimension.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-158">You can also filter the amounts by date and dimension.</span></span>  
3.  <span data-ttu-id="5e5c0-159">Choose the **Print** action to print the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="5e5c0-159">Choose the **Print** action to print the cash flow forecast.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5e5c0-160">See Also</span><span class="sxs-lookup"><span data-stu-id="5e5c0-160">See Also</span></span>  
 <span data-ttu-id="5e5c0-161">[How to: Work with Account Schedules](bi-how-work-account-schedule.md) </span><span class="sxs-lookup"><span data-stu-id="5e5c0-161">[How to: Work with Account Schedules](bi-how-work-account-schedule.md) </span></span>  
 [<span data-ttu-id="5e5c0-162">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="5e5c0-162">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="5e5c0-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5e5c0-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
