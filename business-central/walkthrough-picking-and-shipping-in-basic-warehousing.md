---
title: Picking and Shipping in Basic Warehouse Configurations | Microsoft Docs
description: In Business Central, the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/24/2020
ms.author: sgroespe
ms.openlocfilehash: 475f32dbaf9b4b80a61e1cad542fbf6db79cb029
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/01/2020
ms.locfileid: "3528317"
---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a><span data-ttu-id="fbfaa-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="fbfaa-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span></span>

[!INCLUDE[complete_sample_data](includes/complete_sample_data.md)]

<span data-ttu-id="fbfaa-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="fbfaa-105">Method</span><span class="sxs-lookup"><span data-stu-id="fbfaa-105">Method</span></span>|<span data-ttu-id="fbfaa-106">Inbound process</span><span class="sxs-lookup"><span data-stu-id="fbfaa-106">Inbound process</span></span>|<span data-ttu-id="fbfaa-107">Bins</span><span class="sxs-lookup"><span data-stu-id="fbfaa-107">Bins</span></span>|<span data-ttu-id="fbfaa-108">Picks</span><span class="sxs-lookup"><span data-stu-id="fbfaa-108">Picks</span></span>|<span data-ttu-id="fbfaa-109">Shipments</span><span class="sxs-lookup"><span data-stu-id="fbfaa-109">Shipments</span></span>|<span data-ttu-id="fbfaa-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="fbfaa-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="fbfaa-111">A</span><span class="sxs-lookup"><span data-stu-id="fbfaa-111">A</span></span>|<span data-ttu-id="fbfaa-112">Post pick and shipment from the order line</span><span class="sxs-lookup"><span data-stu-id="fbfaa-112">Post pick and shipment from the order line</span></span>|<span data-ttu-id="fbfaa-113">X</span><span class="sxs-lookup"><span data-stu-id="fbfaa-113">X</span></span>|||<span data-ttu-id="fbfaa-114">2</span><span class="sxs-lookup"><span data-stu-id="fbfaa-114">2</span></span>|  
|<span data-ttu-id="fbfaa-115">B</span><span class="sxs-lookup"><span data-stu-id="fbfaa-115">B</span></span>|<span data-ttu-id="fbfaa-116">Post pick and shipment from an inventory pick document</span><span class="sxs-lookup"><span data-stu-id="fbfaa-116">Post pick and shipment from an inventory pick document</span></span>||<span data-ttu-id="fbfaa-117">X</span><span class="sxs-lookup"><span data-stu-id="fbfaa-117">X</span></span>||<span data-ttu-id="fbfaa-118">3</span><span class="sxs-lookup"><span data-stu-id="fbfaa-118">3</span></span>|  
|<span data-ttu-id="fbfaa-119">C</span><span class="sxs-lookup"><span data-stu-id="fbfaa-119">C</span></span>|<span data-ttu-id="fbfaa-120">Post pick and shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="fbfaa-120">Post pick and shipment from a warehouse shipment document</span></span>|||<span data-ttu-id="fbfaa-121">X</span><span class="sxs-lookup"><span data-stu-id="fbfaa-121">X</span></span>|<span data-ttu-id="fbfaa-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="fbfaa-122">4/5/6</span></span>|  
|<span data-ttu-id="fbfaa-123">D</span><span class="sxs-lookup"><span data-stu-id="fbfaa-123">D</span></span>|<span data-ttu-id="fbfaa-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="fbfaa-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span></span>||<span data-ttu-id="fbfaa-125">X</span><span class="sxs-lookup"><span data-stu-id="fbfaa-125">X</span></span>|<span data-ttu-id="fbfaa-126">X</span><span class="sxs-lookup"><span data-stu-id="fbfaa-126">X</span></span>|<span data-ttu-id="fbfaa-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="fbfaa-127">4/5/6</span></span>|  

<span data-ttu-id="fbfaa-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="fbfaa-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="fbfaa-129">The following walkthrough demonstrates method B in the previous table.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="fbfaa-130">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="fbfaa-130">About This Walkthrough</span></span>

<span data-ttu-id="fbfaa-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span></span> <span data-ttu-id="fbfaa-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span></span>  

<span data-ttu-id="fbfaa-133">This walkthrough demonstrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="fbfaa-133">This walkthrough demonstrates the following tasks:</span></span>  

