---
title: Invoice your bookings in Business Central | Microsoft Docs
description: Learn how you can do bulk invoicing from Microsoft Bookings in Business Central .
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: invoicing, bookings
ms.date: 01/07/2019
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a98027c3ef3171491f84197897f93cbed4e288c2
ms.openlocfilehash: 65542f3855eff3a5ed117bff3247adbf05def6e2
ms.contentlocale: en-ca
ms.lasthandoff: 01/07/2019

---
# <a name="bulk-invoicing-for-microsoft-bookings-in-included365finincludesd365finmdmd"></a><span data-ttu-id="9d26e-103">Bulk Invoicing for Microsoft Bookings in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="9d26e-103">Bulk Invoicing for Microsoft Bookings in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
<span data-ttu-id="9d26e-104">If your company uses the Bookings app in Office 365, you can do bulk invoicing for appointments.</span><span class="sxs-lookup"><span data-stu-id="9d26e-104">If your company uses the Bookings app in Office 365, you can do bulk invoicing for appointments.</span></span> <span data-ttu-id="9d26e-105">The **Uninvoiced Bookings** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] provides a list of the company's completed bookings.</span><span class="sxs-lookup"><span data-stu-id="9d26e-105">The **Uninvoiced Bookings** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] provides a list of the company's completed bookings.</span></span> <span data-ttu-id="9d26e-106">In this page you can quickly select the appointments that you want to invoice and create draft invoices for the services provided.</span><span class="sxs-lookup"><span data-stu-id="9d26e-106">In this page you can quickly select the appointments that you want to invoice and create draft invoices for the services provided.</span></span>  

## <a name="connect-to-bookings"></a><span data-ttu-id="9d26e-107">Connect to Bookings</span><span class="sxs-lookup"><span data-stu-id="9d26e-107">Connect to Bookings</span></span>
<span data-ttu-id="9d26e-108">To connect your [!INCLUDE[d365fin](includes/d365fin_md.md)] with Bookings, you must specify your Bookings company, what to synchronize with Bookings, how often to synchronize, and which templates to use.</span><span class="sxs-lookup"><span data-stu-id="9d26e-108">To connect your [!INCLUDE[d365fin](includes/d365fin_md.md)] with Bookings, you must specify your Bookings company, what to synchronize with Bookings, how often to synchronize, and which templates to use.</span></span> <span data-ttu-id="9d26e-109">You set up this information on the **Booking Sync. Setup** page, which you can launch from the **Exchange Sync. Setup** page, which you can find through [Search](ui-search.md).</span><span class="sxs-lookup"><span data-stu-id="9d26e-109">You set up this information on the **Booking Sync. Setup** page, which you can launch from the **Exchange Sync. Setup** page, which you can find through [Search](ui-search.md).</span></span>  

<span data-ttu-id="9d26e-110">For example, if you want to synchronize customers between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the default template to use to add new customers in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on the customers in your Bookings company.</span><span class="sxs-lookup"><span data-stu-id="9d26e-110">For example, if you want to synchronize customers between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the default template to use to add new customers in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on the customers in your Bookings company.</span></span>  

> [!NOTE]
> <span data-ttu-id="9d26e-111">The Bookings app is designed to book appointments for individual customers rather than companies.</span><span class="sxs-lookup"><span data-stu-id="9d26e-111">The Bookings app is designed to book appointments for individual customers rather than companies.</span></span> <span data-ttu-id="9d26e-112">The synchronization with [!INCLUDE[d365fin](includes/d365fin_md.md)] will, therefore, only synchronize customer contacts with a Type of "Person".</span><span class="sxs-lookup"><span data-stu-id="9d26e-112">The synchronization with [!INCLUDE[d365fin](includes/d365fin_md.md)] will, therefore, only synchronize customer contacts with a Type of "Person".</span></span> <span data-ttu-id="9d26e-113">An email address is also required for the contact to synchronize.</span><span class="sxs-lookup"><span data-stu-id="9d26e-113">An email address is also required for the contact to synchronize.</span></span>  

<span data-ttu-id="9d26e-114">Similarly, if you want to synchronize service items between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the default template to use to add new service items in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on the services in our Bookings company.</span><span class="sxs-lookup"><span data-stu-id="9d26e-114">Similarly, if you want to synchronize service items between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the default template to use to add new service items in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on the services in our Bookings company.</span></span>  

> [!NOTE]
> <span data-ttu-id="9d26e-115">Only items of type *Service* will synchronize between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="9d26e-115">Only items of type *Service* will synchronize between Bookings and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="9d26e-116">The template that you set up in the **Configuration Templates** page so it can be used for the item synchronization must define the type as *Service*.</span><span class="sxs-lookup"><span data-stu-id="9d26e-116">The template that you set up in the **Configuration Templates** page so it can be used for the item synchronization must define the type as *Service*.</span></span>

## <a name="invoice-appointments"></a><span data-ttu-id="9d26e-117">Invoice Appointments</span><span class="sxs-lookup"><span data-stu-id="9d26e-117">Invoice Appointments</span></span>
<span data-ttu-id="9d26e-118">When it is time to send invoices for the completed bookings, you go to the **Uninvoiced Bookings** page.</span><span class="sxs-lookup"><span data-stu-id="9d26e-118">When it is time to send invoices for the completed bookings, you go to the **Uninvoiced Bookings** page.</span></span> <span data-ttu-id="9d26e-119">Depending on how often the information is synchronized, the list is long or short.</span><span class="sxs-lookup"><span data-stu-id="9d26e-119">Depending on how often the information is synchronized, the list is long or short.</span></span> <span data-ttu-id="9d26e-120">You can create invoices for all bookings in the list or one booking at a time.</span><span class="sxs-lookup"><span data-stu-id="9d26e-120">You can create invoices for all bookings in the list or one booking at a time.</span></span> <span data-ttu-id="9d26e-121">You can select one or more entries in the list and invoice those only.</span><span class="sxs-lookup"><span data-stu-id="9d26e-121">You can select one or more entries in the list and invoice those only.</span></span>  

<span data-ttu-id="9d26e-122">The support for invoicing appointments from Bookings is simpler than the fuller workflow of working with sales quotes, sales orders, and sales invoices.</span><span class="sxs-lookup"><span data-stu-id="9d26e-122">The support for invoicing appointments from Bookings is simpler than the fuller workflow of working with sales quotes, sales orders, and sales invoices.</span></span> <span data-ttu-id="9d26e-123">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="9d26e-123">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span> <span data-ttu-id="9d26e-124">You can choose to sell your services using [!INCLUDE[d365fin](includes/d365fin_md.md)] or choose to use Bookings, depending on your business needs.</span><span class="sxs-lookup"><span data-stu-id="9d26e-124">You can choose to sell your services using [!INCLUDE[d365fin](includes/d365fin_md.md)] or choose to use Bookings, depending on your business needs.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9d26e-125">See Also</span><span class="sxs-lookup"><span data-stu-id="9d26e-125">See Also</span></span>
[<span data-ttu-id="9d26e-126">Finance</span><span class="sxs-lookup"><span data-stu-id="9d26e-126">Finance</span></span>](finance.md)  
[<span data-ttu-id="9d26e-127">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="9d26e-127">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="9d26e-128">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="9d26e-128">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="9d26e-129">Microsoft Bookings</span><span class="sxs-lookup"><span data-stu-id="9d26e-129">Microsoft Bookings</span></span>](https://products.office.com/en-us/business/scheduling-and-booking-app)  
