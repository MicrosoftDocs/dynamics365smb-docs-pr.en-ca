---
title: Walkthrough - Making Cash Flow Forecasts by Using Account Schedules | Microsoft Docs
description: This walkthrough describes how you can use account schedules to make cash flow forecasts. Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts. In the account schedules, you can set up subtotals for cash flow receipts and disbursements. These subtotals can be included in new totals that can then be used in making cash flow forecasts.
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
ms.openlocfilehash: 59264fada4455f3f0a40ba225d45159d2fb77194
ms.contentlocale: en-ca
ms.lasthandoff: 09/28/2018

---
# <a name="walkthrough-making-cash-flow-forecasts-by-using-account-schedules"></a><span data-ttu-id="18e06-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span><span class="sxs-lookup"><span data-stu-id="18e06-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span></span>
<span data-ttu-id="18e06-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="18e06-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span></span> <span data-ttu-id="18e06-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span><span class="sxs-lookup"><span data-stu-id="18e06-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span></span> <span data-ttu-id="18e06-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span><span class="sxs-lookup"><span data-stu-id="18e06-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span></span> <span data-ttu-id="18e06-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="18e06-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="18e06-111">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="18e06-111">About This Walkthrough</span></span>  
<span data-ttu-id="18e06-112">This walkthrough describes the following tasks:</span><span class="sxs-lookup"><span data-stu-id="18e06-112">This walkthrough describes the following tasks:</span></span>  

- <span data-ttu-id="18e06-113">Setting up a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="18e06-113">Setting up a new cash flow account schedule name.</span></span>  
- <span data-ttu-id="18e06-114">Setting up account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="18e06-114">Setting up account schedule lines.</span></span>  
- <span data-ttu-id="18e06-115">Setting up a new column layout.</span><span class="sxs-lookup"><span data-stu-id="18e06-115">Setting up a new column layout.</span></span>  
- <span data-ttu-id="18e06-116">Assigning a column layout to an account schedule.</span><span class="sxs-lookup"><span data-stu-id="18e06-116">Assigning a column layout to an account schedule.</span></span>  
- <span data-ttu-id="18e06-117">Viewing and printing the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="18e06-117">Viewing and printing the cash flow forecast.</span></span>  

### <a name="prerequisites"></a><span data-ttu-id="18e06-118">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="18e06-118">Prerequisites</span></span>  
<span data-ttu-id="18e06-119">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="18e06-119">To complete this walkthrough, you will need:</span></span>  

