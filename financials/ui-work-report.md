---
title: Scheduling a Report to Run at a Specific Date and Time | Microsoft Docs
description: Learn about entering a report into a job queue and scheduling it to be processed at a specific date and time.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process, report
ms.date: 07/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f29ae6b0a87f24a5201dd05b1d631adcc69b116d
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="working-with-reports"></a><span data-ttu-id="8e792-103">Working with Reports</span><span class="sxs-lookup"><span data-stu-id="8e792-103">Working with Reports</span></span>
<span data-ttu-id="8e792-104">A report gathers information based on a specified set of criteria, and organizes and presents the information in an easy-to-read, printable format.</span><span class="sxs-lookup"><span data-stu-id="8e792-104">A report gathers information based on a specified set of criteria, and organizes and presents the information in an easy-to-read, printable format.</span></span> <span data-ttu-id="8e792-105">There are many reports that you can access throughout the application.</span><span class="sxs-lookup"><span data-stu-id="8e792-105">There are many reports that you can access throughout the application.</span></span> <span data-ttu-id="8e792-106">The reports typically provide information relative to the context of the page you are on.</span><span class="sxs-lookup"><span data-stu-id="8e792-106">The reports typically provide information relative to the context of the page you are on.</span></span> <span data-ttu-id="8e792-107">For example, the **Customer** page includes reports for the top 10 customers and the sales statistics, and more.</span><span class="sxs-lookup"><span data-stu-id="8e792-107">For example, the **Customer** page includes reports for the top 10 customers and the sales statistics, and more.</span></span>

<span data-ttu-id="8e792-108">You can find reports in the **Reports** tab on selected pages, or you can use search to find reports by name.</span><span class="sxs-lookup"><span data-stu-id="8e792-108">You can find reports in the **Reports** tab on selected pages, or you can use search to find reports by name.</span></span> <span data-ttu-id="8e792-109">When you open a report, you are presented with a page that let's you specify information (options and filters) that determines want to include in the report.</span><span class="sxs-lookup"><span data-stu-id="8e792-109">When you open a report, you are presented with a page that let's you specify information (options and filters) that determines want to include in the report.</span></span> <span data-ttu-id="8e792-110">For example, depending on the report, you can specify a date range, a specific record such as a customer, or sorting order.</span><span class="sxs-lookup"><span data-stu-id="8e792-110">For example, depending on the report, you can specify a date range, a specific record such as a customer, or sorting order.</span></span> <span data-ttu-id="8e792-111">Here is an example:</span><span class="sxs-lookup"><span data-stu-id="8e792-111">Here is an example:</span></span>

<span data-ttu-id="8e792-112">![Report options](media/report_options.png "Report options")</span><span class="sxs-lookup"><span data-stu-id="8e792-112">![Report options](media/report_options.png "Report options")</span></span>

## <a name="previewing-a-report"></a><span data-ttu-id="8e792-113">Previewing a report</span><span class="sxs-lookup"><span data-stu-id="8e792-113">Previewing a report</span></span>
<span data-ttu-id="8e792-114">Choose **Preview** to see the report in the Internet browser.</span><span class="sxs-lookup"><span data-stu-id="8e792-114">Choose **Preview** to see the report in the Internet browser.</span></span> <span data-ttu-id="8e792-115">Point to an area of the report to show the menu bar.</span><span class="sxs-lookup"><span data-stu-id="8e792-115">Point to an area of the report to show the menu bar.</span></span>  

<span data-ttu-id="8e792-116">![Report preview toolbar](media/report_viewer.png "Report preview toolbar")</span><span class="sxs-lookup"><span data-stu-id="8e792-116">![Report preview toolbar](media/report_viewer.png "Report preview toolbar")</span></span>

<span data-ttu-id="8e792-117">Use the menu bar to:</span><span class="sxs-lookup"><span data-stu-id="8e792-117">Use the menu bar to:</span></span>

-   <span data-ttu-id="8e792-118">Move through pages</span><span class="sxs-lookup"><span data-stu-id="8e792-118">Move through pages</span></span>
-   <span data-ttu-id="8e792-119">Zoom in and out</span><span class="sxs-lookup"><span data-stu-id="8e792-119">Zoom in and out</span></span>
-   <span data-ttu-id="8e792-120">Resize to fit the window</span><span class="sxs-lookup"><span data-stu-id="8e792-120">Resize to fit the window</span></span>
-   <span data-ttu-id="8e792-121">Select text</span><span class="sxs-lookup"><span data-stu-id="8e792-121">Select text</span></span>

    <span data-ttu-id="8e792-122">You can copy text from a report, and then paste it somewhere else, like a page in [!INCLUDE[d365fin](includes/d365fin_md.md)] or Microsoft Word.</span><span class="sxs-lookup"><span data-stu-id="8e792-122">You can copy text from a report, and then paste it somewhere else, like a page in [!INCLUDE[d365fin](includes/d365fin_md.md)] or Microsoft Word.</span></span>  <span data-ttu-id="8e792-123">Using a mouse, for example, you press and hold where you want to start, and then move the mouse to select one or more words, sentences, or paragraphs.</span><span class="sxs-lookup"><span data-stu-id="8e792-123">Using a mouse, for example, you press and hold where you want to start, and then move the mouse to select one or more words, sentences, or paragraphs.</span></span> <span data-ttu-id="8e792-124">You can then press the right mouse button, and select **Copy**.</span><span class="sxs-lookup"><span data-stu-id="8e792-124">You can then press the right mouse button, and select **Copy**.</span></span> <span data-ttu-id="8e792-125">You can the paste the selected text where ever you want it.</span><span class="sxs-lookup"><span data-stu-id="8e792-125">You can the paste the selected text where ever you want it.</span></span>
