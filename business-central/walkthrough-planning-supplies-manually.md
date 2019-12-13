---
title: Walkthrough - Planning Supplies Manually | Microsoft Docs
description: This walkthrough demonstrates the process of planning supply orders to fulfill new demand. You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 0da12af6eb5a165c717cd112735a91aebe3ae85d
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/03/2019
ms.locfileid: "2876974"
---
# <a name="walkthrough-planning-supplies-manually"></a><span data-ttu-id="98aaa-104">Walkthrough: Planning Supplies Manually</span><span class="sxs-lookup"><span data-stu-id="98aaa-104">Walkthrough: Planning Supplies Manually</span></span>

<span data-ttu-id="98aaa-105">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="98aaa-105">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span></span> <span data-ttu-id="98aaa-106">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span><span class="sxs-lookup"><span data-stu-id="98aaa-106">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span></span>

<span data-ttu-id="98aaa-107">This walkthrough demonstrates the process of planning supply orders to fulfil new demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-107">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span></span> <span data-ttu-id="98aaa-108">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-108">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span></span> <span data-ttu-id="98aaa-109">In this walkthrough you will use the **Order Planning** page, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span><span class="sxs-lookup"><span data-stu-id="98aaa-109">In this walkthrough you will use the **Order Planning** page, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="98aaa-110">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="98aaa-110">About This Walkthrough</span></span>  
 <span data-ttu-id="98aaa-111">This walkthrough illustrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="98aaa-111">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="98aaa-112">Planning a purchase order for manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="98aaa-112">Planning a purchase order for manufacturing components.</span></span>  
-   <span data-ttu-id="98aaa-113">Planning a transfer order to fulfill sales demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-113">Planning a transfer order to fulfill sales demand.</span></span>  
-   <span data-ttu-id="98aaa-114">Planning a production order for a multilevel item.</span><span class="sxs-lookup"><span data-stu-id="98aaa-114">Planning a production order for a multilevel item.</span></span>  

## <a name="roles"></a><span data-ttu-id="98aaa-115">Roles</span><span class="sxs-lookup"><span data-stu-id="98aaa-115">Roles</span></span>  
 <span data-ttu-id="98aaa-116">This walkthrough demonstrates tasks performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="98aaa-116">This walkthrough demonstrates tasks performed by the following user roles:</span></span>  

-   <span data-ttu-id="98aaa-117">Production Planner</span><span class="sxs-lookup"><span data-stu-id="98aaa-117">Production Planner</span></span>  
-   <span data-ttu-id="98aaa-118">Purchasing Agent</span><span class="sxs-lookup"><span data-stu-id="98aaa-118">Purchasing Agent</span></span>  
-   <span data-ttu-id="98aaa-119">Sales Order Processor</span><span class="sxs-lookup"><span data-stu-id="98aaa-119">Sales Order Processor</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="98aaa-120">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="98aaa-120">Prerequisites</span></span>  
 <span data-ttu-id="98aaa-121">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="98aaa-121">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="98aaa-122">The following modifications must be made to the database:</span><span class="sxs-lookup"><span data-stu-id="98aaa-122">The following modifications must be made to the database:</span></span>  

-   <span data-ttu-id="98aaa-123">Delete all existing sales orders for bicycles.</span><span class="sxs-lookup"><span data-stu-id="98aaa-123">Delete all existing sales orders for bicycles.</span></span>  
-   <span data-ttu-id="98aaa-124">Create one sales order for 10 bicycles at BLUE location.</span><span class="sxs-lookup"><span data-stu-id="98aaa-124">Create one sales order for 10 bicycles at BLUE location.</span></span>  
-   <span data-ttu-id="98aaa-125">Delete all planned and firm planned production orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-125">Delete all planned and firm planned production orders.</span></span> <span data-ttu-id="98aaa-126">Do not delete started orders with entries that are already posted.</span><span class="sxs-lookup"><span data-stu-id="98aaa-126">Do not delete started orders with entries that are already posted.</span></span>  

 <span data-ttu-id="98aaa-127">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span><span class="sxs-lookup"><span data-stu-id="98aaa-127">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span></span>  