- [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="18e06-120">installed.</span><span class="sxs-lookup"><span data-stu-id="18e06-120">installed.</span></span>  
- <span data-ttu-id="18e06-121">The cash flow worksheet lines are registered.</span><span class="sxs-lookup"><span data-stu-id="18e06-121">The cash flow worksheet lines are registered.</span></span>  

## <a name="roles"></a><span data-ttu-id="18e06-122">Roles</span><span class="sxs-lookup"><span data-stu-id="18e06-122">Roles</span></span>  
<span data-ttu-id="18e06-123">This walkthrough demonstrates tasks that are performed by the following user role:</span><span class="sxs-lookup"><span data-stu-id="18e06-123">This walkthrough demonstrates tasks that are performed by the following user role:</span></span>  

- <span data-ttu-id="18e06-124">Controller</span><span class="sxs-lookup"><span data-stu-id="18e06-124">Controller</span></span>  

## <a name="story"></a><span data-ttu-id="18e06-125">Story</span><span class="sxs-lookup"><span data-stu-id="18e06-125">Story</span></span>  
<span data-ttu-id="18e06-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="18e06-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span></span> <span data-ttu-id="18e06-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span><span class="sxs-lookup"><span data-stu-id="18e06-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span></span>  

## <a name="setting-up-a-new-account-schedule-name"></a><span data-ttu-id="18e06-128">Setting Up a New Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="18e06-128">Setting Up a New Account Schedule Name</span></span>  
<span data-ttu-id="18e06-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span><span class="sxs-lookup"><span data-stu-id="18e06-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span></span>  

### <a name="to-set-up-a-new-account-schedule-name"></a><span data-ttu-id="18e06-130">To set up a new account schedule name</span><span class="sxs-lookup"><span data-stu-id="18e06-130">To set up a new account schedule name</span></span>  

1.  <span data-ttu-id="18e06-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18e06-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="18e06-132">In the **Account Schedule Names** window, choose the **New** to create a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="18e06-132">In the **Account Schedule Names** window, choose the **New** to create a new cash flow account schedule name.</span></span>  
3.  <span data-ttu-id="18e06-133">In the **Name** field, enter **Forecast**.</span><span class="sxs-lookup"><span data-stu-id="18e06-133">In the **Name** field, enter **Forecast**.</span></span>  
4.  <span data-ttu-id="18e06-134">In the **Description** field, enter **Cash Flow Forecast**.</span><span class="sxs-lookup"><span data-stu-id="18e06-134">In the **Description** field, enter **Cash Flow Forecast**.</span></span>  
5.  <span data-ttu-id="18e06-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span><span class="sxs-lookup"><span data-stu-id="18e06-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span></span>  

## <a name="setting-up-account-schedule-lines"></a><span data-ttu-id="18e06-136">Setting Up Account Schedule Lines</span><span class="sxs-lookup"><span data-stu-id="18e06-136">Setting Up Account Schedule Lines</span></span>  
<span data-ttu-id="18e06-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span><span class="sxs-lookup"><span data-stu-id="18e06-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span></span> <span data-ttu-id="18e06-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span><span class="sxs-lookup"><span data-stu-id="18e06-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span></span>  

### <a name="to-set-up-account-schedule-lines"></a><span data-ttu-id="18e06-139">To set up account schedule lines</span><span class="sxs-lookup"><span data-stu-id="18e06-139">To set up account schedule lines</span></span>  

1.  <span data-ttu-id="18e06-140">In the **Account Schedule Names** window, select the new **Forecast** account schedule name that you have created.</span><span class="sxs-lookup"><span data-stu-id="18e06-140">In the **Account Schedule Names** window, select the new **Forecast** account schedule name that you have created.</span></span> <span data-ttu-id="18e06-141">On the **Home** tab, in the **Process** group, choose **Edit Account Schedule**.</span><span class="sxs-lookup"><span data-stu-id="18e06-141">On the **Home** tab, in the **Process** group, choose **Edit Account Schedule**.</span></span>  
2.  <span data-ttu-id="18e06-142">In the **Account Schedule** window, enter each line exactly as shown in the following table.</span><span class="sxs-lookup"><span data-stu-id="18e06-142">In the **Account Schedule** window, enter each line exactly as shown in the following table.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="18e06-143">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="18e06-143">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span></span>  

    <span data-ttu-id="18e06-144">|Row No.|Description|Totalling Type|Totalling|Row Type|Amount Type|Show|</span><span class="sxs-lookup"><span data-stu-id="18e06-144">|Row No.|Description|Totaling Type|Totaling|Row Type|Amount Type|Show|</span></span>  
    <span data-ttu-id="18e06-145">|-------|-----------|-------------|--------|--------|---  ------|----| |C10|Amount|Net Change|Entries|Net Amount|Always|</span><span class="sxs-lookup"><span data-stu-id="18e06-145">|-------|-----------|-------------|--------|--------|---  ------|----| |C10|Amount|Net Change|Entries|Net Amount|Always|</span></span>  
    <span data-ttu-id="18e06-146">|C20|Amount until Date|Balance at Date|Entries|Net Amount|Always|</span><span class="sxs-lookup"><span data-stu-id="18e06-146">|C20|Amount until Date|Balance at Date|Entries|Net Amount|Always|</span></span>  
    <span data-ttu-id="18e06-147">|C30|Entire Fiscal Year|Entire Fiscal Year|Entries|Net Amount|Always|</span><span class="sxs-lookup"><span data-stu-id="18e06-147">|C30|Entire Fiscal Year|Entire Fiscal Year|Entries|Net Amount|Always|</span></span>  

4.  <span data-ttu-id="18e06-148">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="18e06-148">Choose the **OK** button.</span></span>  

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="18e06-149">Assigning the Column Layout to the Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="18e06-149">Assigning the Column Layout to the Account Schedule Name</span></span>  
<span data-ttu-id="18e06-150">Ken is now ready to assign the column layout to the account schedule name.</span><span class="sxs-lookup"><span data-stu-id="18e06-150">Ken is now ready to assign the column layout to the account schedule name.</span></span>  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="18e06-151">To assign the column layout to the account schedule name</span><span class="sxs-lookup"><span data-stu-id="18e06-151">To assign the column layout to the account schedule name</span></span>  

1.  <span data-ttu-id="18e06-152">In the **Account Schedule Names** window, select **Forecast** in the **Name** field.</span><span class="sxs-lookup"><span data-stu-id="18e06-152">In the **Account Schedule Names** window, select **Forecast** in the **Name** field.</span></span>  
2.  <span data-ttu-id="18e06-153">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span><span class="sxs-lookup"><span data-stu-id="18e06-153">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span></span>  

### <a name="to-view-and-print-the-cash-flow-forecast"></a><span data-ttu-id="18e06-154">To view and print the cash flow forecast</span><span class="sxs-lookup"><span data-stu-id="18e06-154">To view and print the cash flow forecast</span></span>  
1.  <span data-ttu-id="18e06-155">In the **Account Schedule Names** window, choose the **Overview** action to view the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="18e06-155">In the **Account Schedule Names** window, choose the **Overview** action to view the cash flow forecast.</span></span>  
2.  <span data-ttu-id="18e06-156">In the **Acc. Schedule Overview** window, you can select an amount and then view the cash flow forecast entries that make up the amount.</span><span class="sxs-lookup"><span data-stu-id="18e06-156">In the **Acc. Schedule Overview** window, you can select an amount and then view the cash flow forecast entries that make up the amount.</span></span> <span data-ttu-id="18e06-157">In addition, you can view the formula that is used to calculate the amount.</span><span class="sxs-lookup"><span data-stu-id="18e06-157">In addition, you can view the formula that is used to calculate the amount.</span></span> <span data-ttu-id="18e06-158">You can also filter the amounts by date and dimension.</span><span class="sxs-lookup"><span data-stu-id="18e06-158">You can also filter the amounts by date and dimension.</span></span>  
3.  <span data-ttu-id="18e06-159">Choose the **Print** action to print the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="18e06-159">Choose the **Print** action to print the cash flow forecast.</span></span>  

## <a name="see-also"></a><span data-ttu-id="18e06-160">See Also</span><span class="sxs-lookup"><span data-stu-id="18e06-160">See Also</span></span>  
 <span data-ttu-id="18e06-161">[Work with Account Schedules](bi-how-work-account-schedule.md) </span><span class="sxs-lookup"><span data-stu-id="18e06-161">[Work with Account Schedules](bi-how-work-account-schedule.md) </span></span>  
 [<span data-ttu-id="18e06-162">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="18e06-162">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="18e06-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="18e06-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

