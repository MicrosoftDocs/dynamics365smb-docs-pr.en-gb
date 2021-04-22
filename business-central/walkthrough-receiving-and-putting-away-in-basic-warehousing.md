---
title: Walkthrough - Receive and put away in basic warehouse configurations
description: In Business Central, the inbound processes for receiving and putting away can be performed in four different ways, depending on the warehouse complexity level.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: c79891af3fbf85b78439cd66d02eafb6ff82c6ca
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772011"
---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a><span data-ttu-id="17234-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="17234-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span></span>

[!INCLUDE[complete_sample_data](includes/complete_sample_data.md)]  

<span data-ttu-id="17234-104">In [!INCLUDE[prod_short](includes/prod_short.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span><span class="sxs-lookup"><span data-stu-id="17234-104">In [!INCLUDE[prod_short](includes/prod_short.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="17234-105">Method</span><span class="sxs-lookup"><span data-stu-id="17234-105">Method</span></span>|<span data-ttu-id="17234-106">Inbound process</span><span class="sxs-lookup"><span data-stu-id="17234-106">Inbound process</span></span>|<span data-ttu-id="17234-107">Bins</span><span class="sxs-lookup"><span data-stu-id="17234-107">Bins</span></span>|<span data-ttu-id="17234-108">Receipts</span><span class="sxs-lookup"><span data-stu-id="17234-108">Receipts</span></span>|<span data-ttu-id="17234-109">Put-aways</span><span class="sxs-lookup"><span data-stu-id="17234-109">Put-aways</span></span>|<span data-ttu-id="17234-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="17234-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="17234-111">A</span><span class="sxs-lookup"><span data-stu-id="17234-111">A</span></span>|<span data-ttu-id="17234-112">Post receipt and put-away from the order line</span><span class="sxs-lookup"><span data-stu-id="17234-112">Post receipt and put-away from the order line</span></span>|<span data-ttu-id="17234-113">X</span><span class="sxs-lookup"><span data-stu-id="17234-113">X</span></span>|||<span data-ttu-id="17234-114">2</span><span class="sxs-lookup"><span data-stu-id="17234-114">2</span></span>|  
|<span data-ttu-id="17234-115">B</span><span class="sxs-lookup"><span data-stu-id="17234-115">B</span></span>|<span data-ttu-id="17234-116">Post receipt and put-away from an inventory put-away document</span><span class="sxs-lookup"><span data-stu-id="17234-116">Post receipt and put-away from an inventory put-away document</span></span>|||<span data-ttu-id="17234-117">X</span><span class="sxs-lookup"><span data-stu-id="17234-117">X</span></span>|<span data-ttu-id="17234-118">3</span><span class="sxs-lookup"><span data-stu-id="17234-118">3</span></span>|  
|<span data-ttu-id="17234-119">C</span><span class="sxs-lookup"><span data-stu-id="17234-119">C</span></span>|<span data-ttu-id="17234-120">Post receipt and put-away from a warehouse receipt document</span><span class="sxs-lookup"><span data-stu-id="17234-120">Post receipt and put-away from a warehouse receipt document</span></span>||<span data-ttu-id="17234-121">X</span><span class="sxs-lookup"><span data-stu-id="17234-121">X</span></span>||<span data-ttu-id="17234-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="17234-122">4/5/6</span></span>|  
|<span data-ttu-id="17234-123">D</span><span class="sxs-lookup"><span data-stu-id="17234-123">D</span></span>|<span data-ttu-id="17234-124">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span><span class="sxs-lookup"><span data-stu-id="17234-124">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span></span>||<span data-ttu-id="17234-125">X</span><span class="sxs-lookup"><span data-stu-id="17234-125">X</span></span>|<span data-ttu-id="17234-126">X</span><span class="sxs-lookup"><span data-stu-id="17234-126">X</span></span>|<span data-ttu-id="17234-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="17234-127">4/5/6</span></span>|  

<span data-ttu-id="17234-128">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="17234-128">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="17234-129">The following walkthrough demonstrates method B in the previous table.</span><span class="sxs-lookup"><span data-stu-id="17234-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="17234-130">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="17234-130">About This Walkthrough</span></span>  
<span data-ttu-id="17234-131">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** page to record and post put-away and receipt information for your inbound source documents.</span><span class="sxs-lookup"><span data-stu-id="17234-131">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** page to record and post put-away and receipt information for your inbound source documents.</span></span> <span data-ttu-id="17234-132">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span><span class="sxs-lookup"><span data-stu-id="17234-132">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span></span>

> [!NOTE]
> <span data-ttu-id="17234-133">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span><span class="sxs-lookup"><span data-stu-id="17234-133">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span></span>  

<span data-ttu-id="17234-134">This walkthrough demonstrates the following tasks.</span><span class="sxs-lookup"><span data-stu-id="17234-134">This walkthrough demonstrates the following tasks.</span></span>  

-   <span data-ttu-id="17234-135">Setting up SILVER location for inventory put aways.</span><span class="sxs-lookup"><span data-stu-id="17234-135">Setting up SILVER location for inventory put aways.</span></span>  
-   <span data-ttu-id="17234-136">Setting up SILVER location for bin handling.</span><span class="sxs-lookup"><span data-stu-id="17234-136">Setting up SILVER location for bin handling.</span></span>  
-   <span data-ttu-id="17234-137">Defining a default bin for item LS-81.</span><span class="sxs-lookup"><span data-stu-id="17234-137">Defining a default bin for item LS-81.</span></span> <span data-ttu-id="17234-138">(LS-75 is already set up in CRONUS.)</span><span class="sxs-lookup"><span data-stu-id="17234-138">(LS-75 is already set up in CRONUS.)</span></span>  
-   <span data-ttu-id="17234-139">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span><span class="sxs-lookup"><span data-stu-id="17234-139">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span></span>  
-   <span data-ttu-id="17234-140">Verifying that the put-away bins are preset by setup.</span><span class="sxs-lookup"><span data-stu-id="17234-140">Verifying that the put-away bins are preset by setup.</span></span>  
-   <span data-ttu-id="17234-141">Releasing the purchase order for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="17234-141">Releasing the purchase order for warehouse handling.</span></span>  
-   <span data-ttu-id="17234-142">Creating an inventory put-away based on a released source document.</span><span class="sxs-lookup"><span data-stu-id="17234-142">Creating an inventory put-away based on a released source document.</span></span>  
-   <span data-ttu-id="17234-143">Verifying that the put-away bins are inherited from the purchase order.</span><span class="sxs-lookup"><span data-stu-id="17234-143">Verifying that the put-away bins are inherited from the purchase order.</span></span>  
-   <span data-ttu-id="17234-144">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span><span class="sxs-lookup"><span data-stu-id="17234-144">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span></span>  

> [!NOTE]
> [!INCLUDE [locations-cronus](includes/locations-cronus.md)]

## <a name="roles"></a><span data-ttu-id="17234-145">Roles</span><span class="sxs-lookup"><span data-stu-id="17234-145">Roles</span></span>  
<span data-ttu-id="17234-146">This walkthrough demonstrates tasks that are performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="17234-146">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

-   <span data-ttu-id="17234-147">Warehouse Manager</span><span class="sxs-lookup"><span data-stu-id="17234-147">Warehouse Manager</span></span>  
-   <span data-ttu-id="17234-148">Purchasing Agent</span><span class="sxs-lookup"><span data-stu-id="17234-148">Purchasing Agent</span></span>  
-   <span data-ttu-id="17234-149">Warehouse Worker</span><span class="sxs-lookup"><span data-stu-id="17234-149">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="17234-150">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="17234-150">Prerequisites</span></span>  
<span data-ttu-id="17234-151">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="17234-151">To complete this walkthrough, you will need:</span></span>  

-   <span data-ttu-id="17234-152">CRONUS International Ltd. installed.</span><span class="sxs-lookup"><span data-stu-id="17234-152">CRONUS International Ltd. installed.</span></span>  
-   <span data-ttu-id="17234-153">To make yourself a warehouse employee at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="17234-153">To make yourself a warehouse employee at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="17234-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="17234-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="17234-155">Choose the **User ID** field, and select your own user account on the **Users** page.</span><span class="sxs-lookup"><span data-stu-id="17234-155">Choose the **User ID** field, and select your own user account on the **Users** page.</span></span>  
    3.  <span data-ttu-id="17234-156">In the **Location Code** field, enter SILVER.</span><span class="sxs-lookup"><span data-stu-id="17234-156">In the **Location Code** field, enter SILVER.</span></span>  
    4.  <span data-ttu-id="17234-157">Select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="17234-157">Select the **Default** field.</span></span>  

## <a name="story"></a><span data-ttu-id="17234-158">Story</span><span class="sxs-lookup"><span data-stu-id="17234-158">Story</span></span>  
<span data-ttu-id="17234-159">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span><span class="sxs-lookup"><span data-stu-id="17234-159">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span></span> <span data-ttu-id="17234-160">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span><span class="sxs-lookup"><span data-stu-id="17234-160">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span></span> <span data-ttu-id="17234-161">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span><span class="sxs-lookup"><span data-stu-id="17234-161">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="17234-162">Setting up the Location</span><span class="sxs-lookup"><span data-stu-id="17234-162">Setting up the Location</span></span>  
 <span data-ttu-id="17234-163">The setup of the **Location Card** page defines the company's warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="17234-163">The setup of the **Location Card** page defines the company's warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="17234-164">To set up the location</span><span class="sxs-lookup"><span data-stu-id="17234-164">To set up the location</span></span>  

1.  <span data-ttu-id="17234-165">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="17234-165">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="17234-166">Open the SILVER location card.</span><span class="sxs-lookup"><span data-stu-id="17234-166">Open the SILVER location card.</span></span>  
3.  <span data-ttu-id="17234-167">Select the **Require Put-away** check box.</span><span class="sxs-lookup"><span data-stu-id="17234-167">Select the **Require Put-away** check box.</span></span>  

    <span data-ttu-id="17234-168">Proceed to set up a default bin for the two item numbers to control where they are put away.</span><span class="sxs-lookup"><span data-stu-id="17234-168">Proceed to set up a default bin for the two item numbers to control where they are put away.</span></span>  

4.  <span data-ttu-id="17234-169">Choose the **Bins** action.</span><span class="sxs-lookup"><span data-stu-id="17234-169">Choose the **Bins** action.</span></span>  
5.  <span data-ttu-id="17234-170">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span><span class="sxs-lookup"><span data-stu-id="17234-170">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span></span>  

    <span data-ttu-id="17234-171">Notice on the **Bin Content** page that item LS-75 is already set up as content in bin S-01-0001.</span><span class="sxs-lookup"><span data-stu-id="17234-171">Notice on the **Bin Content** page that item LS-75 is already set up as content in bin S-01-0001.</span></span>  

6.  <span data-ttu-id="17234-172">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="17234-172">Choose the **New** action.</span></span>  
7.  <span data-ttu-id="17234-173">Select the **Fixed** and the **Default** fields.</span><span class="sxs-lookup"><span data-stu-id="17234-173">Select the **Fixed** and the **Default** fields.</span></span>  
8.  <span data-ttu-id="17234-174">In the **Item No.** field, enter LS-81.</span><span class="sxs-lookup"><span data-stu-id="17234-174">In the **Item No.** field, enter LS-81.</span></span>  

## <a name="creating-the-purchase-order"></a><span data-ttu-id="17234-175">Creating the Purchase Order</span><span class="sxs-lookup"><span data-stu-id="17234-175">Creating the Purchase Order</span></span>  
<span data-ttu-id="17234-176">Purchase orders are the most common type of inbound source document.</span><span class="sxs-lookup"><span data-stu-id="17234-176">Purchase orders are the most common type of inbound source document.</span></span>  

### <a name="to-create-the-purchase-order"></a><span data-ttu-id="17234-177">To create the purchase order</span><span class="sxs-lookup"><span data-stu-id="17234-177">To create the purchase order</span></span>  

1.  <span data-ttu-id="17234-178">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="17234-178">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="17234-179">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="17234-179">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="17234-180">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span><span class="sxs-lookup"><span data-stu-id="17234-180">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span></span>  

    |<span data-ttu-id="17234-181">Item</span><span class="sxs-lookup"><span data-stu-id="17234-181">Item</span></span>|<span data-ttu-id="17234-182">Location code</span><span class="sxs-lookup"><span data-stu-id="17234-182">Location code</span></span>|<span data-ttu-id="17234-183">Bin code</span><span class="sxs-lookup"><span data-stu-id="17234-183">Bin code</span></span>|<span data-ttu-id="17234-184">Quantity</span><span class="sxs-lookup"><span data-stu-id="17234-184">Quantity</span></span>|  
    |----------|-------------------|--------------|--------------|  
    |<span data-ttu-id="17234-185">LS_75</span><span class="sxs-lookup"><span data-stu-id="17234-185">LS_75</span></span>|<span data-ttu-id="17234-186">SILVER</span><span class="sxs-lookup"><span data-stu-id="17234-186">SILVER</span></span>|<span data-ttu-id="17234-187">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="17234-187">S-01-0001</span></span>|<span data-ttu-id="17234-188">10</span><span class="sxs-lookup"><span data-stu-id="17234-188">10</span></span>|  
    |<span data-ttu-id="17234-189">LS-81</span><span class="sxs-lookup"><span data-stu-id="17234-189">LS-81</span></span>|<span data-ttu-id="17234-190">SILVER</span><span class="sxs-lookup"><span data-stu-id="17234-190">SILVER</span></span>|<span data-ttu-id="17234-191">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="17234-191">S-01-0001</span></span>|<span data-ttu-id="17234-192">30</span><span class="sxs-lookup"><span data-stu-id="17234-192">30</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="17234-193">The bin code is entered automatically according to the setup that you performed in the "Setting up the Location" section.</span><span class="sxs-lookup"><span data-stu-id="17234-193">The bin code is entered automatically according to the setup that you performed in the "Setting up the Location" section.</span></span>  

    <span data-ttu-id="17234-194">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span><span class="sxs-lookup"><span data-stu-id="17234-194">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span></span>  

4.  <span data-ttu-id="17234-195">Choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="17234-195">Choose the **Release** action.</span></span>  

    <span data-ttu-id="17234-196">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span><span class="sxs-lookup"><span data-stu-id="17234-196">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span></span>  

## <a name="receiving-and-putting-the-items-away"></a><span data-ttu-id="17234-197">Receiving and Putting the Items Away</span><span class="sxs-lookup"><span data-stu-id="17234-197">Receiving and Putting the Items Away</span></span>  
<span data-ttu-id="17234-198">On the **Inventory Put-away** page, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span><span class="sxs-lookup"><span data-stu-id="17234-198">On the **Inventory Put-away** page, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span></span>  

### <a name="to-receive-and-put-the-items-away"></a><span data-ttu-id="17234-199">To receive and put the items away</span><span class="sxs-lookup"><span data-stu-id="17234-199">To receive and put the items away</span></span>  

1.  <span data-ttu-id="17234-200">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Put-aways**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="17234-200">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Put-aways**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="17234-201">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="17234-201">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="17234-202">Select the **Source Document** field, and then select **Purchase Order**.</span><span class="sxs-lookup"><span data-stu-id="17234-202">Select the **Source Document** field, and then select **Purchase Order**.</span></span>  
4.  <span data-ttu-id="17234-203">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="17234-203">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="17234-204">Alternatively, choose the **Get Source Document** action, and then select the purchase order.</span><span class="sxs-lookup"><span data-stu-id="17234-204">Alternatively, choose the **Get Source Document** action, and then select the purchase order.</span></span>  

5.  <span data-ttu-id="17234-205">Choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="17234-205">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="17234-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span><span class="sxs-lookup"><span data-stu-id="17234-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span></span>  

6.  <span data-ttu-id="17234-207">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="17234-207">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="17234-208">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span><span class="sxs-lookup"><span data-stu-id="17234-208">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span></span>  

## <a name="see-also"></a><span data-ttu-id="17234-209">See Also</span><span class="sxs-lookup"><span data-stu-id="17234-209">See Also</span></span>  
 <span data-ttu-id="17234-210">[Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span><span class="sxs-lookup"><span data-stu-id="17234-210">[Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span></span>  
 <span data-ttu-id="17234-211">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span><span class="sxs-lookup"><span data-stu-id="17234-211">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span></span>  
 <span data-ttu-id="17234-212">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="17234-212">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="17234-213">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span><span class="sxs-lookup"><span data-stu-id="17234-213">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span></span>  
 <span data-ttu-id="17234-214">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="17234-214">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="17234-215">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span><span class="sxs-lookup"><span data-stu-id="17234-215">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span></span>  
 [<span data-ttu-id="17234-216">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="17234-216">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="17234-217">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="17234-217">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]