---
title: Basic Experience Extension | Microsoft Docs
description: This extension is a modernized alternative to Microsoft Dynamics C5.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: C5, financials, extension
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: e7377d1413e2f1969543374f1b819e6fc8a2a263
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927745"
---
# <a name="the-basic-experience-extension"></a>The Basic Experience Extension
If you have been using Microsoft Dynamics C5, Microsoft partners can help you transition to a more modern solution that is based on [!INCLUDE[d365fin](includes/d365fin_md.md)], so you can continue to enjoy the same streamlined capabilities as Dynamics C5.

This extension is intended for small businesses and can support up to three users. If you need more users you must upgrade to a [!INCLUDE[d365fin](includes/d365fin_md.md)] licence and uninstall this extension.

> [!NOTE]
> As of now, this extension is available only for customers in Denmark and Iceland. 

## <a name="whats-available"></a>What's Available
The following table describes the capabilities that are available if you install the Basic Experience extension.

|Area  |Functionality  |
|---------|---------|
|**General Ledger** |Basic Finance, Account Schedules, Fixed Assets, Bank Management, Bank Reconciliation, Payments, Direct Debit, Dimensions, Multiple Currencies, Budgets, Workflow, Document Management/OCR, Consolidation, Unlimited Companies|
|**Account Receivables/Sales** |Basic Receivables, Sales Invoicing, Sales Discounts, Pricing, Sales Tax, Contact Management |
|**Account Payables/Purchase** |Basic Payables, Purchase Invoicing |
|**Project Management** |Jobs, Job Pricing, Time Sheets, Assignment, Tasks, Resources |
|**Inventory** |Basic Inventory, Item Substitutions, Item Cross Reference |

## <a name="getting-started"></a>Getting Started
This extension is a bit different than most, and you will need help from a Microsoft partner to install and set it up. Just so that you know what to expect, here's a high-level view of what the Microsoft partner will do.

1. Create a new [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant. This can be either a trial or a CSP version.
2. Add at least one user who is assigned to a Basic Experience licence in your Azure Active Directory account.
3. Remove all companies, including the sample Cronus company.
4. Create a new company that does not contain any sample data or setups.
5. Add the **Demo RapidStart** package. <!--what does the pockage contain?-->
6. Download and install the Basic Experience extension from AppSource.

## <a name="migrating-data"></a>Migrating Data
Bring your Dynamics C5 data along. After your Microsoft partner installs the Basic Experience extension you will have an empty company. An easy way to move your data from Dynamics C5 to Basic Experience is to use the C5 Data Migration extension, which is included in [!INCLUDE[d365fin](includes/d365fin_md.md)]. The extension migrates customers, vendors, items, and your general ledger accounts and their entries.

## <a name="see-also"></a>See Also
[The C5 Data Migration Extension](ui-extensions-c5-data-migration.md)