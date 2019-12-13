---
title: How to Reverse Output Posting | Microsoft Docs
description: There are times when output posting must be reversed. An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 2cdda8a01d6391f97bfae5600ce35d2ab989ae54
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 12/03/2019
ms.locfileid: "2877861"
---
# <a name="reverse-output-posting"></a><span data-ttu-id="2cfd9-104">Reverse Output Posting</span><span class="sxs-lookup"><span data-stu-id="2cfd9-104">Reverse Output Posting</span></span>
<span data-ttu-id="2cfd9-105">There are times when output posting must be reversed.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="2cfd9-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="2cfd9-107">To reverse an output posting</span><span class="sxs-lookup"><span data-stu-id="2cfd9-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="2cfd9-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="2cfd9-109">Select your batch.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-109">Select your batch.</span></span>  
2. <span data-ttu-id="2cfd9-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="2cfd9-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="2cfd9-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="2cfd9-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="2cfd9-113">This reverses the capacity and item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="2cfd9-114">Post the reversal by posting the journal.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="2cfd9-115">The output journal entries are posted to the item ledger as a positive adjustment.</span><span class="sxs-lookup"><span data-stu-id="2cfd9-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2cfd9-116">See Also</span><span class="sxs-lookup"><span data-stu-id="2cfd9-116">See Also</span></span>  
 <span data-ttu-id="2cfd9-117">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="2cfd9-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="2cfd9-118">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="2cfd9-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="2cfd9-119">[Planning](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="2cfd9-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="2cfd9-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="2cfd9-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="2cfd9-121">Purchasing</span><span class="sxs-lookup"><span data-stu-id="2cfd9-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="2cfd9-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2cfd9-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
