---
title: Set Up Time Sheets and Their Approval| Microsoft Docs
description: You set up time sheets to track the time used on jobs and using resources, helping you with project management, staffing, and capacity
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff, resource
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 057497cfee69ed91c5d37828ea290749585f93d8
ms.contentlocale: en-ca
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-time-sheets"></a><span data-ttu-id="deafc-103">Set Up Time Sheets</span><span class="sxs-lookup"><span data-stu-id="deafc-103">Set Up Time Sheets</span></span>
<span data-ttu-id="deafc-104">Time sheets in [!INCLUDE[d365fin](includes/d365fin_md.md)] handle time registration in weekly increments of seven days.</span><span class="sxs-lookup"><span data-stu-id="deafc-104">Time sheets in [!INCLUDE[d365fin](includes/d365fin_md.md)] handle time registration in weekly increments of seven days.</span></span> <span data-ttu-id="deafc-105">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span><span class="sxs-lookup"><span data-stu-id="deafc-105">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span></span> <span data-ttu-id="deafc-106">Before you can use time sheets, you must specify how you want them to be set up and configured.</span><span class="sxs-lookup"><span data-stu-id="deafc-106">Before you can use time sheets, you must specify how you want them to be set up and configured.</span></span>

<span data-ttu-id="deafc-107">After you have set up how your organization will use time sheets, you can specify if and how time sheets are approved.</span><span class="sxs-lookup"><span data-stu-id="deafc-107">After you have set up how your organization will use time sheets, you can specify if and how time sheets are approved.</span></span> <span data-ttu-id="deafc-108">Depending on the needs of your organization, you can designate:</span><span class="sxs-lookup"><span data-stu-id="deafc-108">Depending on the needs of your organization, you can designate:</span></span>

* <span data-ttu-id="deafc-109">One or more users as the time sheet administrator and approver for all time sheets.</span><span class="sxs-lookup"><span data-stu-id="deafc-109">One or more users as the time sheet administrator and approver for all time sheets.</span></span>
* <span data-ttu-id="deafc-110">A time sheet approver for each resource.</span><span class="sxs-lookup"><span data-stu-id="deafc-110">A time sheet approver for each resource.</span></span>

<span data-ttu-id="deafc-111">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span><span class="sxs-lookup"><span data-stu-id="deafc-111">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span></span> <span data-ttu-id="deafc-112">For more information, see [Use Time Sheets](projects-how-use-time-sheets.md).</span><span class="sxs-lookup"><span data-stu-id="deafc-112">For more information, see [Use Time Sheets](projects-how-use-time-sheets.md).</span></span>

## <a name="to-set-up-general-information-for-time-sheets"></a><span data-ttu-id="deafc-113">To set up general information for time sheets</span><span class="sxs-lookup"><span data-stu-id="deafc-113">To set up general information for time sheets</span></span>
1. <span data-ttu-id="deafc-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="deafc-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="deafc-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="deafc-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="deafc-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="deafc-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span></span>

| <span data-ttu-id="deafc-117">Option</span><span class="sxs-lookup"><span data-stu-id="deafc-117">Option</span></span> | <span data-ttu-id="deafc-118">Description</span><span class="sxs-lookup"><span data-stu-id="deafc-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="deafc-119">**Never**</span><span class="sxs-lookup"><span data-stu-id="deafc-119">**Never**</span></span> |<span data-ttu-id="deafc-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="deafc-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span> |
| <span data-ttu-id="deafc-121">**Always**</span><span class="sxs-lookup"><span data-stu-id="deafc-121">**Always**</span></span> |<span data-ttu-id="deafc-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="deafc-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span></span> |
| <span data-ttu-id="deafc-123">**Machine Only**</span><span class="sxs-lookup"><span data-stu-id="deafc-123">**Machine Only**</span></span> |<span data-ttu-id="deafc-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="deafc-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span></span> <span data-ttu-id="deafc-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="deafc-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span> |

## <a name="to-assign-a-time-sheet-administrator"></a><span data-ttu-id="deafc-126">To assign a time sheet administrator</span><span class="sxs-lookup"><span data-stu-id="deafc-126">To assign a time sheet administrator</span></span>
1. <span data-ttu-id="deafc-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="deafc-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="deafc-128">Add a new user if the user list does not include the person who you want to be the time sheet administrator.</span><span class="sxs-lookup"><span data-stu-id="deafc-128">Add a new user if the user list does not include the person who you want to be the time sheet administrator.</span></span> <span data-ttu-id="deafc-129">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="deafc-129">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span></span>
3. <span data-ttu-id="deafc-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.** check box.</span><span class="sxs-lookup"><span data-stu-id="deafc-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.** check box.</span></span>  

> [!TIP]  
>   <span data-ttu-id="deafc-131">It is recommended that you designate only one user to be the time sheet administrator for a company.</span><span class="sxs-lookup"><span data-stu-id="deafc-131">It is recommended that you designate only one user to be the time sheet administrator for a company.</span></span> <span data-ttu-id="deafc-132">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span><span class="sxs-lookup"><span data-stu-id="deafc-132">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span></span>  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a><span data-ttu-id="deafc-133">To assign a time sheets owner and approver</span><span class="sxs-lookup"><span data-stu-id="deafc-133">To assign a time sheets owner and approver</span></span>
1. <span data-ttu-id="deafc-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="deafc-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources**, and then choose the related link.</span></span>
2. <span data-ttu-id="deafc-135">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span><span class="sxs-lookup"><span data-stu-id="deafc-135">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span></span>  
3. <span data-ttu-id="deafc-136">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="deafc-136">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span></span> <span data-ttu-id="deafc-137">The owner can enter time usage on a time sheet and submit it for approval.</span><span class="sxs-lookup"><span data-stu-id="deafc-137">The owner can enter time usage on a time sheet and submit it for approval.</span></span> <span data-ttu-id="deafc-138">In general, when the resource is a person, that person is also the owner.</span><span class="sxs-lookup"><span data-stu-id="deafc-138">In general, when the resource is a person, that person is also the owner.</span></span>  
4. <span data-ttu-id="deafc-139">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="deafc-139">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span></span> <span data-ttu-id="deafc-140">The approver can approve, reject, or reopen a time sheet.</span><span class="sxs-lookup"><span data-stu-id="deafc-140">The approver can approve, reject, or reopen a time sheet.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="deafc-141">You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span><span class="sxs-lookup"><span data-stu-id="deafc-141">You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span></span>

## <a name="see-also"></a><span data-ttu-id="deafc-142">See Also</span><span class="sxs-lookup"><span data-stu-id="deafc-142">See Also</span></span>
[<span data-ttu-id="deafc-143">Setting Up Project Management</span><span class="sxs-lookup"><span data-stu-id="deafc-143">Setting Up Project Management</span></span>](projects-setup-projects.md)  
[<span data-ttu-id="deafc-144">Project Management</span><span class="sxs-lookup"><span data-stu-id="deafc-144">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="deafc-145">Finance</span><span class="sxs-lookup"><span data-stu-id="deafc-145">Finance</span></span>](finance.md)  
<span data-ttu-id="deafc-146">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="deafc-146">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="deafc-147">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="deafc-147">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="deafc-148">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="deafc-148">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

