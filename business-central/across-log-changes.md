---
title: Auditing changes| Microsoft Docs
description: You can activate a user log so that you have a history of any changes made to data in tracked tables. You can also track activities with certain types of activity logs.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: cb091a54b7b8da571117c807a621ed298842444c
ms.sourcegitcommit: d0dc5e5c46b932899e2a9c7183959d0ff37738d6
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 02/20/2020
ms.locfileid: "3076668"
---
# <a name="auditing-changes-in-business-central"></a><span data-ttu-id="a307d-104">Auditing Changes in Business Central</span><span class="sxs-lookup"><span data-stu-id="a307d-104">Auditing Changes in Business Central</span></span>

<span data-ttu-id="a307d-105">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span><span class="sxs-lookup"><span data-stu-id="a307d-105">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="a307d-106">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span><span class="sxs-lookup"><span data-stu-id="a307d-106">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="a307d-107">The change log collects all changes that are made to the table.</span><span class="sxs-lookup"><span data-stu-id="a307d-107">The change log collects all changes that are made to the table.</span></span>

> [!Important]
> <span data-ttu-id="a307d-108">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span><span class="sxs-lookup"><span data-stu-id="a307d-108">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span></span>
<br />
> * <span data-ttu-id="a307d-109">The session expired and was refreshed.</span><span class="sxs-lookup"><span data-stu-id="a307d-109">The session expired and was refreshed.</span></span>
> * <span data-ttu-id="a307d-110">The user selected another company or Role Centre.</span><span class="sxs-lookup"><span data-stu-id="a307d-110">The user selected another company or Role Center.</span></span>
> * <span data-ttu-id="a307d-111">The user signed out and back in.</span><span class="sxs-lookup"><span data-stu-id="a307d-111">The user signed out and back in.</span></span>

## <a name="working-with-the-change-log"></a><span data-ttu-id="a307d-112">Working with the Change Log</span><span class="sxs-lookup"><span data-stu-id="a307d-112">Working with the Change Log</span></span>

<span data-ttu-id="a307d-113">A common problem in many financial systems is to locate the origin of errors and changes in data.</span><span class="sxs-lookup"><span data-stu-id="a307d-113">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="a307d-114">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="a307d-114">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="a307d-115">The change log lets you track all direct modifications a user makes to data in the database.</span><span class="sxs-lookup"><span data-stu-id="a307d-115">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="a307d-116">You must specify each table and field that you want the system to log, and then you must activate the change log.</span><span class="sxs-lookup"><span data-stu-id="a307d-116">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="a307d-117">You activate and deactivate the change log on the **Change Log Setup** page.</span><span class="sxs-lookup"><span data-stu-id="a307d-117">You activate and deactivate the change log on the **Change Log Setup** page.</span></span> <span data-ttu-id="a307d-118">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span><span class="sxs-lookup"><span data-stu-id="a307d-118">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span>

<span data-ttu-id="a307d-119">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span><span class="sxs-lookup"><span data-stu-id="a307d-119">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="a307d-120">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span><span class="sxs-lookup"><span data-stu-id="a307d-120">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span></span> <span data-ttu-id="a307d-121">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span><span class="sxs-lookup"><span data-stu-id="a307d-121">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span></span>  

## <a name="working-with-activity-logs"></a><span data-ttu-id="a307d-122">Working with Activity Logs</span><span class="sxs-lookup"><span data-stu-id="a307d-122">Working with Activity Logs</span></span>

<span data-ttu-id="a307d-123">From some pages in [!INCLUDE [prodshort](includes/prodshort.md)], you can view an activity log that shows the status and any errors from files that you export from or import into [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="a307d-123">From some pages in [!INCLUDE [prodshort](includes/prodshort.md)], you can view an activity log that shows the status and any errors from files that you export from or import into [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>  

<span data-ttu-id="a307d-124">The information is displayed in the **Activity Log** page, according to the context that it is opened from.</span><span class="sxs-lookup"><span data-stu-id="a307d-124">The information is displayed in the **Activity Log** page, according to the context that it is opened from.</span></span> <span data-ttu-id="a307d-125">You can open the window from the **Document Exchange Service Setup**, **Incoming Document**, **Posted Sales Invoice**, and **Posted Sales Credit Memo** pages, for example.</span><span class="sxs-lookup"><span data-stu-id="a307d-125">You can open the window from the **Document Exchange Service Setup**, **Incoming Document**, **Posted Sales Invoice**, and **Posted Sales Credit Memo** pages, for example.</span></span> <span data-ttu-id="a307d-126">You can empty the list of log entries, or just clear the list of entries older than 7 days.</span><span class="sxs-lookup"><span data-stu-id="a307d-126">You can empty the list of log entries, or just clear the list of entries older than 7 days.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a307d-127">See Also</span><span class="sxs-lookup"><span data-stu-id="a307d-127">See Also</span></span>
[<span data-ttu-id="a307d-128">Change Basic Settings</span><span class="sxs-lookup"><span data-stu-id="a307d-128">Change Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="a307d-129">Sorting, Searching, and Filtering</span><span class="sxs-lookup"><span data-stu-id="a307d-129">Sorting, Searching, and Filtering</span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="a307d-130">Finding Pages and Information with Tell Me</span><span class="sxs-lookup"><span data-stu-id="a307d-130">Finding Pages and Information with Tell Me</span></span>](ui-search.md)  
<span data-ttu-id="a307d-131">[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="a307d-131">[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  </span></span>  
<span data-ttu-id="a307d-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a307d-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