## <a name="story"></a><span data-ttu-id="98aaa-128">Story</span><span class="sxs-lookup"><span data-stu-id="98aaa-128">Story</span></span>  
 <span data-ttu-id="98aaa-129">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-129">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span></span>  

 <span data-ttu-id="98aaa-130">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** page to manually create supply orders, one product level at a time.</span><span class="sxs-lookup"><span data-stu-id="98aaa-130">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** page to manually create supply orders, one product level at a time.</span></span>  

 <span data-ttu-id="98aaa-131">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span><span class="sxs-lookup"><span data-stu-id="98aaa-131">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span></span>  

## <a name="setting-up-the-sample-data"></a><span data-ttu-id="98aaa-132">Setting Up the Sample Data</span><span class="sxs-lookup"><span data-stu-id="98aaa-132">Setting Up the Sample Data</span></span>  
 <span data-ttu-id="98aaa-133">The standard CRONUS demonstration company currently has lots of unplanned demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-133">The standard CRONUS demonstration company currently has lots of unplanned demand.</span></span> <span data-ttu-id="98aaa-134">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span><span class="sxs-lookup"><span data-stu-id="98aaa-134">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span></span>  

## <a name="using-the-order-planning-page"></a><span data-ttu-id="98aaa-135">Using the Order Planning Page</span><span class="sxs-lookup"><span data-stu-id="98aaa-135">Using the Order Planning Page</span></span>  

<span data-ttu-id="98aaa-136">The **Order Planning** page can be accessed from several different locations:</span><span class="sxs-lookup"><span data-stu-id="98aaa-136">The **Order Planning** page can be accessed from several different locations:</span></span>  

-   <span data-ttu-id="98aaa-137">Manufacturing, Planning</span><span class="sxs-lookup"><span data-stu-id="98aaa-137">Manufacturing, Planning</span></span>  
-   <span data-ttu-id="98aaa-138">Sales & Marketing, Order Processing</span><span class="sxs-lookup"><span data-stu-id="98aaa-138">Sales & Marketing, Order Processing</span></span>  
-   <span data-ttu-id="98aaa-139">Purchase, Planning</span><span class="sxs-lookup"><span data-stu-id="98aaa-139">Purchase, Planning</span></span>  
-   <span data-ttu-id="98aaa-140">In addition, you can open this page for a specific production order by choosing the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-140">In addition, you can open this page for a specific production order by choosing the **Planning** action.</span></span>

### <a name="to-use-the-order-planning-page"></a><span data-ttu-id="98aaa-141">To use the Order Planning page</span><span class="sxs-lookup"><span data-stu-id="98aaa-141">To use the Order Planning page</span></span>  

1.  <span data-ttu-id="98aaa-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Order Planning**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="98aaa-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Order Planning**, and then choose the related link.</span></span>  

     <span data-ttu-id="98aaa-143">When the **Order Planning** page first opens, a plan must be calculated to show the new demand since it was last calculated.</span><span class="sxs-lookup"><span data-stu-id="98aaa-143">When the **Order Planning** page first opens, a plan must be calculated to show the new demand since it was last calculated.</span></span>  

2.  <span data-ttu-id="98aaa-144">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-144">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="98aaa-145">The planning system analyzes any new demand that has been introduced, such as new sales, changed sales, or production orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-145">The planning system analyzes any new demand that has been introduced, such as new sales, changed sales, or production orders.</span></span>  

     <span data-ttu-id="98aaa-146">Based on total availability, the quantity needed for each demand line is calculated.</span><span class="sxs-lookup"><span data-stu-id="98aaa-146">Based on total availability, the quantity needed for each demand line is calculated.</span></span> <span data-ttu-id="98aaa-147">This calculation is performed order-by-order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-147">This calculation is performed order-by-order.</span></span> <span data-ttu-id="98aaa-148">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span><span class="sxs-lookup"><span data-stu-id="98aaa-148">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span></span> <span data-ttu-id="98aaa-149">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span><span class="sxs-lookup"><span data-stu-id="98aaa-149">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span></span>  

