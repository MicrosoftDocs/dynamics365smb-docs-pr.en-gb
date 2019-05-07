---
title: Walkthrough - Receiving and Putting Away in Basic Warehouse Configurations | Microsoft Docs
description: In Business Central, the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 1738e60fe78b0ef9e11b277bb19f4e8f830ec882
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "922045"
---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a><span data-ttu-id="9beab-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="9beab-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span></span>

<span data-ttu-id="9beab-104">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="9beab-104">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span></span> <span data-ttu-id="9beab-105">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span><span class="sxs-lookup"><span data-stu-id="9beab-105">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span></span>

<span data-ttu-id="9beab-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span><span class="sxs-lookup"><span data-stu-id="9beab-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="9beab-107">Method</span><span class="sxs-lookup"><span data-stu-id="9beab-107">Method</span></span>|<span data-ttu-id="9beab-108">Inbound process</span><span class="sxs-lookup"><span data-stu-id="9beab-108">Inbound process</span></span>|<span data-ttu-id="9beab-109">Bins</span><span class="sxs-lookup"><span data-stu-id="9beab-109">Bins</span></span>|<span data-ttu-id="9beab-110">Receipts</span><span class="sxs-lookup"><span data-stu-id="9beab-110">Receipts</span></span>|<span data-ttu-id="9beab-111">Put-aways</span><span class="sxs-lookup"><span data-stu-id="9beab-111">Put-aways</span></span>|<span data-ttu-id="9beab-112">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="9beab-112">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="9beab-113">A</span><span class="sxs-lookup"><span data-stu-id="9beab-113">A</span></span>|<span data-ttu-id="9beab-114">Post receipt and put-away from the order line</span><span class="sxs-lookup"><span data-stu-id="9beab-114">Post receipt and put-away from the order line</span></span>|<span data-ttu-id="9beab-115">X</span><span class="sxs-lookup"><span data-stu-id="9beab-115">X</span></span>|||<span data-ttu-id="9beab-116">2</span><span class="sxs-lookup"><span data-stu-id="9beab-116">2</span></span>|  
|<span data-ttu-id="9beab-117">B</span><span class="sxs-lookup"><span data-stu-id="9beab-117">B</span></span>|<span data-ttu-id="9beab-118">Post receipt and put-away from an inventory put-away document</span><span class="sxs-lookup"><span data-stu-id="9beab-118">Post receipt and put-away from an inventory put-away document</span></span>|||<span data-ttu-id="9beab-119">X</span><span class="sxs-lookup"><span data-stu-id="9beab-119">X</span></span>|<span data-ttu-id="9beab-120">3</span><span class="sxs-lookup"><span data-stu-id="9beab-120">3</span></span>|  
|<span data-ttu-id="9beab-121">C</span><span class="sxs-lookup"><span data-stu-id="9beab-121">C</span></span>|<span data-ttu-id="9beab-122">Post receipt and put-away from a warehouse receipt document</span><span class="sxs-lookup"><span data-stu-id="9beab-122">Post receipt and put-away from a warehouse receipt document</span></span>||<span data-ttu-id="9beab-123">X</span><span class="sxs-lookup"><span data-stu-id="9beab-123">X</span></span>||<span data-ttu-id="9beab-124">4/5/6</span><span class="sxs-lookup"><span data-stu-id="9beab-124">4/5/6</span></span>|  
|<span data-ttu-id="9beab-125">D</span><span class="sxs-lookup"><span data-stu-id="9beab-125">D</span></span>|<span data-ttu-id="9beab-126">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span><span class="sxs-lookup"><span data-stu-id="9beab-126">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span></span>||<span data-ttu-id="9beab-127">X</span><span class="sxs-lookup"><span data-stu-id="9beab-127">X</span></span>|<span data-ttu-id="9beab-128">X</span><span class="sxs-lookup"><span data-stu-id="9beab-128">X</span></span>|<span data-ttu-id="9beab-129">4/5/6</span><span class="sxs-lookup"><span data-stu-id="9beab-129">4/5/6</span></span>|  

<span data-ttu-id="9beab-130">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="9beab-130">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="9beab-131">The following walkthrough demonstrates method B in the previous table.</span><span class="sxs-lookup"><span data-stu-id="9beab-131">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="9beab-132">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="9beab-132">About This Walkthrough</span></span>  
<span data-ttu-id="9beab-133">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** page to record and post put-away and receipt information for your inbound source documents.</span><span class="sxs-lookup"><span data-stu-id="9beab-133">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** page to record and post put-away and receipt information for your inbound source documents.</span></span> <span data-ttu-id="9beab-134">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span><span class="sxs-lookup"><span data-stu-id="9beab-134">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span></span>

