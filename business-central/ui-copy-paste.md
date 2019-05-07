---
title: Copy and paste data
description: Copy fields and rows from Business Central pages and paste somewhere else.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accessibility, shortcuts, keyboarding
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 2db4fb00567c98b1133cd031a3d7d9f1d1955626
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "922320"
---
# <a name="copying-and-pasting"></a>Copying and Pasting
You can copy one or more rows from a list or a single field on a page, and then paste what you copied into the same page, another page, or an external document (like Microsoft Excel and Outlook email). In short, to copy, you press CTRL+C (cmd+C in macOS) on your keyboard. To paste, you press CTRL+V (cmd+V in macOS).

There are several other keyboard shortcuts for copying and pasting that help you save time when entering data. For more information about these, see [Keyboard Shortcuts](keyboard-shortcuts.md#CopyRows).

This article answers common questions you might have about copying and pasting.  

## <a name="what-can-i-copy-and-paste"></a>What can I copy and paste?
-   Copy one or more rows in [!INCLUDE[d365fin](includes/d365fin_md.md)] to the same list, or to any list with identical columns.
-   Copy one or more rows in [!INCLUDE[d365fin](includes/d365fin_md.md)] and paste into Excel or other applications.
-   Copy one or more rows in Excel and paste into a [!INCLUDE[d365fin](includes/d365fin_md.md)] list.
-   Copy the value of an individual field in [!INCLUDE[d365fin](includes/d365fin_md.md)] and paste it anywhere.

## <a name="how-do-i-copy-rows"></a>How do I copy rows?
To copy a single row, select it, and press Ctrl+C.

If you want to copy more rows, you can:
-   Press Ctrl+Click on another row or press Shift+Click to select the row and all rows in between. See [Keyboard Shortcuts](keyboard-shortcuts.md#CopyRows) for more mouse and keyboard combinations for selecting rows.
-   Select ![Show more options](media/show-more-options-icon.png "Show more options icon") in the first column of a row, choose **Select More**, select the check box next to each row that you want to copy, and then press Ctrl+C.

## <a name="how-do-i-paste-rows"></a>How do I paste rows?
Select an empty row, and press Crtl+V. If you want to replace existing rows, select the rows and press Crtl+V. In this case, you can only paste the same number of rows that you selected.

<!-- Rows are pasted directly where your cursor is located. If you paste into an empty line, any existing subsequent lines will be moved after the pasted lines. If you paste into an existing line or lines, this will be overwritten.-->

## <a name="can-i-paste-rows-into-an-outlook-email-or-onenote"></a>Can I paste rows into an Outlook email or OneNote?
Yes. This is pasted as a nicely-formatted table that preserves indentation, numeric alignment and colouring, just as you would see in [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="does-copy-and-paste-work-with-tiles"></a>Does copy and paste work with tiles?
No. The list must be viewed as rows (List View) for you to copy and paste.

## <a name="in-which-lists-can-i-copy-and-paste-rows"></a>In which lists can I copy and paste rows?
You can copy rows in any kind of list, including worksheets, FactBoxes, or list that are embedded on a page (like lines of a sales order). However, to paste rows, the list must be editable.

In some pages, the application design may prevent you from pasting of rows. Contact your administrator or application developer to change the [Editable property](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-editable-property) on the page or [PasteIsValid property](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-pasteisvalid-property) on the source table.

## <a name="on-which-clients-is-copy-and-paste-available"></a>On which clients is copy and paste available?
Copy and paste are available in the browser or the [!INCLUDE[d365fin](includes/d365fin_md.md)] app for Windows 10.

## <a name="what-is-the-maximum-number-of-rows-that-can-be-copied"></a>What is the maximum number of rows that can be copied?
You can copy as many rows as you have scrolled into view. For example, to copy all 1000 rows in a page, you must first scroll to the bottom of the page and wait for the rows to appear before copying. The maximum number of rows you can copy is only limited by the memory of your device.

## <a name="must-i-have-the-exact-same-number-of-columns-when-pasting-rows"></a>Must I have the exact same number of columns when pasting rows?
Yes. Whether you are copying from [!INCLUDE[d365fin](includes/d365fin_md.md)], from Excel, or from some other table source, the rows that you paste must have the exact matching columns - no more no less.

## <a name="why-do-i-get-errors-when-pasting-rows"></a>Why do I get errors when pasting rows?
When pasting into [!INCLUDE[d365fin](includes/d365fin_md.md)], each row is checked to make sure that values in each column are valid. If a column contains a value that is not valid, the pasting is stopped, and an error message is displayed. To avoid this, make sure that the columns have valid values before you paste them.


## <a name="see-also"></a>See also 
[Assistive Features](ui-accessibility.md)  
[Getting Started](product-get-started.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Frequently Asked Questions](across-faq.md)  