3.  <span data-ttu-id="98aaa-150">Be sure that the **Order Planning** page is maximised and that column fields are resized to show all the default field names.</span><span class="sxs-lookup"><span data-stu-id="98aaa-150">Be sure that the **Order Planning** page is maximized and that column fields are resized to show all the default field names.</span></span>  

     <span data-ttu-id="98aaa-151">When the calculation is completed, the page displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span><span class="sxs-lookup"><span data-stu-id="98aaa-151">When the calculation is completed, the page displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span></span>  

     <span data-ttu-id="98aaa-152">Notice that CRONUS has several orders with unfulfilled demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-152">Notice that CRONUS has several orders with unfulfilled demand.</span></span> <span data-ttu-id="98aaa-153">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span><span class="sxs-lookup"><span data-stu-id="98aaa-153">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span></span>  

4.  <span data-ttu-id="98aaa-154">In the **Show Demand As** field, select the **All Demand** filter.</span><span class="sxs-lookup"><span data-stu-id="98aaa-154">In the **Show Demand As** field, select the **All Demand** filter.</span></span>  

     <span data-ttu-id="98aaa-155">With the **Demand Type** field, you can choose which order types that you want to display.</span><span class="sxs-lookup"><span data-stu-id="98aaa-155">With the **Demand Type** field, you can choose which order types that you want to display.</span></span>  

     <span data-ttu-id="98aaa-156">Orders that do not have availability problems are not shown.</span><span class="sxs-lookup"><span data-stu-id="98aaa-156">Orders that do not have availability problems are not shown.</span></span> <span data-ttu-id="98aaa-157">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span><span class="sxs-lookup"><span data-stu-id="98aaa-157">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span></span>  

## <a name="planning-a-purchase-order-to-fulfill-component-demand"></a><span data-ttu-id="98aaa-158">Planning a Purchase Order to Fulfill Component Demand</span><span class="sxs-lookup"><span data-stu-id="98aaa-158">Planning a Purchase Order to Fulfill Component Demand</span></span>  
 <span data-ttu-id="98aaa-159">In this procedure, you create a purchase order for needed manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="98aaa-159">In this procedure, you create a purchase order for needed manufacturing components.</span></span>  

### <a name="to-plan-a-purchase-order-to-fulfill-component-need-in-production"></a><span data-ttu-id="98aaa-160">To plan a purchase order to fulfill component need in production</span><span class="sxs-lookup"><span data-stu-id="98aaa-160">To plan a purchase order to fulfill component need in production</span></span>  

1.  <span data-ttu-id="98aaa-161">Expand the first line (choose the + symbol).</span><span class="sxs-lookup"><span data-stu-id="98aaa-161">Expand the first line (choose the + symbol).</span></span>  
2.  <span data-ttu-id="98aaa-162">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-162">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span></span>  
3.  <span data-ttu-id="98aaa-163">Close the opened production order to return to the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="98aaa-163">Close the opened production order to return to the **Order Planning** page.</span></span>  
4.  <span data-ttu-id="98aaa-164">In the **Replenishment System** field, select **Purchase**.</span><span class="sxs-lookup"><span data-stu-id="98aaa-164">In the **Replenishment System** field, select **Purchase**.</span></span>  

     <span data-ttu-id="98aaa-165">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span><span class="sxs-lookup"><span data-stu-id="98aaa-165">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span></span>  

    -   <span data-ttu-id="98aaa-166">**Purchase** – To create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-166">**Purchase** – To create a purchase order.</span></span>  
    -   <span data-ttu-id="98aaa-167">**Transfer** – To create a transfer order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-167">**Transfer** – To create a transfer order.</span></span>  
    -   <span data-ttu-id="98aaa-168">**Prod. Order** – To create a production order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-168">**Prod. Order** – To create a production order.</span></span>  