- <span data-ttu-id="fbfaa-134">Setting up SILVER location for inventory picks.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-134">Setting up SILVER location for inventory picks.</span></span>  
- <span data-ttu-id="fbfaa-135">Creating a sales order for customer 10000 for 30 loudspeakers.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-135">Creating a sales order for customer 10000 for 30 loudspeakers.</span></span>  
- <span data-ttu-id="fbfaa-136">Releasing the sales order for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-136">Releasing the sales order for warehouse handling.</span></span>  
- <span data-ttu-id="fbfaa-137">Creating an inventory pick based on a released source document.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-137">Creating an inventory pick based on a released source document.</span></span>  
- <span data-ttu-id="fbfaa-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span></span>  

## <a name="roles"></a><span data-ttu-id="fbfaa-139">Roles</span><span class="sxs-lookup"><span data-stu-id="fbfaa-139">Roles</span></span>

<span data-ttu-id="fbfaa-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="fbfaa-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

- <span data-ttu-id="fbfaa-141">Warehouse Manager</span><span class="sxs-lookup"><span data-stu-id="fbfaa-141">Warehouse Manager</span></span>  
- <span data-ttu-id="fbfaa-142">Order Processor</span><span class="sxs-lookup"><span data-stu-id="fbfaa-142">Order Processor</span></span>  
- <span data-ttu-id="fbfaa-143">Warehouse Worker</span><span class="sxs-lookup"><span data-stu-id="fbfaa-143">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="fbfaa-144">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="fbfaa-144">Prerequisites</span></span>

<span data-ttu-id="fbfaa-145">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="fbfaa-145">To complete this walkthrough, you will need:</span></span>  

- <span data-ttu-id="fbfaa-146">For [!INCLUDE[prodshort](includes/prodshort.md)] online, a company based on the **Advanced Evaluation - Complete Sample Data** option in a sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-146">For [!INCLUDE[prodshort](includes/prodshort.md)] online, a company based on the **Advanced Evaluation - Complete Sample Data** option in a sandbox environment.</span></span> <span data-ttu-id="fbfaa-147">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, CRONUS International Ltd. installed.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-147">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, CRONUS International Ltd. installed.</span></span>  
- <span data-ttu-id="fbfaa-148">To make yourself a warehouse employee at the location SILVER by following these steps:</span><span class="sxs-lookup"><span data-stu-id="fbfaa-148">To make yourself a warehouse employee at the location SILVER by following these steps:</span></span>  

  1. <span data-ttu-id="fbfaa-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="fbfaa-150">Choose the **User ID** field, and select your own user account on the **Users** page.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-150">Choose the **User ID** field, and select your own user account on the **Users** page.</span></span>  
  3. <span data-ttu-id="fbfaa-151">In the **Location Code** field, enter SILVER.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-151">In the **Location Code** field, enter SILVER.</span></span>  
  4. <span data-ttu-id="fbfaa-152">Select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-152">Select the **Default** field.</span></span>  

- <span data-ttu-id="fbfaa-153">Make item LS-81 available at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="fbfaa-153">Make item LS-81 available at SILVER location by following these steps:</span></span>  

  1. <span data-ttu-id="fbfaa-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="fbfaa-155">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span><span class="sxs-lookup"><span data-stu-id="fbfaa-155">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span></span>  

        |<span data-ttu-id="fbfaa-156">Entry Type</span><span class="sxs-lookup"><span data-stu-id="fbfaa-156">Entry Type</span></span>|<span data-ttu-id="fbfaa-157">Item Number</span><span class="sxs-lookup"><span data-stu-id="fbfaa-157">Item Number</span></span>|<span data-ttu-id="fbfaa-158">Location Code</span><span class="sxs-lookup"><span data-stu-id="fbfaa-158">Location Code</span></span>|<span data-ttu-id="fbfaa-159">Bin Code</span><span class="sxs-lookup"><span data-stu-id="fbfaa-159">Bin Code</span></span>|<span data-ttu-id="fbfaa-160">Quantity</span><span class="sxs-lookup"><span data-stu-id="fbfaa-160">Quantity</span></span>|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |<span data-ttu-id="fbfaa-161">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-161">Positive Adjmt.</span></span>|<span data-ttu-id="fbfaa-162">LS-81</span><span class="sxs-lookup"><span data-stu-id="fbfaa-162">LS-81</span></span>|<span data-ttu-id="fbfaa-163">SILVER</span><span class="sxs-lookup"><span data-stu-id="fbfaa-163">SILVER</span></span>|<span data-ttu-id="fbfaa-164">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="fbfaa-164">S-01-0001</span></span>|<span data-ttu-id="fbfaa-165">20</span><span class="sxs-lookup"><span data-stu-id="fbfaa-165">20</span></span>|  
        |<span data-ttu-id="fbfaa-166">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-166">Positive Adjmt.</span></span>|<span data-ttu-id="fbfaa-167">LS-81</span><span class="sxs-lookup"><span data-stu-id="fbfaa-167">LS-81</span></span>|<span data-ttu-id="fbfaa-168">SILVER</span><span class="sxs-lookup"><span data-stu-id="fbfaa-168">SILVER</span></span>|<span data-ttu-id="fbfaa-169">S-01-0002</span><span class="sxs-lookup"><span data-stu-id="fbfaa-169">S-01-0002</span></span>|<span data-ttu-id="fbfaa-170">20</span><span class="sxs-lookup"><span data-stu-id="fbfaa-170">20</span></span>|  

  3. <span data-ttu-id="fbfaa-171">Choose the **Post** action, and then select the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-171">Choose the **Post** action, and then select the **Yes** button.</span></span>  

