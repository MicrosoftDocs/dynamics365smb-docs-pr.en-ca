---
title: How to Set Up a Document Exchange Service | Microsoft Docs
description: You use an external service provider to exchange electronic documents with your trading partners.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0217f077c9c38603b9e3ff945fd47394c5b943bb
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5384383"
---
# <a name="set-up-a-document-exchange-service"></a><span data-ttu-id="c96bd-103">Set Up a Document Exchange Service</span><span class="sxs-lookup"><span data-stu-id="c96bd-103">Set Up a Document Exchange Service</span></span>
<span data-ttu-id="c96bd-104">You use an external service provider to exchange electronic documents with your trading partners.</span><span class="sxs-lookup"><span data-stu-id="c96bd-104">You use an external service provider to exchange electronic documents with your trading partners.</span></span> <span data-ttu-id="c96bd-105">For more information, see [Exchanging Data Electronically](across-data-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="c96bd-105">For more information, see [Exchanging Data Electronically](across-data-exchange.md).</span></span>  

## <a name="to-set-up-a-document-exchange-service"></a><span data-ttu-id="c96bd-106">To set up a document exchange service</span><span class="sxs-lookup"><span data-stu-id="c96bd-106">To set up a document exchange service</span></span>  
1. <span data-ttu-id="c96bd-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Doc. Exch. Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c96bd-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Doc. Exch. Service Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="c96bd-108">Fill the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="c96bd-108">Fill the fields as described in the following table.</span></span>  

    |<span data-ttu-id="c96bd-109">Field</span><span class="sxs-lookup"><span data-stu-id="c96bd-109">Field</span></span>|<span data-ttu-id="c96bd-110">Description</span><span class="sxs-lookup"><span data-stu-id="c96bd-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="c96bd-111">**User Agent**</span><span class="sxs-lookup"><span data-stu-id="c96bd-111">**User Agent**</span></span>|<span data-ttu-id="c96bd-112">Enter any text that can be used to identify your company in document exchange processes.</span><span class="sxs-lookup"><span data-stu-id="c96bd-112">Enter any text that can be used to identify your company in document exchange processes.</span></span>|  
    |<span data-ttu-id="c96bd-113">**Doc. Exch. Tenant ID**</span><span class="sxs-lookup"><span data-stu-id="c96bd-113">**Doc. Exch. Tenant ID**</span></span>|<span data-ttu-id="c96bd-114">Enter the tenant in the document exchange service that represents your company.</span><span class="sxs-lookup"><span data-stu-id="c96bd-114">Enter the tenant in the document exchange service that represents your company.</span></span> <span data-ttu-id="c96bd-115">This is provided by the document exchange service provider.</span><span class="sxs-lookup"><span data-stu-id="c96bd-115">This is provided by the document exchange service provider.</span></span>|  
    |<span data-ttu-id="c96bd-116">**Enabled**</span><span class="sxs-lookup"><span data-stu-id="c96bd-116">**Enabled**</span></span>|<span data-ttu-id="c96bd-117">Specify if the service is enabled.</span><span class="sxs-lookup"><span data-stu-id="c96bd-117">Specify if the service is enabled.</span></span> <span data-ttu-id="c96bd-118">**Note:**  As soon as you enable the service, at least two job queue entries are created to process the traffic of electronic documents in and out of [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="c96bd-118">**Note:**  As soon as you enable the service, at least two job queue entries are created to process the traffic of electronic documents in and out of [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="c96bd-119">When you disable the service, the job queue entries are deleted.</span><span class="sxs-lookup"><span data-stu-id="c96bd-119">When you disable the service, the job queue entries are deleted.</span></span>|  
    |<span data-ttu-id="c96bd-120">**Signup URL**</span><span class="sxs-lookup"><span data-stu-id="c96bd-120">**Signup URL**</span></span>|<span data-ttu-id="c96bd-121">Specify the web page where you sign up for the document exchange service.</span><span class="sxs-lookup"><span data-stu-id="c96bd-121">Specify the web page where you sign up for the document exchange service.</span></span>|  
    |<span data-ttu-id="c96bd-122">**Service URL**</span><span class="sxs-lookup"><span data-stu-id="c96bd-122">**Service URL**</span></span>|<span data-ttu-id="c96bd-123">Specify the address of the document exchange service, which will be called when you send and receive electronic documents.</span><span class="sxs-lookup"><span data-stu-id="c96bd-123">Specify the address of the document exchange service, which will be called when you send and receive electronic documents.</span></span>|  
    |<span data-ttu-id="c96bd-124">**Login URL**</span><span class="sxs-lookup"><span data-stu-id="c96bd-124">**Login URL**</span></span>|<span data-ttu-id="c96bd-125">Specify the logon page for the document exchange service, which is where you enter your company’s user name and password to log on to the service.</span><span class="sxs-lookup"><span data-stu-id="c96bd-125">Specify the logon page for the document exchange service, which is where you enter your company’s user name and password to log on to the service.</span></span>|  
    |<span data-ttu-id="c96bd-126">**Consumer Key**</span><span class="sxs-lookup"><span data-stu-id="c96bd-126">**Consumer Key**</span></span>|<span data-ttu-id="c96bd-127">Enter the 3-legged OAuth key for the consumer key.</span><span class="sxs-lookup"><span data-stu-id="c96bd-127">Enter the 3-legged OAuth key for the consumer key.</span></span> <span data-ttu-id="c96bd-128">This is provided by the document exchange service provider.</span><span class="sxs-lookup"><span data-stu-id="c96bd-128">This is provided by the document exchange service provider.</span></span>|  
    |<span data-ttu-id="c96bd-129">**Consumer Secret**</span><span class="sxs-lookup"><span data-stu-id="c96bd-129">**Consumer Secret**</span></span>|<span data-ttu-id="c96bd-130">Enter the secret that protects the consumer key.</span><span class="sxs-lookup"><span data-stu-id="c96bd-130">Enter the secret that protects the consumer key.</span></span> <span data-ttu-id="c96bd-131">This is provided by the document exchange service provider.</span><span class="sxs-lookup"><span data-stu-id="c96bd-131">This is provided by the document exchange service provider.</span></span>|  
    |<span data-ttu-id="c96bd-132">**Token**</span><span class="sxs-lookup"><span data-stu-id="c96bd-132">**Token**</span></span>|<span data-ttu-id="c96bd-133">Enter the 3-legged OAuth key for the token.</span><span class="sxs-lookup"><span data-stu-id="c96bd-133">Enter the 3-legged OAuth key for the token.</span></span> <span data-ttu-id="c96bd-134">This is provided by the document exchange service provider.</span><span class="sxs-lookup"><span data-stu-id="c96bd-134">This is provided by the document exchange service provider.</span></span>|  
    |<span data-ttu-id="c96bd-135">**Token Secret**</span><span class="sxs-lookup"><span data-stu-id="c96bd-135">**Token Secret**</span></span>|<span data-ttu-id="c96bd-136">Enter the secret that protects the token.</span><span class="sxs-lookup"><span data-stu-id="c96bd-136">Enter the secret that protects the token.</span></span> <span data-ttu-id="c96bd-137">This is provided by the document exchange service provider.</span><span class="sxs-lookup"><span data-stu-id="c96bd-137">This is provided by the document exchange service provider.</span></span>|  

    > [!NOTE]  
    > <span data-ttu-id="c96bd-138">You login data is automatically encrypted.</span><span class="sxs-lookup"><span data-stu-id="c96bd-138">You login data is automatically encrypted.</span></span>

## <a name="see-also"></a><span data-ttu-id="c96bd-139">See Also</span><span class="sxs-lookup"><span data-stu-id="c96bd-139">See Also</span></span>  
[<span data-ttu-id="c96bd-140">Setting Up Data Exchange</span><span class="sxs-lookup"><span data-stu-id="c96bd-140">Setting Up Data Exchange</span></span>](across-set-up-data-exchange.md)  
[<span data-ttu-id="c96bd-141">Exchanging Data Electronically</span><span class="sxs-lookup"><span data-stu-id="c96bd-141">Exchanging Data Electronically</span></span>](across-data-exchange.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]