> [!NOTE]
> <span data-ttu-id="9beab-135">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span><span class="sxs-lookup"><span data-stu-id="9beab-135">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span></span>  

<span data-ttu-id="9beab-136">This walkthrough demonstrates the following tasks.</span><span class="sxs-lookup"><span data-stu-id="9beab-136">This walkthrough demonstrates the following tasks.</span></span>  

-   <span data-ttu-id="9beab-137">Setting up SILVER location for inventory put aways.</span><span class="sxs-lookup"><span data-stu-id="9beab-137">Setting up SILVER location for inventory put aways.</span></span>  
-   <span data-ttu-id="9beab-138">Setting up SILVER location for bin handling.</span><span class="sxs-lookup"><span data-stu-id="9beab-138">Setting up SILVER location for bin handling.</span></span>  
-   <span data-ttu-id="9beab-139">Defining a default bin for item LS-81.</span><span class="sxs-lookup"><span data-stu-id="9beab-139">Defining a default bin for item LS-81.</span></span> <span data-ttu-id="9beab-140">(LS-75 is already set up in CRONUS.)</span><span class="sxs-lookup"><span data-stu-id="9beab-140">(LS-75 is already set up in CRONUS.)</span></span>  
-   <span data-ttu-id="9beab-141">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span><span class="sxs-lookup"><span data-stu-id="9beab-141">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span></span>  
-   <span data-ttu-id="9beab-142">Verifying that the put-away bins are preset by setup.</span><span class="sxs-lookup"><span data-stu-id="9beab-142">Verifying that the put-away bins are preset by setup.</span></span>  
-   <span data-ttu-id="9beab-143">Releasing the purchase order for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="9beab-143">Releasing the purchase order for warehouse handling.</span></span>  
-   <span data-ttu-id="9beab-144">Creating an inventory put-away based on a released source document.</span><span class="sxs-lookup"><span data-stu-id="9beab-144">Creating an inventory put-away based on a released source document.</span></span>  
-   <span data-ttu-id="9beab-145">Verifying that the put-away bins are inherited from the purchase order.</span><span class="sxs-lookup"><span data-stu-id="9beab-145">Verifying that the put-away bins are inherited from the purchase order.</span></span>  
-   <span data-ttu-id="9beab-146">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span><span class="sxs-lookup"><span data-stu-id="9beab-146">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span></span>  

## <a name="roles"></a><span data-ttu-id="9beab-147">Roles</span><span class="sxs-lookup"><span data-stu-id="9beab-147">Roles</span></span>  
<span data-ttu-id="9beab-148">This walkthrough demonstrates tasks that are performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="9beab-148">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

-   <span data-ttu-id="9beab-149">Warehouse Manager</span><span class="sxs-lookup"><span data-stu-id="9beab-149">Warehouse Manager</span></span>  
-   <span data-ttu-id="9beab-150">Purchasing Agent</span><span class="sxs-lookup"><span data-stu-id="9beab-150">Purchasing Agent</span></span>  
-   <span data-ttu-id="9beab-151">Warehouse Worker</span><span class="sxs-lookup"><span data-stu-id="9beab-151">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="9beab-152">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="9beab-152">Prerequisites</span></span>  
<span data-ttu-id="9beab-153">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="9beab-153">To complete this walkthrough, you will need:</span></span>  

-   <span data-ttu-id="9beab-154">CRONUS International Ltd. installed.</span><span class="sxs-lookup"><span data-stu-id="9beab-154">CRONUS International Ltd. installed.</span></span>  
-   <span data-ttu-id="9beab-155">To make yourself a warehouse employee at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="9beab-155">To make yourself a warehouse employee at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="9beab-156">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9beab-156">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="9beab-157">Choose the **User ID** field, and select your own user account on the **Users** page.</span><span class="sxs-lookup"><span data-stu-id="9beab-157">Choose the **User ID** field, and select your own user account on the **Users** page.</span></span>  
    3.  <span data-ttu-id="9beab-158">In the **Location Code** field, enter SILVER.</span><span class="sxs-lookup"><span data-stu-id="9beab-158">In the **Location Code** field, enter SILVER.</span></span>  
    4.  <span data-ttu-id="9beab-159">Select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="9beab-159">Select the **Default** field.</span></span>  

