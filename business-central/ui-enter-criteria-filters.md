---
title: Sorting, Searching, and Filtering Lists | Microsoft Docs
description: Work efficiently in lists by searching across your data, sorting columns, and refining results using powerful filter symbols and keyboard shortcuts.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter, totals, limit, advanced
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: f0cdb045d314a630e795ec744f2f4470d930835a
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="sorting-searching-and-filtering-lists"></a><span data-ttu-id="7cfa1-103">Sorting, Searching, and Filtering Lists</span><span class="sxs-lookup"><span data-stu-id="7cfa1-103">Sorting, Searching, and Filtering Lists</span></span>
<span data-ttu-id="7cfa1-104">There are a few things that you can do that will help you scan, find, and limit records in a list.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-104">There are a few things that you can do that will help you scan, find, and limit records in a list.</span></span> <span data-ttu-id="7cfa1-105">These include sorting, searching and filtering.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-105">These include sorting, searching and filtering.</span></span> <span data-ttu-id="7cfa1-106">You can apply some or all of these simultaneously to quickly find or analyse your data.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-106">You can apply some or all of these simultaneously to quickly find or analyze your data.</span></span>

> [!TIP]
> <span data-ttu-id="7cfa1-107">When viewing your data as tiles, you can search and use basic filtering.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-107">When viewing your data as tiles, you can search and use basic filtering.</span></span> <span data-ttu-id="7cfa1-108">To use the full set of powerful features for sorting, searching and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to show as a list.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-108">To use the full set of powerful features for sorting, searching and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to show as a list.</span></span>

<!--
When you want to search for data, such as customer names, addresses, or product groups, you enter criteria. In search criteria you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.
-->

## <a name="sorting"></a><span data-ttu-id="7cfa1-109">Sorting</span><span class="sxs-lookup"><span data-stu-id="7cfa1-109">Sorting</span></span>
<span data-ttu-id="7cfa1-110">Sorting makes it easy for you to get a quick overview of your data.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-110">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="7cfa1-111">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **VAT Registration No.** to get the overview you need.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-111">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="7cfa1-112">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small down arrow in the column heading, and then choose **Ascending** or **Descending**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-112">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small down arrow in the column heading, and then choose **Ascending** or **Descending**.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="7cfa1-113">Sorting is not supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-113">Sorting is not supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching"></a><span data-ttu-id="7cfa1-114">Searching</span><span class="sxs-lookup"><span data-stu-id="7cfa1-114">Searching</span></span>
<span data-ttu-id="7cfa1-115"><!--## Searching by using the Quick Filter --> At the top of each list page, there is a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** icon that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you are interested in seeing.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-115"><!--## Searching by using the Quick Filter --> At the top of each list page, there is a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** icon that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you are interested in seeing.</span></span>

<span data-ttu-id="7cfa1-116">To search, simply select the search icon, and then in the box, type the text that you are looking for.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-116">To search, simply select the search icon, and then in the box, type the text that you are looking for.</span></span> <span data-ttu-id="7cfa1-117">You can enter letters, numbers, and other symbols.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-117">You can enter letters, numbers, and other symbols.</span></span>

### <a name="fine-tune-the-search"></a><span data-ttu-id="7cfa1-118">Fine-tune the search</span><span class="sxs-lookup"><span data-stu-id="7cfa1-118">Fine-tune the search</span></span>
<span data-ttu-id="7cfa1-119">In general, search will attempt to match text across all fields; it does not distinguish between uppercase and lowercase characters (in other words, case insensitive), and will match text placed anwhere in the field (at the beginning, end, or in the middle).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-119">In general, search will attempt to match text across all fields; it does not distinguish between uppercase and lowercase characters (in other words, case insensitive), and will match text placed anwhere in the field (at the beginning, end, or in the middle).</span></span>

<span data-ttu-id="7cfa1-120">However, you can make a more exact search by using the following special characters:</span><span class="sxs-lookup"><span data-stu-id="7cfa1-120">However, you can make a more exact search by using the following special characters:</span></span>

- <span data-ttu-id="7cfa1-121">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-121">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span></span>

- <span data-ttu-id="7cfa1-122">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-122">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span></span>

- <span data-ttu-id="7cfa1-123">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-123">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span></span>

