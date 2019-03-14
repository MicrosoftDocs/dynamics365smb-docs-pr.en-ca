---
title: Manage users and roles | Microsoft Docs
description: Learn how to manage users and Role Centres in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: profiles, users
ms.date: 10/24/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 7ecd8a5ad2b321d4d1683047e70ede90c7ce229f
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="understanding-users-profiles-and-role-centers"></a><span data-ttu-id="056bb-103">Understanding Users, Profiles, and Role Centres</span><span class="sxs-lookup"><span data-stu-id="056bb-103">Understanding Users, Profiles, and Role Centers</span></span>

<span data-ttu-id="056bb-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span><span class="sxs-lookup"><span data-stu-id="056bb-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span></span>  

<span data-ttu-id="056bb-105">Access to functionality is managed through *user groups* and *profiles*.</span><span class="sxs-lookup"><span data-stu-id="056bb-105">Access to functionality is managed through *user groups* and *profiles*.</span></span> <span data-ttu-id="056bb-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span><span class="sxs-lookup"><span data-stu-id="056bb-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span></span>  

## <a name="adding-users"></a><span data-ttu-id="056bb-107">Adding Users</span><span class="sxs-lookup"><span data-stu-id="056bb-107">Adding Users</span></span>

<span data-ttu-id="056bb-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Centre.</span><span class="sxs-lookup"><span data-stu-id="056bb-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Center.</span></span> <span data-ttu-id="056bb-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span><span class="sxs-lookup"><span data-stu-id="056bb-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span></span>

<span data-ttu-id="056bb-110">Then, the administrator can assign permissions to each user and groups of users.</span><span class="sxs-lookup"><span data-stu-id="056bb-110">Then, the administrator can assign permissions to each user and groups of users.</span></span> <span data-ttu-id="056bb-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="056bb-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span></span>  

<span data-ttu-id="056bb-112">The most powerful permissions that a user can have is the SUPER permission set.</span><span class="sxs-lookup"><span data-stu-id="056bb-112">The most powerful permissions that a user can have is the SUPER permission set.</span></span> <span data-ttu-id="056bb-113">Each company must have at least one user with this permission set, but it is a best practice to give each user permissions that match their work needs in [!INCLUDE[prodshort](includes/prodshort.md)] and not more than that.</span><span class="sxs-lookup"><span data-stu-id="056bb-113">Each company must have at least one user with this permission set, but it is a best practice to give each user permissions that match their work needs in [!INCLUDE[prodshort](includes/prodshort.md)] and not more than that.</span></span> <span data-ttu-id="056bb-114">This helps ensure that users only have access to data that is relevant to their work, for example.</span><span class="sxs-lookup"><span data-stu-id="056bb-114">This helps ensure that users only have access to data that is relevant to their work, for example.</span></span>  

> [!TIP]
> <span data-ttu-id="056bb-115">It's a best practice to make sure that the Office 365 administrator also has the SUPER permission set in [!INCLUDE[prodshort](includes/prodshort.md)] because that makes many administrative tasks easier, including setting up integration with other apps.</span><span class="sxs-lookup"><span data-stu-id="056bb-115">It's a best practice to make sure that the Office 365 administrator also has the SUPER permission set in [!INCLUDE[prodshort](includes/prodshort.md)] because that makes many administrative tasks easier, including setting up integration with other apps.</span></span>

### <a name="users-of-on-premises-deployments"></a><span data-ttu-id="056bb-116">Users of on-premises deployments</span><span class="sxs-lookup"><span data-stu-id="056bb-116">Users of on-premises deployments</span></span>

<span data-ttu-id="056bb-117">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorization mechanisms for users.</span><span class="sxs-lookup"><span data-stu-id="056bb-117">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorization mechanisms for users.</span></span> <span data-ttu-id="056bb-118">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span><span class="sxs-lookup"><span data-stu-id="056bb-118">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span></span> <span data-ttu-id="056bb-119">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="056bb-119">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="profiles"></a><span data-ttu-id="056bb-120">Profiles</span><span class="sxs-lookup"><span data-stu-id="056bb-120">Profiles</span></span>

