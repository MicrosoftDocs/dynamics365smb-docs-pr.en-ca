---
title: Custom and Built-In Layouts for Reports and Documents | Microsoft Docs
description: Use report layouts to customize documents, for example, to personalize the font, logo, or page settings of PDF files you send to customers.
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 10/01/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 2066c62221c0f3161877e53d2e8ffa0c5fa1315b
ms.contentlocale: en-ca
ms.lasthandoff: 09/28/2018

---
# <a name="managing-report-and-document-layouts"></a><span data-ttu-id="3a4d0-103">Managing Report and Document Layouts</span><span class="sxs-lookup"><span data-stu-id="3a4d0-103">Managing Report and Document Layouts</span></span>
<span data-ttu-id="3a4d0-104">A report layout controls content and format of the report, including which data fields of a report dataset appear on the report and how they are arranged, text style, images, and more.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-104">A report layout controls content and format of the report, including which data fields of a report dataset appear on the report and how they are arranged, text style, images, and more.</span></span> <span data-ttu-id="3a4d0-105">From [!INCLUDE[d365fin](includes/d365fin_md.md)], you can change which layout is used on a report, create new layout, or modify the existing layouts.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-105">From [!INCLUDE[d365fin](includes/d365fin_md.md)], you can change which layout is used on a report, create new layout, or modify the existing layouts.</span></span>

> [!NOTE]  
>   <span data-ttu-id="3a4d0-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the term "report" also covers externally-facing documents, such as sales invoices and order confirmations that you send to customers as PDF files.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the term "report" also covers externally-facing documents, such as sales invoices and order confirmations that you send to customers as PDF files.</span></span>

<span data-ttu-id="3a4d0-107">In particular, a report layout sets up the following:</span><span class="sxs-lookup"><span data-stu-id="3a4d0-107">In particular, a report layout sets up the following:</span></span>

* <span data-ttu-id="3a4d0-108">The label and data fields to include from the dataset of the [!INCLUDE[d365fin](includes/d365fin_md.md)] report.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-108">The label and data fields to include from the dataset of the [!INCLUDE[d365fin](includes/d365fin_md.md)] report.</span></span>
* <span data-ttu-id="3a4d0-109">The text format, such as font type, size, and colour.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-109">The text format, such as font type, size, and color.</span></span>
* <span data-ttu-id="3a4d0-110">The company logo and its position.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-110">The company logo and its position.</span></span>
* <span data-ttu-id="3a4d0-111">General page settings, such as margins and background images.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-111">General page settings, such as margins and background images.</span></span>

