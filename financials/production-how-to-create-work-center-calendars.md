---
title: How to Set Up Shop Calendars | Microsoft Docs
description: "A work centre calendar specifies the working days and hours, shifts, holidays, and absences that determine the work centre’s gross available capacity, measured in time, according to its defined efficiency and capacity values. Creating and enabling a work centre calendar involves several preparatory tasks."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: cf54f63e94ab3249f30d2fcdbef2c35e323e4cd8
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-shop-calendars"></a><span data-ttu-id="c8d94-104">Set Up Shop Calendars</span><span class="sxs-lookup"><span data-stu-id="c8d94-104">Set Up Shop Calendars</span></span>
<span data-ttu-id="c8d94-105">A work centre or machine calendar specifies the working days and hours, shifts, holidays, and absences that determine the centre’s gross available capacity, measured in time, according to its defined efficiency and capacity values.</span><span class="sxs-lookup"><span data-stu-id="c8d94-105">A work center or machine calendar specifies the working days and hours, shifts, holidays, and absences that determine the center’s gross available capacity, measured in time, according to its defined efficiency and capacity values.</span></span>

<span data-ttu-id="c8d94-106">As a foundation for calculating a specific work or machine centre calendar, you must first set up one or more general shop calendars.</span><span class="sxs-lookup"><span data-stu-id="c8d94-106">As a foundation for calculating a specific work or machine center calendar, you must first set up one or more general shop calendars.</span></span> <span data-ttu-id="c8d94-107">A shop calendar defines a standard work week according to start and end times of each working day and the work shift relation.</span><span class="sxs-lookup"><span data-stu-id="c8d94-107">A shop calendar defines a standard work week according to start and end times of each working day and the work shift relation.</span></span> <span data-ttu-id="c8d94-108">In addition, the shop calendar defines the fixed holidays during a year.</span><span class="sxs-lookup"><span data-stu-id="c8d94-108">In addition, the shop calendar defines the fixed holidays during a year.</span></span>  

<span data-ttu-id="c8d94-109">The following describes how to set up work centre calendars.</span><span class="sxs-lookup"><span data-stu-id="c8d94-109">The following describes how to set up work center calendars.</span></span> <span data-ttu-id="c8d94-110">The steps are similar when setting up machine centre calendars.</span><span class="sxs-lookup"><span data-stu-id="c8d94-110">The steps are similar when setting up machine center calendars.</span></span>  

## <a name="to-create-work-shifts"></a><span data-ttu-id="c8d94-111">To create work shifts</span><span class="sxs-lookup"><span data-stu-id="c8d94-111">To create work shifts</span></span>  
1.  <span data-ttu-id="c8d94-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Shifts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c8d94-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Shifts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c8d94-113">On a blank line, enter a number in the **Code** field to identify the work shift, for example, **1**.</span><span class="sxs-lookup"><span data-stu-id="c8d94-113">On a blank line, enter a number in the **Code** field to identify the work shift, for example, **1**.</span></span>  
3.  <span data-ttu-id="c8d94-114">Describe the work shift in the **Description** field, for example, **1st shift**.</span><span class="sxs-lookup"><span data-stu-id="c8d94-114">Describe the work shift in the **Description** field, for example, **1st shift**.</span></span>  
4.  <span data-ttu-id="c8d94-115">Optionally, fill in lines for a second or third work shift.</span><span class="sxs-lookup"><span data-stu-id="c8d94-115">Optionally, fill in lines for a second or third work shift.</span></span>  

<span data-ttu-id="c8d94-116">Even if your work centres do not work in different work shifts, enter at least one work shift code.</span><span class="sxs-lookup"><span data-stu-id="c8d94-116">Even if your work centers do not work in different work shifts, enter at least one work shift code.</span></span>  