## <a name="story"></a><span data-ttu-id="fbfaa-172">Story</span><span class="sxs-lookup"><span data-stu-id="fbfaa-172">Story</span></span>

<span data-ttu-id="fbfaa-173">Ellen, the warehouse manager at CRONUS, sets up SILVER warehouse for basic pick handling where warehouse workers process outbound orders individually.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-173">Ellen, the warehouse manager at CRONUS, sets up SILVER warehouse for basic pick handling where warehouse workers process outbound orders individually.</span></span> <span data-ttu-id="fbfaa-174">Susan, the order processor, creates a sales order for 30 units of item LS-81 to be shipped to customer 10000 from the SILVER Warehouse.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-174">Susan, the order processor, creates a sales order for 30 units of item LS-81 to be shipped to customer 10000 from the SILVER Warehouse.</span></span> <span data-ttu-id="fbfaa-175">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-175">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span></span> <span data-ttu-id="fbfaa-176">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where LS-81 is stored.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-176">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where LS-81 is stored.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="fbfaa-177">Setting Up the Location</span><span class="sxs-lookup"><span data-stu-id="fbfaa-177">Setting Up the Location</span></span>

<span data-ttu-id="fbfaa-178">The setup of the **Location Card** page defines the company’s warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-178">The setup of the **Location Card** page defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="fbfaa-179">To set up the location</span><span class="sxs-lookup"><span data-stu-id="fbfaa-179">To set up the location</span></span>

1. <span data-ttu-id="fbfaa-180">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-180">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fbfaa-181">Open the SILVER location card.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-181">Open the SILVER location card.</span></span>  
3. <span data-ttu-id="fbfaa-182">On the **Warehouse** FastTab, choose the **Require Pick** check box.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-182">On the **Warehouse** FastTab, choose the **Require Pick** check box.</span></span>  

## <a name="creating-the-sales-order"></a><span data-ttu-id="fbfaa-183">Creating the Sales Order</span><span class="sxs-lookup"><span data-stu-id="fbfaa-183">Creating the Sales Order</span></span>

<span data-ttu-id="fbfaa-184">Sales orders are the most common type of outbound source document.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-184">Sales orders are the most common type of outbound source document.</span></span>  

### <a name="to-create-the-sales-order"></a><span data-ttu-id="fbfaa-185">To create the sales order</span><span class="sxs-lookup"><span data-stu-id="fbfaa-185">To create the sales order</span></span>

1. <span data-ttu-id="fbfaa-186">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-186">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fbfaa-187">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-187">Choose the **New** action.</span></span>  
3. <span data-ttu-id="fbfaa-188">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-188">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span></span>  

    |<span data-ttu-id="fbfaa-189">Item</span><span class="sxs-lookup"><span data-stu-id="fbfaa-189">Item</span></span>|<span data-ttu-id="fbfaa-190">Location Code</span><span class="sxs-lookup"><span data-stu-id="fbfaa-190">Location Code</span></span>|<span data-ttu-id="fbfaa-191">Quantity</span><span class="sxs-lookup"><span data-stu-id="fbfaa-191">Quantity</span></span>|  
    |----|-------------|--------|  
    |<span data-ttu-id="fbfaa-192">LS_81</span><span class="sxs-lookup"><span data-stu-id="fbfaa-192">LS_81</span></span>|<span data-ttu-id="fbfaa-193">SILVER</span><span class="sxs-lookup"><span data-stu-id="fbfaa-193">SILVER</span></span>|<span data-ttu-id="fbfaa-194">30</span><span class="sxs-lookup"><span data-stu-id="fbfaa-194">30</span></span>|  

     <span data-ttu-id="fbfaa-195">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-195">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span></span>  

