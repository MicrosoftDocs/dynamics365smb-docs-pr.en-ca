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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 95ccd88d94359f595e2e8332786ac3f20877648e
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 10/01/2020
ms.locfileid: "3916438"
---
# <a name="reporting-sales-tax-and-goodsservices-tax-in-canada"></a><span data-ttu-id="e933d-103">Reporting Sales Tax and Goods/Services Tax in Canada</span><span class="sxs-lookup"><span data-stu-id="e933d-103">Reporting Sales Tax and Goods/Services Tax in Canada</span></span>
<span data-ttu-id="e933d-104">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span><span class="sxs-lookup"><span data-stu-id="e933d-104">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span></span> <span data-ttu-id="e933d-105">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span><span class="sxs-lookup"><span data-stu-id="e933d-105">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span></span> <span data-ttu-id="e933d-106">When a Provincial Tax Area Code is selected, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span><span class="sxs-lookup"><span data-stu-id="e933d-106">When a Provincial Tax Area Code is selected, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span></span> <span data-ttu-id="e933d-107">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span><span class="sxs-lookup"><span data-stu-id="e933d-107">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span></span>  

## <a name="submitting-the-gsthst-file"></a><span data-ttu-id="e933d-108">Submitting the GST/HST File</span><span class="sxs-lookup"><span data-stu-id="e933d-108">Submitting the GST/HST File</span></span>
<span data-ttu-id="e933d-109">The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities.</span><span class="sxs-lookup"><span data-stu-id="e933d-109">The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities.</span></span> <span data-ttu-id="e933d-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span><span class="sxs-lookup"><span data-stu-id="e933d-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span></span> <span data-ttu-id="e933d-111">The file is created in a .tax file format, which can be transferred online.</span><span class="sxs-lookup"><span data-stu-id="e933d-111">The file is created in a .tax file format, which can be transferred online.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e933d-112">See Also</span><span class="sxs-lookup"><span data-stu-id="e933d-112">See Also</span></span>
[<span data-ttu-id="e933d-113">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="e933d-113">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="e933d-114">Finance</span><span class="sxs-lookup"><span data-stu-id="e933d-114">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="e933d-115">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="e933d-115">Setting Up Finance</span></span>](../../finance-setup-finance.md)  
[<span data-ttu-id="e933d-116">Reporting Sales Tax in Canada</span><span class="sxs-lookup"><span data-stu-id="e933d-116">Reporting Sales Tax in Canada</span></span>](ca-sales-tax.md)  
<span data-ttu-id="e933d-117">[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e933d-117">[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)</span></span>