<span data-ttu-id="3a4d0-112">A [!INCLUDE[d365fin](includes/d365fin_md.md)] can be set up with multiple report layouts, which you can switch among as required.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-112">A [!INCLUDE[d365fin](includes/d365fin_md.md)] can be set up with multiple report layouts, which you can switch among as required.</span></span> <span data-ttu-id="3a4d0-113">You can use one of the built-in report layouts or you can create custom report layouts and assign them to your reports as needed.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-113">You can use one of the built-in report layouts or you can create custom report layouts and assign them to your reports as needed.</span></span> <span data-ttu-id="3a4d0-114">For more information, see [Create a Custom Report or Document Layout](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-114">For more information, see [Create a Custom Report or Document Layout](ui-how-create-custom-report-layout.md).</span></span>

<span data-ttu-id="3a4d0-115">There are two types of report layouts that you can use on reports; Word and RDLC.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-115">There are two types of report layouts that you can use on reports; Word and RDLC.</span></span>

## <a name="word-report-layout-overview"></a><span data-ttu-id="3a4d0-116">Word report layout overview</span><span class="sxs-lookup"><span data-stu-id="3a4d0-116">Word report layout overview</span></span>
<span data-ttu-id="3a4d0-117">A Word report layout is a based on Word document (.docx file type).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-117">A Word report layout is a based on Word document (.docx file type).</span></span> <span data-ttu-id="3a4d0-118">Word report layouts enable you to design report layouts by using Microsoft Word 2013 or later.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-118">Word report layouts enable you to design report layouts by using Microsoft Word 2013 or later.</span></span> <span data-ttu-id="3a4d0-119">A Word report layout determines the report's content - controlling how that content elements are arranged and how they look.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-119">A Word report layout determines the report's content - controlling how that content elements are arranged and how they look.</span></span> <span data-ttu-id="3a4d0-120">A Word report layout document will typically use tables to arrange content, where the cells can contain data fields, text, or pictures.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-120">A Word report layout document will typically use tables to arrange content, where the cells can contain data fields, text, or pictures.</span></span>

 <span data-ttu-id="3a4d0-121">![Example of a word report layout document for NAV](media/nav_wordreportlayout_edit_in_word_example.png "NAV_WordReportLayout_Edit_In_Word_Example")</span><span class="sxs-lookup"><span data-stu-id="3a4d0-121">![Example of a word report layout document for NAV](media/nav_wordreportlayout_edit_in_word_example.png "NAV_WordReportLayout_Edit_In_Word_Example")</span></span>  

## <a name="rdlc-layout-overview"></a><span data-ttu-id="3a4d0-122">RDLC layout overview</span><span class="sxs-lookup"><span data-stu-id="3a4d0-122">RDLC layout overview</span></span>
<span data-ttu-id="3a4d0-123">RDLC layouts are based on client report definition layouts (.rdlc or .rdl file types).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-123">RDLC layouts are based on client report definition layouts (.rdlc or .rdl file types).</span></span> <span data-ttu-id="3a4d0-124">These layouts are created and modified by using SQL Server Report Builder.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-124">These layouts are created and modified by using SQL Server Report Builder.</span></span> <span data-ttu-id="3a4d0-125">The design concept for RDLC layouts is similar to Word layouts, where the layout defines the general format of the report and determines the fields from the dataset to include.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-125">The design concept for RDLC layouts is similar to Word layouts, where the layout defines the general format of the report and determines the fields from the dataset to include.</span></span> <span data-ttu-id="3a4d0-126">Designing RDLC layouts is more advanced than Word layouts.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-126">Designing RDLC layouts is more advanced than Word layouts.</span></span> <span data-ttu-id="3a4d0-127">For more information, see [Designing RDLC Report Layouts](/dynamics-nav/Designing-RDLC-Report-Layouts).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-127">For more information, see [Designing RDLC Report Layouts](/dynamics-nav/Designing-RDLC-Report-Layouts).</span></span>

## <a name="built-in-and-custom-report-layouts"></a><span data-ttu-id="3a4d0-128">Built-in and custom report layouts</span><span class="sxs-lookup"><span data-stu-id="3a4d0-128">Built-in and custom report layouts</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="3a4d0-129">includes several built-in layouts.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-129">includes several built-in layouts.</span></span> <span data-ttu-id="3a4d0-130">Built-in layouts are predefined layouts that are designed for specific reports.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-130">Built-in layouts are predefined layouts that are designed for specific reports.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="3a4d0-131">reports will have a built-in layout as either an RDLC report layout, Word report layout, or in some cases both.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-131">reports will have a built-in layout as either an RDLC report layout, Word report layout, or in some cases both.</span></span> <span data-ttu-id="3a4d0-132">You cannot modify a built-in report layout from [!INCLUDE[d365fin](includes/d365fin_md.md)] but you use them as a starting point for building your own custom report layouts.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-132">You cannot modify a built-in report layout from [!INCLUDE[d365fin](includes/d365fin_md.md)] but you use them as a starting point for building your own custom report layouts.</span></span>

<span data-ttu-id="3a4d0-133">Custom layouts are report layouts that you design to change the appearance of a report.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-133">Custom layouts are report layouts that you design to change the appearance of a report.</span></span> <span data-ttu-id="3a4d0-134">You typically create a custom layout based on a built-in layout, but you can create them from scratch or from a copy of an existing custom layout.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-134">You typically create a custom layout based on a built-in layout, but you can create them from scratch or from a copy of an existing custom layout.</span></span> <span data-ttu-id="3a4d0-135">Custom layouts enable you to have multiple layouts for the same report, which you switch among as needed.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-135">Custom layouts enable you to have multiple layouts for the same report, which you switch among as needed.</span></span> <span data-ttu-id="3a4d0-136">For example, you can have different layouts for each [!INCLUDE[d365fin](includes/d365fin_md.md)] company, or you can have different layouts for the same company for specific occasions or events, like a special campaign or holiday season.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-136">For example, you can have different layouts for each [!INCLUDE[d365fin](includes/d365fin_md.md)] company, or you can have different layouts for the same company for specific occasions or events, like a special campaign or holiday season.</span></span>

## <a name="deciding-whether-to-use-a-word-or-rdlc-report-layout"></a><span data-ttu-id="3a4d0-137">Deciding whether to use a Word or RDLC report layout</span><span class="sxs-lookup"><span data-stu-id="3a4d0-137">Deciding whether to use a Word or RDLC report layout</span></span>
<span data-ttu-id="3a4d0-138">A report layout can be based on either a Word document or RDLC file.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-138">A report layout can be based on either a Word document or RDLC file.</span></span> <span data-ttu-id="3a4d0-139">Deciding on whether to use a Word report layout or RDLC report layout type will depend on how you want the generated report to look and your knowledge of Word and SQL Server Report Builder.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-139">Deciding on whether to use a Word report layout or RDLC report layout type will depend on how you want the generated report to look and your knowledge of Word and SQL Server Report Builder.</span></span>

<span data-ttu-id="3a4d0-140">The general design concepts for Word and RDLC layouts are very similar.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-140">The general design concepts for Word and RDLC layouts are very similar.</span></span> <span data-ttu-id="3a4d0-141">However each type has certain design features that affect how the generated report is appears in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3a4d0-141">However each type has certain design features that affect how the generated report is appears in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="3a4d0-142">This means that the same report might look different when using the Word report layout compared to the RDLC report layout.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-142">This means that the same report might look different when using the Word report layout compared to the RDLC report layout.</span></span>

<span data-ttu-id="3a4d0-143">The process for setting up Word report layouts and RDLC report layouts on reports is the same.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-143">The process for setting up Word report layouts and RDLC report layouts on reports is the same.</span></span> <span data-ttu-id="3a4d0-144">The main difference is in the way you modify the layouts.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-144">The main difference is in the way you modify the layouts.</span></span> <span data-ttu-id="3a4d0-145">Word report layouts are typically easier to create and modify than RDLC report layouts because you can use Word.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-145">Word report layouts are typically easier to create and modify than RDLC report layouts because you can use Word.</span></span> <span data-ttu-id="3a4d0-146">RDLC report layouts are modified by using SQL Server Report builder which targets more advanced users.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-146">RDLC report layouts are modified by using SQL Server Report builder which targets more advanced users.</span></span>

<span data-ttu-id="3a4d0-147">For information on how to change which layout to use, see [Change Which Layout is Currently Used on a Report](ui-how-change-layout-currently-used-report.md).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-147">For information on how to change which layout to use, see [Change Which Layout is Currently Used on a Report](ui-how-change-layout-currently-used-report.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="3a4d0-148">See Also</span><span class="sxs-lookup"><span data-stu-id="3a4d0-148">See Also</span></span>
[<span data-ttu-id="3a4d0-149">Updating Report or Document Layouts</span><span class="sxs-lookup"><span data-stu-id="3a4d0-149">Updating Report or Document Layouts</span></span>](ui-update-report-layouts.md)  
<span data-ttu-id="3a4d0-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3a4d0-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="3a4d0-151">Create and Modify a Custom Report or Document Layout</span><span class="sxs-lookup"><span data-stu-id="3a4d0-151">Create and Modify a Custom Report or Document Layout</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="3a4d0-152">Import and Export a Custom Report or Document Layout</span><span class="sxs-lookup"><span data-stu-id="3a4d0-152">Import and Export a Custom Report or Document Layout</span></span>](ui-how-import-and-export-report-layout.md)  
[<span data-ttu-id="3a4d0-153">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="3a4d0-153">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
[<span data-ttu-id="3a4d0-154">Working with Reports</span><span class="sxs-lookup"><span data-stu-id="3a4d0-154">Working with Reports</span></span>](ui-work-report.md)  