4. <span data-ttu-id="fbfaa-196">Choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-196">Choose the **Release** action.</span></span>  

    <span data-ttu-id="fbfaa-197">John proceeds to pick and ship the sold items.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-197">John proceeds to pick and ship the sold items.</span></span>  

## <a name="picking-and-shipping-items"></a><span data-ttu-id="fbfaa-198">Picking and Shipping Items</span><span class="sxs-lookup"><span data-stu-id="fbfaa-198">Picking and Shipping Items</span></span>

<span data-ttu-id="fbfaa-199">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-199">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span></span> [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

### <a name="to-pick-and-ship-items"></a><span data-ttu-id="fbfaa-200">To pick and ship items</span><span class="sxs-lookup"><span data-stu-id="fbfaa-200">To pick and ship items</span></span>

1. <span data-ttu-id="fbfaa-201">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-201">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fbfaa-202">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-202">Choose the **New** action.</span></span>  

    <span data-ttu-id="fbfaa-203">Make sure that the **No.**</span><span class="sxs-lookup"><span data-stu-id="fbfaa-203">Make sure that the **No.**</span></span> <span data-ttu-id="fbfaa-204">field on the **General** FastTab is filled in.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-204">field on the **General** FastTab is filled in.</span></span>
3. <span data-ttu-id="fbfaa-205">Select the **Source Document** field, and then select **Sales Order**.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-205">Select the **Source Document** field, and then select **Sales Order**.</span></span>  
4. <span data-ttu-id="fbfaa-206">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-206">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="fbfaa-207">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-207">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span></span>  
5. <span data-ttu-id="fbfaa-208">Choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-208">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="fbfaa-209">Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two inventory pick lines.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-209">Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two inventory pick lines.</span></span>  
6. <span data-ttu-id="fbfaa-210">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-210">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="fbfaa-211">The 30 loudspeakers are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span><span class="sxs-lookup"><span data-stu-id="fbfaa-211">The 30 loudspeakers are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fbfaa-212">See Also</span><span class="sxs-lookup"><span data-stu-id="fbfaa-212">See Also</span></span>

[<span data-ttu-id="fbfaa-213">Pick Items with Inventory Picks</span><span class="sxs-lookup"><span data-stu-id="fbfaa-213">Pick Items with Inventory Picks</span></span>](warehouse-how-to-pick-items-with-inventory-picks.md)  
[<span data-ttu-id="fbfaa-214">Pick Items for Warehouse Shipment</span><span class="sxs-lookup"><span data-stu-id="fbfaa-214">Pick Items for Warehouse Shipment</span></span>](warehouse-how-to-pick-items-for-warehouse-shipment.md)  
[<span data-ttu-id="fbfaa-215">Set Up Basic Warehouses with Operations Areas</span><span class="sxs-lookup"><span data-stu-id="fbfaa-215">Set Up Basic Warehouses with Operations Areas</span></span>](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)  
[<span data-ttu-id="fbfaa-216">Move Components to an Operation Area in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="fbfaa-216">Move Components to an Operation Area in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  
[<span data-ttu-id="fbfaa-217">Pick for Production or Assembly</span><span class="sxs-lookup"><span data-stu-id="fbfaa-217">Pick for Production or Assembly</span></span>](warehouse-how-to-pick-for-production.md)  
[<span data-ttu-id="fbfaa-218">Move Items Ad Hoc in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="fbfaa-218">Move Items Ad Hoc in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)  
[<span data-ttu-id="fbfaa-219">Design Details: Outbound Warehouse Flow</span><span class="sxs-lookup"><span data-stu-id="fbfaa-219">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="fbfaa-220">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="fbfaa-220">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
<span data-ttu-id="fbfaa-221">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fbfaa-221">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