5.  <span data-ttu-id="98aaa-169">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span><span class="sxs-lookup"><span data-stu-id="98aaa-169">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span></span>  

    -   <span data-ttu-id="98aaa-170">**Vendor** – For purchases</span><span class="sxs-lookup"><span data-stu-id="98aaa-170">**Vendor** – For purchases</span></span>  
    -   <span data-ttu-id="98aaa-171">**Location** – For transfers</span><span class="sxs-lookup"><span data-stu-id="98aaa-171">**Location** – For transfers</span></span>  

     <span data-ttu-id="98aaa-172">If the field is not filled in, an error message will display when you try to create the supply orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-172">If the field is not filled in, an error message will display when you try to create the supply orders.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="98aaa-173">If the components have a default vendor number set up on the item cards, the lines will be preset.</span><span class="sxs-lookup"><span data-stu-id="98aaa-173">If the components have a default vendor number set up on the item cards, the lines will be preset.</span></span>  

6.  <span data-ttu-id="98aaa-174">Choose the **Supply From**  field.</span><span class="sxs-lookup"><span data-stu-id="98aaa-174">Choose the **Supply From**  field.</span></span>  
7.  <span data-ttu-id="98aaa-175">On the **Item Vendor Catalogue** page, choose the **New** action, and then select vendor **30000**.</span><span class="sxs-lookup"><span data-stu-id="98aaa-175">On the **Item Vendor Catalogue** page, choose the **New** action, and then select vendor **30000**.</span></span>  
8.  <span data-ttu-id="98aaa-176">Choose the **OK** button to return to the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="98aaa-176">Choose the **OK** button to return to the **Order Planning** page.</span></span>  
9. <span data-ttu-id="98aaa-177">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-177">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span></span>  

     <span data-ttu-id="98aaa-178">You are now ready to create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-178">You are now ready to create a purchase order.</span></span>  

10. <span data-ttu-id="98aaa-179">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-179">Choose the **Make Orders** action.</span></span> <span data-ttu-id="98aaa-180">The **Make Supply Orders** page opens.</span><span class="sxs-lookup"><span data-stu-id="98aaa-180">The **Make Supply Orders** page opens.</span></span>  
11. <span data-ttu-id="98aaa-181">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="98aaa-181">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span></span>  
12. <span data-ttu-id="98aaa-182">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span><span class="sxs-lookup"><span data-stu-id="98aaa-182">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span></span>  
13. <span data-ttu-id="98aaa-183">Choose the **OK** button to create purchase orders for all the components of the order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-183">Choose the **OK** button to create purchase orders for all the components of the order.</span></span>  

     <span data-ttu-id="98aaa-184">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-184">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span></span>  

## <a name="planning-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="98aaa-185">Planning a Transfer Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="98aaa-185">Planning a Transfer Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="98aaa-186">In this procedure, you will plan for demand from a sales order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-186">In this procedure, you will plan for demand from a sales order.</span></span> <span data-ttu-id="98aaa-187">Demand lines represent sales lines and not component lines, as in production demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-187">Demand lines represent sales lines and not component lines, as in production demand.</span></span>  

### <a name="to-plan-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="98aaa-188">To plan a transfer order to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="98aaa-188">To plan a transfer order to fulfill sales demand</span></span>  

1.  <span data-ttu-id="98aaa-189">Move the pointer to the planning line for order **2008**.</span><span class="sxs-lookup"><span data-stu-id="98aaa-189">Move the pointer to the planning line for order **2008**.</span></span>  
2.  <span data-ttu-id="98aaa-190">Expand the line and move the pointer to the demand line.</span><span class="sxs-lookup"><span data-stu-id="98aaa-190">Expand the line and move the pointer to the demand line.</span></span>  

     <span data-ttu-id="98aaa-191">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span><span class="sxs-lookup"><span data-stu-id="98aaa-191">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span></span>  

     <span data-ttu-id="98aaa-192">The item’s defined replenishment system and default vendor will display.</span><span class="sxs-lookup"><span data-stu-id="98aaa-192">The item’s defined replenishment system and default vendor will display.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="98aaa-193">At the bottom of the page, there are four information fields.</span><span class="sxs-lookup"><span data-stu-id="98aaa-193">At the bottom of the page, there are four information fields.</span></span> <span data-ttu-id="98aaa-194">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span><span class="sxs-lookup"><span data-stu-id="98aaa-194">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span></span> <span data-ttu-id="98aaa-195">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span><span class="sxs-lookup"><span data-stu-id="98aaa-195">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span></span> <span data-ttu-id="98aaa-196">You will want to plan for this stock.</span><span class="sxs-lookup"><span data-stu-id="98aaa-196">You will want to plan for this stock.</span></span>  

