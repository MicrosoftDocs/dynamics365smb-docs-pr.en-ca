---
title: Searching Data and Entering Filter Criteria | Microsoft Docs
description: Describes how to work with filters, such as the Quick Filter, to refine the results you get when you search for data.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 11d7ef56e980ba263dba6328b2f2f08b86410242
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="searching-filtering-and-sorting-data"></a><span data-ttu-id="80a88-103">Searching, Filtering, and Sorting Data</span><span class="sxs-lookup"><span data-stu-id="80a88-103">Searching, Filtering, and Sorting Data</span></span>
<span data-ttu-id="80a88-104">There are a few things that you can do that will help you find, pinpoint, and scan records in a list.</span><span class="sxs-lookup"><span data-stu-id="80a88-104">There are a few things that you can do that will help you find, pinpoint, and scan records in a list.</span></span> <span data-ttu-id="80a88-105">These include sorting, searching and filtering.</span><span class="sxs-lookup"><span data-stu-id="80a88-105">These include sorting, searching and filtering.</span></span>

<span data-ttu-id="80a88-106">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span><span class="sxs-lookup"><span data-stu-id="80a88-106">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="80a88-107">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span><span class="sxs-lookup"><span data-stu-id="80a88-107">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="80a88-108">In addition, you can use special symbols to further filter the results.</span><span class="sxs-lookup"><span data-stu-id="80a88-108">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="80a88-109">There are two ways to search: using the Quick Filter or column filters.</span><span class="sxs-lookup"><span data-stu-id="80a88-109">There are two ways to search: using the Quick Filter or column filters.</span></span>

## <a name="sorting"></a><span data-ttu-id="80a88-110">Sorting</span><span class="sxs-lookup"><span data-stu-id="80a88-110">Sorting</span></span>
<span data-ttu-id="80a88-111">Sorting makes it easy for you to get a quick overview of your data.</span><span class="sxs-lookup"><span data-stu-id="80a88-111">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="80a88-112">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span><span class="sxs-lookup"><span data-stu-id="80a88-112">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="80a88-113">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small downs arrow in the column heading, and then choose **Ascending** or **Descending**.</span><span class="sxs-lookup"><span data-stu-id="80a88-113">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small downs arrow in the column heading, and then choose **Ascending** or **Descending**.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="80a88-114">Sorting is not supported images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span><span class="sxs-lookup"><span data-stu-id="80a88-114">Sorting is not supported images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching-by-using-the-quick-filter"></a><span data-ttu-id="80a88-115">Searching by using the Quick Filter</span><span class="sxs-lookup"><span data-stu-id="80a88-115">Searching by using the Quick Filter</span></span>
<span data-ttu-id="80a88-116">You can add filters to all pages by using the Quick Filter.</span><span class="sxs-lookup"><span data-stu-id="80a88-116">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="80a88-117">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span><span class="sxs-lookup"><span data-stu-id="80a88-117">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="80a88-118">This filtering type is used for a fast entry of criteria.</span><span class="sxs-lookup"><span data-stu-id="80a88-118">This filtering type is used for a fast entry of criteria.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="80a88-119">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span><span class="sxs-lookup"><span data-stu-id="80a88-119">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="80a88-120">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span><span class="sxs-lookup"><span data-stu-id="80a88-120">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  

