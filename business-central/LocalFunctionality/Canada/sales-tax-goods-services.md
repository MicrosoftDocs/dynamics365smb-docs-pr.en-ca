---
title: Sales Tax in Canada| Microsoft Docs
description: Learn about local sales tax and goods and services tax in Canada.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales tax, local
ms.date: 04/01/2019
ms.author: edupont
ms.openlocfilehash: a1ecb0a4c3ee855ef51bf44987d97171e02a3f26
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/31/2019
ms.locfileid: "935490"
---
# <a name="reporting-sales-tax-and-goodsservices-tax-in-canada"></a><span data-ttu-id="0fc15-103">Reporting Sales Tax and Goods/Services Tax in Canada</span><span class="sxs-lookup"><span data-stu-id="0fc15-103">Reporting Sales Tax and Goods/Services Tax in Canada</span></span>
<span data-ttu-id="0fc15-104">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span><span class="sxs-lookup"><span data-stu-id="0fc15-104">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span></span> <span data-ttu-id="0fc15-105">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span><span class="sxs-lookup"><span data-stu-id="0fc15-105">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span></span> <span data-ttu-id="0fc15-106">When a Provincial Tax Area Code is selected, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span><span class="sxs-lookup"><span data-stu-id="0fc15-106">When a Provincial Tax Area Code is selected, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span></span> <span data-ttu-id="0fc15-107">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span><span class="sxs-lookup"><span data-stu-id="0fc15-107">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span></span>  

## <a name="submitting-the-gsthst-file"></a><span data-ttu-id="0fc15-108">Submitting the GST/HST File</span><span class="sxs-lookup"><span data-stu-id="0fc15-108">Submitting the GST/HST File</span></span>
<span data-ttu-id="0fc15-109">The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities.</span><span class="sxs-lookup"><span data-stu-id="0fc15-109">The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities.</span></span> <span data-ttu-id="0fc15-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span><span class="sxs-lookup"><span data-stu-id="0fc15-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span></span> <span data-ttu-id="0fc15-111">The file is created in a .tax file format, which can be transferred online.</span><span class="sxs-lookup"><span data-stu-id="0fc15-111">The file is created in a .tax file format, which can be transferred online.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0fc15-112">See Also</span><span class="sxs-lookup"><span data-stu-id="0fc15-112">See Also</span></span>
[<span data-ttu-id="0fc15-113">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="0fc15-113">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="0fc15-114">Finance</span><span class="sxs-lookup"><span data-stu-id="0fc15-114">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="0fc15-115">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="0fc15-115">Setting Up Finance</span></span>](../../finance-setup-finance.md)  
[<span data-ttu-id="0fc15-116">Reporting Sales Tax in Canada</span><span class="sxs-lookup"><span data-stu-id="0fc15-116">Reporting Sales Tax in Canada</span></span>](ca-sales-tax.md)  
<span data-ttu-id="0fc15-117">[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0fc15-117">[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)</span></span>