## <a name="story"></a><span data-ttu-id="9beab-160">Story</span><span class="sxs-lookup"><span data-stu-id="9beab-160">Story</span></span>  
<span data-ttu-id="9beab-161">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span><span class="sxs-lookup"><span data-stu-id="9beab-161">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span></span> <span data-ttu-id="9beab-162">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span><span class="sxs-lookup"><span data-stu-id="9beab-162">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span></span> <span data-ttu-id="9beab-163">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span><span class="sxs-lookup"><span data-stu-id="9beab-163">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="9beab-164">Setting up the Location</span><span class="sxs-lookup"><span data-stu-id="9beab-164">Setting up the Location</span></span>  
 <span data-ttu-id="9beab-165">The setup of the **Location Card** page defines the company’s warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="9beab-165">The setup of the **Location Card** page defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="9beab-166">To set up the location</span><span class="sxs-lookup"><span data-stu-id="9beab-166">To set up the location</span></span>  

1.  <span data-ttu-id="9beab-167">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9beab-167">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9beab-168">Open the SILVER location card.</span><span class="sxs-lookup"><span data-stu-id="9beab-168">Open the SILVER location card.</span></span>  
3.  <span data-ttu-id="9beab-169">Select the **Require Put-away** check box.</span><span class="sxs-lookup"><span data-stu-id="9beab-169">Select the **Require Put-away** check box.</span></span>  

    <span data-ttu-id="9beab-170">Proceed to set up a default bin for the two item numbers to control where they are put away.</span><span class="sxs-lookup"><span data-stu-id="9beab-170">Proceed to set up a default bin for the two item numbers to control where they are put away.</span></span>  

4.  <span data-ttu-id="9beab-171">Choose the **Bins** action.</span><span class="sxs-lookup"><span data-stu-id="9beab-171">Choose the **Bins** action.</span></span>  
5.  <span data-ttu-id="9beab-172">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span><span class="sxs-lookup"><span data-stu-id="9beab-172">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span></span>  

    <span data-ttu-id="9beab-173">Notice on the **Bin Content** page that item LS-75 is already set up as content in bin S-01-0001.</span><span class="sxs-lookup"><span data-stu-id="9beab-173">Notice on the **Bin Content** page that item LS-75 is already set up as content in bin S-01-0001.</span></span>  

6.  <span data-ttu-id="9beab-174">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="9beab-174">Choose the **New** action.</span></span>  
7.  <span data-ttu-id="9beab-175">Select the **Fixed** and the **Default** fields.</span><span class="sxs-lookup"><span data-stu-id="9beab-175">Select the **Fixed** and the **Default** fields.</span></span>  
8.  <span data-ttu-id="9beab-176">In the **Item No.** field, enter LS-81.</span><span class="sxs-lookup"><span data-stu-id="9beab-176">In the **Item No.** field, enter LS-81.</span></span>  

## <a name="creating-the-purchase-order"></a><span data-ttu-id="9beab-177">Creating the Purchase Order</span><span class="sxs-lookup"><span data-stu-id="9beab-177">Creating the Purchase Order</span></span>  
<span data-ttu-id="9beab-178">Purchase orders are the most common type of inbound source document.</span><span class="sxs-lookup"><span data-stu-id="9beab-178">Purchase orders are the most common type of inbound source document.</span></span>  

### <a name="to-create-the-purchase-order"></a><span data-ttu-id="9beab-179">To create the purchase order</span><span class="sxs-lookup"><span data-stu-id="9beab-179">To create the purchase order</span></span>  