* <span data-ttu-id="80a88-121">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span><span class="sxs-lookup"><span data-stu-id="80a88-121">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
* <span data-ttu-id="80a88-122">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-122">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="80a88-123">Quick filter criteria</span><span class="sxs-lookup"><span data-stu-id="80a88-123">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="80a88-124">Search Criteria</span><span class="sxs-lookup"><span data-stu-id="80a88-124">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="80a88-125">Interpreted as...</span><span class="sxs-lookup"><span data-stu-id="80a88-125">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="80a88-126">Returns...</span><span class="sxs-lookup"><span data-stu-id="80a88-126">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="80a88-127">man</span><span class="sxs-lookup"><span data-stu-id="80a88-127">man</span></span></TD>
    <TD><span data-ttu-id="80a88-128">@&#42;man&#42;</span><span class="sxs-lookup"><span data-stu-id="80a88-128">@&#42;man&#42;</span></span></TD>
    <TD><span data-ttu-id="80a88-129">All records that contain the text <b>man</b> and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-129">All records that contain the text <b>man</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="80a88-130">se</span><span class="sxs-lookup"><span data-stu-id="80a88-130">se</span></span></TD>
    <TD><span data-ttu-id="80a88-131">@&#42;se&#42;</span><span class="sxs-lookup"><span data-stu-id="80a88-131">@&#42;se&#42;</span></span></TD>
    <TD><span data-ttu-id="80a88-132">All records that contain the text <b>se</b> and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-132">All records that contain the text <b>se</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="80a88-133">Man&#42;</span><span class="sxs-lookup"><span data-stu-id="80a88-133">Man&#42;</span></span></TD>
    <TD><span data-ttu-id="80a88-134">Starts with <b>Man</b> and case sensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-134">Starts with <b>Man</b> and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="80a88-135">All records that start with the text <b>Man</b>.</span><span class="sxs-lookup"><span data-stu-id="80a88-135">All records that start with the text <b>Man</b>.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="80a88-136">'man'</span><span class="sxs-lookup"><span data-stu-id="80a88-136">'man'</span></span></TD>
    <TD><span data-ttu-id="80a88-137">An exact text and case sensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-137">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="80a88-138">All records that match <b>man</b> exactly.</span><span class="sxs-lookup"><span data-stu-id="80a88-138">All records that match <b>man</b> exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="80a88-139">@man\*</span><span class="sxs-lookup"><span data-stu-id="80a88-139">@man\*</span></span> </TD>
    <TD><span data-ttu-id="80a88-140">Starts with and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-140">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="80a88-141">All records that start with <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="80a88-141">All records that start with <b>man</b>.</span></span></TD>
  </TR>
    <TR>
    <TD><span data-ttu-id="80a88-142">@&#42;man</span><span class="sxs-lookup"><span data-stu-id="80a88-142">@&#42;man</span></span></TD>
    <TD><span data-ttu-id="80a88-143">Ends with and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-143">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="80a88-144">All records that end with <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="80a88-144">All records that end with <b>man</b>.</span></span></TD>
  </TR>
</TABLE>

> [!NOTE]  
>   <span data-ttu-id="80a88-145">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span><span class="sxs-lookup"><span data-stu-id="80a88-145">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="80a88-146">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span><span class="sxs-lookup"><span data-stu-id="80a88-146">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="80a88-147">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span><span class="sxs-lookup"><span data-stu-id="80a88-147">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span> 

## <a name="searching-by-using-column-filters"></a><span data-ttu-id="80a88-148">Searching by using column Filters</span><span class="sxs-lookup"><span data-stu-id="80a88-148">Searching by using column Filters</span></span>
<span data-ttu-id="80a88-149">You can add a filter on one or more columns in a list.</span><span class="sxs-lookup"><span data-stu-id="80a88-149">You can add a filter on one or more columns in a list.</span></span> <span data-ttu-id="80a88-150">Filtering on columns is more flexible and enhanced than the Quick Filter.</span><span class="sxs-lookup"><span data-stu-id="80a88-150">Filtering on columns is more flexible and enhanced than the Quick Filter.</span></span> 

### <a name="to-add-a-filter-on-a-column"></a><span data-ttu-id="80a88-151">To add a filter on a column</span><span class="sxs-lookup"><span data-stu-id="80a88-151">To add a filter on a column</span></span>
1.  <span data-ttu-id="80a88-152">Before you add a filter, choose ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to change to the list view.</span><span class="sxs-lookup"><span data-stu-id="80a88-152">Before you add a filter, choose ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to change to the list view.</span></span>
2. <span data-ttu-id="80a88-153">Choose the downwards arrow in the column heading, and then choose **Filter**.</span><span class="sxs-lookup"><span data-stu-id="80a88-153">Choose the downwards arrow in the column heading, and then choose **Filter**.</span></span>
3. <span data-ttu-id="80a88-154">Do one of the following:</span><span class="sxs-lookup"><span data-stu-id="80a88-154">Do one of the following:</span></span> 
  -  <span data-ttu-id="80a88-155">Choose *...* next to the box to select a value from a list.</span><span class="sxs-lookup"><span data-stu-id="80a88-155">Choose *...* next to the box to select a value from a list.</span></span>
  -  <span data-ttu-id="80a88-156">Enter filter criteria in the box.</span><span class="sxs-lookup"><span data-stu-id="80a88-156">Enter filter criteria in the box.</span></span> <span data-ttu-id="80a88-157">See the next section for details.</span><span class="sxs-lookup"><span data-stu-id="80a88-157">See the next section for details.</span></span>
