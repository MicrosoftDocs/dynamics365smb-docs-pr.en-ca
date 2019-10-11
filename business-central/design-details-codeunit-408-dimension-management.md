---
title: Design Details - Codeunit 408 Dimension Management | Microsoft Docs
description: Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: design-details-dimension-set-entries
ms.openlocfilehash: 3b3cc817ac79fa18a5f0b68b97a54fab9ac6711b
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 10/01/2019
ms.locfileid: "2307333"
---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="19c6b-103">Design Details: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="19c6b-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="19c6b-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="19c6b-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="19c6b-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span><span class="sxs-lookup"><span data-stu-id="19c6b-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="19c6b-106">Many functions are deleted because there is no need for copying between dimension tables.</span><span class="sxs-lookup"><span data-stu-id="19c6b-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="19c6b-107">Modified Functions</span><span class="sxs-lookup"><span data-stu-id="19c6b-107">Modified Functions</span></span>  

|<span data-ttu-id="19c6b-108">Function Name</span><span class="sxs-lookup"><span data-stu-id="19c6b-108">Function Name</span></span>|<span data-ttu-id="19c6b-109">Modification Description</span><span class="sxs-lookup"><span data-stu-id="19c6b-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="19c6b-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="19c6b-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="19c6b-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span><span class="sxs-lookup"><span data-stu-id="19c6b-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="19c6b-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="19c6b-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="19c6b-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="19c6b-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="19c6b-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="19c6b-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="19c6b-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="19c6b-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="19c6b-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="19c6b-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="19c6b-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="19c6b-117">CheckDimValueComb</span></span>|<span data-ttu-id="19c6b-118">Delete.</span><span class="sxs-lookup"><span data-stu-id="19c6b-118">Delete.</span></span> <span data-ttu-id="19c6b-119">All usage should be changed to CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="19c6b-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="19c6b-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-120">GetDefaultDim</span></span>|<span data-ttu-id="19c6b-121">Modify to return an integer Dimension Set ID instead of a set of records.</span><span class="sxs-lookup"><span data-stu-id="19c6b-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="19c6b-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="19c6b-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="19c6b-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="19c6b-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="19c6b-126">Modify to work with DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="19c6b-127">Deleted Functions</span><span class="sxs-lookup"><span data-stu-id="19c6b-127">Deleted Functions</span></span>  
 <span data-ttu-id="19c6b-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span><span class="sxs-lookup"><span data-stu-id="19c6b-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="19c6b-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="19c6b-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="19c6b-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span><span class="sxs-lookup"><span data-stu-id="19c6b-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="19c6b-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="19c6b-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="19c6b-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="19c6b-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="19c6b-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-136">InsertDocDim</span></span>  

 <span data-ttu-id="19c6b-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="19c6b-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="19c6b-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="19c6b-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="19c6b-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-141">InsertServContractDim</span></span>  

 <span data-ttu-id="19c6b-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="19c6b-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="19c6b-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="19c6b-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-144">GetDocDim</span></span>  

 <span data-ttu-id="19c6b-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-145">GetProdDocDim</span></span>  

 <span data-ttu-id="19c6b-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="19c6b-146">TypeToTableID1</span></span>  

 <span data-ttu-id="19c6b-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="19c6b-147">TypeToTableID2</span></span>  

 <span data-ttu-id="19c6b-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="19c6b-148">TypeToTableID3</span></span>  

 <span data-ttu-id="19c6b-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="19c6b-149">TypeToTableID4</span></span>  

 <span data-ttu-id="19c6b-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="19c6b-150">TypeToTableID5</span></span>  

 <span data-ttu-id="19c6b-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-152">DeleteDocDim</span></span>  

 <span data-ttu-id="19c6b-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="19c6b-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="19c6b-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="19c6b-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="19c6b-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="19c6b-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-160">ShowDocDim</span></span>  

 <span data-ttu-id="19c6b-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-161">SaveDocDim</span></span>  

 <span data-ttu-id="19c6b-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="19c6b-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="19c6b-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-164">ShowTempDim</span></span>  

 <span data-ttu-id="19c6b-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-165">SaveTempDim</span></span>  

 <span data-ttu-id="19c6b-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="19c6b-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="19c6b-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-168">SaveServContractDim</span></span>  

 <span data-ttu-id="19c6b-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="19c6b-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="19c6b-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="19c6b-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="19c6b-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="19c6b-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="19c6b-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="19c6b-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="19c6b-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="19c6b-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="19c6b-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="19c6b-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="19c6b-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="19c6b-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="19c6b-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="19c6b-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="19c6b-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="19c6b-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="19c6b-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="19c6b-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="19c6b-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="19c6b-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="19c6b-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="19c6b-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="19c6b-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="19c6b-198">TestDimValue</span></span>  

 <span data-ttu-id="19c6b-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="19c6b-199">TestNewDimValue</span></span>  

 <span data-ttu-id="19c6b-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="19c6b-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="19c6b-201">(Delete because the ItemBudgetDim Table is deleted.)</span><span class="sxs-lookup"><span data-stu-id="19c6b-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="19c6b-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-202">GetServContractDim</span></span>  

 <span data-ttu-id="19c6b-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="19c6b-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="19c6b-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="19c6b-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="19c6b-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="19c6b-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="19c6b-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="19c6b-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="19c6b-207">See Also</span><span class="sxs-lookup"><span data-stu-id="19c6b-207">See Also</span></span>
 <span data-ttu-id="19c6b-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="19c6b-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="19c6b-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="19c6b-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="19c6b-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="19c6b-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 [<span data-ttu-id="19c6b-211">Design Details: Table Structure</span><span class="sxs-lookup"><span data-stu-id="19c6b-211">Design Details: Table Structure</span></span>](design-details-table-structure.md)   
 