## <a name="to-set-up-a-shop-calendar"></a><span data-ttu-id="c8d94-117">To set up a shop calendar</span><span class="sxs-lookup"><span data-stu-id="c8d94-117">To set up a shop calendar</span></span>  
1.  <span data-ttu-id="c8d94-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Shop Calendars**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c8d94-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Shop Calendars**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c8d94-119">On a blank line, enter a number in the **Code** field to identify the shop calendar.</span><span class="sxs-lookup"><span data-stu-id="c8d94-119">On a blank line, enter a number in the **Code** field to identify the shop calendar.</span></span>  
3.  <span data-ttu-id="c8d94-120">Describe the shop calendar in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="c8d94-120">Describe the shop calendar in the **Description** field.</span></span>  
4.  <span data-ttu-id="c8d94-121">Choose the **Working Days** action.</span><span class="sxs-lookup"><span data-stu-id="c8d94-121">Choose the **Working Days** action.</span></span>
5.  <span data-ttu-id="c8d94-122">In the **Shop Calendar Working Days** window, define a complete work week, with the start and end times for each day.</span><span class="sxs-lookup"><span data-stu-id="c8d94-122">In the **Shop Calendar Working Days** window, define a complete work week, with the start and end times for each day.</span></span>  

    <span data-ttu-id="c8d94-123">In the **Work Shift Code** field, select one of the shifts that you previously defined.</span><span class="sxs-lookup"><span data-stu-id="c8d94-123">In the **Work Shift Code** field, select one of the shifts that you previously defined.</span></span> <span data-ttu-id="c8d94-124">Add a line for every working day and every shift.</span><span class="sxs-lookup"><span data-stu-id="c8d94-124">Add a line for every working day and every shift.</span></span> <span data-ttu-id="c8d94-125">For example:</span><span class="sxs-lookup"><span data-stu-id="c8d94-125">For example:</span></span>  

    <span data-ttu-id="c8d94-126">Monday  07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="c8d94-126">Monday  07:00 15:00 1</span></span>   
    <span data-ttu-id="c8d94-127">Tuesday 07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="c8d94-127">Tuesday 07:00 15:00 1</span></span>  

    <span data-ttu-id="c8d94-128">If you need a shop calendar with two work shifts, you must fill it in in this manner:</span><span class="sxs-lookup"><span data-stu-id="c8d94-128">If you need a shop calendar with two work shifts, you must fill it in in this manner:</span></span>  

    <span data-ttu-id="c8d94-129">Monday 07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="c8d94-129">Monday 07:00 15:00 1</span></span>   
    <span data-ttu-id="c8d94-130">Monday 15:00 23:00 2</span><span class="sxs-lookup"><span data-stu-id="c8d94-130">Monday 15:00 23:00 2</span></span>  
    <span data-ttu-id="c8d94-131">Tuesday 07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="c8d94-131">Tuesday 07:00 15:00 1</span></span>  
    <span data-ttu-id="c8d94-132">Tuesday 15:00 23:00 2</span><span class="sxs-lookup"><span data-stu-id="c8d94-132">Tuesday 15:00 23:00 2</span></span>  

    <span data-ttu-id="c8d94-133">Any week days that you do not define in the shop calendar, such as Saturday and Sunday, are considered non-working days and will have zero available capacity in a work centre calendar.</span><span class="sxs-lookup"><span data-stu-id="c8d94-133">Any week days that you do not define in the shop calendar, such as Saturday and Sunday, are considered non-working days and will have zero available capacity in a work center calendar.</span></span>  

    <span data-ttu-id="c8d94-134">When all the working days of a week are defined, you can close the **Shop Calendar Working Days** window and proceed to enter holidays.</span><span class="sxs-lookup"><span data-stu-id="c8d94-134">When all the working days of a week are defined, you can close the **Shop Calendar Working Days** window and proceed to enter holidays.</span></span>  

6.  <span data-ttu-id="c8d94-135">In the **Shop Calendars** window, select the shop calendar, and then choose the **Holidays** action.</span><span class="sxs-lookup"><span data-stu-id="c8d94-135">In the **Shop Calendars** window, select the shop calendar, and then choose the **Holidays** action.</span></span>
7. <span data-ttu-id="c8d94-136">In the **Shop Calendar Holidays** window, define the holidays of the year by entering the start date and time, the end time, and description of each holiday on individual lines.</span><span class="sxs-lookup"><span data-stu-id="c8d94-136">In the **Shop Calendar Holidays** window, define the holidays of the year by entering the start date and time, the end time, and description of each holiday on individual lines.</span></span> <span data-ttu-id="c8d94-137">For example:</span><span class="sxs-lookup"><span data-stu-id="c8d94-137">For example:</span></span>  

    <span data-ttu-id="c8d94-138">04/07/14 0:00:00 23:59:00 Summer Holiday</span><span class="sxs-lookup"><span data-stu-id="c8d94-138">04/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  
    <span data-ttu-id="c8d94-139">05/07/14 0:00:00 23:59:00 Summer Holiday</span><span class="sxs-lookup"><span data-stu-id="c8d94-139">05/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  
    <span data-ttu-id="c8d94-140">06/07/14 0:00:00 23:59:00 Summer Holiday</span><span class="sxs-lookup"><span data-stu-id="c8d94-140">06/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  