-   <span data-ttu-id="8e792-126">Pan the document</span><span class="sxs-lookup"><span data-stu-id="8e792-126">Pan the document</span></span>

    <span data-ttu-id="8e792-127">You can move the visible area of the report in any direction so you can view other areas or the report.</span><span class="sxs-lookup"><span data-stu-id="8e792-127">You can move the visible area of the report in any direction so you can view other areas or the report.</span></span> <span data-ttu-id="8e792-128">This is helpful when you have zoomed in to see details.</span><span class="sxs-lookup"><span data-stu-id="8e792-128">This is helpful when you have zoomed in to see details.</span></span>  <span data-ttu-id="8e792-129">Using your mouse, for example, press and hold the mouse button anywhere in the report preview, and then move your mouse.</span><span class="sxs-lookup"><span data-stu-id="8e792-129">Using your mouse, for example, press and hold the mouse button anywhere in the report preview, and then move your mouse.</span></span>

-   <span data-ttu-id="8e792-130">Download to a PDF file on your computer or network.</span><span class="sxs-lookup"><span data-stu-id="8e792-130">Download to a PDF file on your computer or network.</span></span>
-   <span data-ttu-id="8e792-131">Print</span><span class="sxs-lookup"><span data-stu-id="8e792-131">Print</span></span>


## <a name="saving-a-report"></a><span data-ttu-id="8e792-132">Saving a Report</span><span class="sxs-lookup"><span data-stu-id="8e792-132">Saving a Report</span></span>
<span data-ttu-id="8e792-133">You can save a report to a PDF document, Microsoft Word document, or Microsoft Excel document by choosing **Send to**, and then making your selection.</span><span class="sxs-lookup"><span data-stu-id="8e792-133">You can save a report to a PDF document, Microsoft Word document, or Microsoft Excel document by choosing **Send to**, and then making your selection.</span></span>

## <a name="ScheduleReport"></a> <span data-ttu-id="8e792-134">Scheduling a Report to Run</span><span class="sxs-lookup"><span data-stu-id="8e792-134">Scheduling a Report to Run</span></span>
<span data-ttu-id="8e792-135">You can schedule a report to run at a specific date and time.</span><span class="sxs-lookup"><span data-stu-id="8e792-135">You can schedule a report to run at a specific date and time.</span></span> <span data-ttu-id="8e792-136">Scheduled reports are entered in the job queue and processed at the scheduled time, similar to other jobs.</span><span class="sxs-lookup"><span data-stu-id="8e792-136">Scheduled reports are entered in the job queue and processed at the scheduled time, similar to other jobs.</span></span> <span data-ttu-id="8e792-137">You can choose to save the processed report to a file, such as an Excel, Word, or PDF, print it to a selected printer, or process the report only.</span><span class="sxs-lookup"><span data-stu-id="8e792-137">You can choose to save the processed report to a file, such as an Excel, Word, or PDF, print it to a selected printer, or process the report only.</span></span> <span data-ttu-id="8e792-138">If you choose to save the report to a file, then the processed report is sent to the **Report Inbox** area on your Role Centre, where you can view it.</span><span class="sxs-lookup"><span data-stu-id="8e792-138">If you choose to save the report to a file, then the processed report is sent to the **Report Inbox** area on your Role Center, where you can view it.</span></span>

<span data-ttu-id="8e792-139">You can schedule a report when you open a report.</span><span class="sxs-lookup"><span data-stu-id="8e792-139">You can schedule a report when you open a report.</span></span> <span data-ttu-id="8e792-140">You choose the **Schedule** action and then you enter information such as printer, and time and date.</span><span class="sxs-lookup"><span data-stu-id="8e792-140">You choose the **Schedule** action and then you enter information such as printer, and time and date.</span></span> <span data-ttu-id="8e792-141">The report is then added to the job queue and will be run at the specified time.</span><span class="sxs-lookup"><span data-stu-id="8e792-141">The report is then added to the job queue and will be run at the specified time.</span></span> <span data-ttu-id="8e792-142">When the report is processed, the item will be removed from the job queue.</span><span class="sxs-lookup"><span data-stu-id="8e792-142">When the report is processed, the item will be removed from the job queue.</span></span> <span data-ttu-id="8e792-143">If you saved the processed report to a file, it will be available in the **Report Inbox** area.</span><span class="sxs-lookup"><span data-stu-id="8e792-143">If you saved the processed report to a file, it will be available in the **Report Inbox** area.</span></span>