4. <span data-ttu-id="80a88-158">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="80a88-158">Choose the **OK** button.</span></span>

## <a name="filter-criteria-and-symbols"></a><span data-ttu-id="80a88-159">Filter criteria and symbols</span><span class="sxs-lookup"><span data-stu-id="80a88-159">Filter criteria and symbols</span></span>
<span data-ttu-id="80a88-160">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span><span class="sxs-lookup"><span data-stu-id="80a88-160">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="80a88-161">In addition, you can use special symbols to further filter the results.</span><span class="sxs-lookup"><span data-stu-id="80a88-161">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="80a88-162">The following tables show the symbols which can be used in filters.</span><span class="sxs-lookup"><span data-stu-id="80a88-162">The following tables show the symbols which can be used in filters.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="80a88-163">There may be instances where field values contain these symbols and you want to filter on them.</span><span class="sxs-lookup"><span data-stu-id="80a88-163">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="80a88-164">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span><span class="sxs-lookup"><span data-stu-id="80a88-164">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="80a88-165">For example, if you want to filter on records that start with the text *S&R*, the filter expression is **'S&R\*'**.</span><span class="sxs-lookup"><span data-stu-id="80a88-165">For example, if you want to filter on records that start with the text *S&R*, the filter expression is **'S&R\*'**.</span></span>  
  
### <a name="-interval"></a><span data-ttu-id="80a88-166">(..) Interval</span><span class="sxs-lookup"><span data-stu-id="80a88-166">(..) Interval</span></span>  
  
|<span data-ttu-id="80a88-167">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-167">Sample Expression</span></span>|<span data-ttu-id="80a88-168">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-168">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-169">1100..2100</span><span class="sxs-lookup"><span data-stu-id="80a88-169">1100..2100</span></span>|<span data-ttu-id="80a88-170">Numbers 1100 through 2100</span><span class="sxs-lookup"><span data-stu-id="80a88-170">Numbers 1100 through 2100</span></span>|  
|<span data-ttu-id="80a88-171">..2500</span><span class="sxs-lookup"><span data-stu-id="80a88-171">..2500</span></span>|<span data-ttu-id="80a88-172">Up to and including 2500</span><span class="sxs-lookup"><span data-stu-id="80a88-172">Up to and including 2500</span></span>|  
|<span data-ttu-id="80a88-173">..12 31 00</span><span class="sxs-lookup"><span data-stu-id="80a88-173">..12 31 00</span></span>|<span data-ttu-id="80a88-174">Dates up to and including 12 31 00</span><span class="sxs-lookup"><span data-stu-id="80a88-174">Dates up to and including 12 31 00</span></span>|  
|<span data-ttu-id="80a88-175">P8..</span><span class="sxs-lookup"><span data-stu-id="80a88-175">P8..</span></span>|<span data-ttu-id="80a88-176">Information for accounting period 8 and thereafter</span><span class="sxs-lookup"><span data-stu-id="80a88-176">Information for accounting period 8 and thereafter</span></span>|  
|<span data-ttu-id="80a88-177">..23</span><span class="sxs-lookup"><span data-stu-id="80a88-177">..23</span></span>|<span data-ttu-id="80a88-178">From the beginning date until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="80a88-178">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|<span data-ttu-id="80a88-179">23..</span><span class="sxs-lookup"><span data-stu-id="80a88-179">23..</span></span>|<span data-ttu-id="80a88-180">From 23-current month-current year 0:00:00 until the end of time</span><span class="sxs-lookup"><span data-stu-id="80a88-180">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|<span data-ttu-id="80a88-181">22..23</span><span class="sxs-lookup"><span data-stu-id="80a88-181">22..23</span></span>|<span data-ttu-id="80a88-182">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="80a88-182">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  
  
### <a name="124-eitheror"></a><span data-ttu-id="80a88-183">(&#124;) Either/or</span><span class="sxs-lookup"><span data-stu-id="80a88-183">(&#124;) Either/or</span></span>  
  
|<span data-ttu-id="80a88-184">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-184">Sample Expression</span></span>|<span data-ttu-id="80a88-185">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-185">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-186">1200&#124;1300</span><span class="sxs-lookup"><span data-stu-id="80a88-186">1200&#124;1300</span></span>|<span data-ttu-id="80a88-187">Numbers with 1200 or 1300</span><span class="sxs-lookup"><span data-stu-id="80a88-187">Numbers with 1200 or 1300</span></span>|  
  