<span data-ttu-id="c8d94-141">The defined holidays will have zero available capacity in a work centre calendar.</span><span class="sxs-lookup"><span data-stu-id="c8d94-141">The defined holidays will have zero available capacity in a work center calendar.</span></span>  

<span data-ttu-id="c8d94-142">The shop calendar can now be assigned to a work centre to calculate the work shop calendar that will govern all operation scheduling at that work centre.</span><span class="sxs-lookup"><span data-stu-id="c8d94-142">The shop calendar can now be assigned to a work center to calculate the work shop calendar that will govern all operation scheduling at that work center.</span></span>  

## <a name="to-calculate-a-work-center-calendar"></a><span data-ttu-id="c8d94-143">To calculate a work centre calendar</span><span class="sxs-lookup"><span data-stu-id="c8d94-143">To calculate a work center calendar</span></span>  

1.  <span data-ttu-id="c8d94-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Centres**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c8d94-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Centers**, and then choose the related link.</span></span>
2. <span data-ttu-id="c8d94-145">Open the work centre that you want to update.</span><span class="sxs-lookup"><span data-stu-id="c8d94-145">Open the work center that you want to update.</span></span>  
3. <span data-ttu-id="c8d94-146">In the **Shop Calendar Code** field, select which shop calendar to use as the foundation for a work centre calendar.</span><span class="sxs-lookup"><span data-stu-id="c8d94-146">In the **Shop Calendar Code** field, select which shop calendar to use as the foundation for a work center calendar.</span></span>  
4. <span data-ttu-id="c8d94-147">Choose the **Calendar** action.</span><span class="sxs-lookup"><span data-stu-id="c8d94-147">Choose the **Calendar** action.</span></span>  
5. <span data-ttu-id="c8d94-148">In the **Work Centre Calendar** window, choose the **Show Matrix** action.</span><span class="sxs-lookup"><span data-stu-id="c8d94-148">In the **Work Center Calendar** window, choose the **Show Matrix** action.</span></span>  

    <span data-ttu-id="c8d94-149">The left side of the matrix window lists the work centres that are set up.</span><span class="sxs-lookup"><span data-stu-id="c8d94-149">The left side of the matrix window lists the work centers that are set up.</span></span> <span data-ttu-id="c8d94-150">The right side shows a calendar displaying the available capacity values for each working day in the defined unit of measure, for example, **480** minutes.</span><span class="sxs-lookup"><span data-stu-id="c8d94-150">The right side shows a calendar displaying the available capacity values for each working day in the defined unit of measure, for example, **480** minutes.</span></span> <span data-ttu-id="c8d94-151">Each line represents the calendar of one work centre.</span><span class="sxs-lookup"><span data-stu-id="c8d94-151">Each line represents the calendar of one work center.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="c8d94-152">You can also select to view the capacity values for each week or month by changing the selection in the **View By** field in the **Work Centre Calendar** window.</span><span class="sxs-lookup"><span data-stu-id="c8d94-152">You can also select to view the capacity values for each week or month by changing the selection in the **View By** field in the **Work Center Calendar** window.</span></span>  

    <span data-ttu-id="c8d94-153">To reflect the new shop calendar as a line on the selected work centre, it must first be calculated.</span><span class="sxs-lookup"><span data-stu-id="c8d94-153">To reflect the new shop calendar as a line on the selected work center, it must first be calculated.</span></span>  

6.  <span data-ttu-id="c8d94-154">Choose the **Calculate** action.</span><span class="sxs-lookup"><span data-stu-id="c8d94-154">Choose the **Calculate** action.</span></span>  
7.  <span data-ttu-id="c8d94-155">On the **Work Centre** FastTab, you can set a filter to only calculate for one work centre.</span><span class="sxs-lookup"><span data-stu-id="c8d94-155">On the **Work Center** FastTab, you can set a filter to only calculate for one work center.</span></span> <span data-ttu-id="c8d94-156">If you do not set a filter, all existing work centre calendars will be calculated.</span><span class="sxs-lookup"><span data-stu-id="c8d94-156">If you do not set a filter, all existing work center calendars will be calculated.</span></span>  
8.  <span data-ttu-id="c8d94-157">Define the starting and ending dates of the calendar period that should be calculated, for example, one year from 01/01/14 to 31/12/14.</span><span class="sxs-lookup"><span data-stu-id="c8d94-157">Define the starting and ending dates of the calendar period that should be calculated, for example, one year from 01/01/14 to 31/12/14.</span></span>
9. <span data-ttu-id="c8d94-158">Choose the **OK** button to calculate capacity.</span><span class="sxs-lookup"><span data-stu-id="c8d94-158">Choose the **OK** button to calculate capacity.</span></span>  