- <span data-ttu-id="7cfa1-124">When using  `''` or `*`, the search is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-124">When using  `''` or `*`, the search is case sensitive.</span></span> <span data-ttu-id="7cfa1-125">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-125">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span></span>

<span data-ttu-id="7cfa1-126">The following table provides some examples to explain how you can use the search.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-126">The following table provides some examples to explain how you can use the search.</span></span>


<!--
In search criteria you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.-->

<!--
The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options. Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.  

* If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.  
* If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.
-->
<!--

|Search Criteria|Interpreted as...|Finds...|
|---------------|----------------|----------|
|`man`<br />or <br />`Man`|Contains the text; case insensitive|All records with fields that contain the text **man**, regardless of the case.|
|`'Man'`|Entire text match; case sensitive.|All records with fields that only contain **Man** exactly.|
|`Man*`|Starts with the text; case sensitive.|All records with fields that start with the text <b>Man</b> exactly.|
|`@Man*`|Starts with the text; case insensitive.|All records with fields that start with **man**, regardless of the case.|
|`@*man`|Ends with the text; case insensitive.|All records that end with **man**, regardless of the case.|
-->

|<span data-ttu-id="7cfa1-127">Search Criteria</span><span class="sxs-lookup"><span data-stu-id="7cfa1-127">Search Criteria</span></span>|<span data-ttu-id="7cfa1-128">Finds...</span><span class="sxs-lookup"><span data-stu-id="7cfa1-128">Finds...</span></span>|
|---------------|----------|
|`man`<br /><span data-ttu-id="7cfa1-129">or</span><span class="sxs-lookup"><span data-stu-id="7cfa1-129">or</span></span> <br />`Man`|<span data-ttu-id="7cfa1-130">All records with fields that contain the text **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-130">All records with fields that contain the text **man**, regardless of the case.</span></span> <span data-ttu-id="7cfa1-131">For example, **Manchester**, **manual**, or **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-131">For example, **Manchester**, **manual**, or **Sportsman**.</span></span> |
|`'Man'`|<span data-ttu-id="7cfa1-132">All records with fields that contain only **Man**, matching the case.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-132">All records with fields that contain only **Man**, matching the case.</span></span>|
|`Man*`|<span data-ttu-id="7cfa1-133">All records with fields that start with the text <b>Man</b>, matching the case.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-133">All records with fields that start with the text <b>Man</b>, matching the case.</span></span> <span data-ttu-id="7cfa1-134">For example, **Manchester** but not **manual** or **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-134">For example, **Manchester** but not **manual** or **Sportsman**.</span></span>|
|`@Man*`|<span data-ttu-id="7cfa1-135">All records with fields that start with **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-135">All records with fields that start with **man**, regardless of the case.</span></span> <span data-ttu-id="7cfa1-136">For example, **Manchester** and **manual**, but not **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-136">For example, **Manchester** and **manual**, but not **Sportsman**.</span></span>|
|`@*man`|<span data-ttu-id="7cfa1-137">All records that end with **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-137">All records that end with **man**, regardless of the case.</span></span> <span data-ttu-id="7cfa1-138">For example **Sportsman**, but not **Manchester** or **manual**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-138">For example **Sportsman**, but not **Manchester** or **manual**.</span></span>|

> [!TIP]
> <span data-ttu-id="7cfa1-139">You can press F3 to activate and deactivate the search box.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-139">You can press F3 to activate and deactivate the search box.</span></span> <span data-ttu-id="7cfa1-140">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-140">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

## <a name="filtering"></a><span data-ttu-id="7cfa1-141">Filtering</span><span class="sxs-lookup"><span data-stu-id="7cfa1-141">Filtering</span></span>
<span data-ttu-id="7cfa1-142">Filtering provides a more advanced and versatile way of controlling which records display in a list.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-142">Filtering provides a more advanced and versatile way of controlling which records display in a list.</span></span> <span data-ttu-id="7cfa1-143">There are two major differences between searching and filtering, as described in the table below.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-143">There are two major differences between searching and filtering, as described in the table below.</span></span>

