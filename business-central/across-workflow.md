---
title: Workflow | Microsoft Docs
description: You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 38092f364d1dee1f34d8aa0c0858ac1bc04d829b
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378807"
---
# <a name="workflows-in-dynamics-365-business-central"></a><span data-ttu-id="16665-105">Workflows in Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="16665-105">Workflows in Dynamics 365 Business Central</span></span>

<span data-ttu-id="16665-106">You can set up and use workflows that connect business-process tasks performed by different users.</span><span class="sxs-lookup"><span data-stu-id="16665-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="16665-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span><span class="sxs-lookup"><span data-stu-id="16665-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="16665-108">Requesting and granting approval to create new records are typical workflow steps.</span><span class="sxs-lookup"><span data-stu-id="16665-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="16665-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="16665-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="16665-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="16665-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="16665-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="16665-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="16665-112">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span><span class="sxs-lookup"><span data-stu-id="16665-112">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="16665-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="16665-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="16665-114">For more information, see the list of workflow templates in the Workflow Templates page.</span><span class="sxs-lookup"><span data-stu-id="16665-114">For more information, see the list of workflow templates in the Workflow Templates page.</span></span>  

 <span data-ttu-id="16665-115">If a business scenario requires a workflow event or response that is not supported, you can either use Power Automate or work with a Microsoft partner to customize the application code.</span><span class="sxs-lookup"><span data-stu-id="16665-115">If a business scenario requires a workflow event or response that is not supported, you can either use Power Automate or work with a Microsoft partner to customize the application code.</span></span> <span data-ttu-id="16665-116">For more information, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="16665-116">For more information, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>

<span data-ttu-id="16665-117">Any workflow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="16665-117">Any workflow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="16665-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="16665-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>  

 <span data-ttu-id="16665-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="16665-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="16665-120">**To**</span><span class="sxs-lookup"><span data-stu-id="16665-120">**To**</span></span>|<span data-ttu-id="16665-121">**See**</span><span class="sxs-lookup"><span data-stu-id="16665-121">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="16665-122">Set up workflow users, specify how users get notified, and create new workflows.</span><span class="sxs-lookup"><span data-stu-id="16665-122">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="16665-123">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span><span class="sxs-lookup"><span data-stu-id="16665-123">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="16665-124">Setting Up Workflows</span><span class="sxs-lookup"><span data-stu-id="16665-124">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="16665-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span><span class="sxs-lookup"><span data-stu-id="16665-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="16665-126">Archive and delete workflows.</span><span class="sxs-lookup"><span data-stu-id="16665-126">Archive and delete workflows.</span></span>|[<span data-ttu-id="16665-127">Using Workflows</span><span class="sxs-lookup"><span data-stu-id="16665-127">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="16665-128">See Also</span><span class="sxs-lookup"><span data-stu-id="16665-128">See Also</span></span>

[<span data-ttu-id="16665-129">Sales</span><span class="sxs-lookup"><span data-stu-id="16665-129">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="16665-130">Purchasing</span><span class="sxs-lookup"><span data-stu-id="16665-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="16665-131">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="16665-131">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="16665-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="16665-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]