---
title: Exchange Data | Microsoft Docs
description: You can exchange data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and external files or streams in connection with common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 8b2e20e694279a8c06188e0e429ef3b4fb43aea2
ms.openlocfilehash: f7ee9914d70474e912414ecd4de9a4cf16fa4e45
ms.contentlocale: en-ca
ms.lasthandoff: 09/27/2017

---
# <a name="exchanging-data"></a><span data-ttu-id="b8dc7-103">Exchanging Data</span><span class="sxs-lookup"><span data-stu-id="b8dc7-103">Exchanging Data</span></span>
<span data-ttu-id="b8dc7-104">You can exchange data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and external files or streams in connection with common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-104">You can exchange data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and external files or streams in connection with common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.</span></span>  

<span data-ttu-id="b8dc7-105">Before you can send and receive electronic documents or import and export bank files, you must set up the data exchange framework to process the involved data files or streams.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-105">Before you can send and receive electronic documents or import and export bank files, you must set up the data exchange framework to process the involved data files or streams.</span></span> <span data-ttu-id="b8dc7-106">In addition, you must set up related areas.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-106">In addition, you must set up related areas.</span></span> <span data-ttu-id="b8dc7-107">These include master data for customers that you send electronic invoices to and the bank data conversion service in case you distribute bank file conversions to an external service provider.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-107">These include master data for customers that you send electronic invoices to and the bank data conversion service in case you distribute bank file conversions to an external service provider.</span></span> <span data-ttu-id="b8dc7-108">For more information, see [Setting Up Data Exchange](across-set-up-data-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b8dc7-108">For more information, see [Setting Up Data Exchange](across-set-up-data-exchange.md).</span></span>  

 <span data-ttu-id="b8dc7-109">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-109">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="b8dc7-110">**To**</span><span class="sxs-lookup"><span data-stu-id="b8dc7-110">**To**</span></span>|<span data-ttu-id="b8dc7-111">**See**</span><span class="sxs-lookup"><span data-stu-id="b8dc7-111">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b8dc7-112">Convert sales document records in [!INCLUDE[d365fin](includes/d365fin_md.md)] to a standardized format and send them as electronic documents that your customers can receive into their system.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-112">Convert sales document records in [!INCLUDE[d365fin](includes/d365fin_md.md)] to a standardized format and send them as electronic documents that your customers can receive into their system.</span></span>|[<span data-ttu-id="b8dc7-113">How to: Send Electronic Documents</span><span class="sxs-lookup"><span data-stu-id="b8dc7-113">How to: Send Electronic Documents</span></span>](sales-how-to-send-electronic-documents.md)|  
