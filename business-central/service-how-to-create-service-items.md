---
title: How to Create Service Items | Microsoft Docs
description: When you receive an unregistered item for servicing, you can register it as a service item.
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
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: c30c0efc931b5970ff426141fa0dc3129d827306
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="create-service-items"></a><span data-ttu-id="9228c-103">Create Service Items</span><span class="sxs-lookup"><span data-stu-id="9228c-103">Create Service Items</span></span>
<span data-ttu-id="9228c-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the term "service item" refers to equipment or items that require service.</span><span class="sxs-lookup"><span data-stu-id="9228c-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the term "service item" refers to equipment or items that require service.</span></span> <span data-ttu-id="9228c-105">When you create a service order, you specify the items that need service.</span><span class="sxs-lookup"><span data-stu-id="9228c-105">When you create a service order, you specify the items that need service.</span></span> <span data-ttu-id="9228c-106">In the order, you can link a service item to an item in inventory or a service item group.</span><span class="sxs-lookup"><span data-stu-id="9228c-106">In the order, you can link a service item to an item in inventory or a service item group.</span></span>    

<span data-ttu-id="9228c-107">When you receive an item that needs service, you can register it as a service item.</span><span class="sxs-lookup"><span data-stu-id="9228c-107">When you receive an item that needs service, you can register it as a service item.</span></span> <span data-ttu-id="9228c-108">There are several ways to do so.</span><span class="sxs-lookup"><span data-stu-id="9228c-108">There are several ways to do so.</span></span> <span data-ttu-id="9228c-109">For example, you can create a service item on the **Service Items** page, or as part of another process, such as when working with a service order.</span><span class="sxs-lookup"><span data-stu-id="9228c-109">For example, you can create a service item on the **Service Items** page, or as part of another process, such as when working with a service order.</span></span>   

## <a name="to-create-a-service-item"></a><span data-ttu-id="9228c-110">To create a service item</span><span class="sxs-lookup"><span data-stu-id="9228c-110">To create a service item</span></span>  
1. <span data-ttu-id="9228c-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9228c-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="9228c-112">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="9228c-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-create-service-items-within-a-service-order"></a><span data-ttu-id="9228c-113">To create service items within a service order</span><span class="sxs-lookup"><span data-stu-id="9228c-113">To create service items within a service order</span></span>  
<span data-ttu-id="9228c-114">When you receive items for service that you want to register as service items, you can create them as service items in the **Service Order** or **Service Quote** pages.</span><span class="sxs-lookup"><span data-stu-id="9228c-114">When you receive items for service that you want to register as service items, you can create them as service items in the **Service Order** or **Service Quote** pages.</span></span>  

1. <span data-ttu-id="9228c-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9228c-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9228c-116">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="9228c-116">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="9228c-117">Choose the **Create Service Item** action.</span><span class="sxs-lookup"><span data-stu-id="9228c-117">Choose the **Create Service Item** action.</span></span>  

    <span data-ttu-id="9228c-118">A number is assigned to the service item and a service item card is created.</span><span class="sxs-lookup"><span data-stu-id="9228c-118">A number is assigned to the service item and a service item card is created.</span></span> <span data-ttu-id="9228c-119">The **Service Item No.** field is filled in with the number of the new service item.</span><span class="sxs-lookup"><span data-stu-id="9228c-119">The **Service Item No.** field is filled in with the number of the new service item.</span></span>

## <a name="to-create-a-service-item-when-shipping-items"></a><span data-ttu-id="9228c-120">To create a service item when shipping items</span><span class="sxs-lookup"><span data-stu-id="9228c-120">To create a service item when shipping items</span></span>  
<span data-ttu-id="9228c-121">When you ship items by posting either service orders or service invoices, the shipped items are automatically registered as service items if the following condition is met.</span><span class="sxs-lookup"><span data-stu-id="9228c-121">When you ship items by posting either service orders or service invoices, the shipped items are automatically registered as service items if the following condition is met.</span></span> <span data-ttu-id="9228c-122">The items must belong to a service item group with the **Create Service Item** check box selected.</span><span class="sxs-lookup"><span data-stu-id="9228c-122">The items must belong to a service item group with the **Create Service Item** check box selected.</span></span> <span data-ttu-id="9228c-123">If the items have serial numbers registered in the Item Tracking Lines page, this information is copied automatically to the **Serial No.** field on the service item card when creating service items.</span><span class="sxs-lookup"><span data-stu-id="9228c-123">If the items have serial numbers registered in the Item Tracking Lines page, this information is copied automatically to the **Serial No.** field on the service item card when creating service items.</span></span>  

<span data-ttu-id="9228c-124">The following procedure shows how to create service items when you ship items on service orders.</span><span class="sxs-lookup"><span data-stu-id="9228c-124">The following procedure shows how to create service items when you ship items on service orders.</span></span>  

