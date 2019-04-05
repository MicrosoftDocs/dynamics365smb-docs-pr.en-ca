---
title: Tips and Tricks - RapidStart Services | Microsoft Docs
description: When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 875ab6f5875a842fb4c2ab906f39ae95607f6ba8
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/08/2019
ms.locfileid: "812639"
---
# <a name="tips-and-tricks-rapidstart-services"></a><span data-ttu-id="10fdf-103">Tips and Tricks: RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="10fdf-103">Tips and Tricks: RapidStart Services</span></span>
<span data-ttu-id="10fdf-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span><span class="sxs-lookup"><span data-stu-id="10fdf-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span></span>  

## <a name="take-advantage-of-configuration-templates"></a><span data-ttu-id="10fdf-105">Take advantage of configuration templates</span><span class="sxs-lookup"><span data-stu-id="10fdf-105">Take advantage of configuration templates</span></span>  
<span data-ttu-id="10fdf-106">Configuration templates can help you streamline your implementation process.</span><span class="sxs-lookup"><span data-stu-id="10fdf-106">Configuration templates can help you streamline your implementation process.</span></span> <span data-ttu-id="10fdf-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span><span class="sxs-lookup"><span data-stu-id="10fdf-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span></span> <span data-ttu-id="10fdf-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span><span class="sxs-lookup"><span data-stu-id="10fdf-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span></span>  

## <a name="configuration-questionnaires"></a><span data-ttu-id="10fdf-109">Configuration questionnaires</span><span class="sxs-lookup"><span data-stu-id="10fdf-109">Configuration questionnaires</span></span>  
<span data-ttu-id="10fdf-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span><span class="sxs-lookup"><span data-stu-id="10fdf-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span></span>  

## <a name="batch-creation-of-journal-lines"></a><span data-ttu-id="10fdf-111">Batch creation of journal lines</span><span class="sxs-lookup"><span data-stu-id="10fdf-111">Batch creation of journal lines</span></span>  
<span data-ttu-id="10fdf-112">We recommend that you use the data migration tools provided to migrate journal entries.</span><span class="sxs-lookup"><span data-stu-id="10fdf-112">We recommend that you use the data migration tools provided to migrate journal entries.</span></span> <span data-ttu-id="10fdf-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span><span class="sxs-lookup"><span data-stu-id="10fdf-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span></span> <span data-ttu-id="10fdf-114">The rest of the journal then has to be completed manually.</span><span class="sxs-lookup"><span data-stu-id="10fdf-114">The rest of the journal then has to be completed manually.</span></span>  

## <a name="migrating-transactions"></a><span data-ttu-id="10fdf-115">Migrating transactions</span><span class="sxs-lookup"><span data-stu-id="10fdf-115">Migrating transactions</span></span>  
<span data-ttu-id="10fdf-116">We recommend that you migrate opening balances in the following order.</span><span class="sxs-lookup"><span data-stu-id="10fdf-116">We recommend that you migrate opening balances in the following order.</span></span>  

1.  <span data-ttu-id="10fdf-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span><span class="sxs-lookup"><span data-stu-id="10fdf-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span></span> <span data-ttu-id="10fdf-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span><span class="sxs-lookup"><span data-stu-id="10fdf-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span></span> <span data-ttu-id="10fdf-119">Set up the offsetting accounts to enable direct postings.</span><span class="sxs-lookup"><span data-stu-id="10fdf-119">Set up the offsetting accounts to enable direct postings.</span></span>  
2.  <span data-ttu-id="10fdf-120">Migrate open customer ledger entries.</span><span class="sxs-lookup"><span data-stu-id="10fdf-120">Migrate open customer ledger entries.</span></span>  
3.  <span data-ttu-id="10fdf-121">Migrate open item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="10fdf-121">Migrate open item ledger entries.</span></span>  
4.  <span data-ttu-id="10fdf-122">Migrate open fixed asset entries.</span><span class="sxs-lookup"><span data-stu-id="10fdf-122">Migrate open fixed asset entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="10fdf-123">See Also</span><span class="sxs-lookup"><span data-stu-id="10fdf-123">See Also</span></span>  
[<span data-ttu-id="10fdf-124">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="10fdf-124">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="10fdf-125">Administration</span><span class="sxs-lookup"><span data-stu-id="10fdf-125">Administration</span></span>](admin-setup-and-administration.md)