<span data-ttu-id="056bb-121">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a *profile* that gives them access to a *Role Centre*.</span><span class="sxs-lookup"><span data-stu-id="056bb-121">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a *profile* that gives them access to a *Role Center*.</span></span>

<span data-ttu-id="056bb-122">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same Role Center.</span><span class="sxs-lookup"><span data-stu-id="056bb-122">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same Role Center.</span></span> <span data-ttu-id="056bb-123">A Role Centre is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span><span class="sxs-lookup"><span data-stu-id="056bb-123">A Role Center is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="056bb-124">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span><span class="sxs-lookup"><span data-stu-id="056bb-124">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span></span>  

### <a name="CreateProfile"></a><span data-ttu-id="056bb-125">Create a profile</span><span class="sxs-lookup"><span data-stu-id="056bb-125">Create a profile</span></span>

1.  <span data-ttu-id="056bb-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profile List**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="056bb-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profile List**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="056bb-127">On the **Profile List** page, choose the **New** action to open the **New Profile Card** page.</span><span class="sxs-lookup"><span data-stu-id="056bb-127">On the **Profile List** page, choose the **New** action to open the **New Profile Card** page.</span></span>  

3.  <span data-ttu-id="056bb-128">In the **Profile ID** field, enter a name that describes the intended role of the users.</span><span class="sxs-lookup"><span data-stu-id="056bb-128">In the **Profile ID** field, enter a name that describes the intended role of the users.</span></span>  

4.  <span data-ttu-id="056bb-129">In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.</span><span class="sxs-lookup"><span data-stu-id="056bb-129">In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.</span></span>  

5.  <span data-ttu-id="056bb-130">Set the **Role Centre ID** field to the Role Centre that you want to assign to the profile.</span><span class="sxs-lookup"><span data-stu-id="056bb-130">Set the **Role Center ID** field to the Role Center that you want to assign to the profile.</span></span>  

<span data-ttu-id="056bb-131">The procedure for modifying an existing profile is the same, except you select an existing profile on the **Profile List** page instead of choosing the **New** action.</span><span class="sxs-lookup"><span data-stu-id="056bb-131">The procedure for modifying an existing profile is the same, except you select an existing profile on the **Profile List** page instead of choosing the **New** action.</span></span>  


### <a name="copy-a-profile"></a><span data-ttu-id="056bb-132">Copy a profile</span><span class="sxs-lookup"><span data-stu-id="056bb-132">Copy a profile</span></span>
<span data-ttu-id="056bb-133">Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.</span><span class="sxs-lookup"><span data-stu-id="056bb-133">Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.</span></span>

1.  <span data-ttu-id="056bb-134">Open the profile that you want to copy, and then choose the **Copy Profile** action.</span><span class="sxs-lookup"><span data-stu-id="056bb-134">Open the profile that you want to copy, and then choose the **Copy Profile** action.</span></span>

2.  <span data-ttu-id="056bb-135">In **New Profile ID** field, enter a name for the profile that you want to copy.</span><span class="sxs-lookup"><span data-stu-id="056bb-135">In **New Profile ID** field, enter a name for the profile that you want to copy.</span></span>

3.  <span data-ttu-id="056bb-136">Set the **New Profile Scope** field to one of the following:</span><span class="sxs-lookup"><span data-stu-id="056bb-136">Set the **New Profile Scope** field to one of the following:</span></span>

    - <span data-ttu-id="056bb-137">**System** to make the new profile available to all tenant databases that use the application.</span><span class="sxs-lookup"><span data-stu-id="056bb-137">**System** to make the new profile available to all tenant databases that use the application.</span></span>
    - <span data-ttu-id="056bb-138">**Tenant** to make the new profile available to just the current tenant database.</span><span class="sxs-lookup"><span data-stu-id="056bb-138">**Tenant** to make the new profile available to just the current tenant database.</span></span>
