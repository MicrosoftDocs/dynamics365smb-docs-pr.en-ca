---
title: Managing Personalization as an Administrator in Financials | Microsoft Docs
description: Learn how to customize the user interface to suit your way of working.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 07/26/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 854dddab2d958e128309aa201b53234d87d2c049
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="managing-personalization-as-an-administrator"></a><span data-ttu-id="9e202-103">Managing Personalization as an Administrator</span><span class="sxs-lookup"><span data-stu-id="9e202-103">Managing Personalization as an Administrator</span></span>
<!--NAV in the Web client-->
<span data-ttu-id="9e202-104">Users can personalize their workspace to suit their own preferences.</span><span class="sxs-lookup"><span data-stu-id="9e202-104">Users can personalize their workspace to suit their own preferences.</span></span> <span data-ttu-id="9e202-105">As an administrator, you can control and manage personalization by disabling the ability for users to personalize pages and clearing any page personalizations that users have made.</span><span class="sxs-lookup"><span data-stu-id="9e202-105">As an administrator, you can control and manage personalization by disabling the ability for users to personalize pages and clearing any page personalizations that users have made.</span></span>

## <a name="disable-personalization-for-a-profile"></a><span data-ttu-id="9e202-106">Disable personalization for a profile</span><span class="sxs-lookup"><span data-stu-id="9e202-106">Disable personalization for a profile</span></span>
<span data-ttu-id="9e202-107">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span><span class="sxs-lookup"><span data-stu-id="9e202-107">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span></span>
1.  <span data-ttu-id="9e202-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9e202-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>
2.  <span data-ttu-id="9e202-109">Select the profile in the list that you want to modify.</span><span class="sxs-lookup"><span data-stu-id="9e202-109">Select the profile in the list that you want to modify.</span></span>
3. <span data-ttu-id="9e202-110">Select the **Disable personalization** check box, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9e202-110">Select the **Disable personalization** check box, and then choose the **OK** button.</span></span>

## <a name="clear-user-personalizations"></a><span data-ttu-id="9e202-111">Clear user personalizations</span><span class="sxs-lookup"><span data-stu-id="9e202-111">Clear user personalizations</span></span>

<span data-ttu-id="9e202-112">Clearing page personalization changes the page back to its original layout before any personalization was made.</span><span class="sxs-lookup"><span data-stu-id="9e202-112">Clearing page personalization changes the page back to its original layout before any personalization was made.</span></span> <span data-ttu-id="9e202-113">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span><span class="sxs-lookup"><span data-stu-id="9e202-113">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span></span>

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a><span data-ttu-id="9e202-114">Clear user personalizations by using the Delete User Personalization page</span><span class="sxs-lookup"><span data-stu-id="9e202-114">Clear user personalizations by using the Delete User Personalization page</span></span>

<span data-ttu-id="9e202-115">The **Delete User Personalization** page enables you to clear personalizations on a per-page basis for each user individually.</span><span class="sxs-lookup"><span data-stu-id="9e202-115">The **Delete User Personalization** page enables you to clear personalizations on a per-page basis for each user individually.</span></span>

1.  <span data-ttu-id="9e202-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalization**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9e202-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="9e202-117">The page lists all the pages that have been personalized and the user it belongs to.</span><span class="sxs-lookup"><span data-stu-id="9e202-117">The page lists all the pages that have been personalized and the user it belongs to.</span></span>

    >[!NOTE]
    > <span data-ttu-id="9e202-118">A check mark in the **Legacy Personalization** columns indicates that the personalization was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalization different than it does now.</span><span class="sxs-lookup"><span data-stu-id="9e202-118">A check mark in the **Legacy Personalization** columns indicates that the personalization was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalization different than it does now.</span></span> <span data-ttu-id="9e202-119">Users who try to personalize these pages are locked from doing so unless they choose to unlock the page.</span><span class="sxs-lookup"><span data-stu-id="9e202-119">Users who try to personalize these pages are locked from doing so unless they choose to unlock the page.</span></span> <span data-ttu-id="9e202-120">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).</span><span class="sxs-lookup"><span data-stu-id="9e202-120">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).</span></span>

2. <span data-ttu-id="9e202-121">Select the entry that you want to delete, and then choose the **Delete** action.</span><span class="sxs-lookup"><span data-stu-id="9e202-121">Select the entry that you want to delete, and then choose the **Delete** action.</span></span>

    <span data-ttu-id="9e202-122">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="9e202-122">The user will see the changes the next time they sign-in.</span></span>

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a><span data-ttu-id="9e202-123">Clear user personalizations by using the User Personalization Card page</span><span class="sxs-lookup"><span data-stu-id="9e202-123">Clear user personalizations by using the User Personalization Card page</span></span>

<span data-ttu-id="9e202-124">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span><span class="sxs-lookup"><span data-stu-id="9e202-124">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span></span> <span data-ttu-id="9e202-125">This requires write permission to Table 2000000072 **Profile**.</span><span class="sxs-lookup"><span data-stu-id="9e202-125">This requires write permission to Table 2000000072 **Profile**.</span></span>

1.  <span data-ttu-id="9e202-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalization**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9e202-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="9e202-127">The **User Personalization** page lists all users who potentially have personalized pages.</span><span class="sxs-lookup"><span data-stu-id="9e202-127">The **User Personalization** page lists all users who potentially have personalized pages.</span></span> <span data-ttu-id="9e202-128">If you cannot find a user in the list, this means that they do not have any personalized pages.</span><span class="sxs-lookup"><span data-stu-id="9e202-128">If you cannot find a user in the list, this means that they do not have any personalized pages.</span></span>

2. <span data-ttu-id="9e202-129">Select the user from the list, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="9e202-129">Select the user from the list, and then choose the **Edit** action.</span></span>

3.  <span data-ttu-id="9e202-130">On the **Actions** tab, choose **Clear Personalized Pages**.</span><span class="sxs-lookup"><span data-stu-id="9e202-130">On the **Actions** tab, choose **Clear Personalized Pages**.</span></span>

    <span data-ttu-id="9e202-131">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="9e202-131">The user will see the changes the next time they sign-in.</span></span>

## <a name="see-also"></a><span data-ttu-id="9e202-132">See Also</span><span class="sxs-lookup"><span data-stu-id="9e202-132">See Also</span></span>
[<span data-ttu-id="9e202-133">Personalizing Your Workspace</span><span class="sxs-lookup"><span data-stu-id="9e202-133">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
<span data-ttu-id="9e202-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9e202-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="9e202-135">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="9e202-135">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
<span data-ttu-id="9e202-136">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="9e202-136">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span></span>  