|<span data-ttu-id="b8dc7-114">Send PDF or image files to a provider of OCR services, and receive them back as electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b8dc7-114">Send PDF or image files to a provider of OCR services, and receive them back as electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|[<span data-ttu-id="b8dc7-115">How to: Use OCR to Turn PDF and Image Files into Electronic Documents</span><span class="sxs-lookup"><span data-stu-id="b8dc7-115">How to: Use OCR to Turn PDF and Image Files into Electronic Documents</span></span>](across-how-use-ocr-pdf-images-files.md)|  
|<span data-ttu-id="b8dc7-116">Receive electronic documents, either from the OCR service or the document exchange service, in a standardized format that you convert to the relevant document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b8dc7-116">Receive electronic documents, either from the OCR service or the document exchange service, in a standardized format that you convert to the relevant document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>|[<span data-ttu-id="b8dc7-117">How to: Receive and Convert Electronic Documents</span><span class="sxs-lookup"><span data-stu-id="b8dc7-117">How to: Receive and Convert Electronic Documents</span></span>](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|<span data-ttu-id="b8dc7-118">Import a bank statement file into the **Payment Reconciliation Journal** window as the first step in reconciling payments or into the **Bank Acc. Reconciliation** window as the first step in reconciling bank accounts.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-118">Import a bank statement file into the **Payment Reconciliation Journal** window as the first step in reconciling payments or into the **Bank Acc. Reconciliation** window as the first step in reconciling bank accounts.</span></span>|[<span data-ttu-id="b8dc7-119">How to: Set Up the Envestnet Yodlee Bank Feeds Service</span><span class="sxs-lookup"><span data-stu-id="b8dc7-119">How to: Set Up the Envestnet Yodlee Bank Feeds Service</span></span>](bank-how-setup-bank-statement-service.md)|  
|<span data-ttu-id="b8dc7-120">Export payments from the **Payment Journal** window to a bank file that you upload to your electronic bank account for processing.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-120">Export payments from the **Payment Journal** window to a bank file that you upload to your electronic bank account for processing.</span></span>|[<span data-ttu-id="b8dc7-121">How to: Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="b8dc7-121">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="b8dc7-122">Instruct your bank to transfer payment amounts from your customers’ bank accounts to your company’s account according to your setup of SEPA direct debit.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-122">Instruct your bank to transfer payment amounts from your customers’ bank accounts to your company’s account according to your setup of SEPA direct debit.</span></span>|[<span data-ttu-id="b8dc7-123">How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File</span><span class="sxs-lookup"><span data-stu-id="b8dc7-123">How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File</span></span>](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|<span data-ttu-id="b8dc7-124">Use a service provider of currency exchange rates to update the **Currencies** window.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-124">Use a service provider of currency exchange rates to update the **Currencies** window.</span></span>|[<span data-ttu-id="b8dc7-125">How to: Update Currency Exchange Rates</span><span class="sxs-lookup"><span data-stu-id="b8dc7-125">How to: Update Currency Exchange Rates</span></span>](finance-how-update-currencies.md)|  
|<span data-ttu-id="b8dc7-126">View which file elements are mapped to fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] when importing SEPA CAMT statement files.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-126">View which file elements are mapped to fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] when importing SEPA CAMT statement files.</span></span>|[<span data-ttu-id="b8dc7-127">Field Mapping When Importing SEPA CAMT Files</span><span class="sxs-lookup"><span data-stu-id="b8dc7-127">Field Mapping When Importing SEPA CAMT Files</span></span>](across-field-mapping-when-importing-sepa-camt-files.md)|  
|<span data-ttu-id="b8dc7-128">View which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] are mapped to file elements when exporting payment files by using the Bank Date Conversion Service feature.</span><span class="sxs-lookup"><span data-stu-id="b8dc7-128">View which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] are mapped to file elements when exporting payment files by using the Bank Date Conversion Service feature.</span></span>|[<span data-ttu-id="b8dc7-129">Field Mapping When Exporting Payment Files Using Bank Data Conversion Service</span><span class="sxs-lookup"><span data-stu-id="b8dc7-129">Field Mapping When Exporting Payment Files Using Bank Data Conversion Service</span></span>](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a><span data-ttu-id="b8dc7-130">See Also</span><span class="sxs-lookup"><span data-stu-id="b8dc7-130">See Also</span></span>  
[<span data-ttu-id="b8dc7-131">Setting Up Data Exchange</span><span class="sxs-lookup"><span data-stu-id="b8dc7-131">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)  
[<span data-ttu-id="b8dc7-132">Exchanging Data Electronically</span><span class="sxs-lookup"><span data-stu-id="b8dc7-132">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
<span data-ttu-id="b8dc7-133">[How to: Invoice Sales](sales-how-invoice-sales.md) </span><span class="sxs-lookup"><span data-stu-id="b8dc7-133">[How to: Invoice Sales](sales-how-invoice-sales.md) </span></span>  
[<span data-ttu-id="b8dc7-134">How to: Record Purchases</span><span class="sxs-lookup"><span data-stu-id="b8dc7-134">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="b8dc7-135">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="b8dc7-135">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="b8dc7-136">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="b8dc7-136">General Business Functionality</span></span>](ui-across-business-areas.md)  
