---
title: Personalising Pages (contains video)
description: Learn how to customise the user interface and personalise your workspace to suit your way of working and personal preferences in Business Central.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields, resize column, change column width
ms.search.form: 9020, 9022, 9026, 9027, 9030, 9000, 9009, 9004, 9005, 9024, 9006, 9007, 9010, 9016, 9017
ms.date: 06/24/2021
ms.author: edupont
ms.openlocfilehash: 7739ead50f07adc5a7a14c6c9e57cc623da275c9
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/19/2022
ms.locfileid: "9528820"
---
# <a name="personalize-your-workspace"></a>Personalise Your Workspace

You can personalise your workspace to suit your work and preferences. Change pages so that they display only the information you need, where you need it. The personalisation changes will only affect what *you* see, not what other users see.

You can personalise all types of pages, including the Role Centre page. For more information about Role Centres, see [Role Centre](ui-change-basic-settings.md#role-center).  

[!INCLUDE [about-ui-learn](includes/about-ui-learn.md)]

You can make various changes, such as move or hide fields, columns, actions, and entire parts, and add new fields. Most personalisation must be done by first activating the **Personalising** banner. You can make simple adjustments, such as the column width, immediately on any list.

> [!NOTE]
> Administrators can perform the same layout changes as users can by customising the workspace for a profile that multiple users are assigned. For more information, see [Customise Pages for Roles](ui-personalization-manage.md)<br /><br />
Administrators can also override or disable users' personalisation, and they can define which features are even available for users to see in all or specific companies. For more information, see [Customising Business Central](ui-customizing-overview.md).

## <a name="video-overview"></a>Video Overview
The following video shows some of the ways in which you can personalise your Role Centre.

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4ArUB?rel=0]

## <a name="to-change-the-width-of-a-column"></a>To change the width of a column

You can easily resize columns on any list. Just drag the boundary between two columns to the left or the right.  

1. In the header of a list, select and drag the boundary between two columns.
2. Alternatively, double-click the boundary between two columns to auto-fit the width of the column. The width adjusts to the optimal size for readability.

As for other personalisation, the changes you make to column width are stored on your account and follow you no matter which device you sign into.

## <a name="to-start-personalizing-a-page-through-the-personalizing-banner"></a>To start personalising a page through the **Personalising** banner

1. Open any page that you want to personalise.
2. In the upper-right corner, select the ![Settings.](media/ui-experience/settings_icon_small.png "Settings icon for role centre") icon, and then choose the **Personalise** action.

    The **Personalising** banner appears at the top to indicate that you can start making changes.

    > [!NOTE]
    > To navigate during personalisation, use Ctrl + Click on an action if it is highlighted by the arrowhead.

    If you see a ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") or ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") on the banner, you can't personalise the page. For more information, see [Why a Page is Locked from Personalisation](ui-personalization-locked.md).