|| <span data-ttu-id="7cfa1-144">**Searching**</span><span class="sxs-lookup"><span data-stu-id="7cfa1-144">**Searching**</span></span> | <span data-ttu-id="7cfa1-145">**Filtering**</span><span class="sxs-lookup"><span data-stu-id="7cfa1-145">**Filtering**</span></span> |
|--|----------|------------|
| <span data-ttu-id="7cfa1-146">**Applicable fields**</span><span class="sxs-lookup"><span data-stu-id="7cfa1-146">**Applicable fields**</span></span> | <span data-ttu-id="7cfa1-147">Searches across all fields that are visible on the page.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-147">Searches across all fields that are visible on the page.</span></span> | <span data-ttu-id="7cfa1-148">Filters one or more fields individually, selecting from any field on the table, including fields that are not visible on the page.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-148">Filters one or more fields individually, selecting from any field on the table, including fields that are not visible on the page.</span></span> |
| <span data-ttu-id="7cfa1-149">**Matching**</span><span class="sxs-lookup"><span data-stu-id="7cfa1-149">**Matching**</span></span> | <span data-ttu-id="7cfa1-150">Displays records with fields that match the search text, irrespective of casing or placement of that text.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-150">Displays records with fields that match the search text, irrespective of casing or placement of that text.</span></span> | <span data-ttu-id="7cfa1-151">Displays records where the field matches the filter exactly and is case sensitive, unless special filter symbols are entered.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-151">Displays records where the field matches the filter exactly and is case sensitive, unless special filter symbols are entered.</span></span>

<span data-ttu-id="7cfa1-152">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-152">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span></span> <span data-ttu-id="7cfa1-153">Only records that match the criteria are displayed.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-153">Only records that match the criteria are displayed.</span></span> <span data-ttu-id="7cfa1-154">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-154">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span></span>

### <a name="working-in-the-filter-pane"></a><span data-ttu-id="7cfa1-155">Working in the filter pane</span><span class="sxs-lookup"><span data-stu-id="7cfa1-155">Working in the filter pane</span></span>
<span data-ttu-id="7cfa1-156">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-156">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields.</span></span> <span data-ttu-id="7cfa1-157">The following figure shows an example filter pane for a Sales Quotes list.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-157">The following figure shows an example filter pane for a Sales Quotes list.</span></span>

<span data-ttu-id="7cfa1-158">![Filter pane overview ](media/filter-pane-overview.png "Filter icon")</span><span class="sxs-lookup"><span data-stu-id="7cfa1-158">![Filter pane overview ](media/filter-pane-overview.png "Filter icon")</span></span>

<span data-ttu-id="7cfa1-159">To display the filter pane, use the **Shift+F3** keyboard shortcut.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-159">To display the filter pane, use the **Shift+F3** keyboard shortcut.</span></span> <span data-ttu-id="7cfa1-160">For lists within the Role Centre, you can also choose the down arrow near the page title in the navigation bar above the list, and then choose **Show filter pane**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-160">For lists within the Role Center, you can also choose the down arrow near the page title in the navigation bar above the list, and then choose **Show filter pane**.</span></span>

<span data-ttu-id="7cfa1-161">![Show filter pane](media/open-filter-pane.png "Show filter pane")</span><span class="sxs-lookup"><span data-stu-id="7cfa1-161">![Show filter pane](media/open-filter-pane.png "Show filter pane")</span></span>

<span data-ttu-id="7cfa1-162">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span><span class="sxs-lookup"><span data-stu-id="7cfa1-162">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span></span>

- <span data-ttu-id="7cfa1-163">**Views**</span><span class="sxs-lookup"><span data-stu-id="7cfa1-163">**Views**</span></span>

  <span data-ttu-id="7cfa1-164">Some lists will include the **Views** section.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-164">Some lists will include the **Views** section.</span></span> <span data-ttu-id="7cfa1-165">Views are variations of the list that have been preconfigured with filters.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-165">Views are variations of the list that have been preconfigured with filters.</span></span> <span data-ttu-id="7cfa1-166">To switch to a different view of your list, simply select another link.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-166">To switch to a different view of your list, simply select another link.</span></span> <span data-ttu-id="7cfa1-167">You can temporarily change the filters on a view, but the changes will not be permanently saved.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-167">You can temporarily change the filters on a view, but the changes will not be permanently saved.</span></span>

