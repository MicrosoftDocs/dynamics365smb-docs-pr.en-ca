---
title: Power BI Integration Component and Architecture Overview for Business Central| Microsoft Docs
description: Getting insight, business intelligence, and KPIs from your Business Central data is easy with the Business Central apps for Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: 9514f0355932c1b1cbd30acfdb9f6dab46db8a0a
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697807"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prodshort"></a><span data-ttu-id="94dea-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="94dea-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prodshort](includes/prodshort.md)]</span></span>

<span data-ttu-id="94dea-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prodshort](includes/prodshort.md)] to help you understand its implementation and use.</span><span class="sxs-lookup"><span data-stu-id="94dea-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prodshort](includes/prodshort.md)] to help you understand its implementation and use.</span></span>

## <a name="components"></a><span data-ttu-id="94dea-105">Components</span><span class="sxs-lookup"><span data-stu-id="94dea-105">Components</span></span>

<span data-ttu-id="94dea-106">The following table describes the major components involved with Power BI integration.</span><span class="sxs-lookup"><span data-stu-id="94dea-106">The following table describes the major components involved with Power BI integration.</span></span>

|<span data-ttu-id="94dea-107">Component</span><span class="sxs-lookup"><span data-stu-id="94dea-107">Component</span></span>|<span data-ttu-id="94dea-108">Description</span><span class="sxs-lookup"><span data-stu-id="94dea-108">Description</span></span>|
|---------|-----------|
|<span data-ttu-id="94dea-109">Power BI</span><span class="sxs-lookup"><span data-stu-id="94dea-109">Power BI</span></span>|<span data-ttu-id="94dea-110">A cloud-based report hosting and management service.</span><span class="sxs-lookup"><span data-stu-id="94dea-110">A cloud-based report hosting and management service.</span></span>|
|<span data-ttu-id="94dea-111">Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="94dea-111">Power BI Desktop</span></span>|<span data-ttu-id="94dea-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span><span class="sxs-lookup"><span data-stu-id="94dea-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span></span> <span data-ttu-id="94dea-113">It's available as a free download on Microsoft Store and is installed locally.</span><span class="sxs-lookup"><span data-stu-id="94dea-113">It's available as a free download on Microsoft Store and is installed locally.</span></span>|
|[!INCLUDE[prodshort](includes/prodshort.md)]|<span data-ttu-id="94dea-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span><span class="sxs-lookup"><span data-stu-id="94dea-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span></span>|

## <a name="whats-available-from-the-start"></a><span data-ttu-id="94dea-115">What's available from the start</span><span class="sxs-lookup"><span data-stu-id="94dea-115">What's available from the start</span></span>

<span data-ttu-id="94dea-116">The following table describes available features.</span><span class="sxs-lookup"><span data-stu-id="94dea-116">The following table describes available features.</span></span>