3.  <span data-ttu-id="98aaa-197">Choose the **Available for Transfer** field to open the **Get Alternative Supply** page.</span><span class="sxs-lookup"><span data-stu-id="98aaa-197">Choose the **Available for Transfer** field to open the **Get Alternative Supply** page.</span></span>  
4.  <span data-ttu-id="98aaa-198">Choose the **OK** button to book the ten items that are available.</span><span class="sxs-lookup"><span data-stu-id="98aaa-198">Choose the **OK** button to book the ten items that are available.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="98aaa-199">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span><span class="sxs-lookup"><span data-stu-id="98aaa-199">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span></span> <span data-ttu-id="98aaa-200">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span><span class="sxs-lookup"><span data-stu-id="98aaa-200">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span></span> <span data-ttu-id="98aaa-201">The **Substitutes Exists** field works in the same way.</span><span class="sxs-lookup"><span data-stu-id="98aaa-201">The **Substitutes Exists** field works in the same way.</span></span>  

5.  <span data-ttu-id="98aaa-202">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-202">Choose the **Make Orders** action.</span></span> <span data-ttu-id="98aaa-203">The **Make Supply Orders** page opens.</span><span class="sxs-lookup"><span data-stu-id="98aaa-203">The **Make Supply Orders** page opens.</span></span>  
6.  <span data-ttu-id="98aaa-204">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="98aaa-204">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span></span>  
7.  <span data-ttu-id="98aaa-205">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span><span class="sxs-lookup"><span data-stu-id="98aaa-205">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span></span>  
8.  <span data-ttu-id="98aaa-206">Choose the **OK** button to create the transfer order to supply the sales order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-206">Choose the **OK** button to create the transfer order to supply the sales order.</span></span>  

     <span data-ttu-id="98aaa-207">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-207">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span></span>  

## <a name="planning-a-multilevel-production-order-to-fulfill-sales-demand"></a><span data-ttu-id="98aaa-208">Planning a Multilevel Production Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="98aaa-208">Planning a Multilevel Production Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="98aaa-209">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-209">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span></span>  

### <a name="to-plan-multilevel-production-to-fulfill-sales-demand"></a><span data-ttu-id="98aaa-210">To plan multilevel production to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="98aaa-210">To plan multilevel production to fulfill sales demand</span></span>  

1.  <span data-ttu-id="98aaa-211">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span><span class="sxs-lookup"><span data-stu-id="98aaa-211">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span></span>  

     <span data-ttu-id="98aaa-212">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span><span class="sxs-lookup"><span data-stu-id="98aaa-212">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span></span> <span data-ttu-id="98aaa-213">Proceed to add an extra bell to the component need of each bicycle.</span><span class="sxs-lookup"><span data-stu-id="98aaa-213">Proceed to add an extra bell to the component need of each bicycle.</span></span>  

2.  <span data-ttu-id="98aaa-214">Choose the **Components** action to open the **Planning Components** page.</span><span class="sxs-lookup"><span data-stu-id="98aaa-214">Choose the **Components** action to open the **Planning Components** page.</span></span>  
3.  <span data-ttu-id="98aaa-215">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span><span class="sxs-lookup"><span data-stu-id="98aaa-215">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span></span>  
4.  <span data-ttu-id="98aaa-216">On the **Order Planning** page, consider your planning alternatives.</span><span class="sxs-lookup"><span data-stu-id="98aaa-216">On the **Order Planning** page, consider your planning alternatives.</span></span> <span data-ttu-id="98aaa-217">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span><span class="sxs-lookup"><span data-stu-id="98aaa-217">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span></span> <span data-ttu-id="98aaa-218">You must create the suggested supply order, a production order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-218">You must create the suggested supply order, a production order.</span></span>  
5.  <span data-ttu-id="98aaa-219">Choose the **Make Orders** action to create the production order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-219">Choose the **Make Orders** action to create the production order.</span></span>  

     <span data-ttu-id="98aaa-220">On the **Order Planning** page, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span><span class="sxs-lookup"><span data-stu-id="98aaa-220">On the **Order Planning** page, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span></span>  