3. To add a field, choose the **+ Field** action.
4. From the **Add Field to Page** pane, drag and drop a field into the desired position on the page.
5. To change a UI element, point to the element, such as an action, a field, or a part. The element is immediately highlighted with an arrowhead or border.
6. Choose the element, and then choose either **Move**, **Remove**, **Hide**, **Show**, **Show under "Show more"**, **Show when collapsed**, **Show always**, **Set/Clear Freeze Pane**, or **Include/Exclude from Quick Entry**, depending on the type and county of the UI element. For more information, see [What You Can Personalise](#What).
7. When you have finished changing the layout of one or more pages, choose the **Done** button on the **Personalising** banner.

## <a name="what-you-can-personalize"></a><a name="What"></a>What You Can Personalise

|What do you want to do|How to do it|Remarks|
|----|------------|-------|
|Move something, like a field, column in list, tile, action, or part|Point anywhere on what you want to move, and drag it to its new position. The position is indicated by either a thick horizontal or vertical line.<br /><br />![Cannot move here icon](media/personalization-cannot-move-here.png "Personalising mode - Cannot move here icon") indicates that you can't move the element to the selected position.|Parts are subdivisions or areas on a page that contain things like multiple fields, another page, a chart, or tiles.<br /><br />For more information about action personalisation, see [Personalising Actions](ui-personalization-user.md#Actions). |
|Hide something, like a field, column in list, tile, action, or part.|Choose the arrowhead, choose <b>Hide</b>.|The element is greyed when you are in personalising mode. If the field you hide is also shown on the FastTab heading when the FastTab is collapsed, the field will no longer appear there.|
|Show hidden actions and parts.|For a greyed (hidden) element, choose the arrowhead, and then choose <b>Show</b>.|The hidden element is visible again.|
|Add a field or column.|In the <b>Personalising</b> banner, choose the <b>+ Field</b> action.<br /></br>The <b>Add Field to Page</b> pane opens on the right. It lists the fields that you can add to the page.<br /><br />To add a field, drag it from the pane to the position that you want it. The position is indicated by either a thick horizontal or vertical line.|Each page includes a predefined set of fields that you can display. Use this procedure to add fields or columns that haven't been previously displayed, or to show fields that you've hidden.|
|Display a field in the heading of a FastTab when it's collapsed.|Choose the arrowhead, and then choose <b>Show when collapsed</b>. <br /> <br />If you don't see this option, then it's already set. In this case, to stop displaying the field on the FastTab heading, choose <b>Show always</b>.|*FastTab* is the term used for a group of fields that appear under a common heading. Use the <b>Show when collapsed</b> option to display the most important fields. If you select a field in the heading, the FastTab will open and focus on the selected field.<br /><br />This option is only applicable if a page has a more than one FastTab. If there is only one FastTab, it can't be collapsed, so the <b>Show when collapsed</b> option isn't available.|
|Make a field display only when you select **Show more**.|Choose the arrowhead, and then choose <b>Show under "Show More"</b>. <br /> <br />If you don't see the <b>Show under "Show More"</b> option, then it's already set. In this case, to make a field display always, not just when you select **Show more**, choose <b>Show always</b>.||
|Change the freeze pane in a list to another column. |Choose the arrowhead of the column that you want as the last column of the freeze pane, and then choose <b>Set Freeze Pane</b>.<br /><br/>If you want to set the freeze pane back to its original designed position, choose the arrowhead for the current freeze pane column, and choose <b>Clear Freeze Pane</b>. Note: You can't remove this freeze pane.|The freeze pane specifies the columns that always appear on the left, even as you scroll horizontally.|  
|Skip over a field when pressing Enter.|Choose the arrowhead next to the field, or column heading in a list, and choose **Exclude from Quick Entry**. <br /><br /> If you don't see this option, then the field is already set to be skipped. In this case, to stop skipping the field, choose **Include in Quick Entry**. |See [Accelerating Data Entry Using Quick Entry](ui-enter-data.md#QuickEntry)|
|Reorder and remove views representing filtered lists.|Choose the arrowhead next to a view, and then choose **Move**, **Remove**, or **Hide**.|See [Save and Personalise List Views](ui-views.md)|  
|Add a new action to a page or report on your Role Centre.|From the target page, report request page, or Tell Me window, choose the bookmark icon.|See [Bookmark a Page or Report on Your Role Centre Role Centre](ui-bookmarks.md)|
|Always start a list as expanded or collapsed|Choose the **Expand All** or **Collapse All** button in the top-left corner of the list. Alternatively, choose the **Expand All** or **Collapse All** action in the menu of the first column. |Applies to collapsible hierarchy lists|

## <a name="personalizing-actions"></a><a name="Actions"></a>Personalising Actions

Personalisation lets you decide which actions to show on the navigation and action bars and on Role Centres and where to show them. You can show, hide, or move individual actions or action groups. Personalising the navigation and action bars is done basically the same way as with other UI elements. However, what you can do with an action or group depends on where the action or group is located. The best way to find out is to enter personalising mode and then let the arrowheads guide you.

There are a couple terms that you should be familiar with to better understand action personalisation: *action group* and *promoted category*.  

An *action group* is an element that expands to display other actions or groups. For example, on the **Sales Orders** page, one action group is the **Functions** action that appears when you choose the **Actions** action.

A *promoted category* is an action group that appears before the vertical line `|` on the action bar. The categories typically include the most commonly used actions, so that you can quickly find them. For example, on the **Sales Orders** page, the **Order**, **Release**, and  **Posting** actions are promoted categories.

> [!NOTE]
> You cannot personalise the action bar that appears in parts on the page (for example, the sales lines part on the **Sales Order** page).

### <a name="to-remove-hide-and-show-actions-and-action-groups"></a>To remove, hide, and show actions and action groups

When you want to show or hide an action, the options under the arrowhead define what can do depending on the action's state. 

1. Choose the arrowhead for an action or action group.
2. Choose from one of the following options:

|Option|What it does|
|------|------------
|**Remove**|This option appears if the selected action is also shown somewhere else on the navigation bar or action bar. Choosing this option deletes the action from the selected location so that it no longer appears. The action or action group will remain in the other locations. |
|**Hide**|This option appears if the action or action group isn't located anywhere else on the navigation bar or action bar. Like **Remove**, choosing this option will make the action or action group disappear from the navigation bar or action bar. However, in personalising mode, the action or action group will still be shown in the current position, except that it appears dimmed.|
|**Show**|This option appears if the action or action group has been previously hidden (dimmed). Choosing this option will make the action or action group appear on the navigation bar or action bar.|

### <a name="to-move-actions-and-action-groups"></a>To move actions and action groups

Where you can drop actions or actions groups is indicated by a horizontal line between two actions or a border around an action group. The following limitations exist:

- You can move individual actions into the promoted categories, but you can't rearrange the order of the actions in the category.
- You can't move an action group into a promoted category.

1. To move an action or action group, drag and drop it to the desired position, like you do with fields and columns.
2. To move an action or action group into another action group that is empty, drag the action or action group to the new group and drop it in the **Drop an action here** box.

## <a name="personalizing-parts"></a><a name="Parts"></a>Personalising Parts

Parts are areas on a page that are typically composed of multiple fields, charts or other content. A part shows a coloured border when you focus on the part. For example, a Role Centre home screen has multiple parts. Because of their well-defined boundary, you can personalise the entire part and its contents.

- To move a part, drag and drop it to the desired position. A coloured line indicates valid positions on the screen. For example, FactBoxes can only be moved next to other FactBoxes in the FactBox pane.
- You can hide a part by choosing the **Hide** option under the arrowhead.
- When you start personalising or navigate to a new page, any parts that are currently hidden will appear on the page with distinctive visuals to indicate they are hidden. You can unhide that part by choosing the **Show** option under the arrowhead.

You can clear all personalisation changes that you have made within a single part by choosing the **Clear personalisation** option under the part's arrowhead. Clearing personalisation of a part only affects changes to the contents of the part, not the placement or visibility of the part on the page.  

## <a name="to-clear-personalization"></a>To clear personalisation
At some point, you might want to undo some or all of the personalisation changes that you have made to a page over time.

1. On the **Personalising** banner, choose the **Clear personalisation** action.
2. Choose one of the following options.  

> [!CAUTION]
> Clearing personalisation can't be undone.

|Option|What it does|
|------|------------
|**Only Navigation Menu**|Clears any personalisation changes that you have ever made to the navigation menu that is shared across the Role Centre and other pages. Such changes include any new actions that were added as bookmarks, and any changes to links and groups in the menu.|  
|**Only Actions**|Clears any personalisation changes that you have ever made on the navigation or action bars on the page.|
|**Only Fields, Columns, and Parts**|Clears any personalisation changes that you have ever made to the page except changes on the navigation or action bar. Such changes include changes to fields, columns, parts, and tiles. |
|**All**|Clears all personalisation changes that you have made to the page so it looks like it did originally. Such changes include changes to navigation and action bars, fields, columns, parts, and tiles.|

## <a name="other-points-of-interest"></a>Other Points of Interest

To help you better understand personalisation, here are some pointers.

- When you make changes to a card page that you open from a list, the changes will take effect on all records that you open from that list. For example, let's say you open a specific customer from the Customers list page, and then personalise the page by adding a field. When you open other customers from the list, the field that you added will also be shown.
- Changes that you make will take effect on all your Role Centres. For example, if you make a change to the Customer list when the Role Centre is set to Business Manager, you will also see the change on the **Customers** page when the Role Centre is set to Sales Order Processor.
- Changes to a page in a pane will take effect on the page where ever it's shown.  
- You can only add fields and columns from a predefined list, which is based on the page. You can't create new ones.

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/personalize-ui-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also
[Customise Pages for Profiles](ui-personalization-manage.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Change Basic Settings](ui-change-basic-settings.md)  
[Change Which Features are Displayed](ui-experiences.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