|<span data-ttu-id="94dea-117">Feature</span><span class="sxs-lookup"><span data-stu-id="94dea-117">Feature</span></span>|[!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="94dea-118">online or on-premises support</span><span class="sxs-lookup"><span data-stu-id="94dea-118">online or on-premises support</span></span>|
|-------|---------------------|
|<span data-ttu-id="94dea-119">Power BI connectors</span><span class="sxs-lookup"><span data-stu-id="94dea-119">Power BI connectors</span></span>|<span data-ttu-id="94dea-120">Both.</span><span class="sxs-lookup"><span data-stu-id="94dea-120">Both.</span></span> <span data-ttu-id="94dea-121">Different connectors for online and on-premises.</span><span class="sxs-lookup"><span data-stu-id="94dea-121">Different connectors for online and on-premises.</span></span> <span data-ttu-id="94dea-122">Same connector used for Power BI Desktop and Power BI Service</span><span class="sxs-lookup"><span data-stu-id="94dea-122">Same connector used for Power BI Desktop and Power BI Service</span></span> |
|<span data-ttu-id="94dea-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="94dea-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prodshort](includes/prodshort.md)]</span></span>|<span data-ttu-id="94dea-124">Both.</span><span class="sxs-lookup"><span data-stu-id="94dea-124">Both.</span></span> <span data-ttu-id="94dea-125">Requires configuration to display reports for on-premises.</span><span class="sxs-lookup"><span data-stu-id="94dea-125">Requires configuration to display reports for on-premises.</span></span>|
|<span data-ttu-id="94dea-126">Power BI report management from [!INCLUDE[prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="94dea-126">Power BI report management from [!INCLUDE[prodshort](includes/prodshort.md)]</span></span>|<span data-ttu-id="94dea-127">Online</span><span class="sxs-lookup"><span data-stu-id="94dea-127">Online</span></span>|
|<span data-ttu-id="94dea-128">Default Power BI reports on role centres deployed to Power BI</span><span class="sxs-lookup"><span data-stu-id="94dea-128">Default Power BI reports on role centers deployed to Power BI</span></span>|<span data-ttu-id="94dea-129">Online</span><span class="sxs-lookup"><span data-stu-id="94dea-129">Online</span></span>|
|<span data-ttu-id="94dea-130">Power BI Apps on Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="94dea-130">Power BI Apps on Microsoft AppSource</span></span>|<span data-ttu-id="94dea-131">Online.</span><span class="sxs-lookup"><span data-stu-id="94dea-131">Online.</span></span>|

## <a name="architecture"></a><span data-ttu-id="94dea-132">Architecture</span><span class="sxs-lookup"><span data-stu-id="94dea-132">Architecture</span></span>

[!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="94dea-133">integrates with Power BI through a connector using OData.</span><span class="sxs-lookup"><span data-stu-id="94dea-133">integrates with Power BI through a connector using OData.</span></span> <span data-ttu-id="94dea-134">The data source for Power BI reports is exposed as OData web services.</span><span class="sxs-lookup"><span data-stu-id="94dea-134">The data source for Power BI reports is exposed as OData web services.</span></span>

![Power BI architecture for integration with Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a><span data-ttu-id="94dea-136">General Flow</span><span class="sxs-lookup"><span data-stu-id="94dea-136">General Flow</span></span>

<span data-ttu-id="94dea-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prodshort](includes/prodshort.md)] to Power BI.</span><span class="sxs-lookup"><span data-stu-id="94dea-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prodshort](includes/prodshort.md)] to Power BI.</span></span>

![Power BI workflow  for integration with Business Central](./media/power-bi-flow.png)

1. <span data-ttu-id="94dea-139">User signs up for a Power BI account.</span><span class="sxs-lookup"><span data-stu-id="94dea-139">User signs up for a Power BI account.</span></span>
2. <span data-ttu-id="94dea-140">User connects to Power BI from [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="94dea-140">User connects to Power BI from [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>
3. [!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="94dea-141">verifies the licence.</span><span class="sxs-lookup"><span data-stu-id="94dea-141">verifies the license.</span></span>
4. [!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="94dea-142">deploys default reports to the Power BI service.</span><span class="sxs-lookup"><span data-stu-id="94dea-142">deploys default reports to the Power BI service.</span></span> <span data-ttu-id="94dea-143">This step only happens for [!INCLUDE[prodshort](includes/prodshort.md)] online.</span><span class="sxs-lookup"><span data-stu-id="94dea-143">This step only happens for [!INCLUDE[prodshort](includes/prodshort.md)] online.</span></span>
5. [!INCLUDE[prodshort](includes/prodshort.md)] <span data-ttu-id="94dea-144">makes reports in Power BI available for selection in [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="94dea-144">makes reports in Power BI available for selection in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="94dea-145">Default reports are automatically displayed in Power BI parts.</span><span class="sxs-lookup"><span data-stu-id="94dea-145">Default reports are automatically displayed in Power BI parts.</span></span>
6. <span data-ttu-id="94dea-146">User creates a report in Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="94dea-146">User creates a report in Power BI Desktop.</span></span>
7. <span data-ttu-id="94dea-147">User publishes the report to the Power BI service.</span><span class="sxs-lookup"><span data-stu-id="94dea-147">User publishes the report to the Power BI service.</span></span> <span data-ttu-id="94dea-148">The reports are then available for selection in [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="94dea-148">The reports are then available for selection in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="94dea-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="94dea-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="94dea-150">See Also</span><span class="sxs-lookup"><span data-stu-id="94dea-150">See Also</span></span>

[<span data-ttu-id="94dea-151">Business Central and Power BI</span><span class="sxs-lookup"><span data-stu-id="94dea-151">Business Central and Power BI</span></span>](admin-powerbi.md)  
[<span data-ttu-id="94dea-152">Power BI for consumers</span><span class="sxs-lookup"><span data-stu-id="94dea-152">Power BI for consumers</span></span>](/power-bi/consumer/end-user-consumer)  
[<span data-ttu-id="94dea-153">The 'new look' of the Power BI service</span><span class="sxs-lookup"><span data-stu-id="94dea-153">The 'new look' of the Power BI service</span></span>](/power-bi/service-new-look)  
[<span data-ttu-id="94dea-154">Quickstart: Connect to data in Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="94dea-154">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
[<span data-ttu-id="94dea-155">Power BI documentation</span><span class="sxs-lookup"><span data-stu-id="94dea-155">Power BI documentation</span></span>](/power-bi/)  
[<span data-ttu-id="94dea-156">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="94dea-156">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="94dea-157">Getting Started</span><span class="sxs-lookup"><span data-stu-id="94dea-157">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="94dea-158">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="94dea-158">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="94dea-159">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="94dea-159">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
<span data-ttu-id="94dea-160">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="94dea-160">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
<span data-ttu-id="94dea-161">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span><span class="sxs-lookup"><span data-stu-id="94dea-161">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span></span>  
<span data-ttu-id="94dea-162">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="94dea-162">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