- <span data-ttu-id="7cfa1-168">**Filter list by**</span><span class="sxs-lookup"><span data-stu-id="7cfa1-168">**Filter list by**</span></span>

  <span data-ttu-id="7cfa1-169">The **Filter list by** section is where you add filters on specific fields to reduce the number of displayed records.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-169">The **Filter list by** section is where you add filters on specific fields to reduce the number of displayed records.</span></span> <span data-ttu-id="7cfa1-170">To add a filter, select **+ Filter**, select the field that you want to filter from any field in the table, and then enter filter criteria in the box.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-170">To add a filter, select **+ Filter**, select the field that you want to filter from any field in the table, and then enter filter criteria in the box.</span></span>

- <span data-ttu-id="7cfa1-171">**Filter totals by**</span><span class="sxs-lookup"><span data-stu-id="7cfa1-171">**Filter totals by**</span></span>

  <span data-ttu-id="7cfa1-172">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-172">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span></span> <span data-ttu-id="7cfa1-173">For example, you can quickly analyse your chart of accounts by filtering amounts to a specific period, or you can view the totals for sales orders only from a specific warehouse.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-173">For example, you can quickly analyze your chart of accounts by filtering amounts to a specific period, or you can view the totals for sales orders only from a specific warehouse.</span></span>

  <span data-ttu-id="7cfa1-174">To add a filter, select **+ Filter**, select one of the predefined dimensions, and then add the filter criteria in the box.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-174">To add a filter, select **+ Filter**, select one of the predefined dimensions, and then add the filter criteria in the box.</span></span>

  > [!NOTE]
  > <span data-ttu-id="7cfa1-175">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-175">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span></span> <span data-ttu-id="7cfa1-176">For technical information, see [FlowFilters](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-176">For technical information, see [FlowFilters](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span></span>


### <a name="entering-filter-criteria-in-the-filter-pane"></a><span data-ttu-id="7cfa1-177">Entering filter criteria in the filter pane</span><span class="sxs-lookup"><span data-stu-id="7cfa1-177">Entering filter criteria in the filter pane</span></span>
<span data-ttu-id="7cfa1-178">To select a field to filter, do one of the following:</span><span class="sxs-lookup"><span data-stu-id="7cfa1-178">To select a field to filter, do one of the following:</span></span>
  - <span data-ttu-id="7cfa1-179">In the filter pane, choose **+ Field**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-179">In the filter pane, choose **+ Field**.</span></span> <span data-ttu-id="7cfa1-180">Type the name of the field you wish to filter, or pick a field from the menu that displays all fields in the table.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-180">Type the name of the field you wish to filter, or pick a field from the menu that displays all fields in the table.</span></span>

  - <span data-ttu-id="7cfa1-181">In a column heading, choose the down arrow, and then choose **Filter...**. This will open the filter pane and add the column to the filter pane.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-181">In a column heading, choose the down arrow, and then choose **Filter...**. This will open the filter pane and add the column to the filter pane.</span></span>

<span data-ttu-id="7cfa1-182">You can now type or select your filter criteria in the box.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-182">You can now type or select your filter criteria in the box.</span></span> <span data-ttu-id="7cfa1-183">The type of field you filter determines which criteria you can enter.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-183">The type of field you filter determines which criteria you can enter.</span></span> <span data-ttu-id="7cfa1-184">For example, filtering a field that has fixed values will only let you choose from those values.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-184">For example, filtering a field that has fixed values will only let you choose from those values.</span></span> <span data-ttu-id="7cfa1-185">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-185">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span></span>

<span data-ttu-id="7cfa1-186">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") in the column heading.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-186">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") in the column heading.</span></span> <span data-ttu-id="7cfa1-187">To remove a filter, select the column heading, then choose **Clear Filter**.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-187">To remove a filter, select the column heading, then choose **Clear Filter**.</span></span>


### <a name="entering-filter-criteria-without-the-filter-pane"></a><span data-ttu-id="7cfa1-188">Entering filter criteria without the filter pane</span><span class="sxs-lookup"><span data-stu-id="7cfa1-188">Entering filter criteria without the filter pane</span></span>
<span data-ttu-id="7cfa1-189">You can specify simple filters directly within the list without having to use the filter pane.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-189">You can specify simple filters directly within the list without having to use the filter pane.</span></span>
<span data-ttu-id="7cfa1-190">With any field selected on a row, use the **Alt+F3** keyboard shortcut to display only the records having that same value.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-190">With any field selected on a row, use the **Alt+F3** keyboard shortcut to display only the records having that same value.</span></span> <span data-ttu-id="7cfa1-191">You can then select another field and use the same shortcut again to continue refining your filters.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-191">You can then select another field and use the same shortcut again to continue refining your filters.</span></span> <span data-ttu-id="7cfa1-192">If the selected field is already filtered, using **Alt+F3** will clear that filter.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-192">If the selected field is already filtered, using **Alt+F3** will clear that filter.</span></span>

> [!TIP]
> <span data-ttu-id="7cfa1-193">Accelerate finding and analysing your data by using combinations of keyboard shortcuts.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-193">Accelerate finding and analyzing your data by using combinations of keyboard shortcuts.</span></span> <span data-ttu-id="7cfa1-194">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-194">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span></span>
<span data-ttu-id="7cfa1-195">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-195">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>


## <span data-ttu-id="7cfa1-196"><a name="FilterCriteria"> </a>Filter criteria and symbols</span><span class="sxs-lookup"><span data-stu-id="7cfa1-196"><a name="FilterCriteria"> </a>Filter criteria and symbols</span></span>
<span data-ttu-id="7cfa1-197">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-197">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="7cfa1-198">In addition, you can use special symbols to further filter the results.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-198">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="7cfa1-199">The following tables show the symbols which can be used in filters.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-199">The following tables show the symbols which can be used in filters.</span></span> <span data-ttu-id="7cfa1-200">For dates and times, you can also refer to [Working with Calendar Dates and Times](ui-enter-date-ranges.md) for more detailed information.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-200">For dates and times, you can also refer to [Working with Calendar Dates and Times](ui-enter-date-ranges.md) for more detailed information.</span></span>

> [!IMPORTANT]  
>  <span data-ttu-id="7cfa1-201">There may be instances where field values contain these symbols and you want to filter on them.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-201">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="7cfa1-202">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span><span class="sxs-lookup"><span data-stu-id="7cfa1-202">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="7cfa1-203">For example, if you want to filter on records that start with the text *S&R*, the filter expression is `'S&R*'`.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-203">For example, if you want to filter on records that start with the text *S&R*, the filter expression is `'S&R*'`.</span></span>  

### <a name="-interval"></a><span data-ttu-id="7cfa1-204">(..) Interval</span><span class="sxs-lookup"><span data-stu-id="7cfa1-204">(..) Interval</span></span>

|<span data-ttu-id="7cfa1-205">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-205">Sample Expression</span></span>|<span data-ttu-id="7cfa1-206">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-206">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1100..2100`|<span data-ttu-id="7cfa1-207">Numbers 1100 through 2100</span><span class="sxs-lookup"><span data-stu-id="7cfa1-207">Numbers 1100 through 2100</span></span>|  
|`..2500`|<span data-ttu-id="7cfa1-208">Up to and including 2500</span><span class="sxs-lookup"><span data-stu-id="7cfa1-208">Up to and including 2500</span></span>|  
|`..12 31 00`|<span data-ttu-id="7cfa1-209">Dates up to and including 12 31 00</span><span class="sxs-lookup"><span data-stu-id="7cfa1-209">Dates up to and including 12 31 00</span></span>|  
|`P8..`|<span data-ttu-id="7cfa1-210">Information for accounting period 8 and thereafter</span><span class="sxs-lookup"><span data-stu-id="7cfa1-210">Information for accounting period 8 and thereafter</span></span>|  
|`..23`|<span data-ttu-id="7cfa1-211">From the beginning date until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="7cfa1-211">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|`23..`|<span data-ttu-id="7cfa1-212">From 23-current month-current year 0:00:00 until the end of time</span><span class="sxs-lookup"><span data-stu-id="7cfa1-212">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|`22..23`|<span data-ttu-id="7cfa1-213">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="7cfa1-213">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  

### <a name="124-eitheror"></a><span data-ttu-id="7cfa1-214">(&#124;) Either/or</span><span class="sxs-lookup"><span data-stu-id="7cfa1-214">(&#124;) Either/or</span></span>  

|<span data-ttu-id="7cfa1-215">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-215">Sample Expression</span></span>|<span data-ttu-id="7cfa1-216">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-216">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="7cfa1-217">\`1200</span><span class="sxs-lookup"><span data-stu-id="7cfa1-217">\`1200</span></span>|<span data-ttu-id="7cfa1-218">1300\`</span><span class="sxs-lookup"><span data-stu-id="7cfa1-218">1300\`</span></span>|<span data-ttu-id="7cfa1-219">Numbers with 1200 or 1300</span><span class="sxs-lookup"><span data-stu-id="7cfa1-219">Numbers with 1200 or 1300</span></span>|  

### <a name="-not-equal-to"></a><span data-ttu-id="7cfa1-220">(<>) Not equal to</span><span class="sxs-lookup"><span data-stu-id="7cfa1-220">(<>) Not equal to</span></span>  

|<span data-ttu-id="7cfa1-221">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-221">Sample Expression</span></span>|<span data-ttu-id="7cfa1-222">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-222">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<>0`|<span data-ttu-id="7cfa1-223">All numbers except 0</span><span class="sxs-lookup"><span data-stu-id="7cfa1-223">All numbers except 0</span></span><br /><br /> <span data-ttu-id="7cfa1-224">The SQL Server Option allows you to combine this symbol with a wild card expression.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-224">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="7cfa1-225">For example, <>A\* meaning not equal to any text that starts with A.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-225">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  

### <a name="-greater-than"></a><span data-ttu-id="7cfa1-226">(>) Greater than</span><span class="sxs-lookup"><span data-stu-id="7cfa1-226">(>) Greater than</span></span>  

|<span data-ttu-id="7cfa1-227">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-227">Sample Expression</span></span>|<span data-ttu-id="7cfa1-228">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-228">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>1200`|<span data-ttu-id="7cfa1-229">Numbers greater than 1200</span><span class="sxs-lookup"><span data-stu-id="7cfa1-229">Numbers greater than 1200</span></span>|  

### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="7cfa1-230">(>=) Greater than or equal to</span><span class="sxs-lookup"><span data-stu-id="7cfa1-230">(>=) Greater than or equal to</span></span>  

|<span data-ttu-id="7cfa1-231">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-231">Sample Expression</span></span>|<span data-ttu-id="7cfa1-232">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-232">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>=1200`|<span data-ttu-id="7cfa1-233">Numbers greater than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="7cfa1-233">Numbers greater than or equal to 1200</span></span>|  

### <a name="-less-than"></a><span data-ttu-id="7cfa1-234">(<) Less than</span><span class="sxs-lookup"><span data-stu-id="7cfa1-234">(<) Less than</span></span>  

|<span data-ttu-id="7cfa1-235">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-235">Sample Expression</span></span>|<span data-ttu-id="7cfa1-236">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-236">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<1200`|<span data-ttu-id="7cfa1-237">Numbers less than 1200</span><span class="sxs-lookup"><span data-stu-id="7cfa1-237">Numbers less than 1200</span></span>|  

### <a name="-less-than-or-equal-to"></a><span data-ttu-id="7cfa1-238">(<=) Less than or equal to</span><span class="sxs-lookup"><span data-stu-id="7cfa1-238">(<=) Less than or equal to</span></span>  

|<span data-ttu-id="7cfa1-239">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-239">Sample Expression</span></span>|<span data-ttu-id="7cfa1-240">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-240">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<=1200`|<span data-ttu-id="7cfa1-241">Numbers less than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="7cfa1-241">Numbers less than or equal to 1200</span></span>|  

### <a name="-and"></a><span data-ttu-id="7cfa1-242">(&) And</span><span class="sxs-lookup"><span data-stu-id="7cfa1-242">(&) And</span></span>  

|<span data-ttu-id="7cfa1-243">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-243">Sample Expression</span></span>|<span data-ttu-id="7cfa1-244">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-244">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>200&<1200`|<span data-ttu-id="7cfa1-245">Numbers greater than 200 and less than 1200</span><span class="sxs-lookup"><span data-stu-id="7cfa1-245">Numbers greater than 200 and less than 1200</span></span>|  

### <a name="-an-exact-character-match"></a><span data-ttu-id="7cfa1-246">('') An exact character match</span><span class="sxs-lookup"><span data-stu-id="7cfa1-246">('') An exact character match</span></span>  

|<span data-ttu-id="7cfa1-247">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-247">Sample Expression</span></span>|<span data-ttu-id="7cfa1-248">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-248">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`'man'`|<span data-ttu-id="7cfa1-249">Text that matches man exactly and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-249">Text that matches man exactly and is case sensitive.</span></span>|  

### <a name="-case-insensitive"></a><span data-ttu-id="7cfa1-250">(@) Case insensitive</span><span class="sxs-lookup"><span data-stu-id="7cfa1-250">(@) Case insensitive</span></span>  

|<span data-ttu-id="7cfa1-251">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-251">Sample Expression</span></span>|<span data-ttu-id="7cfa1-252">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-252">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`@man*`|<span data-ttu-id="7cfa1-253">Text that starts with man and is case insensitive.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-253">Text that starts with man and is case insensitive.</span></span>|  

### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="7cfa1-254">(\*) An indefinite number of unknown characters</span><span class="sxs-lookup"><span data-stu-id="7cfa1-254">(\*) An indefinite number of unknown characters</span></span>

|<span data-ttu-id="7cfa1-255">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-255">Sample Expression</span></span>|<span data-ttu-id="7cfa1-256">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-256">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`*Co*`|<span data-ttu-id="7cfa1-257">Text that contains "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-257">Text that contains "Co" and is case sensitive.</span></span>|  
|`*Co`|<span data-ttu-id="7cfa1-258">Text that ends with "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-258">Text that ends with "Co" and is case sensitive.</span></span>|  
|`Co*`|<span data-ttu-id="7cfa1-259">Text that begins with "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-259">Text that begins with "Co" and is case sensitive.</span></span>|  

> [!NOTE]  
>   <span data-ttu-id="7cfa1-260">You cannot use `*` when filtering on option (enumeration) fields, such as the **Status** field on sales orders.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-260">You cannot use `*` when filtering on option (enumeration) fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="7cfa1-261">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-261">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="7cfa1-262">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values `0`, `1`, `2`, and `3` to filter for these options.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-262">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values `0`, `1`, `2`, and `3` to filter for these options.</span></span>

### <a name="-one-unknown-character"></a><span data-ttu-id="7cfa1-263">(?) One unknown character</span><span class="sxs-lookup"><span data-stu-id="7cfa1-263">(?) One unknown character</span></span>  

|<span data-ttu-id="7cfa1-264">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-264">Sample Expression</span></span>|<span data-ttu-id="7cfa1-265">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-265">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`Hans?n`|<span data-ttu-id="7cfa1-266">Text such as Hansen or Hanson</span><span class="sxs-lookup"><span data-stu-id="7cfa1-266">Text such as Hansen or Hanson</span></span>|  

### <a name="combined-format-expressions"></a><span data-ttu-id="7cfa1-267">Combined format expressions</span><span class="sxs-lookup"><span data-stu-id="7cfa1-267">Combined format expressions</span></span>  

|<span data-ttu-id="7cfa1-268">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-268">Sample Expression</span></span>|<span data-ttu-id="7cfa1-269">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-269">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="7cfa1-270">\`5999</span><span class="sxs-lookup"><span data-stu-id="7cfa1-270">\`5999</span></span>|<span data-ttu-id="7cfa1-271">8100..8490\`</span><span class="sxs-lookup"><span data-stu-id="7cfa1-271">8100..8490\`</span></span>|<span data-ttu-id="7cfa1-272">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-272">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|<span data-ttu-id="7cfa1-273">\`..1299</span><span class="sxs-lookup"><span data-stu-id="7cfa1-273">\`..1299</span></span>|<span data-ttu-id="7cfa1-274">1400..\`</span><span class="sxs-lookup"><span data-stu-id="7cfa1-274">1400..\`</span></span>|<span data-ttu-id="7cfa1-275">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-275">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|`>50&<100`|<span data-ttu-id="7cfa1-276">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span><span class="sxs-lookup"><span data-stu-id="7cfa1-276">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  


## <span data-ttu-id="7cfa1-277"><a name="FilterTokens"> </a>Filter tokens</span><span class="sxs-lookup"><span data-stu-id="7cfa1-277"><a name="FilterTokens"> </a>Filter tokens</span></span>
<span data-ttu-id="7cfa1-278">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-278">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span></span> <span data-ttu-id="7cfa1-279">After entering the token word, the word is replaced by the value or values that it represents.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-279">After entering the token word, the word is replaced by the value or values that it represents.</span></span> <span data-ttu-id="7cfa1-280">This makes filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-280">This makes filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span></span> <span data-ttu-id="7cfa1-281">The tables below describe some of the tokens you can type as filter criteria.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-281">The tables below describe some of the tokens you can type as filter criteria.</span></span>

> [!TIP]
> <span data-ttu-id="7cfa1-282">Your organisation may use custom tokens.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-282">Your organization may use custom tokens.</span></span> <span data-ttu-id="7cfa1-283">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-283">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span></span> <span data-ttu-id="7cfa1-284">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens)</span><span class="sxs-lookup"><span data-stu-id="7cfa1-284">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens)</span></span>


### <a name="me-or-userid-records-assigned-to-you"></a><span data-ttu-id="7cfa1-285">(%me or %userid) Records assigned to you</span><span class="sxs-lookup"><span data-stu-id="7cfa1-285">(%me or %userid) Records assigned to you</span></span>

<span data-ttu-id="7cfa1-286">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-286">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span></span>

|<span data-ttu-id="7cfa1-287">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-287">Sample Expression</span></span>|<span data-ttu-id="7cfa1-288">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-288">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%me`<br /><span data-ttu-id="7cfa1-289">or</span><span class="sxs-lookup"><span data-stu-id="7cfa1-289">or</span></span><br />`%userid`|<span data-ttu-id="7cfa1-290">Records the are assigned to your user account.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-290">Records the are assigned to your user account.</span></span> |  

### <a name="mycustomers-customers-in-my-customers"></a><span data-ttu-id="7cfa1-291">(%mycustomers) Customers in My Customers</span><span class="sxs-lookup"><span data-stu-id="7cfa1-291">(%mycustomers) Customers in My Customers</span></span>

<span data-ttu-id="7cfa1-292">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-292">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Center.</span></span>

|<span data-ttu-id="7cfa1-293">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-293">Sample Expression</span></span>|<span data-ttu-id="7cfa1-294">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-294">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%mycustomers`|<span data-ttu-id="7cfa1-295">Customers in the **My Customers** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-295">Customers in the **My Customers** on your Role Center.</span></span> |  

### <a name="myitems-items-in-my-items"></a><span data-ttu-id="7cfa1-296">(%myitems) Items in My Items</span><span class="sxs-lookup"><span data-stu-id="7cfa1-296">(%myitems) Items in My Items</span></span>

<span data-ttu-id="7cfa1-297">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-297">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Center.</span></span>

|<span data-ttu-id="7cfa1-298">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-298">Sample Expression</span></span>|<span data-ttu-id="7cfa1-299">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-299">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myitems`|<span data-ttu-id="7cfa1-300">Items in the **My Items** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-300">Items in the **My Items** on your Role Center.</span></span> |  

### <a name="myvendors-vendors-in-my-vendors"></a><span data-ttu-id="7cfa1-301">(%myvendors) Vendors in My Vendors</span><span class="sxs-lookup"><span data-stu-id="7cfa1-301">(%myvendors) Vendors in My Vendors</span></span>

<span data-ttu-id="7cfa1-302">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-302">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Center.</span></span>

|<span data-ttu-id="7cfa1-303">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="7cfa1-303">Sample Expression</span></span>|<span data-ttu-id="7cfa1-304">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="7cfa1-304">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myvendors`|<span data-ttu-id="7cfa1-305">Venders in the **My Vendors** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="7cfa1-305">Venders in the **My Vendors** on your Role Center.</span></span> |  


## <a name="see-also"></a><span data-ttu-id="7cfa1-306">See Also</span><span class="sxs-lookup"><span data-stu-id="7cfa1-306">See Also</span></span>
<span data-ttu-id="7cfa1-307">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7cfa1-307">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="7cfa1-308">Common questions about Searching and Filtering</span><span class="sxs-lookup"><span data-stu-id="7cfa1-308">Common questions about Searching and Filtering</span></span>](ui-search-filter-faq.md)