1. <span data-ttu-id="9228c-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9228c-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9228c-126">Open the relevant service order.</span><span class="sxs-lookup"><span data-stu-id="9228c-126">Open the relevant service order.</span></span>  
3. <span data-ttu-id="9228c-127">Choose the **Post** or **Post and Print** action.</span><span class="sxs-lookup"><span data-stu-id="9228c-127">Choose the **Post** or **Post and Print** action.</span></span>  
4. <span data-ttu-id="9228c-128">Choose the **Ship** or **Ship and Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="9228c-128">Choose the **Ship** or **Ship and Invoice** action.</span></span>  
5. <span data-ttu-id="9228c-129">The service items are automatically created for the items on the order, provided these belong to a service item group that you have set up to create service items.</span><span class="sxs-lookup"><span data-stu-id="9228c-129">The service items are automatically created for the items on the order, provided these belong to a service item group that you have set up to create service items.</span></span> <span data-ttu-id="9228c-130">If you registered specific serial numbers on the **Item Tracking Lines** page, they will be assigned to these service items.</span><span class="sxs-lookup"><span data-stu-id="9228c-130">If you registered specific serial numbers on the **Item Tracking Lines** page, they will be assigned to these service items.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9228c-131">If an item is a BOM and you have exploded the BOM, the exploded BOM items are processed in the same way as regular items.</span><span class="sxs-lookup"><span data-stu-id="9228c-131">If an item is a BOM and you have exploded the BOM, the exploded BOM items are processed in the same way as regular items.</span></span> <span data-ttu-id="9228c-132">Service items are created based on the service items group condition and, optionally, the serial numbers condition.</span><span class="sxs-lookup"><span data-stu-id="9228c-132">Service items are created based on the service items group condition and, optionally, the serial numbers condition.</span></span> <span data-ttu-id="9228c-133">Additionally, if a service item is created for an exploded BOM item that is made up of other BOM components, these items are created as service item components for the exploded BOM service item.</span><span class="sxs-lookup"><span data-stu-id="9228c-133">Additionally, if a service item is created for an exploded BOM item that is made up of other BOM components, these items are created as service item components for the exploded BOM service item.</span></span>  
>   
>  <span data-ttu-id="9228c-134">If an item is a BOM and you have not exploded the BOM, a service item is created for it based on the service item group condition and, optionally, the serial numbers condition.</span><span class="sxs-lookup"><span data-stu-id="9228c-134">If an item is a BOM and you have not exploded the BOM, a service item is created for it based on the service item group condition and, optionally, the serial numbers condition.</span></span>  

## <a name="to-insert-a-starting-fee-for-a-service-item"></a><span data-ttu-id="9228c-135">To insert a starting fee for a service item</span><span class="sxs-lookup"><span data-stu-id="9228c-135">To insert a starting fee for a service item</span></span>
1. <span data-ttu-id="9228c-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Tasks**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9228c-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Tasks**, and then choose the related link.</span></span>
2. <span data-ttu-id="9228c-137">Choose the **Item Worksheet** action.</span><span class="sxs-lookup"><span data-stu-id="9228c-137">Choose the **Item Worksheet** action.</span></span>
3. <span data-ttu-id="9228c-138">Choose the service line, and then choose **Actions**, choose **Functions**, and then choose **Insert Starting Fee** action.</span><span class="sxs-lookup"><span data-stu-id="9228c-138">Choose the service line, and then choose **Actions**, choose **Functions**, and then choose **Insert Starting Fee** action.</span></span>  

    <span data-ttu-id="9228c-139">A service line of type **Cost** is inserted with the starting fee.</span><span class="sxs-lookup"><span data-stu-id="9228c-139">A service line of type **Cost** is inserted with the starting fee.</span></span> <span data-ttu-id="9228c-140">The starting fee applies to the selected service item.</span><span class="sxs-lookup"><span data-stu-id="9228c-140">The starting fee applies to the selected service item.</span></span>

## <a name="see-also"></a><span data-ttu-id="9228c-141">See Also</span><span class="sxs-lookup"><span data-stu-id="9228c-141">See Also</span></span>  
[<span data-ttu-id="9228c-142">Set Up Service Items and Service Item Components</span><span class="sxs-lookup"><span data-stu-id="9228c-142">Set Up Service Items and Service Item Components</span></span>](service-how-setup-service-items.md)  
[<span data-ttu-id="9228c-143">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="9228c-143">Setting Up Service Management</span></span>](service-setup-service.md)  
[<span data-ttu-id="9228c-144">Service Management</span><span class="sxs-lookup"><span data-stu-id="9228c-144">Service Management</span></span>](service-service.md)  
