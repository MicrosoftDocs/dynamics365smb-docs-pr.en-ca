---
title: Process Incoming Documents| Microsoft Docs
description: To record an external document, such as a PDF,  in Business Central , you first create or complete an incoming document record.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: 62400d6e5f6e67aca59ce836e9f20400e7b37635
ms.contentlocale: en-ca
ms.lasthandoff: 11/22/2018

---
# <a name="processing-incoming-documents"></a><span data-ttu-id="bf3b7-103">Processing Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="bf3b7-103">Processing Incoming Documents</span></span>
<span data-ttu-id="bf3b7-104">To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-104">To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record.</span></span> <span data-ttu-id="bf3b7-105">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-105">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="bf3b7-106">From PDF or image files that you receive from your trading partners, you can have an external OCR service (Optical Character Recognition) generate electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="bf3b7-106">From PDF or image files that you receive from your trading partners, you can have an external OCR service (Optical Character Recognition) generate electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="bf3b7-107">For example, when you receive an invoice in PDF format from your vendor, you can send it to the OCR service from the **Incoming Documents** page.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-107">For example, when you receive an invoice in PDF format from your vendor, you can send it to the OCR service from the **Incoming Documents** page.</span></span> <span data-ttu-id="bf3b7-108">Alternatively, you can send the file to the OCR service by email.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-108">Alternatively, you can send the file to the OCR service by email.</span></span> <span data-ttu-id="bf3b7-109">Then, when you receive the electronic document back, a related incoming document record is created automatically.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-109">Then, when you receive the electronic document back, a related incoming document record is created automatically.</span></span> <span data-ttu-id="bf3b7-110">After some seconds, you receive the file back from the OCR service as an electronic invoice that can be converted to a purchase invoice for the vendor.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-110">After some seconds, you receive the file back from the OCR service as an electronic invoice that can be converted to a purchase invoice for the vendor.</span></span>

| <span data-ttu-id="bf3b7-111">To</span><span class="sxs-lookup"><span data-stu-id="bf3b7-111">To</span></span> | <span data-ttu-id="bf3b7-112">See</span><span class="sxs-lookup"><span data-stu-id="bf3b7-112">See</span></span> |
| --- | --- |
| <span data-ttu-id="bf3b7-113">Create incoming document records manually or automatically by taking a photo of a paper receipt, for example.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-113">Create incoming document records manually or automatically by taking a photo of a paper receipt, for example.</span></span> |[<span data-ttu-id="bf3b7-114">Create Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="bf3b7-114">Create Incoming Document Records</span></span>](across-how-create-income-document-records.md) |
| <span data-ttu-id="bf3b7-115">Use an OCR service to turn PDF and image files into electronic documents that can be converted to purchase invoices in [!INCLUDE[d365fin](includes/d365fin_md.md)], for example.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-115">Use an OCR service to turn PDF and image files into electronic documents that can be converted to purchase invoices in [!INCLUDE[d365fin](includes/d365fin_md.md)], for example.</span></span> <span data-ttu-id="bf3b7-116">Train the OCR service to avoid errors next time it processes similar data.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-116">Train the OCR service to avoid errors next time it processes similar data.</span></span> |[<span data-ttu-id="bf3b7-117">Use OCR to Turn PDF and Image Files into Electronic Documents</span><span class="sxs-lookup"><span data-stu-id="bf3b7-117">Use OCR to Turn PDF and Image Files into Electronic Documents</span></span>](across-how-use-ocr-pdf-images-files.md) |
| <span data-ttu-id="bf3b7-118">Connect or remove incoming document records for any non-posted sales or purchase document and to any customer, vendor, or general ledger entry from the document or entry.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-118">Connect or remove incoming document records for any non-posted sales or purchase document and to any customer, vendor, or general ledger entry from the document or entry.</span></span> |[<span data-ttu-id="bf3b7-119">Create Incoming Document Records Directly from Documents and Entries</span><span class="sxs-lookup"><span data-stu-id="bf3b7-119">Create Incoming Document Records Directly from Documents and Entries</span></span>](across-how-connect-disconnect-income-document-records.md) |
| <span data-ttu-id="bf3b7-120">From the **Chart of Accounts** and **General Ledger Entries** pages, use a search function to find general ledger entries for posted documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-120">From the **Chart of Accounts** and **General Ledger Entries** pages, use a search function to find general ledger entries for posted documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span> |[<span data-ttu-id="bf3b7-121">Find Posted Documents without Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="bf3b7-121">Find Posted Documents without Incoming Document Records</span></span>](across-how-find-posted-documents-without-income-document-records.md) |
| <span data-ttu-id="bf3b7-122">Get better overview by setting incoming document records to Processed to remove them from the default view.</span><span class="sxs-lookup"><span data-stu-id="bf3b7-122">Get better overview by setting incoming document records to Processed to remove them from the default view.</span></span> |[<span data-ttu-id="bf3b7-123">Manage Many Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="bf3b7-123">Manage Many Incoming Document Records</span></span>](across-how-manage-many-income-document-records.md) |

## <a name="see-also"></a><span data-ttu-id="bf3b7-124">See Also</span><span class="sxs-lookup"><span data-stu-id="bf3b7-124">See Also</span></span>
[<span data-ttu-id="bf3b7-125">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="bf3b7-125">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="bf3b7-126">Purchasing</span><span class="sxs-lookup"><span data-stu-id="bf3b7-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="bf3b7-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bf3b7-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