6.  <span data-ttu-id="98aaa-221">Close the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="98aaa-221">Close the **Order Planning** page.</span></span>  

     <span data-ttu-id="98aaa-222">Now, you could choose to stay in this view and complete all the planning tasks.</span><span class="sxs-lookup"><span data-stu-id="98aaa-222">Now, you could choose to stay in this view and complete all the planning tasks.</span></span> <span data-ttu-id="98aaa-223">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="98aaa-223">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** page.</span></span>  

 <span data-ttu-id="98aaa-224">As a production planner you now must plan a specific production order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-224">As a production planner you now must plan a specific production order.</span></span>  

### <a name="to-plan-a-specific-production-order"></a><span data-ttu-id="98aaa-225">To plan a specific production order</span><span class="sxs-lookup"><span data-stu-id="98aaa-225">To plan a specific production order</span></span>  

1.  <span data-ttu-id="98aaa-226">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span><span class="sxs-lookup"><span data-stu-id="98aaa-226">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span></span>  
2.  <span data-ttu-id="98aaa-227">Open the **Prod. Order Components** page to check that the extra bell is reflected on the production order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-227">Open the **Prod. Order Components** page to check that the extra bell is reflected on the production order.</span></span>  
3.  <span data-ttu-id="98aaa-228">Choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-228">Choose the **Planning** action.</span></span>  

     <span data-ttu-id="98aaa-229">The **Order Planning** page opens in a view that is always filtered on the specific production demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-229">The **Order Planning** page opens in a view that is always filtered on the specific production demand.</span></span> <span data-ttu-id="98aaa-230">Sales demand is not displayed.</span><span class="sxs-lookup"><span data-stu-id="98aaa-230">Sales demand is not displayed.</span></span> <span data-ttu-id="98aaa-231">You must calculate a plan before you can see any additional demand.</span><span class="sxs-lookup"><span data-stu-id="98aaa-231">You must calculate a plan before you can see any additional demand.</span></span>  

4.  <span data-ttu-id="98aaa-232">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-232">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="98aaa-233">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span><span class="sxs-lookup"><span data-stu-id="98aaa-233">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span></span> <span data-ttu-id="98aaa-234">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-234">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span></span>  

5.  <span data-ttu-id="98aaa-235">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-235">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span></span>  

     <span data-ttu-id="98aaa-236">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span><span class="sxs-lookup"><span data-stu-id="98aaa-236">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span></span>  

     <span data-ttu-id="98aaa-237">Now you must supply ten of each component.</span><span class="sxs-lookup"><span data-stu-id="98aaa-237">Now you must supply ten of each component.</span></span>  

     <span data-ttu-id="98aaa-238">Note that four of the demand lines have replenishment system Prod. Order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-238">Note that four of the demand lines have replenishment system Prod. Order.</span></span> <span data-ttu-id="98aaa-239">These four subassemblies represent the second product level of the bicycle.</span><span class="sxs-lookup"><span data-stu-id="98aaa-239">These four subassemblies represent the second product level of the bicycle.</span></span>  

     <span data-ttu-id="98aaa-240">The default replenishment settings are already filled in and you can proceed to make orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-240">The default replenishment settings are already filled in and you can proceed to make orders.</span></span>  

6.  <span data-ttu-id="98aaa-241">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-241">Choose the **Make Orders** action.</span></span>  

     <span data-ttu-id="98aaa-242">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span><span class="sxs-lookup"><span data-stu-id="98aaa-242">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span></span> <span data-ttu-id="98aaa-243">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-243">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span></span>  