<span data-ttu-id="c8d94-159">Calendar entries are now created or updated displaying the available capacity for each period according to the following three sets of master data:</span><span class="sxs-lookup"><span data-stu-id="c8d94-159">Calendar entries are now created or updated displaying the available capacity for each period according to the following three sets of master data:</span></span>  

- <span data-ttu-id="c8d94-160">The working days and shift defined in the assigned shop calendar.</span><span class="sxs-lookup"><span data-stu-id="c8d94-160">The working days and shift defined in the assigned shop calendar.</span></span>  
- <span data-ttu-id="c8d94-161">The value in the **Capacity** field on the work centre card.</span><span class="sxs-lookup"><span data-stu-id="c8d94-161">The value in the **Capacity** field on the work center card.</span></span>  
- <span data-ttu-id="c8d94-162">The value in the **Efficiency** field on the work centre card.</span><span class="sxs-lookup"><span data-stu-id="c8d94-162">The value in the **Efficiency** field on the work center card.</span></span>  

<span data-ttu-id="c8d94-163">The calculated work centre calendar will now define when and how much capacity is available at this work centre.</span><span class="sxs-lookup"><span data-stu-id="c8d94-163">The calculated work center calendar will now define when and how much capacity is available at this work center.</span></span> <span data-ttu-id="c8d94-164">This controls the detailed scheduling of operations performed at the work centre.</span><span class="sxs-lookup"><span data-stu-id="c8d94-164">This controls the detailed scheduling of operations performed at the work center.</span></span>  

## <a name="to-record-work-center-absence"></a><span data-ttu-id="c8d94-165">To record work centre absence</span><span class="sxs-lookup"><span data-stu-id="c8d94-165">To record work center absence</span></span>  
1.  <span data-ttu-id="c8d94-166">In the **Work Centre Calendar** window, choose the **Show Matrix** action.</span><span class="sxs-lookup"><span data-stu-id="c8d94-166">In the **Work Center Calendar** window, choose the **Show Matrix** action.</span></span>
2. <span data-ttu-id="c8d94-167">In the **Work Centre Calendar Matrix** window, select the work centre and calendar day when the absence time should be recorded, and then choose the **Absence** action.</span><span class="sxs-lookup"><span data-stu-id="c8d94-167">In the **Work Center Calendar Matrix** window, select the work center and calendar day when the absence time should be recorded, and then choose the **Absence** action.</span></span>  
3.  <span data-ttu-id="c8d94-168">In the **Absence** window, define the starting time, ending time, and description of that day’s absence.</span><span class="sxs-lookup"><span data-stu-id="c8d94-168">In the **Absence** window, define the starting time, ending time, and description of that day’s absence.</span></span> <span data-ttu-id="c8d94-169">For example:</span><span class="sxs-lookup"><span data-stu-id="c8d94-169">For example:</span></span>  

    <span data-ttu-id="c8d94-170">25/01/01 08:00 10:00 Maintenance</span><span class="sxs-lookup"><span data-stu-id="c8d94-170">25/01/01 08:00 10:00 Maintenance</span></span>  

4.  <span data-ttu-id="c8d94-171">Choose the **Update** action, and then close the **Absence** window.</span><span class="sxs-lookup"><span data-stu-id="c8d94-171">Choose the **Update** action, and then close the **Absence** window.</span></span>  

<span data-ttu-id="c8d94-172">The capacity of the selected day has now decreased by the recorded absence time.</span><span class="sxs-lookup"><span data-stu-id="c8d94-172">The capacity of the selected day has now decreased by the recorded absence time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c8d94-173">See Also</span><span class="sxs-lookup"><span data-stu-id="c8d94-173">See Also</span></span>  
[<span data-ttu-id="c8d94-174">Set Up Base Calendars</span><span class="sxs-lookup"><span data-stu-id="c8d94-174">Set Up Base Calendars</span></span>](across-how-to-assign-base-calendars.md)  
[<span data-ttu-id="c8d94-175">Set Up Work Centres and Machine Centres</span><span class="sxs-lookup"><span data-stu-id="c8d94-175">Set Up Work Centers and Machine Centers</span></span>](production-how-to-set-up-work-and-machine-centers.md)  
[<span data-ttu-id="c8d94-176">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="c8d94-176">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
[<span data-ttu-id="c8d94-177">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="c8d94-177">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="c8d94-178">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c8d94-178">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