## <a name="PrintReport"></a><span data-ttu-id="8e792-144">Printing a Report</span><span class="sxs-lookup"><span data-stu-id="8e792-144">Printing a Report</span></span>
<span data-ttu-id="8e792-145">You can print a report from the **Print** button on the options page that appears when you open the report or from the menu bar in Preview.</span><span class="sxs-lookup"><span data-stu-id="8e792-145">You can print a report from the **Print** button on the options page that appears when you open the report or from the menu bar in Preview.</span></span>

## <a name="using-saved-settings"></a><span data-ttu-id="8e792-146">Using Saved Settings</span><span class="sxs-lookup"><span data-stu-id="8e792-146">Using Saved Settings</span></span>
<span data-ttu-id="8e792-147">A report can include one or more entries in the **Saved Settings** box.</span><span class="sxs-lookup"><span data-stu-id="8e792-147">A report can include one or more entries in the **Saved Settings** box.</span></span> <span data-ttu-id="8e792-148">*Saved settings* are basically a predefined group of options and filters that you can apply to the report before previewing or sending the report to a file.</span><span class="sxs-lookup"><span data-stu-id="8e792-148">*Saved settings* are basically a predefined group of options and filters that you can apply to the report before previewing or sending the report to a file.</span></span> <span data-ttu-id="8e792-149">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span><span class="sxs-lookup"><span data-stu-id="8e792-149">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span></span>

<span data-ttu-id="8e792-150">The saved settings entry called **Last used options and filters** is always available.</span><span class="sxs-lookup"><span data-stu-id="8e792-150">The saved settings entry called **Last used options and filters** is always available.</span></span> <span data-ttu-id="8e792-151">This entry sets the report to use options and filters that were used the last time you looked at the report.</span><span class="sxs-lookup"><span data-stu-id="8e792-151">This entry sets the report to use options and filters that were used the last time you looked at the report.</span></span>

>[!NOTE]
><span data-ttu-id="8e792-152">As an administrator, you can create and manage the saved settings for reports for all users.</span><span class="sxs-lookup"><span data-stu-id="8e792-152">As an administrator, you can create and manage the saved settings for reports for all users.</span></span> <span data-ttu-id="8e792-153">For more information, see [Managing Saved Settings on Reports](reports-saving-reusing-settings.md).</span><span class="sxs-lookup"><span data-stu-id="8e792-153">For more information, see [Managing Saved Settings on Reports](reports-saving-reusing-settings.md).</span></span>

## <a name="changing-the-layout-and-look-of-a-report"></a><span data-ttu-id="8e792-154">Changing the layout and look of a report</span><span class="sxs-lookup"><span data-stu-id="8e792-154">Changing the layout and look of a report</span></span>
<span data-ttu-id="8e792-155">A report layout controls what is shown on a report, how it is arranged, and how it is styled.</span><span class="sxs-lookup"><span data-stu-id="8e792-155">A report layout controls what is shown on a report, how it is arranged, and how it is styled.</span></span> <span data-ttu-id="8e792-156">If you want to switch to a different layout, see [Change Which Layout is Currently Used on a Report](ui-how-change-layout-currently-used-report.md).</span><span class="sxs-lookup"><span data-stu-id="8e792-156">If you want to switch to a different layout, see [Change Which Layout is Currently Used on a Report](ui-how-change-layout-currently-used-report.md).</span></span> <span data-ttu-id="8e792-157">Or, if you want to customize your own report layout, see [Create and Modify a Custom Report Layout](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="8e792-157">Or, if you want to customize your own report layout, see [Create and Modify a Custom Report Layout](ui-how-create-custom-report-layout.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="8e792-158">See Also</span><span class="sxs-lookup"><span data-stu-id="8e792-158">See Also</span></span>
[<span data-ttu-id="8e792-159">Specify Printer Selection for Reports</span><span class="sxs-lookup"><span data-stu-id="8e792-159">Specify Printer Selection for Reports</span></span>](ui-specify-printer-selection-reports.md)  
[<span data-ttu-id="8e792-160">Managing Report and Document Layouts</span><span class="sxs-lookup"><span data-stu-id="8e792-160">Managing Report and Document Layouts</span></span>](ui-manage-report-layouts.md)  
<span data-ttu-id="8e792-161">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8e792-161">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
