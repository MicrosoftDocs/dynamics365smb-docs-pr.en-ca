---
title: Automatic Transfer and Combined Entries | Microsoft Docs
description: In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting. You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition. The following table describes the different options.
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
ms.openlocfilehash: bd80d0a7a701256dfdae3346e899b84eeb990a40
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="d7845-105">Automatic Transfer and Combined Entries</span><span class="sxs-lookup"><span data-stu-id="d7845-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="d7845-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span><span class="sxs-lookup"><span data-stu-id="d7845-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="d7845-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span><span class="sxs-lookup"><span data-stu-id="d7845-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="d7845-108">The following table describes the different options.</span><span class="sxs-lookup"><span data-stu-id="d7845-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="d7845-109">Combine entries</span><span class="sxs-lookup"><span data-stu-id="d7845-109">Combine entries</span></span>|<span data-ttu-id="d7845-110">Description</span><span class="sxs-lookup"><span data-stu-id="d7845-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="d7845-111">None</span><span class="sxs-lookup"><span data-stu-id="d7845-111">None</span></span>|<span data-ttu-id="d7845-112">Each general ledger entry is transferred individually to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="d7845-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="d7845-113">Day</span><span class="sxs-lookup"><span data-stu-id="d7845-113">Day</span></span>|<span data-ttu-id="d7845-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="d7845-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="d7845-115">Month</span><span class="sxs-lookup"><span data-stu-id="d7845-115">Month</span></span>|<span data-ttu-id="d7845-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="d7845-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="d7845-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="d7845-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="d7845-118">Combined entries are not possible.</span><span class="sxs-lookup"><span data-stu-id="d7845-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d7845-119">See Also</span><span class="sxs-lookup"><span data-stu-id="d7845-119">See Also</span></span>  
 <span data-ttu-id="d7845-120">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="d7845-120">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="d7845-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="d7845-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="d7845-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="d7845-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 [<span data-ttu-id="d7845-123">Transferring and Posting Cost Entries</span><span class="sxs-lookup"><span data-stu-id="d7845-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 <span data-ttu-id="d7845-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d7845-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

