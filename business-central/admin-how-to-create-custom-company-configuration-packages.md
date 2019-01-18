---
title: How to Create Custom Company Configuration Packages | Microsoft Docs
description: As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers. You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: 868972e4d53d858834ba5985a3de3ffa1d4dcc6b
ms.contentlocale: en-ca
ms.lasthandoff: 11/22/2018

---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="45134-104">Create Custom Company Configuration Packages</span><span class="sxs-lookup"><span data-stu-id="45134-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="45134-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span><span class="sxs-lookup"><span data-stu-id="45134-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="45134-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span><span class="sxs-lookup"><span data-stu-id="45134-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="45134-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span><span class="sxs-lookup"><span data-stu-id="45134-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="45134-108">That lets you apply and set up new areas in a company as you need them</span><span class="sxs-lookup"><span data-stu-id="45134-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="45134-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span><span class="sxs-lookup"><span data-stu-id="45134-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="45134-110">Fixed Asset Setup</span><span class="sxs-lookup"><span data-stu-id="45134-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="45134-111">General Ledger Setup</span><span class="sxs-lookup"><span data-stu-id="45134-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="45134-112">Inventory Setup</span><span class="sxs-lookup"><span data-stu-id="45134-112">Inventory Setup</span></span>  
-   <span data-ttu-id="45134-113">Manufacturing Setup</span><span class="sxs-lookup"><span data-stu-id="45134-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="45134-114">Purchases and Payables Setup</span><span class="sxs-lookup"><span data-stu-id="45134-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="45134-115">Marketing Setup</span><span class="sxs-lookup"><span data-stu-id="45134-115">Marketing Setup</span></span>  
-   <span data-ttu-id="45134-116">Service Setup</span><span class="sxs-lookup"><span data-stu-id="45134-116">Service Setup</span></span>  
-   <span data-ttu-id="45134-117">Sales and Receivables Setup</span><span class="sxs-lookup"><span data-stu-id="45134-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="45134-118">Warehouse Setup</span><span class="sxs-lookup"><span data-stu-id="45134-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="45134-119">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="45134-119">General Posting Setup</span></span>  
-   <span data-ttu-id="45134-120">Tax Posting Setup</span><span class="sxs-lookup"><span data-stu-id="45134-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="45134-121">Inventory Posting Setup</span><span class="sxs-lookup"><span data-stu-id="45134-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="45134-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="45134-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="45134-123">To create a custom company configuration package</span><span class="sxs-lookup"><span data-stu-id="45134-123">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="45134-124">Create a new [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="45134-124">Create a new [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="45134-125">***NOT POSSIBLE Link to help for "Creating a New Tenant"***.</span><span class="sxs-lookup"><span data-stu-id="45134-125">***NOT POSSIBLE Link to help for "Creating a New Tenant"***.</span></span>   
2.  <span data-ttu-id="45134-126">Create a new company for the industry or solution template.</span><span class="sxs-lookup"><span data-stu-id="45134-126">Create a new company for the industry or solution template.</span></span> <span data-ttu-id="45134-127">For more information, see [Create a New Company](admin-how-to-create-a-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="45134-127">For more information, see [Create a New Company](admin-how-to-create-a-new-company.md).</span></span>  
3.  <span data-ttu-id="45134-128">Setup the new company in the way you need.</span><span class="sxs-lookup"><span data-stu-id="45134-128">Setup the new company in the way you need.</span></span> <span data-ttu-id="45134-129">Fill in all required setup tables.</span><span class="sxs-lookup"><span data-stu-id="45134-129">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="45134-130">Open the new company.</span><span class="sxs-lookup"><span data-stu-id="45134-130">Open the new company.</span></span>
5. <span data-ttu-id="45134-131">Open the **Configuration Worksheet** page.</span><span class="sxs-lookup"><span data-stu-id="45134-131">Open the **Configuration Worksheet** page.</span></span>  
6.  <span data-ttu-id="45134-132">Add the tables that you want to transfer to another company to the worksheet.</span><span class="sxs-lookup"><span data-stu-id="45134-132">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="45134-133">Assign the worksheet lines to the package.</span><span class="sxs-lookup"><span data-stu-id="45134-133">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="45134-134">Create a questionnaire for the most frequently used setup tables.</span><span class="sxs-lookup"><span data-stu-id="45134-134">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="45134-135">Create configuration templates to make it easier to create master data, such as customers or items.</span><span class="sxs-lookup"><span data-stu-id="45134-135">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="45134-136">Export your package as a .rapidstart file.</span><span class="sxs-lookup"><span data-stu-id="45134-136">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="45134-137">See Also</span><span class="sxs-lookup"><span data-stu-id="45134-137">See Also</span></span>  
[<span data-ttu-id="45134-138">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="45134-138">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="45134-139">Administration</span><span class="sxs-lookup"><span data-stu-id="45134-139">Administration</span></span>](admin-setup-and-administration.md)