7.  <span data-ttu-id="98aaa-244">On the **Make Supply Order** page, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span><span class="sxs-lookup"><span data-stu-id="98aaa-244">On the **Make Supply Order** page, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span></span>  

     <span data-ttu-id="98aaa-245">Note that the top-level production demand for production order 101001 no longer exists.</span><span class="sxs-lookup"><span data-stu-id="98aaa-245">Note that the top-level production demand for production order 101001 no longer exists.</span></span> <span data-ttu-id="98aaa-246">This means that the initial production demand for subassemblies has been planned for.</span><span class="sxs-lookup"><span data-stu-id="98aaa-246">This means that the initial production demand for subassemblies has been planned for.</span></span>  

     <span data-ttu-id="98aaa-247">On the **Order Planning** page, you calculate a plan again in order to plan the bicycle structure.</span><span class="sxs-lookup"><span data-stu-id="98aaa-247">On the **Order Planning** page, you calculate a plan again in order to plan the bicycle structure.</span></span>  

8.  <span data-ttu-id="98aaa-248">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span><span class="sxs-lookup"><span data-stu-id="98aaa-248">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span></span>  

     <span data-ttu-id="98aaa-249">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span><span class="sxs-lookup"><span data-stu-id="98aaa-249">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span></span> <span data-ttu-id="98aaa-250">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span><span class="sxs-lookup"><span data-stu-id="98aaa-250">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span></span>  

9. <span data-ttu-id="98aaa-251">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-251">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span></span>  

     <span data-ttu-id="98aaa-252">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span><span class="sxs-lookup"><span data-stu-id="98aaa-252">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span></span> <span data-ttu-id="98aaa-253">You decide to make the proposed orders.</span><span class="sxs-lookup"><span data-stu-id="98aaa-253">You decide to make the proposed orders.</span></span>  

10. <span data-ttu-id="98aaa-254">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-254">Choose the **Make Orders** action.</span></span>  
11. <span data-ttu-id="98aaa-255">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="98aaa-255">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span></span> <span data-ttu-id="98aaa-256">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span><span class="sxs-lookup"><span data-stu-id="98aaa-256">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span></span>  
12. <span data-ttu-id="98aaa-257">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="98aaa-257">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="98aaa-258">The message indicates that all required items are now supplied.</span><span class="sxs-lookup"><span data-stu-id="98aaa-258">The message indicates that all required items are now supplied.</span></span> <span data-ttu-id="98aaa-259">Verify the firm planned production orders that are created.</span><span class="sxs-lookup"><span data-stu-id="98aaa-259">Verify the firm planned production orders that are created.</span></span>  

13. <span data-ttu-id="98aaa-260">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="98aaa-260">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  

     <span data-ttu-id="98aaa-261">On the **Firm Planned Prod. Orders** page review how start times and end times of individual orders are scheduled according to the product structure.</span><span class="sxs-lookup"><span data-stu-id="98aaa-261">On the **Firm Planned Prod. Orders** page review how start times and end times of individual orders are scheduled according to the product structure.</span></span> <span data-ttu-id="98aaa-262">The lowest-level components are produced first.</span><span class="sxs-lookup"><span data-stu-id="98aaa-262">The lowest-level components are produced first.</span></span> <span data-ttu-id="98aaa-263">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span><span class="sxs-lookup"><span data-stu-id="98aaa-263">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="98aaa-264">See Also</span><span class="sxs-lookup"><span data-stu-id="98aaa-264">See Also</span></span>  
 <span data-ttu-id="98aaa-265">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span><span class="sxs-lookup"><span data-stu-id="98aaa-265">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span></span>  
 [<span data-ttu-id="98aaa-266">Walkthrough: Planning Supplies Automatically</span><span class="sxs-lookup"><span data-stu-id="98aaa-266">Walkthrough: Planning Supplies Automatically</span></span>](walkthrough-planning-supplies-automatically.md)
