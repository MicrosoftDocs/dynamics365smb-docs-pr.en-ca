---
title: Search for Documents without Attachments| Microsoft Docs
Description: You can search for general ledger entries for posted purchase and sales documents that do not have incoming electronic documents, such as imported invoices.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: c355657821f5f4d18c707d296d9607cf5ec60442
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="f4a1f-102">Find Posted Documents without Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="f4a1f-102">Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="f4a1f-103">From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-103">From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="f4a1f-104">To find posted documents without incoming document records</span><span class="sxs-lookup"><span data-stu-id="f4a1f-104">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="f4a1f-105">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-105">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="f4a1f-106">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-106">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="f4a1f-107">Alternatively, choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-107">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="f4a1f-108">In the **General Ledger Entries** window, choose the **Posted Documents without Incoming Documents** action.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-108">In the **General Ledger Entries** window, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="f4a1f-109">The **Posted Documents without Incoming Document** window opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the window for.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-109">The **Posted Documents without Incoming Document** window opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the window for.</span></span> <span data-ttu-id="f4a1f-110">The window can show a maximum of 1000 lines.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-110">The window can show a maximum of 1000 lines.</span></span> <span data-ttu-id="f4a1f-111">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-111">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="f4a1f-112">To connect found documents to existing incoming document records</span><span class="sxs-lookup"><span data-stu-id="f4a1f-112">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="f4a1f-113">In the **Posted Documents without Incoming Document** window, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-113">In the **Posted Documents without Incoming Document** window, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="f4a1f-114">In the **Incoming Documents** window, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-114">In the **Incoming Documents** window, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="f4a1f-115">In the **Posted Documents without Incoming Document** window, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-115">In the **Posted Documents without Incoming Document** window, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="f4a1f-116">If a relevant incoming document record does not exist in the **Incoming Documents** window, then you can create it.</span><span class="sxs-lookup"><span data-stu-id="f4a1f-116">If a relevant incoming document record does not exist in the **Incoming Documents** window, then you can create it.</span></span> <span data-ttu-id="f4a1f-117">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="f4a1f-117">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="f4a1f-118">See Also</span><span class="sxs-lookup"><span data-stu-id="f4a1f-118">See Also</span></span>
[<span data-ttu-id="f4a1f-119">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="f4a1f-119">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="f4a1f-120">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="f4a1f-120">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="f4a1f-121">Purchasing</span><span class="sxs-lookup"><span data-stu-id="f4a1f-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="f4a1f-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f4a1f-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