4. <span data-ttu-id="056bb-139">Choose the **OK** button when done.</span><span class="sxs-lookup"><span data-stu-id="056bb-139">Choose the **OK** button when done.</span></span>

### <a name="ExportImportProfile"></a><span data-ttu-id="056bb-140">Export and import profiles</span><span class="sxs-lookup"><span data-stu-id="056bb-140">Export and import profiles</span></span>

<span data-ttu-id="056bb-141">You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database.</span><span class="sxs-lookup"><span data-stu-id="056bb-141">You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database.</span></span> <span data-ttu-id="056bb-142">Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch.</span><span class="sxs-lookup"><span data-stu-id="056bb-142">Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch.</span></span> <span data-ttu-id="056bb-143">If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file.</span><span class="sxs-lookup"><span data-stu-id="056bb-143">If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file.</span></span> <span data-ttu-id="056bb-144">Then, you can import the profile XML file into the other database.</span><span class="sxs-lookup"><span data-stu-id="056bb-144">Then, you can import the profile XML file into the other database.</span></span>

-   <span data-ttu-id="056bb-145">To export a profile, you can either choose the **Export Profiles** action from the **Profile List** or **Profile Card** page or you can search for and open the **Export Profiles** page.</span><span class="sxs-lookup"><span data-stu-id="056bb-145">To export a profile, you can either choose the **Export Profiles** action from the **Profile List** or **Profile Card** page or you can search for and open the **Export Profiles** page.</span></span> <span data-ttu-id="056bb-146">Save the XML file to a location on your computer or network.</span><span class="sxs-lookup"><span data-stu-id="056bb-146">Save the XML file to a location on your computer or network.</span></span>

-   <span data-ttu-id="056bb-147">To import a profile, you can either choose the **Import Profile** action from the **Profile List** page, or you can search for and open the **Import Profiles** page.</span><span class="sxs-lookup"><span data-stu-id="056bb-147">To import a profile, you can either choose the **Import Profile** action from the **Profile List** page, or you can search for and open the **Import Profiles** page.</span></span> 

    > [!NOTE]  
    >  <span data-ttu-id="056bb-148">You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content.</span><span class="sxs-lookup"><span data-stu-id="056bb-148">You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content.</span></span> <span data-ttu-id="056bb-149">You must delete the existing profile before you can import the new profile.</span><span class="sxs-lookup"><span data-stu-id="056bb-149">You must delete the existing profile before you can import the new profile.</span></span>


## <a name="configuration-and-personalization"></a><span data-ttu-id="056bb-150">Configuration and Personalization</span><span class="sxs-lookup"><span data-stu-id="056bb-150">Configuration and Personalization</span></span>
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->

<span data-ttu-id="056bb-151">Users personalize the user interface of their personal version by customizing the user interface under their own user logon.</span><span class="sxs-lookup"><span data-stu-id="056bb-151">Users personalize the user interface of their personal version by customizing the user interface under their own user logon.</span></span> <span data-ttu-id="056bb-152">This personalization can be deleted by the administrator.</span><span class="sxs-lookup"><span data-stu-id="056bb-152">This personalization can be deleted by the administrator.</span></span> <span data-ttu-id="056bb-153">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="056bb-153">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="056bb-154">See Also</span><span class="sxs-lookup"><span data-stu-id="056bb-154">See Also</span></span>  
[<span data-ttu-id="056bb-155">Managing Users and Permissions</span><span class="sxs-lookup"><span data-stu-id="056bb-155">Managing Users and Permissions</span></span>](ui-how-users-permissions.md)  
[<span data-ttu-id="056bb-156">Managing Personalization as an Administrator</span><span class="sxs-lookup"><span data-stu-id="056bb-156">Managing Personalization as an Administrator</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="056bb-157">Personalizing Your Workspace</span><span class="sxs-lookup"><span data-stu-id="056bb-157">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