### <a name="-not-equal-to"></a><span data-ttu-id="80a88-188">(<>) Not equal to</span><span class="sxs-lookup"><span data-stu-id="80a88-188">(<>) Not equal to</span></span>  
  
|<span data-ttu-id="80a88-189">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-189">Sample Expression</span></span>|<span data-ttu-id="80a88-190">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-190">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-191"><>0</span><span class="sxs-lookup"><span data-stu-id="80a88-191"><>0</span></span>|<span data-ttu-id="80a88-192">All numbers except 0</span><span class="sxs-lookup"><span data-stu-id="80a88-192">All numbers except 0</span></span><br /><br /> <span data-ttu-id="80a88-193">The SQL Server Option allows you to combine this symbol with a wild card expression.</span><span class="sxs-lookup"><span data-stu-id="80a88-193">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="80a88-194">For example, <>A\* meaning not equal to any text that starts with A.</span><span class="sxs-lookup"><span data-stu-id="80a88-194">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  
  
### <a name="-greater-than"></a><span data-ttu-id="80a88-195">(>) Greater than</span><span class="sxs-lookup"><span data-stu-id="80a88-195">(>) Greater than</span></span>  
  
|<span data-ttu-id="80a88-196">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-196">Sample Expression</span></span>|<span data-ttu-id="80a88-197">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-197">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-198">>1200</span><span class="sxs-lookup"><span data-stu-id="80a88-198">>1200</span></span>|<span data-ttu-id="80a88-199">Numbers greater than 1200</span><span class="sxs-lookup"><span data-stu-id="80a88-199">Numbers greater than 1200</span></span>|  
  
### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="80a88-200">(>=) Greater than or equal to</span><span class="sxs-lookup"><span data-stu-id="80a88-200">(>=) Greater than or equal to</span></span>  
  
|<span data-ttu-id="80a88-201">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-201">Sample Expression</span></span>|<span data-ttu-id="80a88-202">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-202">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-203">>=1200</span><span class="sxs-lookup"><span data-stu-id="80a88-203">>=1200</span></span>|<span data-ttu-id="80a88-204">Numbers greater than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="80a88-204">Numbers greater than or equal to 1200</span></span>|  
  
### <a name="-less-than"></a><span data-ttu-id="80a88-205">(<) Less than</span><span class="sxs-lookup"><span data-stu-id="80a88-205">(<) Less than</span></span>  
  
|<span data-ttu-id="80a88-206">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-206">Sample Expression</span></span>|<span data-ttu-id="80a88-207">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-207">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-208"><1200</span><span class="sxs-lookup"><span data-stu-id="80a88-208"><1200</span></span>|<span data-ttu-id="80a88-209">Numbers less than 1200</span><span class="sxs-lookup"><span data-stu-id="80a88-209">Numbers less than 1200</span></span>|  
  
### <a name="-less-than-or-equal-to"></a><span data-ttu-id="80a88-210">(<=) Less than or equal to</span><span class="sxs-lookup"><span data-stu-id="80a88-210">(<=) Less than or equal to</span></span>  
  
|<span data-ttu-id="80a88-211">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-211">Sample Expression</span></span>|<span data-ttu-id="80a88-212">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-212">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-213"><=1200</span><span class="sxs-lookup"><span data-stu-id="80a88-213"><=1200</span></span>|<span data-ttu-id="80a88-214">Numbers less than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="80a88-214">Numbers less than or equal to 1200</span></span>|  
  
### <a name="-and"></a><span data-ttu-id="80a88-215">(&) And</span><span class="sxs-lookup"><span data-stu-id="80a88-215">(&) And</span></span>  
  
|<span data-ttu-id="80a88-216">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-216">Sample Expression</span></span>|<span data-ttu-id="80a88-217">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-217">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-218">>200&<1200</span><span class="sxs-lookup"><span data-stu-id="80a88-218">>200&<1200</span></span>|<span data-ttu-id="80a88-219">Numbers greater than 200 and less than 1200</span><span class="sxs-lookup"><span data-stu-id="80a88-219">Numbers greater than 200 and less than 1200</span></span>|  
  