1.  <span data-ttu-id="9beab-180">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9beab-180">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9beab-181">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="9beab-181">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="9beab-182">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span><span class="sxs-lookup"><span data-stu-id="9beab-182">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span></span>  

    |<span data-ttu-id="9beab-183">Item</span><span class="sxs-lookup"><span data-stu-id="9beab-183">Item</span></span>|<span data-ttu-id="9beab-184">Location code</span><span class="sxs-lookup"><span data-stu-id="9beab-184">Location code</span></span>|<span data-ttu-id="9beab-185">Bin code</span><span class="sxs-lookup"><span data-stu-id="9beab-185">Bin code</span></span>|<span data-ttu-id="9beab-186">Quantity</span><span class="sxs-lookup"><span data-stu-id="9beab-186">Quantity</span></span>|  
    |----------|-------------------|--------------|--------------|  
    |<span data-ttu-id="9beab-187">LS_75</span><span class="sxs-lookup"><span data-stu-id="9beab-187">LS_75</span></span>|<span data-ttu-id="9beab-188">SILVER</span><span class="sxs-lookup"><span data-stu-id="9beab-188">SILVER</span></span>|<span data-ttu-id="9beab-189">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="9beab-189">S-01-0001</span></span>|<span data-ttu-id="9beab-190">10</span><span class="sxs-lookup"><span data-stu-id="9beab-190">10</span></span>|  
    |<span data-ttu-id="9beab-191">LS-81</span><span class="sxs-lookup"><span data-stu-id="9beab-191">LS-81</span></span>|<span data-ttu-id="9beab-192">SILVER</span><span class="sxs-lookup"><span data-stu-id="9beab-192">SILVER</span></span>|<span data-ttu-id="9beab-193">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="9beab-193">S-01-0001</span></span>|<span data-ttu-id="9beab-194">30</span><span class="sxs-lookup"><span data-stu-id="9beab-194">30</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="9beab-195">The bin code is entered automatically according to the setup that you performed in the “Setting up the Location” section.</span><span class="sxs-lookup"><span data-stu-id="9beab-195">The bin code is entered automatically according to the setup that you performed in the “Setting up the Location” section.</span></span>  

    <span data-ttu-id="9beab-196">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span><span class="sxs-lookup"><span data-stu-id="9beab-196">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span></span>  

4.  <span data-ttu-id="9beab-197">Choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="9beab-197">Choose the **Release** action.</span></span>  

    <span data-ttu-id="9beab-198">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span><span class="sxs-lookup"><span data-stu-id="9beab-198">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span></span>  

## <a name="receiving-and-putting-the-items-away"></a><span data-ttu-id="9beab-199">Receiving and Putting the Items Away</span><span class="sxs-lookup"><span data-stu-id="9beab-199">Receiving and Putting the Items Away</span></span>  
<span data-ttu-id="9beab-200">On the **Inventory Put-away** page, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span><span class="sxs-lookup"><span data-stu-id="9beab-200">On the **Inventory Put-away** page, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span></span>  

### <a name="to-receive-and-put-the-items-away"></a><span data-ttu-id="9beab-201">To receive and put the items away</span><span class="sxs-lookup"><span data-stu-id="9beab-201">To receive and put the items away</span></span>  

1.  <span data-ttu-id="9beab-202">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Put-aways**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9beab-202">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Put-aways**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9beab-203">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="9beab-203">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="9beab-204">Select the **Source Document** field, and then select **Purchase Order**.</span><span class="sxs-lookup"><span data-stu-id="9beab-204">Select the **Source Document** field, and then select **Purchase Order**.</span></span>  
4.  <span data-ttu-id="9beab-205">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9beab-205">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="9beab-206">Alternatively, on the **Actions** tab, in the **Functions** group, choose **Get Source Document**, and then select the purchase order.</span><span class="sxs-lookup"><span data-stu-id="9beab-206">Alternatively, on the **Actions** tab, in the **Functions** group, choose **Get Source Document**, and then select the purchase order.</span></span>  

5.  <span data-ttu-id="9beab-207">Choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="9beab-207">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="9beab-208">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span><span class="sxs-lookup"><span data-stu-id="9beab-208">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span></span>  

6.  <span data-ttu-id="9beab-209">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9beab-209">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="9beab-210">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span><span class="sxs-lookup"><span data-stu-id="9beab-210">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9beab-211">See Also</span><span class="sxs-lookup"><span data-stu-id="9beab-211">See Also</span></span>  
 <span data-ttu-id="9beab-212">[Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span><span class="sxs-lookup"><span data-stu-id="9beab-212">[Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span></span>  
 <span data-ttu-id="9beab-213">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span><span class="sxs-lookup"><span data-stu-id="9beab-213">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span></span>  
 <span data-ttu-id="9beab-214">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="9beab-214">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="9beab-215">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span><span class="sxs-lookup"><span data-stu-id="9beab-215">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span></span>  
 <span data-ttu-id="9beab-216">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="9beab-216">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="9beab-217">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span><span class="sxs-lookup"><span data-stu-id="9beab-217">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span></span>  
 [<span data-ttu-id="9beab-218">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="9beab-218">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="9beab-219">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9beab-219">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