### <a name="-an-exact-character-match"></a><span data-ttu-id="80a88-220">('') An exact character match</span><span class="sxs-lookup"><span data-stu-id="80a88-220">('') An exact character match</span></span>  
  
|<span data-ttu-id="80a88-221">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-221">Sample Expression</span></span>|<span data-ttu-id="80a88-222">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-222">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-223">'man'</span><span class="sxs-lookup"><span data-stu-id="80a88-223">'man'</span></span>|<span data-ttu-id="80a88-224">Text that matches man exactly and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-224">Text that matches man exactly and is case sensitive.</span></span>|  
  
### <a name="-case-insensitive"></a><span data-ttu-id="80a88-225">(@) Case insensitive</span><span class="sxs-lookup"><span data-stu-id="80a88-225">(@) Case insensitive</span></span>  
  
|<span data-ttu-id="80a88-226">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-226">Sample Expression</span></span>|<span data-ttu-id="80a88-227">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-227">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-228">@man\*</span><span class="sxs-lookup"><span data-stu-id="80a88-228">@man\*</span></span>|<span data-ttu-id="80a88-229">Text that starts with man and is case insensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-229">Text that starts with man and is case insensitive.</span></span>|  
  
### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="80a88-230">(\*) An indefinite number of unknown characters</span><span class="sxs-lookup"><span data-stu-id="80a88-230">(\*) An indefinite number of unknown characters</span></span>  
  
|<span data-ttu-id="80a88-231">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-231">Sample Expression</span></span>|<span data-ttu-id="80a88-232">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-232">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-233">*Co*</span><span class="sxs-lookup"><span data-stu-id="80a88-233">*Co*</span></span>|<span data-ttu-id="80a88-234">Text that contains "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-234">Text that contains "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="80a88-235">\*Co</span><span class="sxs-lookup"><span data-stu-id="80a88-235">\*Co</span></span>|<span data-ttu-id="80a88-236">Text that ends with "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-236">Text that ends with "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="80a88-237">Co\*</span><span class="sxs-lookup"><span data-stu-id="80a88-237">Co\*</span></span>|<span data-ttu-id="80a88-238">Text that begins with "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="80a88-238">Text that begins with "Co" and is case sensitive.</span></span>|  
  
### <a name="-one-unknown-character"></a><span data-ttu-id="80a88-239">(?) One unknown character</span><span class="sxs-lookup"><span data-stu-id="80a88-239">(?) One unknown character</span></span>  
  
|<span data-ttu-id="80a88-240">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-240">Sample Expression</span></span>|<span data-ttu-id="80a88-241">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-241">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-242">Hans?n</span><span class="sxs-lookup"><span data-stu-id="80a88-242">Hans?n</span></span>|<span data-ttu-id="80a88-243">Text such as Hansen or Hanson</span><span class="sxs-lookup"><span data-stu-id="80a88-243">Text such as Hansen or Hanson</span></span>|  
  
### <a name="combined-format-expressions"></a><span data-ttu-id="80a88-244">Combined format expressions</span><span class="sxs-lookup"><span data-stu-id="80a88-244">Combined format expressions</span></span>  
  
|<span data-ttu-id="80a88-245">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="80a88-245">Sample Expression</span></span>|<span data-ttu-id="80a88-246">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="80a88-246">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="80a88-247">5999&#124;8100..8490</span><span class="sxs-lookup"><span data-stu-id="80a88-247">5999&#124;8100..8490</span></span>|<span data-ttu-id="80a88-248">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span><span class="sxs-lookup"><span data-stu-id="80a88-248">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|<span data-ttu-id="80a88-249">..1299&#124;1400..</span><span class="sxs-lookup"><span data-stu-id="80a88-249">..1299&#124;1400..</span></span>|<span data-ttu-id="80a88-250">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span><span class="sxs-lookup"><span data-stu-id="80a88-250">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|<span data-ttu-id="80a88-251">>50&<100</span><span class="sxs-lookup"><span data-stu-id="80a88-251">>50&<100</span></span>|<span data-ttu-id="80a88-252">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span><span class="sxs-lookup"><span data-stu-id="80a88-252">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  
 
## <a name="see-also"></a><span data-ttu-id="80a88-253">See Also</span><span class="sxs-lookup"><span data-stu-id="80a88-253">See Also</span></span>
<span data-ttu-id="80a88-254">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="80a88-254">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
